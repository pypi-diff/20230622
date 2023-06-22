# Comparing `tmp/pyspark_delta_scd2-0.3.1.tar.gz` & `tmp/pyspark_delta_scd2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_delta_scd2-0.3.1.tar", max compression
+gzip compressed data, was "pyspark_delta_scd2-0.4.0.tar", max compression
```

## Comparing `pyspark_delta_scd2-0.3.1.tar` & `pyspark_delta_scd2-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.3.1/LICENSE
--rw-r--r--   0        0        0      698 2023-06-22 04:57:06.047889 pyspark_delta_scd2-0.3.1/README.md
--rw-r--r--   0        0        0      750 2023-06-22 04:57:29.426160 pyspark_delta_scd2-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/__init__.py
--rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/base.py
--rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/utils.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1453 2023-06-22 10:22:47.629911 pyspark_delta_scd2-0.4.0/README.md
+-rw-r--r--   0        0        0      787 2023-06-22 10:20:04.539500 pyspark_delta_scd2-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.4.0/pyspark_delta_scd2/__init__.py
+-rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.4.0/pyspark_delta_scd2/base.py
+-rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.4.0/pyspark_delta_scd2/utils.py
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.4.0/PKG-INFO
```

### Comparing `pyspark_delta_scd2-0.3.1/LICENSE` & `pyspark_delta_scd2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.1/pyproject.toml` & `pyspark_delta_scd2-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "pyspark-delta-scd2"
-version = "0.3.1"
+version = "0.4.0"
 description = "This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination."
 authors = ["Sury Soni <github@suryasoni.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/spsoni/pyspark-delta-scd2"
 keywords = ["Faker, PySpark", "DeltaTable"]
 repository = "https://github.com/spsoni/pyspark-delta-scd2"
 packages = [{include = "pyspark_delta_scd2"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-faker-pyspark = "^0.3.0"
-delta-spark = "^2.4.0"
 
+[tool.poetry.group.dev.dependencies]
+delta-spark = "^2.4.0"
+faker-pyspark = "^0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/base.py` & `pyspark_delta_scd2-0.4.0/pyspark_delta_scd2/base.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/utils.py` & `pyspark_delta_scd2-0.4.0/pyspark_delta_scd2/utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.1/PKG-INFO` & `pyspark_delta_scd2-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: pyspark-delta-scd2
-Version: 0.3.1
+Version: 0.4.0
 Summary: This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination.
 Home-page: https://github.com/spsoni/pyspark-delta-scd2
 License: MIT
 Keywords: Faker, PySpark,DeltaTable
 Author: Sury Soni
 Author-email: github@suryasoni.info
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: delta-spark (>=2.4.0,<3.0.0)
-Requires-Dist: faker-pyspark (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/spsoni/pyspark-delta-scd2
 Description-Content-Type: text/markdown
 
-
 # Demo PySpark Delta Table SCD2 implementation
 
+[![Python package](https://github.com/spsoni/pyspark-delta-scd2/actions/workflows/python-package.yml/badge.svg)](https://github.com/spsoni/pyspark-delta-scd2/actions/workflows/python-package.yml)
+[![CodeQL](https://github.com/spsoni/pyspark-delta-scd2/actions/workflows/codeql.yml/badge.svg)](https://github.com/spsoni/pyspark-delta-scd2/actions/workflows/codeql.yml)
+
 This project utilizes `faker-pyspark` to generate random schema and dataframes to mimic data table snapshots.
 
 Using these snapshots to process and apply SCD2 pattern into delta table as the destination. 
 
+Source of Inspiration for SCD2 pattern: https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/BDB-2547/glue/scd-deltalake-employee-etl-job.py 
+
 ## Installation
 
 Install with pip:
 
 ``` bash
-pip install pyspark-delta-scd2
+pip install pyspark-delta-scd2 delta-spark faker-pyspark
 
 ```
 
+Please note, this package do not enforce version of delta-spark, PySpark and faker-pyspark.
+
+When you want to use this example in AWS Glue environment, enforced versions conflict with the target environment.
+
 ### Generate incremental updates to dataframe and apply scd2
 
 ``` python
 >>> from pyspark_delta_scd2 import get_spark, PySparkDeltaScd2
 >>> spark = get_spark()
 >>> demo  = PySparkDeltaScd2(spark=spark)
 >>> # initial load
```

