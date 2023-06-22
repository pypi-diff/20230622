# Comparing `tmp/mikkoo-2.1.1.tar.gz` & `tmp/mikkoo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikkoo-2.1.1.tar", last modified: Thu Jun 22 18:01:14 2023, max compression
+gzip compressed data, was "mikkoo-2.2.0.tar", last modified: Thu Jun 22 18:48:48 2023, max compression
```

## Comparing `mikkoo-2.1.1.tar` & `mikkoo-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     1481 2023-06-22 18:01:13.000000 mikkoo-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:01:14.930294 mikkoo-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17870 2023-06-22 18:01:13.000000 mikkoo-2.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/mikkoo/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/controller.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/mcp.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/state.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/stats.py
--rw-r--r--   0 root         (0) root         (0)    29525 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/mikkoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 18:01:14.934294 mikkoo-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 18:01:13.000000 mikkoo-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.968052 mikkoo-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-06-22 18:48:46.000000 mikkoo-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:48:47.968052 mikkoo-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-06-22 18:48:46.000000 mikkoo-2.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.964053 mikkoo-2.2.0/mikkoo/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/controller.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/mcp.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/state.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/stats.py
+-rw-r--r--   0 root         (0) root         (0)    29898 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.968052 mikkoo-2.2.0/mikkoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 18:48:47.968052 mikkoo-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 18:48:46.000000 mikkoo-2.2.0/setup.py
```

### Comparing `mikkoo-2.1.1/LICENSE` & `mikkoo-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/PKG-INFO` & `mikkoo-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.1.1
+Version: 2.2.0
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
```

### Comparing `mikkoo-2.1.1/README.rst` & `mikkoo-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/mikkoo/controller.py` & `mikkoo-2.2.0/mikkoo/controller.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/mikkoo/mcp.py` & `mikkoo-2.2.0/mikkoo/mcp.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/mikkoo/state.py` & `mikkoo-2.2.0/mikkoo/state.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/mikkoo/stats.py` & `mikkoo-2.2.0/mikkoo/stats.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.1/mikkoo/worker.py` & `mikkoo-2.2.0/mikkoo/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,28 +139,34 @@
 
     def build_sql(self, proc_name: str, *args) -> str:
         return sql.SQL('SELECT * FROM {proc_name}({values})'.format(
             proc_name=proc_name,
             values=','.join('%s' for _a in range(0, len(args))))).as_string(
                 self.postgres)
 
-    async def callproc(self, proc_name: str, *args) -> typing.Sequence[dict]:
+    async def callproc(self, proc_name: str, *args) \
+            -> typing.Optional[typing.Sequence[dict]]:
         """Call the stored procedure in Postgres with the specified
         arguments.
 
         """
         sentry_sdk.set_context('mikkoo', {'function': proc_name})
         with self.stats.track_duration(f'db.{proc_name}.query_time'):
             sql = self.build_sql(proc_name, *args)
             LOGGER.debug('Query: %r, %r', sql, args or [])
             try:
                 await self.postgres_cursor.execute(sql, args or [])
                 result = await self.postgres_cursor.fetchall()
                 LOGGER.debug('Fetchall Result: %r', result)
                 return result
+            except psycopg.OperationalError as error:
+                LOGGER.warning('Postgres OperationalError: %s', error)
+                self.send_exception_to_sentry()
+                self.log_db_error(proc_name, error)
+                await self.connect_to_postgres()
             except psycopg.InternalError as error:
                 self.send_exception_to_sentry()
                 self.log_db_error(proc_name, error)
                 raise PgQError(str(error))
             except psycopg.Error as error:
                 self.send_exception_to_sentry()
                 self.log_db_error(proc_name, error)
@@ -417,23 +423,25 @@
         """
         if not self.is_idle:
             LOGGER.warning('Process batch invoked while %s',
                            self.state_description)
             return
 
         self.set_state(self.STATE_PROCESSING)
+        batch = None
         try:
             batch = await self.callproc(
                 'pgq.next_batch', self.worker_name, self.consumer_name)
         except PgQError:
-            batch = {}
+            pass
 
-        if batch and batch[0].get('next_batch') is None:
+        if not batch or (batch and batch[0].get('next_batch') is None):
             self.stats.incr('empty_queue')
-            LOGGER.debug('Sleeping for %.2f seconds', self.wait_duration)
+            LOGGER.debug('Empty queue, sleeping for %.2f seconds',
+                         self.wait_duration)
             self.set_state(self.STATE_IDLE)
             self.stats.add_timing('sleep', self.wait_duration)
             self.ioloop.call_later(
                 self.wait_duration,
                 lambda: asyncio.ensure_future(self.process_batch()))
             return
```

### Comparing `mikkoo-2.1.1/mikkoo.egg-info/PKG-INFO` & `mikkoo-2.2.0/mikkoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.1.1
+Version: 2.2.0
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
```

### Comparing `mikkoo-2.1.1/setup.cfg` & `mikkoo-2.2.0/setup.cfg`

 * *Files identical despite different names*

