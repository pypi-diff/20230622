# Comparing `tmp/sql_field_report-1.0.5.tar.gz` & `tmp/sql_field_report-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-1.0.5.tar", max compression
+gzip compressed data, was "sql_field_report-1.0.7.tar", max compression
```

## Comparing `sql_field_report-1.0.5.tar` & `sql_field_report-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      826 2023-06-21 22:06:35.348427 sql_field_report-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.5/README.md
--rw-r--r--   0        0        0       83 2023-06-21 21:42:32.562380 sql_field_report-1.0.5/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.5/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4798 2023-06-21 21:41:20.296504 sql_field_report-1.0.5/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.5/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0    11352 2023-06-21 22:06:30.278285 sql_field_report-1.0.5/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.5/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.5/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      826 2023-06-22 08:40:09.982321 sql_field_report-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.7/README.md
+-rw-r--r--   0        0        0      123 2023-06-22 08:39:56.322632 sql_field_report-1.0.7/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.7/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4798 2023-06-21 21:41:20.296504 sql_field_report-1.0.7/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.7/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0    11624 2023-06-22 08:37:32.888724 sql_field_report-1.0.7/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.7/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.7/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0      796 2023-06-22 08:38:51.367899 sql_field_report-1.0.7/sql_field_report/utils/file_utils.py
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.7/PKG-INFO
```

### Comparing `sql_field_report-1.0.5/pyproject.toml` & `sql_field_report-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "1.0.5"
+version = "1.0.7"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sql_field_report-1.0.5/README.md` & `sql_field_report-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.5/sql_field_report/sql_field_report.py` & `sql_field_report-1.0.7/sql_field_report/sql_field_report.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.5/sql_field_report/utils/analysis.py` & `sql_field_report-1.0.7/sql_field_report/utils/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,40 +235,49 @@
                     ]
                 )
             )
 
         for i in res:
             column = i.columns[0]
             if i.dtypes[0] == pl.Utf8:
-                e = i.filter(pl.col(column) == "").select(pl.col("counts"))
+                e = i.filter((pl.col(column) == "") | (pl.col(column).is_null())).select(pl.col("counts"))
                 if e.shape[0] > 0:
                     empty = e.rows(named=True)[0].get("counts")
                 else:
                     empty = 0
             elif i.dtypes[0] in pl.INTEGER_DTYPES or i.dtypes[0] in pl.FLOAT_DTYPES:
-                e = i.filter(pl.col(column).is_null()).select(pl.col("counts"))
+                e = i.filter(pl.col(column).is_null() | pl.col(column).is_nan()).select(pl.col("counts"))
                 if e.shape[0] > 0:
                     empty = e.rows(named=True)[0].get("counts")
                 else:
                     empty = 0
             else:
                 print(i.dtypes[0])
                 empty = 0
             populated = length - empty
-            unique = i.shape[0]
+            if populated == 0:
+                unique = 0
+            else:
+                unique = i.shape[0]
+
+
             choice_ratio = float(unique) / float(length)
             choice_flag = get_choice_flag(unique, choice_ratio, length)
 
-            types = list(
-                [
-                    estimate_dealcloud_datatype(v, choice_flag)
-                    for v in i.select(pl.col(column))
-                ]
-            )
-            datatype = most_common(types)
+            if populated ==0:
+                datatype = "EMPTY"
+            else:
+                types = list(
+                    [
+                        estimate_dealcloud_datatype(v, choice_flag)
+                        for v in i.select(pl.col(column))
+                    ]
+                )
+                datatype = most_common(types)
+            
 
             logger.info("Analyzed: {}".format(str((table, column, length, populated, unique, datatype))))
 
             report.append((table, column, length, populated, unique, datatype))
     else:
         for i in data.columns:
             column = i
```

### Comparing `sql_field_report-1.0.5/sql_field_report/utils/databases.py` & `sql_field_report-1.0.7/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.5/sql_field_report/utils/excel.py` & `sql_field_report-1.0.7/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.5/PKG-INFO` & `sql_field_report-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 1.0.5
+Version: 1.0.7
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

