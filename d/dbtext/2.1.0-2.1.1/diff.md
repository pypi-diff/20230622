# Comparing `tmp/dbtext-2.1.0.tar.gz` & `tmp/dbtext-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtext-2.1.0.tar", last modified: Tue Jan 10 10:08:59 2023, max compression
+gzip compressed data, was "dbtext-2.1.1.tar", last modified: Thu Jun 22 14:12:38 2023, max compression
```

## Comparing `dbtext-2.1.0.tar` & `dbtext-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 10:08:59.291094 dbtext-2.1.0/
--rw-rw-rw-   0        0        0     7817 2022-01-19 10:02:50.000000 dbtext-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    13095 2023-01-10 10:08:59.290091 dbtext-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3351 2022-08-11 09:30:42.000000 dbtext-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-10 10:08:59.266128 dbtext-2.1.0/dbtext/
--rw-rw-rw-   0        0        0      254 2022-12-09 10:34:31.000000 dbtext-2.1.0/dbtext/__init__.py
--rw-rw-rw-   0        0        0    31875 2022-12-07 15:56:16.000000 dbtext-2.1.0/dbtext/base_odbc.py
--rw-rw-rw-   0        0        0      675 2022-09-13 08:08:31.000000 dbtext-2.1.0/dbtext/db_to_text.py
--rw-rw-rw-   0        0        0     3355 2022-09-28 06:43:25.000000 dbtext-2.1.0/dbtext/increments.py
--rw-rw-rw-   0        0        0      659 2022-09-28 06:43:25.000000 dbtext-2.1.0/dbtext/jsonutils.py
--rw-rw-rw-   0        0        0    13489 2023-01-10 07:54:35.000000 dbtext-2.1.0/dbtext/mongodb.py
--rw-rw-rw-   0        0        0     3935 2022-08-11 07:06:57.000000 dbtext-2.1.0/dbtext/mssql_server.py
--rw-rw-rw-   0        0        0     2130 2022-12-07 14:34:56.000000 dbtext-2.1.0/dbtext/mysql.py
--rw-rw-rw-   0        0        0     1303 2022-08-11 07:08:27.000000 dbtext-2.1.0/dbtext/sqlite3db.py
--rw-rw-rw-   0        0        0     1021 2022-12-09 10:32:43.000000 dbtext-2.1.0/dbtext/wait.py
-drwxrwxrwx   0        0        0        0 2023-01-10 10:08:59.288090 dbtext-2.1.0/dbtext.egg-info/
--rw-rw-rw-   0        0        0    13095 2023-01-10 10:08:59.000000 dbtext-2.1.0/dbtext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-01-10 10:08:59.000000 dbtext-2.1.0/dbtext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 10:08:59.000000 dbtext-2.1.0/dbtext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-10 10:08:59.000000 dbtext-2.1.0/dbtext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      719 2023-01-10 10:06:01.000000 dbtext-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-10 10:08:59.291094 dbtext-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 14:12:38.968937 dbtext-2.1.1/
+-rw-rw-rw-   0        0        0     7817 2022-01-19 10:02:50.000000 dbtext-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    13095 2023-06-22 14:12:38.967935 dbtext-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3351 2022-08-11 09:30:42.000000 dbtext-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 14:12:38.947892 dbtext-2.1.1/dbtext/
+-rw-rw-rw-   0        0        0      254 2022-12-09 10:34:31.000000 dbtext-2.1.1/dbtext/__init__.py
+-rw-rw-rw-   0        0        0    31875 2022-12-07 15:56:16.000000 dbtext-2.1.1/dbtext/base_odbc.py
+-rw-rw-rw-   0        0        0      675 2022-09-13 08:08:31.000000 dbtext-2.1.1/dbtext/db_to_text.py
+-rw-rw-rw-   0        0        0     3355 2022-09-28 06:43:25.000000 dbtext-2.1.1/dbtext/increments.py
+-rw-rw-rw-   0        0        0      659 2022-09-28 06:43:25.000000 dbtext-2.1.1/dbtext/jsonutils.py
+-rw-rw-rw-   0        0        0    13595 2023-06-22 14:07:49.000000 dbtext-2.1.1/dbtext/mongodb.py
+-rw-rw-rw-   0        0        0     3935 2022-08-11 07:06:57.000000 dbtext-2.1.1/dbtext/mssql_server.py
+-rw-rw-rw-   0        0        0     2130 2022-12-07 14:34:56.000000 dbtext-2.1.1/dbtext/mysql.py
+-rw-rw-rw-   0        0        0     1303 2022-08-11 07:08:27.000000 dbtext-2.1.1/dbtext/sqlite3db.py
+-rw-rw-rw-   0        0        0     1021 2022-12-09 10:32:43.000000 dbtext-2.1.1/dbtext/wait.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:12:38.956894 dbtext-2.1.1/dbtext.egg-info/
+-rw-rw-rw-   0        0        0    13095 2023-06-22 14:12:37.000000 dbtext-2.1.1/dbtext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-22 14:12:37.000000 dbtext-2.1.1/dbtext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:12:37.000000 dbtext-2.1.1/dbtext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 14:12:37.000000 dbtext-2.1.1/dbtext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      719 2023-06-22 14:10:17.000000 dbtext-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 14:12:38.968937 dbtext-2.1.1/setup.cfg
```

### Comparing `dbtext-2.1.0/LICENSE` & `dbtext-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/PKG-INFO` & `dbtext-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtext
-Version: 2.1.0
+Version: 2.1.1
 Summary: Database to text utility for approval testing
 Author: Johan Andersson
 Author-email: Geoff Bache <geoff.bache@pobox.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dbtext-2.1.0/README.md` & `dbtext-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/base_odbc.py` & `dbtext-2.1.1/dbtext/base_odbc.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/db_to_text.py` & `dbtext-2.1.1/dbtext/db_to_text.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/increments.py` & `dbtext-2.1.1/dbtext/increments.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/jsonutils.py` & `dbtext-2.1.1/dbtext/jsonutils.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/mongodb.py` & `dbtext-2.1.1/dbtext/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,20 +197,20 @@
                             doc["_id"] = bson.ObjectId(doc["_id"])
                         except bson.errors.InvalidId:
                             # IDs are not necessarily object ids, if they aren't just assume they're strings...
                             pass
                 collection.insert_many(docs)
 
 class Mongo_DBText:
