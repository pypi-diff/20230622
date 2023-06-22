# Comparing `tmp/faker_pyspark-0.7.0.tar.gz` & `tmp/faker_pyspark-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_pyspark-0.7.0.tar", max compression
+gzip compressed data, was "faker_pyspark-0.8.0.tar", max compression
```

## Comparing `faker_pyspark-0.7.0.tar` & `faker_pyspark-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.7.0/LICENSE
--rw-r--r--   0        0        0     1345 2023-06-22 06:45:27.764210 faker_pyspark-0.7.0/README.md
--rw-r--r--   0        0        0      112 2023-06-22 06:46:45.273695 faker_pyspark-0.7.0/faker_pyspark/__init__.py
--rw-r--r--   0        0        0     6090 2023-06-22 06:46:45.274238 faker_pyspark-0.7.0/faker_pyspark/pyspark.py
--rw-r--r--   0        0        0      650 2023-06-22 10:13:59.687039 faker_pyspark-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 faker_pyspark-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-22 10:47:21.344947 faker_pyspark-0.8.0/README.md
+-rw-r--r--   0        0        0      100 2023-06-22 10:29:18.557503 faker_pyspark-0.8.0/faker_pyspark/__init__.py
+-rw-r--r--   0        0        0     6119 2023-06-22 10:42:36.687903 faker_pyspark-0.8.0/faker_pyspark/pyspark.py
+-rw-r--r--   0        0        0      650 2023-06-22 10:41:42.847251 faker_pyspark-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 faker_pyspark-0.8.0/PKG-INFO
```

### Comparing `faker_pyspark-0.7.0/LICENSE` & `faker_pyspark-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.7.0/README.md` & `faker_pyspark-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: faker-pyspark
+Version: 0.8.0
+Summary: faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package
+Home-page: https://github.com/spsoni/faker-pyspark
+License: MIT
+Keywords: Faker, PySpark
+Author: Sury Soni
+Author-email: github@suryasoni.info
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/spsoni/faker-pyspark
+Description-Content-Type: text/markdown
+
 
 # PySpark provider for Faker
 
 [![Python package](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml/badge.svg)](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml)
 [![CodeQL](https://github.com/spsoni/faker-pyspark/actions/workflows/codeql.yml/badge.svg)](https://github.com/spsoni/faker-pyspark/actions/workflows/codeql.yml)
 
 `faker-pyspark` is a PySpark DataFrame and Schema (StructType) provider for the `Faker` Python package.
@@ -39,7 +57,18 @@
 >>> schema       = fake.pyspark_schema()
 >>> df_updated   = fake.pyspark_update_dataframe(df)
 >>> column_names = fake.pyspark_column_names()
 >>> data         = fake.pyspark_data_dict_using_schema(schema)
 >>> data         = fake.pyspark_data_dict()
 
 ```
+
+### CLI `faker`
+
+```bash
+$ faker pyspark_schema       -i faker_pyspark
+$ faker pyspark_dataframe    -i faker_pyspark
+$ faker pyspark_schema       -i faker_pyspark
+$ faker pyspark_column_names -i faker_pyspark
+$ faker pyspark_data_dict    -i faker_pyspark
+```
+
```

### Comparing `faker_pyspark-0.7.0/faker_pyspark/pyspark.py` & `faker_pyspark-0.8.0/faker_pyspark/pyspark.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,7 +164,10 @@
 
         if uid_column_name:
             sorted_columns.remove(uid_column_name)
             sorted_columns.insert(0, uid_column_name)
 
         schema = spark.createDataFrame([data, ]).select(sorted_columns).schema
         return self._add_metadata_to_schema(schema, uid_column_name)
+
+
+Provider = PySparkProvider
```

### Comparing `faker_pyspark-0.7.0/pyproject.toml` & `faker_pyspark-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faker-pyspark"
-version = "0.7.0"
+version = "0.8.0"
 description = "faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package"
 authors = ["Sury Soni <github@suryasoni.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/spsoni/faker-pyspark"
 keywords = ["Faker, PySpark"]
 repository = "https://github.com/spsoni/faker-pyspark"
```

