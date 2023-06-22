# Comparing `tmp/cbcdb-1.3.1.tar.gz` & `tmp/cbcdb-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cbcdb-1.3.1.tar", last modified: Thu Jun 22 19:39:04 2023, max compression
+gzip compressed data, was "dist/cbcdb-1.3.2.tar", last modified: Thu Jun 22 19:48:53 2023, max compression
```

## Comparing `cbcdb-1.3.1.tar` & `cbcdb-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:39:04.000000 cbcdb-1.3.1/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.3.1/.gitignore
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.3.1/LICENSE
--rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:39:04.000000 cbcdb-1.3.1/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      723 2023-06-22 19:33:07.000000 cbcdb-1.3.1/README.md
--rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.3.1/build-deploy.sh
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb/
--rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.3.1/cbcdb/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    24217 2023-06-22 19:39:01.000000 cbcdb-1.3.1/cbcdb/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.3.1/cbcdb/test.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.3.1/cbcdb.egg-info/not-zip-safe
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2023-06-22 19:39:04.000000 cbcdb-1.3.1/cbcdb.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.3.1/pyproject.toml
--rw-r--r--   0 craiglathrop   (501) staff       (20)      160 2023-06-22 19:27:40.000000 cbcdb-1.3.1/requirements.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      993 2023-06-22 19:39:04.000000 cbcdb-1.3.1/setup.cfg
--rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.3.1/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:39:04.000000 cbcdb-1.3.1/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.3.1/tests/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.3.1/tests/docker-compose.yml
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.3.1/tests/docker_test_setup.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.3.1/tests/test_db_manager.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.3.2/.gitignore
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.3.2/LICENSE
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:48:53.000000 cbcdb-1.3.2/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      723 2023-06-22 19:33:07.000000 cbcdb-1.3.2/README.md
+-rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.3.2/build-deploy.sh
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/cbcdb/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.3.2/cbcdb/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    24175 2023-06-22 19:48:49.000000 cbcdb-1.3.2/cbcdb/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.3.2/cbcdb/test.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/cbcdb.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.3.2/cbcdb.egg-info/not-zip-safe
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.3.2/pyproject.toml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      160 2023-06-22 19:27:40.000000 cbcdb-1.3.2/requirements.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      993 2023-06-22 19:48:53.000000 cbcdb-1.3.2/setup.cfg
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.3.2/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.3.2/tests/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.3.2/tests/docker-compose.yml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.3.2/tests/docker_test_setup.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.3.2/tests/test_db_manager.py
```

### Comparing `cbcdb-1.3.1/.gitignore` & `cbcdb-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.1/LICENSE` & `cbcdb-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.1/PKG-INFO` & `cbcdb-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcdb
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to help facilitate postgres and Redshift database communication over SSH.
 Home-page: https://github.com/Cold-Bore-Capital/cbc-dbmanager
 Author: Cold Bore Capital
 Author-email: it-group@coldborecapital.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `cbcdb-1.3.1/README.md` & `cbcdb-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.1/cbcdb/main.py` & `cbcdb-1.3.2/cbcdb/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
             execute_values(curs, sql, params)
             duration = time.time() - start_time
             self._print_debug_output(f'Inserted {len(params)} rows in {round(duration, 2)} seconds')
             conn.commit()
         else:
             self._get_connection(sql, params, self.insert_many)
 
-    def update_batch_from_df(self, df: pd.DataFrame, update_cols: list, static_cols: list, schema: str,
+    def update_batch_from_df(self, df, update_cols: list, static_cols: list, schema: str,
                              table: str) -> None:
         """
         Generates and executes an update from a dataframe.
 
 
         Args:
             df: A dataframe where each record contains a new value that will replace a value in a relational db.
@@ -484,15 +484,15 @@
             input_list: A list containing the parameters for a SQL call
 
         Returns: A string with parameters represented by %s placeholders.
         """
         print('make_variable_replacements has been depreciated and will be removed in a future version.')
         return self.make_param_string(input_list)
 
-    def build_sql_from_dataframe(self, df: pd.DataFrame, table_name: str, schema: str) -> Tuple[str, list]:
+    def build_sql_from_dataframe(self, df, table_name: str, schema: str) -> Tuple[str, list]:
         """
         Builds a SQL string and params from dataframe
         This method will return a string SQL call and a list of params. The column names of the
         dataframe must match the column names in the table.
         Args:
             df: DataFrame to use for SQL call
             table_name: Name of the target table
@@ -508,15 +508,15 @@
         schema = f'{schema}.' if schema else ''
         sql = f'insert into {schema}{table_name} ({columns_str}) values %s;'
         vals = list(df.values)
         # This returns a list of arrays. Need to convert to list of lists.
         params = [list(x) for x in vals]
         return sql, params
 
-    def save_dataframe(self, df: pd.DataFrame, table_name: str, schema: str) -> None:
+    def save_dataframe(self, df, table_name: str, schema: str) -> None:
         """
         Saves a dataframe to a table in redshift/postgres.
         Args:
             df: DataFrame to use for SQL call
             table_name: Name of the target table
             schema: Name of the target schema.
         Returns:
```

### Comparing `cbcdb-1.3.1/cbcdb.egg-info/PKG-INFO` & `cbcdb-1.3.2/cbcdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcdb
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to help facilitate postgres and Redshift database communication over SSH.
 Home-page: https://github.com/Cold-Bore-Capital/cbc-dbmanager
 Author: Cold Bore Capital
 Author-email: it-group@coldborecapital.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `cbcdb-1.3.1/setup.cfg` & `cbcdb-1.3.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cbcdb
-version = 1.3.1
+version = 1.3.2
 author = Cold Bore Capital
 author_email = it-group@coldborecapital.com
 home_page = https://github.com/Cold-Bore-Capital/cbc-dbmanager
 description = A package to help facilitate postgres and Redshift database communication over SSH.
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
```

### Comparing `cbcdb-1.3.1/tests/docker_test_setup.py` & `cbcdb-1.3.2/tests/docker_test_setup.py`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.1/tests/test_db_manager.py` & `cbcdb-1.3.2/tests/test_db_manager.py`

 * *Files identical despite different names*

