# Comparing `tmp/Netio-1.0.8.tar.gz` & `tmp/Netio-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Netio-1.0.8.tar", last modified: Tue Feb 21 16:09:45 2023, max compression
+gzip compressed data, was "Netio-1.0.9.tar", last modified: Tue Feb 21 16:22:20 2023, max compression
```

## Comparing `Netio-1.0.8.tar` & `Netio-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:09:45.377095 Netio-1.0.8/
--rwxrwxrwx   0 averner   (1000) averner   (1000)     1089 2020-11-20 13:27:27.000000 Netio-1.0.8/LICENSE
-drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:09:45.154312 Netio-1.0.8/Netio/
--rwxrwxrwx   0 averner   (1000) averner   (1000)     6520 2023-02-21 14:50:00.000000 Netio-1.0.8/Netio/Device.py
--rwxrwxrwx   0 averner   (1000) averner   (1000)       64 2020-11-20 13:27:27.000000 Netio-1.0.8/Netio/__init__.py
--rwxrwxrwx   0 averner   (1000) averner   (1000)       65 2020-11-20 13:27:27.000000 Netio-1.0.8/Netio/__main__.py
--rwxrwxrwx   0 averner   (1000) averner   (1000)    10985 2021-04-07 16:27:01.000000 Netio-1.0.8/Netio/cli.py
--rwxrwxrwx   0 averner   (1000) averner   (1000)      321 2020-11-20 13:27:27.000000 Netio-1.0.8/Netio/exceptions.py
-drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:09:45.354921 Netio-1.0.8/Netio.egg-info/
--rwxrwxrwx   0 averner   (1000) averner   (1000)     8162 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/PKG-INFO
--rwxrwxrwx   0 averner   (1000) averner   (1000)      293 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/SOURCES.txt
--rwxrwxrwx   0 averner   (1000) averner   (1000)        1 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/dependency_links.txt
--rwxrwxrwx   0 averner   (1000) averner   (1000)       75 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/entry_points.txt
--rwxrwxrwx   0 averner   (1000) averner   (1000)       31 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/requires.txt
--rwxrwxrwx   0 averner   (1000) averner   (1000)        6 2023-02-21 16:09:44.000000 Netio-1.0.8/Netio.egg-info/top_level.txt
--rwxrwxrwx   0 averner   (1000) averner   (1000)     8162 2023-02-21 16:09:45.377095 Netio-1.0.8/PKG-INFO
--rwxrwxrwx   0 averner   (1000) averner   (1000)     6447 2020-11-20 13:27:27.000000 Netio-1.0.8/README.md
--rwxrwxrwx   0 averner   (1000) averner   (1000)      949 2023-02-21 16:06:52.000000 Netio-1.0.8/pyproject.toml
--rwxrwxrwx   0 averner   (1000) averner   (1000)       38 2023-02-21 16:09:45.392719 Netio-1.0.8/setup.cfg
+drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:22:20.233053 Netio-1.0.9/
+-rwxrwxrwx   0 averner   (1000) averner   (1000)     1089 2020-11-20 13:27:27.000000 Netio-1.0.9/LICENSE
+drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:22:20.032488 Netio-1.0.9/Netio/
+-rwxrwxrwx   0 averner   (1000) averner   (1000)     6520 2023-02-21 14:50:00.000000 Netio-1.0.9/Netio/Device.py
+-rwxrwxrwx   0 averner   (1000) averner   (1000)       64 2020-11-20 13:27:27.000000 Netio-1.0.9/Netio/__init__.py
+-rwxrwxrwx   0 averner   (1000) averner   (1000)       65 2020-11-20 13:27:27.000000 Netio-1.0.9/Netio/__main__.py
+-rwxrwxrwx   0 averner   (1000) averner   (1000)    10985 2021-04-07 16:27:01.000000 Netio-1.0.9/Netio/cli.py
+-rwxrwxrwx   0 averner   (1000) averner   (1000)      321 2020-11-20 13:27:27.000000 Netio-1.0.9/Netio/exceptions.py
+drwxrwxrwx   0 averner   (1000) averner   (1000)        0 2023-02-21 16:22:20.195277 Netio-1.0.9/Netio.egg-info/
+-rwxrwxrwx   0 averner   (1000) averner   (1000)     8162 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/PKG-INFO
+-rwxrwxrwx   0 averner   (1000) averner   (1000)      293 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/SOURCES.txt
+-rwxrwxrwx   0 averner   (1000) averner   (1000)        1 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/dependency_links.txt
+-rwxrwxrwx   0 averner   (1000) averner   (1000)       41 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/entry_points.txt
+-rwxrwxrwx   0 averner   (1000) averner   (1000)       31 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/requires.txt
+-rwxrwxrwx   0 averner   (1000) averner   (1000)        6 2023-02-21 16:22:19.000000 Netio-1.0.9/Netio.egg-info/top_level.txt
+-rwxrwxrwx   0 averner   (1000) averner   (1000)     8162 2023-02-21 16:22:20.226526 Netio-1.0.9/PKG-INFO
+-rwxrwxrwx   0 averner   (1000) averner   (1000)     6447 2020-11-20 13:27:27.000000 Netio-1.0.9/README.md
+-rwxrwxrwx   0 averner   (1000) averner   (1000)      912 2023-02-21 16:21:59.000000 Netio-1.0.9/pyproject.toml
+-rwxrwxrwx   0 averner   (1000) averner   (1000)       38 2023-02-21 16:22:20.233053 Netio-1.0.9/setup.cfg
```

### Comparing `Netio-1.0.8/LICENSE` & `Netio-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Netio-1.0.8/Netio/Device.py` & `Netio-1.0.9/Netio/Device.py`

 * *Files identical despite different names*

### Comparing `Netio-1.0.8/Netio/cli.py` & `Netio-1.0.9/Netio/cli.py`

 * *Files identical despite different names*

### Comparing `Netio-1.0.8/Netio.egg-info/PKG-INFO` & `Netio-1.0.9/Netio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Netio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Interface to control NETIO Products devices
 Author-email: Adam Verner <averner@netio.eu>
 License: MIT License
         
         Copyright (c) 2019 Adam Verner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Netio-1.0.8/PKG-INFO` & `Netio-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Netio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Interface to control NETIO Products devices
 Author-email: Adam Verner <averner@netio.eu>
 License: MIT License
         
         Copyright (c) 2019 Adam Verner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Netio-1.0.8/README.md` & `Netio-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Netio-1.0.8/pyproject.toml` & `Netio-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Netio"
-version = "1.0.8"
+version = "1.0.9"
 description = "Interface to control NETIO Products devices"
 readme = "README.md"
 authors = [{ name = "Adam Verner", email = "averner@netio.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -25,10 +25,9 @@
 ]
 requires-python = ">=3.6"
 
 [project.urls]
 Homepage = "https://github.com/netioproducts/PyNetio"
 
 [project.scripts]
-realpython = "reader.__main__:main"
 Netio = 'Netio.cli:main'
```

