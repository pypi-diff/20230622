# Comparing `tmp/citros-23.25.1.tar.gz` & `tmp/citros-23.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.25.1.tar", last modified: Thu Jun 22 19:45:47 2023, max compression
+gzip compressed data, was "citros-23.25.2.tar", last modified: Thu Jun 22 21:05:02 2023, max compression
```

## Comparing `citros-23.25.1.tar` & `citros-23.25.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 19:45:30.000000 citros-23.25.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 19:45:47.279244 citros-23.25.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 19:45:30.000000 citros-23.25.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.271244 citros-23.25.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-22 19:45:30.000000 citros-23.25.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 19:45:30.000000 citros-23.25.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 19:45:30.000000 citros-23.25.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-22 19:45:30.000000 citros-23.25.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 19:45:30.000000 citros-23.25.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:45:47.279244 citros-23.25.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 19:45:30.000000 citros-23.25.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 21:04:46.000000 citros-23.25.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 21:05:02.189785 citros-23.25.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 21:04:46.000000 citros-23.25.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-22 21:04:46.000000 citros-23.25.2/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 21:04:46.000000 citros-23.25.2/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 21:04:46.000000 citros-23.25.2/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 21:04:46.000000 citros-23.25.2/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-22 21:04:46.000000 citros-23.25.2/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 21:04:46.000000 citros-23.25.2/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 21:04:46.000000 citros-23.25.2/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 21:04:46.000000 citros-23.25.2/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 21:04:46.000000 citros-23.25.2/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 21:04:46.000000 citros-23.25.2/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-22 21:04:46.000000 citros-23.25.2/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 21:04:46.000000 citros-23.25.2/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 21:04:46.000000 citros-23.25.2/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 21:04:46.000000 citros-23.25.2/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-22 21:04:46.000000 citros-23.25.2/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 21:05:02.000000 citros-23.25.2/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 21:05:02.000000 citros-23.25.2/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:05:02.000000 citros-23.25.2/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 21:05:02.000000 citros-23.25.2/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 21:05:02.000000 citros-23.25.2/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 21:04:46.000000 citros-23.25.2/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:05:02.189785 citros-23.25.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 21:04:46.000000 citros-23.25.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:02.189785 citros-23.25.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-22 21:04:46.000000 citros-23.25.2/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 21:04:46.000000 citros-23.25.2/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 21:04:46.000000 citros-23.25.2/tests/test_parse_xml.py
```

### Comparing `citros-23.25.1/LICENSE` & `citros-23.25.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/PKG-INFO` & `citros-23.25.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.25.1
+Version: 23.25.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.25.1/README.md` & `citros-23.25.2/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/bin/citros` & `citros-23.25.2/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/__init__.py` & `citros-23.25.2/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros.py` & `citros-23.25.2/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros_bag.py` & `citros-23.25.2/citros/citros_bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,17 @@
                 self.log.debug(f" \tinserting buffer size: { (size / 1024 ) / 1024 } MB")
                 if size == 0:
                     continue
                 cursor.execute(f'SET search_path TO data_bucket')
                 try:           
                     cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), null="", columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])                
                 except (Exception, psycopg2.Error) as error:
-                    buffer.seek(0)                      
+                    buffer.seek(0) 
+                    # added log to see the buffer when it fails.
+                    self.log.debug(buffer)
                     self.log.error(f" Failed to insert record into table, aboring uploading to PG DB.", error) 
                     self.log.exception(error)     
                     return False, "got exception from pgdb", str(error)
                 
                 connection.commit()
             self.log.debug(f" --- done uploading to PG")
             return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {(total_size / 1024)/1024} MB]", None
```

### Comparing `citros-23.25.1/citros/citros_batch.py` & `citros-23.25.2/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros_events.py` & `citros-23.25.2/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros_integration.py` & `citros-23.25.2/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros_params.py` & `citros-23.25.2/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/citros_utils.py` & `citros-23.25.2/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/launches/__init__.py` & `citros-23.25.2/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/launches/launch.py` & `citros-23.25.2/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/logger/__init__.py` & `citros-23.25.2/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/logger/logger.py` & `citros-23.25.2/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/logger/logger_pg_handler.py` & `citros-23.25.2/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/parsers/__init__.py` & `citros-23.25.2/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/parsers/parser_ros2.py` & `citros-23.25.2/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/rosbag/__init__.py` & `citros-23.25.2/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/rosbag/reader_base.py` & `citros-23.25.2/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/rosbag/reader_mcap.py` & `citros-23.25.2/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/citros/rosbag/reader_sqlite.py` & `citros-23.25.2/citros/rosbag/reader_sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CHUNK_SIZE = 50 * 1024 * 1024
 
 # Issue with Postgrers, json object doesnt support infinity, -infinity or nan
 def remove_inf(o):
     if o is None:
         return "nan"
     if isinstance(o, float): 
-        print(o, " ", type(o))
+        # print(o, " ", type(o))
         if o == float('inf'):
             return "inf"
         if o == -float('inf'):
             return "-inf"
         if o == float('nan'):
             return "nan"
         return o
@@ -67,9 +67,15 @@
                 rid = rid + 1
                 bytes_wrote = buffer.write(row + '\n')
                 size = size + bytes_wrote
                 # 10MB chunks max
                 if size >= CHUNK_SIZE:                    
                     yield buffer
                     buffer, size = StringIO(), 0
+            
+            # upload topic by topic so it one topic has an error it wont effect the whole bag. 
+            if size >= CHUNK_SIZE:                    
+                yield buffer
+                buffer, size = StringIO(), 0
+                    
         # return the rest of the file.
         yield buffer
```

### Comparing `citros-23.25.1/citros.egg-info/PKG-INFO` & `citros-23.25.2/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.25.1
+Version: 23.25.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.25.1/citros.egg-info/SOURCES.txt` & `citros-23.25.2/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/setup.py` & `citros-23.25.2/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/tests/test_parse_makefile.py` & `citros-23.25.2/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/tests/test_parse_setup_py.py` & `citros-23.25.2/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.1/tests/test_parse_xml.py` & `citros-23.25.2/tests/test_parse_xml.py`

 * *Files identical despite different names*