-    def __init__(self, port=None, dbMapping=None, transactions=True, logfile=None, **kw):
+    def __init__(self, port=None, dbMapping=None, transactions=True, logfile=None, bindipall=False, **kw):
         self.port = port
         self.dbdir = os.path.abspath("mongo")
         if not os.path.isdir(self.dbdir):
             os.mkdir(self.dbdir)
-        self.start_mongo(transactions, logfile)
+        self.start_mongo(transactions, logfile, bindipall)
         self.data_dir = os.path.abspath("mongodata")
         self.initial_data = MongoTextClient.parse_data_directory(self.data_dir, dbMapping)
         self.text_client = self.make_text_client(**kw)
         if self.wait_for_all_primary():
             self.text_client.insert_data(self.initial_data)
         else:
             print("Database was not primary even after waiting 60 seconds, aborting.", file=sys.stderr)
@@ -275,24 +275,26 @@
             time.sleep(0.1)
         return False
 
 
         
 class LocalMongo_DBText(Mongo_DBText):
     mongo_exe = None
-    def start_mongo(self, transactions, logfile):
+    def start_mongo(self, transactions, logfile, bindipall):
         if not self.set_mongo_exe():
             raise RuntimeError("Could not find MongoDB, have you installed it?")
 
         # must use replica set to allow transactions. Use unique one based on process id
         self.rsId = None
         cmdArgs = [ self.mongo_exe, "--port", "0", "--dbpath", self.dbdir, "--quiet" ]
         if transactions:
             self.rsId = "rs" + str(os.getpid())
             cmdArgs += [ "--replSet", self.rsId ]
+        if bindipall:
+            cmdArgs += [ "--bind_ip_all" ]
         self.proc = subprocess.Popen(cmdArgs, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         self.pipeThread = wait.PipeReaderThread(self.proc, "Waiting for connections", logfile)
         self.pipeThread.start()
 
     def parse_port(self, line):
         lineDict = json.loads(line.strip())
         attrDict = lineDict.get("attr", {})
```

### Comparing `dbtext-2.1.0/dbtext/mssql_server.py` & `dbtext-2.1.1/dbtext/mssql_server.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/mysql.py` & `dbtext-2.1.1/dbtext/mysql.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/sqlite3db.py` & `dbtext-2.1.1/dbtext/sqlite3db.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext/wait.py` & `dbtext-2.1.1/dbtext/wait.py`

 * *Files identical despite different names*

### Comparing `dbtext-2.1.0/dbtext.egg-info/PKG-INFO` & `dbtext-2.1.1/dbtext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtext
-Version: 2.1.0
+Version: 2.1.1
 Summary: Database to text utility for approval testing
 Author: Johan Andersson
 Author-email: Geoff Bache <geoff.bache@pobox.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dbtext-2.1.0/pyproject.toml` & `dbtext-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbtext"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     { name="Geoff Bache", email="geoff.bache@pobox.com" },
     { name="Johan Andersson"},
 ]
 description = "Database to text utility for approval testing"
 readme = "README.md"
 license = { file="LICENSE" }
```

