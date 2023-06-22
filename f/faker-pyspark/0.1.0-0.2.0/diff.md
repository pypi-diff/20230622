# Comparing `tmp/faker_pyspark-0.1.0.tar.gz` & `tmp/faker_pyspark-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_pyspark-0.1.0.tar", max compression
+gzip compressed data, was "faker_pyspark-0.2.0.tar", max compression
```

## Comparing `faker_pyspark-0.1.0.tar` & `faker_pyspark-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.1.0/LICENSE
--rw-r--r--   0        0        0      849 2023-06-21 14:51:41.262685 faker_pyspark-0.1.0/README.md
--rw-r--r--   0        0        0      112 2023-06-21 11:30:49.437769 faker_pyspark-0.1.0/faker_pyspark/__init__.py
--rw-r--r--   0        0        0     6090 2023-06-21 14:12:57.348776 faker_pyspark-0.1.0/faker_pyspark/pyspark.py
--rw-r--r--   0        0        0      507 2023-06-21 14:29:53.284993 faker_pyspark-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 faker_pyspark-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1078 2023-06-22 01:31:39.061918 faker_pyspark-0.2.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-21 11:30:49.437769 faker_pyspark-0.2.0/faker_pyspark/__init__.py
+-rw-r--r--   0        0        0     6090 2023-06-21 14:12:57.348776 faker_pyspark-0.2.0/faker_pyspark/pyspark.py
+-rw-r--r--   0        0        0      686 2023-06-22 01:29:16.748118 faker_pyspark-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 faker_pyspark-0.2.0/PKG-INFO
```

### Comparing `faker_pyspark-0.1.0/LICENSE` & `faker_pyspark-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.1.0/README.md` & `faker_pyspark-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 
 # PySpark provider for Faker
 
-`faker_pyspark` is a provider for the `Faker` Python package.
+[![Python package](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml/badge.svg)](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml)
+
+`faker-pyspark` is a PySpark DataFrame and Schema (StructType) provider for the `Faker` Python package.
 
 
 ## Description
 
-`faker_pyspark` provides PySpark based fake data for testing purposes.  The definition of "fake" in this context really means "random," as the data may look real.  However, I make no claims about accuracy, so do not use this as real data!
+`faker-pyspark` provides PySpark based fake data for testing purposes.  The definition of "fake" in this context really means "random," as the data may look real.  However, I make no claims about accuracy, so do not use this as real data!
 
 
 ## Installation
 
 Install with pip:
 
 ``` bash
-pip install faker_pyspark
+pip install faker-pyspark
 
 ```
 
 Add as a provider to your Faker instance:
 
 ``` python
```

### Comparing `faker_pyspark-0.1.0/faker_pyspark/pyspark.py` & `faker_pyspark-0.2.0/faker_pyspark/pyspark.py`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.1.0/PKG-INFO` & `faker_pyspark-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: faker-pyspark
-Version: 0.1.0
-Summary: faker_pyspark is a PySpark provider for the Faker python package
+Version: 0.2.0
+Summary: faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package
+Home-page: https://github.com/spsoni/faker-pyspark
 License: MIT
+Keywords: Faker, PySpark
 Author: Sury Soni
 Author-email: github@suryasoni.info
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Faker (>=18.11.1,<19.0.0)
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
+Project-URL: Repository, https://github.com/spsoni/faker-pyspark
 Description-Content-Type: text/markdown
 
 
 # PySpark provider for Faker
 
-`faker_pyspark` is a provider for the `Faker` Python package.
+[![Python package](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml/badge.svg)](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml)
+
+`faker-pyspark` is a PySpark DataFrame and Schema (StructType) provider for the `Faker` Python package.
 
 
 ## Description
 
-`faker_pyspark` provides PySpark based fake data for testing purposes.  The definition of "fake" in this context really means "random," as the data may look real.  However, I make no claims about accuracy, so do not use this as real data!
+`faker-pyspark` provides PySpark based fake data for testing purposes.  The definition of "fake" in this context really means "random," as the data may look real.  However, I make no claims about accuracy, so do not use this as real data!
 
 
 ## Installation
 
 Install with pip:
 
 ``` bash
-pip install faker_pyspark
+pip install faker-pyspark
 
 ```
 
 Add as a provider to your Faker instance:
 
 ``` python
```

