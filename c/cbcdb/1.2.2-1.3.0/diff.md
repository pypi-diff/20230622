# Comparing `tmp/cbcdb-1.2.2.tar.gz` & `tmp/cbcdb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcdb-1.2.2.tar", last modified: Sun Oct  2 23:41:14 2022, max compression
+gzip compressed data, was "dist/cbcdb-1.3.0.tar", last modified: Thu Jun 22 19:34:12 2023, max compression
```

## Comparing `cbcdb-1.2.2.tar` & `cbcdb-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2022-10-02 23:41:14.940403 cbcdb-1.2.2/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.2.2/.gitignore
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.2.2/LICENSE
--rw-r--r--   0 craiglathrop   (501) staff       (20)      542 2022-10-02 23:41:14.940542 cbcdb-1.2.2/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      484 2021-06-27 01:18:04.000000 cbcdb-1.2.2/README.md
--rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.2.2/build-deploy.sh
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2022-10-02 23:41:14.935491 cbcdb-1.2.2/cbcdb/
--rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.2.2/cbcdb/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    24113 2022-10-02 23:39:46.000000 cbcdb-1.2.2/cbcdb/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.2.2/cbcdb/test.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2022-10-02 23:41:14.937811 cbcdb-1.2.2/cbcdb.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      542 2022-10-02 23:41:14.000000 cbcdb-1.2.2/cbcdb.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2022-10-02 23:41:14.000000 cbcdb-1.2.2/cbcdb.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2022-10-02 23:41:14.000000 cbcdb-1.2.2/cbcdb.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.2.2/cbcdb.egg-info/not-zip-safe
--rw-r--r--   0 craiglathrop   (501) staff       (20)       55 2022-10-02 23:41:14.000000 cbcdb-1.2.2/cbcdb.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2022-10-02 23:41:14.000000 cbcdb-1.2.2/cbcdb.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.2.2/pyproject.toml
--rw-r--r--   0 craiglathrop   (501) staff       (20)       86 2022-10-02 23:40:34.000000 cbcdb-1.2.2/requirements.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      753 2022-10-02 23:41:14.941113 cbcdb-1.2.2/setup.cfg
--rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.2.2/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2022-10-02 23:41:14.939870 cbcdb-1.2.2/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.2.2/tests/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.2.2/tests/docker-compose.yml
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.2.2/tests/docker_test_setup.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.2.2/tests/test_db_manager.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:34:12.000000 cbcdb-1.3.0/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.3.0/.gitignore
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.3.0/LICENSE
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:34:12.000000 cbcdb-1.3.0/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      723 2023-06-22 19:33:07.000000 cbcdb-1.3.0/README.md
+-rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.3.0/build-deploy.sh
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:34:12.000000 cbcdb-1.3.0/cbcdb/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.3.0/cbcdb/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    24233 2023-06-22 19:31:33.000000 cbcdb-1.3.0/cbcdb/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.3.0/cbcdb/test.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:34:12.000000 cbcdb-1.3.0/cbcdb.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:34:11.000000 cbcdb-1.3.0/cbcdb.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2023-06-22 19:34:11.000000 cbcdb-1.3.0/cbcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2023-06-22 19:34:11.000000 cbcdb-1.3.0/cbcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.3.0/cbcdb.egg-info/not-zip-safe
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2023-06-22 19:34:11.000000 cbcdb-1.3.0/cbcdb.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2023-06-22 19:34:11.000000 cbcdb-1.3.0/cbcdb.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.3.0/pyproject.toml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      160 2023-06-22 19:27:40.000000 cbcdb-1.3.0/requirements.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      993 2023-06-22 19:34:12.000000 cbcdb-1.3.0/setup.cfg
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.3.0/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:34:12.000000 cbcdb-1.3.0/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.3.0/tests/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.3.0/tests/docker-compose.yml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.3.0/tests/docker_test_setup.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.3.0/tests/test_db_manager.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cbcdb-1.2.2/.gitignore` & `cbcdb-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cbcdb-1.2.2/LICENSE` & `cbcdb-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbcdb-1.2.2/cbcdb/main.py` & `cbcdb-1.3.0/cbcdb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import random
 import socket
 import time
 from datetime import datetime, date
 from typing import List, Any, Dict, Tuple
 
-import pandas as pd
 from configservice.config import Config
 from numpy import inf
 from psycopg2 import connect
 from psycopg2.extras import execute_values
 
 
 class DBManager:
@@ -149,14 +148,15 @@
             curs: An instance of a database cursor. Will be false when method is first called, then populated when
                   method is called recursively.
             conn: An instance of a database connection or false on first call.
 
         Returns: A Pandas DataFrame.
 
         """
+        import pandas as pd
         if conn:
             self._print_debug_output(f"Getting query:\n {sql}")
             if params:
                 df = pd.read_sql_query(sql, params=params, con=conn)
             else:
                 df = pd.read_sql_query(sql, con=conn)
         else:
@@ -334,14 +334,15 @@
             update_cols: Column names which contain the values a user will replace in a relational db.
             static_cols: Column names used as a unique identifier to update data in relational db.
             schema: The schema for the table to replace values in
             table: Table name to replace values in
         Returns:
             None
         """
+        import pandas as pd
         df_ = df[update_cols + static_cols].drop_duplicates()
         df_ = df_.where(pd.notnull(df_), None)
         updated_statements = []
         static_statements = []
 
         quote_col_dict = self._get_table_column_dtypes(schema, table, list(df_.columns))
 
@@ -497,14 +498,15 @@
             table_name: Name of the target table
             schema: Name of the target schema
 
         Returns:
             A sql string template for the insert statement.
             A list of params
         """
+        import pandas as pd
         columns = list(df.columns)
         columns_str = self.make_column_names(columns)
         schema = f'{schema}.' if schema else ''
         sql = f'insert into {schema}{table_name} ({columns_str}) values %s;'
         vals = list(df.values)
         # This returns a list of arrays. Need to convert to list of lists.
         params = [list(x) for x in vals]
@@ -531,14 +533,15 @@
         nan to None. Panda's built in null replacement functions are just not reliable.
 
         Args:
             params: A list of parameters
 
         Returns: A list of parameters with pd.nan's converted to None
         """
+        import pandas as pd
         row_counter = 0
         for row in params:
             value_counter = 0
             if isinstance(row, list):
                 for v in row:
                     # A note on inf. inf, or np.inf shows up sometimes. It can be positive or negative (oddly).
                     # It's important to remove this or SQL Server will throw an error about floating point precision.
@@ -570,14 +573,15 @@
         Returns:
             A string with the set or filter text. Example return formats:
                 1. Set portion string type value "col = 'val',"
                 2. Set portion numeric or bool value "col = val,"
                 3. Set portion string type value "col = 'val' and"
                 4. Set portion numeric or bool value "col = val and"
         """
+        import pandas as pd
         if pd.isnull(val):
             return f"{col}=null{sep} "
         if quote_flag_dict[col]:
             # Value should be wrapped in quotes
             # Check if value is a datetime or date type.
 
             if isinstance(val, pd.Timestamp) or isinstance(val, datetime):
```

### Comparing `cbcdb-1.2.2/tests/docker_test_setup.py` & `cbcdb-1.3.0/tests/docker_test_setup.py`

 * *Files identical despite different names*

### Comparing `cbcdb-1.2.2/tests/test_db_manager.py` & `cbcdb-1.3.0/tests/test_db_manager.py`

 * *Files identical despite different names*

