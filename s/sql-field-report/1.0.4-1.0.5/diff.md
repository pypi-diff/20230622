# Comparing `tmp/sql_field_report-1.0.4.tar.gz` & `tmp/sql_field_report-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-1.0.4.tar", max compression
+gzip compressed data, was "sql_field_report-1.0.5.tar", max compression
```

## Comparing `sql_field_report-1.0.4.tar` & `sql_field_report-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      826 2023-06-21 22:04:41.324515 sql_field_report-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.4/README.md
--rw-r--r--   0        0        0       83 2023-06-21 21:42:32.562380 sql_field_report-1.0.4/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.4/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4798 2023-06-21 21:41:20.296504 sql_field_report-1.0.4/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.4/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0    11292 2023-06-21 22:04:34.329581 sql_field_report-1.0.4/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.4/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.4/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      826 2023-06-21 22:06:35.348427 sql_field_report-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.5/README.md
+-rw-r--r--   0        0        0       83 2023-06-21 21:42:32.562380 sql_field_report-1.0.5/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.5/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4798 2023-06-21 21:41:20.296504 sql_field_report-1.0.5/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.5/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0    11352 2023-06-21 22:06:30.278285 sql_field_report-1.0.5/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.5/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.5/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.5/PKG-INFO
```

### Comparing `sql_field_report-1.0.4/pyproject.toml` & `sql_field_report-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sql_field_report-1.0.4/README.md` & `sql_field_report-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.4/sql_field_report/sql_field_report.py` & `sql_field_report-1.0.5/sql_field_report/sql_field_report.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.4/sql_field_report/utils/analysis.py` & `sql_field_report-1.0.5/sql_field_report/utils/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,16 @@
         get_data (Callable[[str], pl.DataFrame]):  A function that will take in a table name and return a Dataframe
 
     Returns:
         tuple: A tuple describing the shape of the data
     """
     res = []
     data = get_data(table)
+    if isinstance(table, tuple):
+        table = table[0]
     length = data.shape[0]
     report = []
     if length != 0:
         for i in data.columns:
             res.append(
                 data.select(pl.col(i).value_counts(sort=True)).select(
                     [
```

### Comparing `sql_field_report-1.0.4/sql_field_report/utils/databases.py` & `sql_field_report-1.0.5/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.4/sql_field_report/utils/excel.py` & `sql_field_report-1.0.5/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.4/PKG-INFO` & `sql_field_report-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

