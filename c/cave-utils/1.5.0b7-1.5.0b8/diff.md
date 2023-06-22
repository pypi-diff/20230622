# Comparing `tmp/cave_utils-1.5.0b7.tar.gz` & `tmp/cave_utils-1.5.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.0b7.tar", last modified: Thu Jun 22 13:26:15 2023, max compression
+gzip compressed data, was "cave_utils-1.5.0b8.tar", last modified: Thu Jun 22 14:03:26 2023, max compression
```

## Comparing `cave_utils-1.5.0b7.tar` & `cave_utils-1.5.0b8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b7/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b7/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b7/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.0b7/cave_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      820 2023-06-22 13:25:50.000000 cave_utils-1.5.0b7/cave_utils/arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.0b7/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.0b7/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    54678 2023-06-16 14:30:37.000000 cave_utils-1.5.0b7/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-22 13:26:15.000000 cave_utils-1.5.0b7/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      360 2023-06-22 13:26:15.000000 cave_utils-1.5.0b7/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-22 13:26:15.000000 cave_utils-1.5.0b7/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-22 13:26:15.000000 cave_utils-1.5.0b7/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-22 13:26:15.000000 cave_utils-1.5.0b7/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b7/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-22 13:26:10.000000 cave_utils-1.5.0b7/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 13:26:15.045476 cave_utils-1.5.0b7/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.0b7/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b8/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b8/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b8/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.0b8/cave_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1492 2023-06-22 14:03:14.000000 cave_utils-1.5.0b8/cave_utils/arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.0b8/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.0b8/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    54678 2023-06-16 14:30:37.000000 cave_utils-1.5.0b8/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-22 14:03:26.000000 cave_utils-1.5.0b8/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-06-22 14:03:26.000000 cave_utils-1.5.0b8/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-22 14:03:26.000000 cave_utils-1.5.0b8/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-22 14:03:26.000000 cave_utils-1.5.0b8/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-22 14:03:26.000000 cave_utils-1.5.0b8/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b8/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-22 14:03:07.000000 cave_utils-1.5.0b8/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-22 14:03:26.706299 cave_utils-1.5.0b8/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      150 2023-06-22 14:01:34.000000 cave_utils-1.5.0b8/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.0b8/test/test_import.py
```

### Comparing `cave_utils-1.5.0b7/LICENSE` & `cave_utils-1.5.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b7/NOTICE.md` & `cave_utils-1.5.0b8/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b7/PKG-INFO` & `cave_utils-1.5.0b8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.0b7
+Version: 1.5.0b8
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b7.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b8.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b7/README.md` & `cave_utils-1.5.0b8/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b7/cave_utils/log.py` & `cave_utils-1.5.0b8/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b7/cave_utils/validator.py` & `cave_utils-1.5.0b8/cave_utils/validator.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b7/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.0b8/cave_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.0b7
+Version: 1.5.0b8
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b7.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b8.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b7/setup.py` & `cave_utils-1.5.0b8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.0b7',
+  version = '1.5.0b8',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b7.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b8.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

