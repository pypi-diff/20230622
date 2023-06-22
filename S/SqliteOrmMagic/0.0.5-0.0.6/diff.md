# Comparing `tmp/SqliteOrmMagic-0.0.5.tar.gz` & `tmp/SqliteOrmMagic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SqliteOrmMagic-0.0.5.tar", last modified: Thu Jun 22 11:31:03 2023, max compression
+gzip compressed data, was "SqliteOrmMagic-0.0.6.tar", last modified: Thu Jun 22 11:49:20 2023, max compression
```

## Comparing `SqliteOrmMagic-0.0.5.tar` & `SqliteOrmMagic-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:31:03.180880 SqliteOrmMagic-0.0.5/
--rw-r--r--   0 practic   (1000) practic   (1000)     1064 2023-06-21 17:40:30.000000 SqliteOrmMagic-0.0.5/LICENSE
--rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:31:03.180880 SqliteOrmMagic-0.0.5/PKG-INFO
--rw-r--r--   0 practic   (1000) practic   (1000)     2952 2023-06-22 10:12:39.000000 SqliteOrmMagic-0.0.5/README.md
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:31:03.180880 SqliteOrmMagic-0.0.5/SqliteOrmMagic/
--rw-r--r--   0 practic   (1000) practic   (1000)     6166 2023-06-22 11:30:04.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic/SqliteOrmMagic.py
--rw-r--r--   0 practic   (1000) practic   (1000)        1 2023-06-21 17:40:30.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic/__init__.py
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:31:03.180880 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/
--rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:31:03.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/PKG-INFO
--rw-r--r--   0 practic   (1000) practic   (1000)      275 2023-06-22 11:31:03.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/SOURCES.txt
--rw-r--r--   0 practic   (1000) practic   (1000)        1 2023-06-22 11:31:03.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/dependency_links.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       48 2023-06-22 11:31:03.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/requires.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       15 2023-06-22 11:31:03.000000 SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/top_level.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       38 2023-06-22 11:31:03.180880 SqliteOrmMagic-0.0.5/setup.cfg
--rw-r--r--   0 practic   (1000) practic   (1000)      816 2023-06-22 11:29:22.000000 SqliteOrmMagic-0.0.5/setup.py
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/
+-rw-r--r--   0 practic   (1000) practic   (1000)     1064 2023-06-21 17:40:30.000000 SqliteOrmMagic-0.0.6/LICENSE
+-rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/PKG-INFO
+-rw-r--r--   0 practic   (1000) practic   (1000)     2952 2023-06-22 10:12:39.000000 SqliteOrmMagic-0.0.6/README.md
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.965798 SqliteOrmMagic-0.0.6/SqliteOrmMagic/
+-rw-r--r--   0 practic   (1000) practic   (1000)     6182 2023-06-22 11:48:37.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic/SqliteOrmMagic.py
+-rw-r--r--   0 practic   (1000) practic   (1000)       23 2023-06-22 11:47:29.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic/__init__.py
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.965798 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/
+-rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/PKG-INFO
+-rw-r--r--   0 practic   (1000) practic   (1000)      275 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/SOURCES.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)        1 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/dependency_links.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)       48 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/requires.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)       15 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/top_level.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)       38 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/setup.cfg
+-rw-r--r--   0 practic   (1000) practic   (1000)      816 2023-06-22 11:48:14.000000 SqliteOrmMagic-0.0.6/setup.py
```

### Comparing `SqliteOrmMagic-0.0.5/LICENSE` & `SqliteOrmMagic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SqliteOrmMagic-0.0.5/PKG-INFO` & `SqliteOrmMagic-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteOrmMagic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Facilitates the complex syntax of SQL queries through the use of standard commands for reading / writing to the SQlite3 database in Python program
 Home-page: https://github.com/Practic1984/SqliteOrmMagic.git
 Author: Practic_old
 Author-email: tda.kub@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `SqliteOrmMagic-0.0.5/README.md` & `SqliteOrmMagic-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SqliteOrmMagic-0.0.5/SqliteOrmMagic/SqliteOrmMagic.py` & `SqliteOrmMagic-0.0.6/SqliteOrmMagic/SqliteOrmMagic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # python3.9.16
+# version 0.0.6
 """
 The script allows you to access the SQlite3 database 
 through a function, which is more convenient than 
 the syntax of direct SQL queries. For questions and 
 comments, write to the author @Practic_old
 """
 import sqlite3
```

### Comparing `SqliteOrmMagic-0.0.5/SqliteOrmMagic.egg-info/PKG-INFO` & `SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteOrmMagic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Facilitates the complex syntax of SQL queries through the use of standard commands for reading / writing to the SQlite3 database in Python program
 Home-page: https://github.com/Practic1984/SqliteOrmMagic.git
 Author: Practic_old
 Author-email: tda.kub@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `SqliteOrmMagic-0.0.5/setup.py` & `SqliteOrmMagic-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["ipython>=6", "nbformat>=4", "nbconvert>=5", "requests>=2"]
 
 setup(
     name="SqliteOrmMagic",
-    version="0.0.5",
+    version="0.0.6",
     author="Practic_old",
     author_email="tda.kub@gmail.com",
     description="Facilitates the complex syntax of SQL queries through the use of standard commands for reading / writing to the SQlite3 database in Python program",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Practic1984/SqliteOrmMagic.git",
     packages=find_packages(),
```

