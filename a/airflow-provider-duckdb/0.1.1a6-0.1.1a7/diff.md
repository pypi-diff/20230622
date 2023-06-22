# Comparing `tmp/airflow-provider-duckdb-0.1.1a6.tar.gz` & `tmp/airflow-provider-duckdb-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.1.1a6.tar", last modified: Wed Jun 21 21:10:50 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.1.1a7.tar", last modified: Thu Jun 22 01:21:19 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.1.1a6.tar` & `airflow-provider-duckdb-0.1.1a7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 21:10:50.458064 airflow-provider-duckdb-0.1.1a6/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a6/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 21:10:50.457869 airflow-provider-duckdb-0.1.1a6/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a6/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 21:10:50.456889 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 21:10:50.000000 airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 21:10:50.457060 airflow-provider-duckdb-0.1.1a6/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a6/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 21:10:50.457486 airflow-provider-duckdb-0.1.1a6/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a6/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     2581 2023-06-21 21:08:49.000000 airflow-provider-duckdb-0.1.1a6/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 21:10:50.458120 airflow-provider-duckdb-0.1.1a6/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 21:10:44.000000 airflow-provider-duckdb-0.1.1a6/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-22 01:21:19.782338 airflow-provider-duckdb-0.1.1a7/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a7/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-22 01:21:19.782154 airflow-provider-duckdb-0.1.1a7/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a7/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-22 01:21:19.781252 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-22 01:21:19.000000 airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-22 01:21:19.781413 airflow-provider-duckdb-0.1.1a7/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a7/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-22 01:21:19.781932 airflow-provider-duckdb-0.1.1a7/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a7/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     2771 2023-06-22 01:21:09.000000 airflow-provider-duckdb-0.1.1a7/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-22 01:21:19.782383 airflow-provider-duckdb-0.1.1a7/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-22 01:21:14.000000 airflow-provider-duckdb-0.1.1a7/setup.py
```

### Comparing `airflow-provider-duckdb-0.1.1a6/LICENSE` & `airflow-provider-duckdb-0.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a6/PKG-INFO` & `airflow-provider-duckdb-0.1.1a7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.1a6/README.md` & `airflow-provider-duckdb-0.1.1a7/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a6/airflow_provider_duckdb.egg-info/PKG-INFO` & `airflow-provider-duckdb-0.1.1a7/airflow_provider_duckdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.1a6/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.1.1a7/duckdb_provider/hooks/duckdb_hook.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,35 +12,40 @@
 
     conn_name_attr = "duckdb_conn_id"
     default_conn_name = "duckdb_default"
     conn_type = "duckdb"
     hook_name = "DuckDB"
     placeholder = "?"
 
+    def __init__(self, *args, **kwargs):
+        "Validates the connection arguments"
+        super().__init__(*args, **kwargs)
+
+        if self.is_motherduck and self.is_local:
+            raise AirflowException(
+                "You cannot set both host and schema! If you're connecting to a local file, set host to the path to the file. If you're connecting to a MotherDuck instance, set schema to the database name."
+            )
+
     def get_conn(self) -> duckdb.DuckDBPyConnection:
         """Returns a duckdb connection object"""
-        uri = self.get_uri()
+        conn_id = getattr(self, self.conn_name_attr)
+        airflow_conn = self.get_connection(conn_id)
 
-        # if we're running against a MotherDuck instance, we can't use the duckdb:///
         if self.is_motherduck:
-            uri = uri.replace("duckdb:///", "")
+            db_name = airflow_conn.schema or ""
+            return duckdb.connect(f"md:{db_name}?token={airflow_conn.password}")
 
-        return duckdb.connect(uri)
+        if self.is_local:
+            return duckdb.connect(airflow_conn.host)
+
+        return duckdb.connect(":memory:")
 
     def get_uri(self) -> str:
         """Override DbApiHook get_uri method for get_sqlalchemy_engine()"""
-        if self.is_motherduck and self.is_local:
-            raise AirflowException(
-                "You cannot set both host and schema! If you're connecting to a local file, set host to the path to the file. If you're connecting to a MotherDuck instance, set schema to the database name."
-            )
-
-        # get the conn_id from the hook
         conn_id = getattr(self, self.conn_name_attr)
-
-        # get the airflow connection object with config
         airflow_conn = self.get_connection(conn_id)
 
         if self.is_motherduck:
             db_name = airflow_conn.schema or ""
             return f"duckdb:///md:{db_name}?motherduck_token={airflow_conn.password}&token={airflow_conn.password}"
 
         if self.is_local:
```

### Comparing `airflow-provider-duckdb-0.1.1a6/setup.py` & `airflow-provider-duckdb-0.1.1a7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.1.1a6",
+    version="0.1.1a7",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

