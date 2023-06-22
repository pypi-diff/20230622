# Comparing `tmp/eparse-0.6.0.tar.gz` & `tmp/eparse-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.6.0.tar", last modified: Thu Jun 15 01:34:00 2023, max compression
+gzip compressed data, was "eparse-0.6.1.tar", last modified: Thu Jun 22 18:58:31 2023, max compression
```

## Comparing `eparse-0.6.0.tar` & `eparse-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.0/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.6.0/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.0/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.0/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12670 2023-06-15 01:34:00.238480 eparse-0.6.0/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11599 2023-06-15 01:31:22.000000 eparse-0.6.0/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-15 01:21:07.000000 eparse-0.6.0/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.0/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-06-15 01:08:49.000000 eparse-0.6.0/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.0/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.0/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12670 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-06-15 01:34:00.238480 eparse-0.6.0/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-15 01:20:56.000000 eparse-0.6.0/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.0/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.0/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.0/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.0/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.0/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.6.0/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.0/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.1/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      681 2023-06-22 18:56:31.000000 eparse-0.6.1/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.1/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.1/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13049 2023-06-22 18:58:31.265839 eparse-0.6.1/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11620 2023-06-16 03:28:39.000000 eparse-0.6.1/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-22 18:51:50.000000 eparse-0.6.1/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.1/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-06-15 01:08:49.000000 eparse-0.6.1/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.1/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.1/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13049 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-06-22 18:58:31.275839 eparse-0.6.1/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-22 18:51:42.000000 eparse-0.6.1/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.1/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.1/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.1/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.1/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.1/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.6.1/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.1/tests/test_interfaces.py
```

### Comparing `eparse-0.6.0/CONTRIBUTING.rst` & `eparse-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/LICENSE` & `eparse-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/PKG-INFO` & `eparse-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.0
+Version: 0.6.1
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -38,15 +38,15 @@
 and querying.
 
 
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
-* Tabular data extraction
+* Sub-tabular data extraction (logical tables)
 * SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
@@ -332,15 +332,15 @@
     $ sudo apt-get install -y sqlite3-tools
     $ sqlite3 .files/<db_file>
     SQLite version 3.37.2 2022-01-06 13:25:41
     Enter ".help" for usage hints.
     sqlite> .schema
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
-    sqlite> SELECT * FROM excelparse limit 1;
+    sqlite> SELECT * FROM excelparse LIMIT 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
 Migrate
 -------
 eparse wouldn't be a solid tool without the ability to migrate your
@@ -393,7 +393,29 @@
 * Updated README
 
 0.2.0 (2023-06-12)
 ==================
 
 * Added migrate command
 * Added 0.1.2 to 0.2.0 migration
+
+0.3.0 (2023-06-14)
+==================
+
+* Added inteface classes
+* Added migrations
+
+0.4.0 (2023-06-14)
+==================
+
+* Added postgresql interface
+
+0.5.0 (2023-06-14)
+==================
+
+* Optimized database interfaces
+
+0.6.1 (2023-06-22)
+==================
+
+* Added get_df_from_file helper function
+* Added contrib with unstructured partition handler
```

### Comparing `eparse-0.6.0/README.rst` & `eparse-0.6.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 and querying.
 
 
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
-* Tabular data extraction
+* Sub-tabular data extraction (logical tables)
 * SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
@@ -311,15 +311,15 @@
     $ sudo apt-get install -y sqlite3-tools
     $ sqlite3 .files/<db_file>
     SQLite version 3.37.2 2022-01-06 13:25:41
     Enter ".help" for usage hints.
     sqlite> .schema
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
-    sqlite> SELECT * FROM excelparse limit 1;
+    sqlite> SELECT * FROM excelparse LIMIT 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
 Migrate
 -------
 eparse wouldn't be a solid tool without the ability to migrate your
```

### Comparing `eparse-0.6.0/docs/Makefile` & `eparse-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/docs/conf.py` & `eparse-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/docs/installation.rst` & `eparse-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/docs/make.bat` & `eparse-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/eparse/cli.py` & `eparse-0.6.1/eparse/cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/eparse/core.py` & `eparse-0.6.1/eparse/core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/eparse/interfaces.py` & `eparse-0.6.1/eparse/interfaces.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/eparse/migrations.py` & `eparse-0.6.1/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/eparse.egg-info/PKG-INFO` & `eparse-0.6.1/eparse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.0
+Version: 0.6.1
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -38,15 +38,15 @@
 and querying.
 
 
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
-* Tabular data extraction
+* Sub-tabular data extraction (logical tables)
 * SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
@@ -332,15 +332,15 @@
     $ sudo apt-get install -y sqlite3-tools
     $ sqlite3 .files/<db_file>
     SQLite version 3.37.2 2022-01-06 13:25:41
     Enter ".help" for usage hints.
     sqlite> .schema
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
-    sqlite> SELECT * FROM excelparse limit 1;
+    sqlite> SELECT * FROM excelparse LIMIT 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
 Migrate
 -------
 eparse wouldn't be a solid tool without the ability to migrate your
@@ -393,7 +393,29 @@
 * Updated README
 
 0.2.0 (2023-06-12)
 ==================
 
 * Added migrate command
 * Added 0.1.2 to 0.2.0 migration
+
+0.3.0 (2023-06-14)
+==================
+
+* Added inteface classes
+* Added migrations
+
+0.4.0 (2023-06-14)
+==================
+
+* Added postgresql interface
+
+0.5.0 (2023-06-14)
+==================
+
+* Optimized database interfaces
+
+0.6.1 (2023-06-22)
+==================
+
+* Added get_df_from_file helper function
+* Added contrib with unstructured partition handler
```

### Comparing `eparse-0.6.0/eparse.egg-info/SOURCES.txt` & `eparse-0.6.1/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/setup.py` & `eparse-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.6.0',
+    version='0.6.1',
     zip_safe=False,
 )
```

### Comparing `eparse-0.6.0/tests/eparse_unit_test_data.xlsx` & `eparse-0.6.1/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/tests/fixtures.py` & `eparse-0.6.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/tests/test.db` & `eparse-0.6.1/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/tests/test_cli.py` & `eparse-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/tests/test_core.py` & `eparse-0.6.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.0/tests/test_interfaces.py` & `eparse-0.6.1/tests/test_interfaces.py`

 * *Files identical despite different names*

