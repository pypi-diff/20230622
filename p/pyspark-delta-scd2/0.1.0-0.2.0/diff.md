# Comparing `tmp/pyspark_delta_scd2-0.1.0.tar.gz` & `tmp/pyspark_delta_scd2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_delta_scd2-0.1.0.tar", max compression
+gzip compressed data, was "pyspark_delta_scd2-0.2.0.tar", max compression
```

## Comparing `pyspark_delta_scd2-0.1.0.tar` & `pyspark_delta_scd2-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.1.0/LICENSE
--rw-r--r--   0        0        0      693 2023-06-22 04:26:02.010420 pyspark_delta_scd2-0.1.0/README.md
--rw-r--r--   0        0        0      574 2023-06-22 04:28:03.163046 pyspark_delta_scd2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.1.0/pyspark_delta_scd2/__init__.py
--rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.1.0/pyspark_delta_scd2/base.py
--rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.1.0/pyspark_delta_scd2/utils.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.2.0/LICENSE
+-rw-r--r--   0        0        0      693 2023-06-22 04:26:02.010420 pyspark_delta_scd2-0.2.0/README.md
+-rw-r--r--   0        0        0      750 2023-06-22 04:36:12.427125 pyspark_delta_scd2-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.2.0/pyspark_delta_scd2/__init__.py
+-rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.2.0/pyspark_delta_scd2/base.py
+-rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.2.0/pyspark_delta_scd2/utils.py
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.2.0/PKG-INFO
```

### Comparing `pyspark_delta_scd2-0.1.0/LICENSE` & `pyspark_delta_scd2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.1.0/README.md` & `pyspark_delta_scd2-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.1.0/pyproject.toml` & `pyspark_delta_scd2-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "pyspark-delta-scd2"
-version = "0.1.0"
-description = "This project utilizes `faker-pyspark` to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination."
+version = "0.2.0"
+description = "This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination."
 authors = ["Sury Soni <github@suryasoni.info>"]
+license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/spsoni/pyspark_delta_scd2"
+keywords = ["Faker, PySpark", "DeltaTable"]
+repository = "https://github.com/spsoni/pyspark_delta_scd2"
 packages = [{include = "pyspark_delta_scd2"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 faker-pyspark = "^0.3.0"
 delta-spark = "^2.4.0"
```

### Comparing `pyspark_delta_scd2-0.1.0/pyspark_delta_scd2/base.py` & `pyspark_delta_scd2-0.2.0/pyspark_delta_scd2/base.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.1.0/pyspark_delta_scd2/utils.py` & `pyspark_delta_scd2-0.2.0/pyspark_delta_scd2/utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.1.0/PKG-INFO` & `pyspark_delta_scd2-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: pyspark-delta-scd2
-Version: 0.1.0
-Summary: This project utilizes `faker-pyspark` to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination.
+Version: 0.2.0
+Summary: This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination.
+Home-page: https://github.com/spsoni/pyspark_delta_scd2
+License: MIT
+Keywords: Faker, PySpark,DeltaTable
 Author: Sury Soni
 Author-email: github@suryasoni.info
 Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: delta-spark (>=2.4.0,<3.0.0)
 Requires-Dist: faker-pyspark (>=0.3.0,<0.4.0)
+Project-URL: Repository, https://github.com/spsoni/pyspark_delta_scd2
 Description-Content-Type: text/markdown
 
 
 # Demo PySpark Delta Table SCD2 implementation
 
 This project utilizes `faker-pyspark` to generate random schema and dataframes to mimic data table snapshots.
```

