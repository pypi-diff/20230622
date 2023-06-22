# Comparing `tmp/faker_pyspark-0.5.0.tar.gz` & `tmp/faker_pyspark-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_pyspark-0.5.0.tar", max compression
+gzip compressed data, was "faker_pyspark-0.6.0.tar", max compression
```

## Comparing `faker_pyspark-0.5.0.tar` & `faker_pyspark-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.5.0/LICENSE
--rw-r--r--   0        0        0     1345 2023-06-22 06:45:27.764210 faker_pyspark-0.5.0/README.md
--rw-r--r--   0        0        0      112 2023-06-22 06:46:45.273695 faker_pyspark-0.5.0/faker_pyspark/__init__.py
--rw-r--r--   0        0        0     6090 2023-06-22 06:46:45.274238 faker_pyspark-0.5.0/faker_pyspark/pyspark.py
--rw-r--r--   0        0        0      686 2023-06-22 06:48:39.861222 faker_pyspark-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 faker_pyspark-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 11:20:30.000000 faker_pyspark-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1345 2023-06-22 06:45:27.764210 faker_pyspark-0.6.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-22 06:46:45.273695 faker_pyspark-0.6.0/faker_pyspark/__init__.py
+-rw-r--r--   0        0        0     6090 2023-06-22 06:46:45.274238 faker_pyspark-0.6.0/faker_pyspark/pyspark.py
+-rw-r--r--   0        0        0      683 2023-06-22 06:54:27.687150 faker_pyspark-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 faker_pyspark-0.6.0/PKG-INFO
```

### Comparing `faker_pyspark-0.5.0/LICENSE` & `faker_pyspark-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.5.0/README.md` & `faker_pyspark-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.5.0/faker_pyspark/pyspark.py` & `faker_pyspark-0.6.0/faker_pyspark/pyspark.py`

 * *Files identical despite different names*

### Comparing `faker_pyspark-0.5.0/pyproject.toml` & `faker_pyspark-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "faker-pyspark"
-version = "0.5.0"
+version = "0.6.0"
 description = "faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package"
 authors = ["Sury Soni <github@suryasoni.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/spsoni/faker-pyspark"
 keywords = ["Faker, PySpark"]
 repository = "https://github.com/spsoni/faker-pyspark"
 packages = [{include = "faker_pyspark"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 Faker = "^18.11.1"
-pyspark = "^3.0.0"
+pyspark = "3.*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
 
 [build-system]
```

### Comparing `faker_pyspark-0.5.0/PKG-INFO` & `faker_pyspark-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: faker-pyspark
-Version: 0.5.0
+Version: 0.6.0
 Summary: faker-pyspark is a PySpark DataFrame and Schema provider for the Faker python package
 Home-page: https://github.com/spsoni/faker-pyspark
 License: MIT
 Keywords: Faker, PySpark
 Author: Sury Soni
 Author-email: github@suryasoni.info
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Faker (>=18.11.1,<19.0.0)
-Requires-Dist: pyspark (>=3.0.0,<4.0.0)
+Requires-Dist: pyspark (==3.*)
 Project-URL: Repository, https://github.com/spsoni/faker-pyspark
 Description-Content-Type: text/markdown
 
 
 # PySpark provider for Faker
 
 [![Python package](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml/badge.svg)](https://github.com/spsoni/faker_pyspark/actions/workflows/python-package.yml)
```

