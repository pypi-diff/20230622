# Comparing `tmp/faker_pyspark-0.2.0.tar.gz` & `tmp/faker_pyspark-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_pyspark-0.2.0.tar", max compression
+gzip compressed data, was "faker_pyspark-0.3.0.tar", max compression
```

## Comparing `faker_pyspark-0.2.0.tar` & `faker_pyspark-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.2.0/LICENSE
--rw-r--r--   0        0        0     1078 2023-06-22 01:31:39.061918 faker_pyspark-0.2.0/README.md
--rw-r--r--   0        0        0      112 2023-06-21 11:30:49.437769 faker_pyspark-0.2.0/faker_pyspark/__init__.py
--rw-r--r--   0        0        0     6090 2023-06-21 14:12:57.348776 faker_pyspark-0.2.0/faker_pyspark/pyspark.py
--rw-r--r--   0        0        0      686 2023-06-22 01:29:16.748118 faker_pyspark-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 faker_pyspark-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1293 2023-06-22 01:39:39.821412 faker_pyspark-0.3.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-21 11:30:49.437769 faker_pyspark-0.3.0/faker_pyspark/__init__.py
+-rw-r--r--   0        0        0     6090 2023-06-21 14:12:57.348776 faker_pyspark-0.3.0/faker_pyspark/pyspark.py
+-rw-r--r--   0        0        0      686 2023-06-22 01:39:50.282027 faker_pyspark-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 faker_pyspark-0.3.0/PKG-INFO
```

### Comparing `faker_pyspark-0.2.0/LICENSE` & `faker_pyspark-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.2.0/README.md` & `faker_pyspark-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 
 ```python
 from faker import Faker
 fake = Faker()
 ```
 
 
-### PySpark DataFrame and Schema (StructType)
+### PySpark DataFrame, Schema and more
 
 ``` python
->>> df = fake.pyspark_dataframe()
-
->>> schema = fake.pyspark_schema()
+>>> df           = fake.pyspark_dataframe()
+>>> schema       = fake.pyspark_schema()
+>>> df_updated   = fake.pyspark_update_dataframe(df)
+>>> column_names = fake.pyspark_column_names()
+>>> data         = fake.pyspark_data_dict_using_schema(schema)
+>>> data         = fake.pyspark_data_dict()
 
 ```
```

### Comparing `faker_pyspark-0.2.0/faker_pyspark/pyspark.py` & `faker_pyspark-0.3.0/faker_pyspark/pyspark.py`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.2.0/pyproject.toml` & `faker_pyspark-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faker-pyspark"
-version = "0.2.0"
+version = "0.3.0"
 description = "faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package"
 authors = ["Sury Soni <github@suryasoni.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/spsoni/faker-pyspark"
 keywords = ["Faker, PySpark"]
 repository = "https://github.com/spsoni/faker-pyspark"
```

### Comparing `faker_pyspark-0.2.0/PKG-INFO` & `faker_pyspark-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-pyspark
-Version: 0.2.0
+Version: 0.3.0
 Summary: faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package
 Home-page: https://github.com/spsoni/faker-pyspark
 License: MIT
 Keywords: Faker, PySpark
 Author: Sury Soni
 Author-email: github@suryasoni.info
 Requires-Python: >=3.8.1,<4.0.0
@@ -54,16 +54,19 @@
 
 ```python
 from faker import Faker
 fake = Faker()
 ```
 
 
-### PySpark DataFrame and Schema (StructType)
+### PySpark DataFrame, Schema and more
 
 ``` python
->>> df = fake.pyspark_dataframe()
-
->>> schema = fake.pyspark_schema()
+>>> df           = fake.pyspark_dataframe()
+>>> schema       = fake.pyspark_schema()
+>>> df_updated   = fake.pyspark_update_dataframe(df)
+>>> column_names = fake.pyspark_column_names()
+>>> data         = fake.pyspark_data_dict_using_schema(schema)
+>>> data         = fake.pyspark_data_dict()
 
 ```
```

