# Comparing `tmp/pyaprilaire-0.7.0.tar.gz` & `tmp/pyaprilaire-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaprilaire-0.7.0.tar", last modified: Thu Jun 22 01:58:51 2023, max compression
+gzip compressed data, was "pyaprilaire-0.7.0b1.tar", last modified: Sat May  6 01:10:08 2023, max compression
```

## Comparing `pyaprilaire-0.7.0.tar` & `pyaprilaire-0.7.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:58:51.373041 pyaprilaire-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-22 01:58:51.373041 pyaprilaire-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:58:51.369042 pyaprilaire-0.7.0/pyaprilaire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyaprilaire/socket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:58:51.373041 pyaprilaire-0.7.0/pyaprilaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-22 01:58:51.000000 pyaprilaire-0.7.0/pyaprilaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 01:58:51.000000 pyaprilaire-0.7.0/pyaprilaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:58:51.000000 pyaprilaire-0.7.0/pyaprilaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:58:51.000000 pyaprilaire-0.7.0/pyaprilaire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 01:58:51.000000 pyaprilaire-0.7.0/pyaprilaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:58:51.373041 pyaprilaire-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:58:51.373041 pyaprilaire-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-22 01:58:41.000000 pyaprilaire-0.7.0/tests/test_socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/pyaprilaire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_socket_client.py
```

### Comparing `pyaprilaire-0.7.0/LICENSE` & `pyaprilaire-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/PKG-INFO` & `pyaprilaire-0.7.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.7.0
+Version: 0.7.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.7.0/README.md` & `pyaprilaire-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire/client.py` & `pyaprilaire-0.7.0b1/pyaprilaire/client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire/const.py` & `pyaprilaire-0.7.0b1/pyaprilaire/const.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire/mock_server.py` & `pyaprilaire-0.7.0b1/pyaprilaire/mock_server.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire/packet.py` & `pyaprilaire-0.7.0b1/pyaprilaire/packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire/socket_client.py` & `pyaprilaire-0.7.0b1/pyaprilaire/socket_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/pyaprilaire.egg-info/PKG-INFO` & `pyaprilaire-0.7.0b1/pyaprilaire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.7.0
+Version: 0.7.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.7.0/pyproject.toml` & `pyaprilaire-0.7.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaprilaire"
-version = "0.7.0"
+version = "0.7.0b1"
 readme = "README.md"
 dependencies = [
     "crc >= 4"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "coverage"]
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyaprilaire-0.7.0/tests/test_client.py` & `pyaprilaire-0.7.0b1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/tests/test_packet.py` & `pyaprilaire-0.7.0b1/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.7.0/tests/test_socket_client.py` & `pyaprilaire-0.7.0b1/tests/test_socket_client.py`

 * *Files identical despite different names*

