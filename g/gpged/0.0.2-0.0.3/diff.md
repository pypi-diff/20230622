# Comparing `tmp/gpged-0.0.2.tar.gz` & `tmp/gpged-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpged-0.0.2.tar", last modified: Thu Jun 22 14:20:27 2023, max compression
+gzip compressed data, was "gpged-0.0.3.tar", last modified: Thu Jun 22 14:38:16 2023, max compression
```

## Comparing `gpged-0.0.2.tar` & `gpged-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.533016 gpged-0.0.2/
--rw-r--r--   0 sky        (501) staff       (20)     1048 2023-06-20 14:50:03.000000 gpged-0.0.2/LICENSE
--rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:20:27.532857 gpged-0.0.2/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)      772 2023-06-22 14:17:28.000000 gpged-0.0.2/README.md
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.531280 gpged-0.0.2/gpged/
--rw-r--r--   0 sky        (501) staff       (20)       72 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/__init__.py
--rw-r--r--   0 sky        (501) staff       (20)      579 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/__main__.py
--rw-r--r--   0 sky        (501) staff       (20)     5830 2023-06-22 13:48:39.000000 gpged-0.0.2/gpged/app.py
--rw-r--r--   0 sky        (501) staff       (20)      215 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/run_gpged.py
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.532574 gpged-0.0.2/gpged.egg-info/
--rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)      248 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/SOURCES.txt
--rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/dependency_links.txt
--rw-r--r--   0 sky        (501) staff       (20)       42 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/entry_points.txt
--rw-r--r--   0 sky        (501) staff       (20)        6 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/top_level.txt
--rw-r--r--   0 sky        (501) staff       (20)      616 2023-06-22 14:17:54.000000 gpged-0.0.2/pyproject.toml
--rw-r--r--   0 sky        (501) staff       (20)       38 2023-06-22 14:20:27.533070 gpged-0.0.2/setup.cfg
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:38:16.846016 gpged-0.0.3/
+-rw-r--r--   0 sky        (501) staff       (20)     1048 2023-06-20 14:50:03.000000 gpged-0.0.3/LICENSE
+-rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:38:16.845816 gpged-0.0.3/PKG-INFO
+-rw-r--r--   0 sky        (501) staff       (20)      772 2023-06-22 14:17:28.000000 gpged-0.0.3/README.md
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:38:16.844411 gpged-0.0.3/gpged/
+-rw-r--r--   0 sky        (501) staff       (20)       72 2023-06-22 13:29:38.000000 gpged-0.0.3/gpged/__init__.py
+-rw-r--r--   0 sky        (501) staff       (20)      579 2023-06-22 13:29:38.000000 gpged-0.0.3/gpged/__main__.py
+-rw-r--r--   0 sky        (501) staff       (20)     5830 2023-06-22 13:48:39.000000 gpged-0.0.3/gpged/app.py
+-rw-r--r--   0 sky        (501) staff       (20)      215 2023-06-22 13:29:38.000000 gpged-0.0.3/gpged/run_gpged.py
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:38:16.845410 gpged-0.0.3/gpged.egg-info/
+-rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:38:16.000000 gpged-0.0.3/gpged.egg-info/PKG-INFO
+-rw-r--r--   0 sky        (501) staff       (20)      248 2023-06-22 14:38:16.000000 gpged-0.0.3/gpged.egg-info/SOURCES.txt
+-rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-22 14:38:16.000000 gpged-0.0.3/gpged.egg-info/dependency_links.txt
+-rw-r--r--   0 sky        (501) staff       (20)       42 2023-06-22 14:38:16.000000 gpged-0.0.3/gpged.egg-info/entry_points.txt
+-rw-r--r--   0 sky        (501) staff       (20)        6 2023-06-22 14:38:16.000000 gpged-0.0.3/gpged.egg-info/top_level.txt
+-rw-r--r--   0 sky        (501) staff       (20)      616 2023-06-22 14:37:38.000000 gpged-0.0.3/pyproject.toml
+-rw-r--r--   0 sky        (501) staff       (20)       38 2023-06-22 14:38:16.846072 gpged-0.0.3/setup.cfg
```

### Comparing `gpged-0.0.2/LICENSE` & `gpged-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpged-0.0.2/PKG-INFO` & `gpged-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpged
-Version: 0.0.2
+Version: 0.0.3
 Summary: GUI for encrypting and decrypting text with GPG.
 Author-email: Sky Moore <i@msky.me>
 License: Copyright 2022 Sky Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `gpged-0.0.2/README.md` & `gpged-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpged-0.0.2/gpged/__main__.py` & `gpged-0.0.3/gpged/__main__.py`

 * *Files identical despite different names*

### Comparing `gpged-0.0.2/gpged/app.py` & `gpged-0.0.3/gpged/app.py`

 * *Files identical despite different names*

### Comparing `gpged-0.0.2/gpged.egg-info/PKG-INFO` & `gpged-0.0.3/gpged.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpged
-Version: 0.0.2
+Version: 0.0.3
 Summary: GUI for encrypting and decrypting text with GPG.
 Author-email: Sky Moore <i@msky.me>
 License: Copyright 2022 Sky Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `gpged-0.0.2/pyproject.toml` & `gpged-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpged"
-version = "0.0.2"
+version = "0.0.3"
 description = "GUI for encrypting and decrypting text with GPG."
 readme = "README.md"
 authors = [{name = "Sky Moore", email = "i@msky.me"}]
 license = {file = "LICENSE"}
 keywords = ["gpg","gnupg", "pgp", "gui", "encryption", "decryption", "cryptography"]
 classifiers = [
   "Intended Audience :: Developers",
```

