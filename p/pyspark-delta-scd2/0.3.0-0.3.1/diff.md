# Comparing `tmp/pyspark_delta_scd2-0.3.0.tar.gz` & `tmp/pyspark_delta_scd2-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_delta_scd2-0.3.0.tar", max compression
+gzip compressed data, was "pyspark_delta_scd2-0.3.1.tar", max compression
```

## Comparing `pyspark_delta_scd2-0.3.0.tar` & `pyspark_delta_scd2-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.3.0/LICENSE
--rw-r--r--   0        0        0      693 2023-06-22 04:26:02.010420 pyspark_delta_scd2-0.3.0/README.md
--rw-r--r--   0        0        0      750 2023-06-22 04:45:59.441333 pyspark_delta_scd2-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.3.0/pyspark_delta_scd2/__init__.py
--rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.3.0/pyspark_delta_scd2/base.py
--rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.3.0/pyspark_delta_scd2/utils.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-06-22 04:16:50.824625 pyspark_delta_scd2-0.3.1/LICENSE
+-rw-r--r--   0        0        0      698 2023-06-22 04:57:06.047889 pyspark_delta_scd2-0.3.1/README.md
+-rw-r--r--   0        0        0      750 2023-06-22 04:57:29.426160 pyspark_delta_scd2-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-22 04:19:23.528085 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/__init__.py
+-rw-r--r--   0        0        0     3333 2023-06-22 04:18:24.217710 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/base.py
+-rw-r--r--   0        0        0     6212 2023-06-22 04:05:33.563620 pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/utils.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 pyspark_delta_scd2-0.3.1/PKG-INFO
```

### Comparing `pyspark_delta_scd2-0.3.0/LICENSE` & `pyspark_delta_scd2-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.0/README.md` & `pyspark_delta_scd2-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```
 
 ### Generate incremental updates to dataframe and apply scd2
 
 ``` python
 >>> from pyspark_delta_scd2 import get_spark, PySparkDeltaScd2
 >>> spark = get_spark()
->>> demo = PySparkDeltaScd2(spark=spark)
+>>> demo  = PySparkDeltaScd2(spark=spark)
 >>> # initial load
->>> df1 = demo.process()
+>>> df1   = demo.process()
 >>> # incremental update
->>> df2 = demo.process()
+>>> df2   = demo.process()
 >>> # df2 should have some deletes, updates and inserts
 
 ```
```

### Comparing `pyspark_delta_scd2-0.3.0/pyproject.toml` & `pyspark_delta_scd2-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspark-delta-scd2"
-version = "0.3.0"
+version = "0.3.1"
 description = "This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination."
 authors = ["Sury Soni <github@suryasoni.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/spsoni/pyspark-delta-scd2"
 keywords = ["Faker, PySpark", "DeltaTable"]
 repository = "https://github.com/spsoni/pyspark-delta-scd2"
```

### Comparing `pyspark_delta_scd2-0.3.0/pyspark_delta_scd2/base.py` & `pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/base.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.0/pyspark_delta_scd2/utils.py` & `pyspark_delta_scd2-0.3.1/pyspark_delta_scd2/utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_delta_scd2-0.3.0/PKG-INFO` & `pyspark_delta_scd2-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-delta-scd2
-Version: 0.3.0
+Version: 0.3.1
 Summary: This project utilizes faker-pyspark to generate random schema and dataframes to mimic data table snapshots. Using these snapshots to process and apply SCD2 pattern into delta table as the destination.
 Home-page: https://github.com/spsoni/pyspark-delta-scd2
 License: MIT
 Keywords: Faker, PySpark,DeltaTable
 Author: Sury Soni
 Author-email: github@suryasoni.info
 Requires-Python: >=3.8.1,<4.0.0
@@ -35,16 +35,16 @@
 ```
 
 ### Generate incremental updates to dataframe and apply scd2
 
 ``` python
 >>> from pyspark_delta_scd2 import get_spark, PySparkDeltaScd2
 >>> spark = get_spark()
->>> demo = PySparkDeltaScd2(spark=spark)
+>>> demo  = PySparkDeltaScd2(spark=spark)
 >>> # initial load
->>> df1 = demo.process()
+>>> df1   = demo.process()
 >>> # incremental update
->>> df2 = demo.process()
+>>> df2   = demo.process()
 >>> # df2 should have some deletes, updates and inserts
 
 ```
```

