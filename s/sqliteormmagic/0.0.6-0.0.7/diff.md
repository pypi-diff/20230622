# Comparing `tmp/SqliteOrmMagic-0.0.6.tar.gz` & `tmp/sqliteormmagic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SqliteOrmMagic-0.0.6.tar", last modified: Thu Jun 22 11:49:20 2023, max compression
+gzip compressed data, was "sqliteormmagic-0.0.7.tar", last modified: Thu Jun 22 12:52:13 2023, max compression
```

## Comparing `SqliteOrmMagic-0.0.6.tar` & `sqliteormmagic-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/
--rw-r--r--   0 practic   (1000) practic   (1000)     1064 2023-06-21 17:40:30.000000 SqliteOrmMagic-0.0.6/LICENSE
--rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/PKG-INFO
--rw-r--r--   0 practic   (1000) practic   (1000)     2952 2023-06-22 10:12:39.000000 SqliteOrmMagic-0.0.6/README.md
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.965798 SqliteOrmMagic-0.0.6/SqliteOrmMagic/
--rw-r--r--   0 practic   (1000) practic   (1000)     6182 2023-06-22 11:48:37.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic/SqliteOrmMagic.py
--rw-r--r--   0 practic   (1000) practic   (1000)       23 2023-06-22 11:47:29.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic/__init__.py
-drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 11:49:20.965798 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/
--rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/PKG-INFO
--rw-r--r--   0 practic   (1000) practic   (1000)      275 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/SOURCES.txt
--rw-r--r--   0 practic   (1000) practic   (1000)        1 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/dependency_links.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       48 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/requires.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       15 2023-06-22 11:49:20.000000 SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/top_level.txt
--rw-r--r--   0 practic   (1000) practic   (1000)       38 2023-06-22 11:49:20.969131 SqliteOrmMagic-0.0.6/setup.cfg
--rw-r--r--   0 practic   (1000) practic   (1000)      816 2023-06-22 11:48:14.000000 SqliteOrmMagic-0.0.6/setup.py
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 12:52:13.373319 sqliteormmagic-0.0.7/
+-rw-r--r--   0 practic   (1000) practic   (1000)     1064 2023-06-21 17:40:30.000000 sqliteormmagic-0.0.7/LICENSE
+-rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 12:52:13.373319 sqliteormmagic-0.0.7/PKG-INFO
+-rw-r--r--   0 practic   (1000) practic   (1000)     2952 2023-06-22 10:12:39.000000 sqliteormmagic-0.0.7/README.md
+-rw-r--r--   0 practic   (1000) practic   (1000)       38 2023-06-22 12:52:13.373319 sqliteormmagic-0.0.7/setup.cfg
+-rw-r--r--   0 practic   (1000) practic   (1000)      835 2023-06-22 12:52:01.000000 sqliteormmagic-0.0.7/setup.py
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 12:52:13.369986 sqliteormmagic-0.0.7/sqliteormmagic/
+-rw-r--r--   0 practic   (1000) practic   (1000)       29 2023-06-22 12:49:04.000000 sqliteormmagic-0.0.7/sqliteormmagic/__init__.py
+-rw-r--r--   0 practic   (1000) practic   (1000)     6182 2023-06-22 11:48:37.000000 sqliteormmagic-0.0.7/sqliteormmagic/sqliteormmagic.py
+drwxr-xr-x   0 practic   (1000) practic   (1000)        0 2023-06-22 12:52:13.373319 sqliteormmagic-0.0.7/sqliteormmagic.egg-info/
+-rw-r--r--   0 practic   (1000) practic   (1000)     3443 2023-06-22 12:52:13.000000 sqliteormmagic-0.0.7/sqliteormmagic.egg-info/PKG-INFO
+-rw-r--r--   0 practic   (1000) practic   (1000)      238 2023-06-22 12:52:13.000000 sqliteormmagic-0.0.7/sqliteormmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)        1 2023-06-22 12:52:13.000000 sqliteormmagic-0.0.7/sqliteormmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 practic   (1000) practic   (1000)       15 2023-06-22 12:52:13.000000 sqliteormmagic-0.0.7/sqliteormmagic.egg-info/top_level.txt
```

### Comparing `SqliteOrmMagic-0.0.6/LICENSE` & `sqliteormmagic-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SqliteOrmMagic-0.0.6/PKG-INFO` & `sqliteormmagic-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SqliteOrmMagic
-Version: 0.0.6
+Name: sqliteormmagic
+Version: 0.0.7
 Summary: Facilitates the complex syntax of SQL queries through the use of standard commands for reading / writing to the SQlite3 database in Python program
 Home-page: https://github.com/Practic1984/SqliteOrmMagic.git
 Author: Practic_old
 Author-email: tda.kub@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `SqliteOrmMagic-0.0.6/README.md` & `sqliteormmagic-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `SqliteOrmMagic-0.0.6/SqliteOrmMagic/SqliteOrmMagic.py` & `sqliteormmagic-0.0.7/sqliteormmagic/sqliteormmagic.py`

 * *Files identical despite different names*

### Comparing `SqliteOrmMagic-0.0.6/SqliteOrmMagic.egg-info/PKG-INFO` & `sqliteormmagic-0.0.7/sqliteormmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SqliteOrmMagic
-Version: 0.0.6
+Name: sqliteormmagic
+Version: 0.0.7
 Summary: Facilitates the complex syntax of SQL queries through the use of standard commands for reading / writing to the SQlite3 database in Python program
 Home-page: https://github.com/Practic1984/SqliteOrmMagic.git
 Author: Practic_old
 Author-email: tda.kub@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

