# Comparing `tmp/isilon_hadoop_tools-5.0.0.tar.gz` & `tmp/isilon_hadoop_tools-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isilon_hadoop_tools-5.0.0.tar", last modified: Wed Mar 15 01:05:32 2023, max compression
+gzip compressed data, was "isilon_hadoop_tools-5.0.1.tar", last modified: Thu Jun 22 19:33:56 2023, max compression
```

## Comparing `isilon_hadoop_tools-5.0.0.tar` & `isilon_hadoop_tools-5.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.149297 isilon_hadoop_tools-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.133298 isilon_hadoop_tools-5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.141297 isilon_hadoop_tools-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/.github/workflows/publication.yml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/.github/workflows/validation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-03-15 01:05:32.149297 isilon_hadoop_tools-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)   590651 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/demo.png
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 01:05:32.149297 isilon_hadoop_tools-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.133298 isilon_hadoop_tools-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.145297 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/identities.py
--rw-r--r--   0 runner    (1001) docker     (123)    50962 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/onefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.145297 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-15 01:05:32.000000 isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:05:32.149297 isilon_hadoop_tools-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test__scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test_identities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tests/test_onefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-15 01:04:50.000000 isilon_hadoop_tools-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.360640 isilon_hadoop_tools-5.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.364640 isilon_hadoop_tools-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/.github/workflows/publication.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/.github/workflows/validation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)   590651 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.360640 isilon_hadoop_tools-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/identities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50962 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/onefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 19:33:56.000000 isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:33:56.368640 isilon_hadoop_tools-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test__scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test_identities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tests/test_onefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 19:33:05.000000 isilon_hadoop_tools-5.0.1/tox.ini
```

### Comparing `isilon_hadoop_tools-5.0.0/.gitignore` & `isilon_hadoop_tools-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/CONTRIBUTING.md` & `isilon_hadoop_tools-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/LICENSE` & `isilon_hadoop_tools-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/PKG-INFO` & `isilon_hadoop_tools-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isilon_hadoop_tools
-Version: 5.0.0
+Version: 5.0.1
 Summary: Tools for Using Hadoop with OneFS
 Home-page: https://github.com/isilon/isilon_hadoop_tools
 Maintainer: Isilon
 Maintainer-email: support@isilon.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isilon_hadoop_tools-5.0.0/README.md` & `isilon_hadoop_tools-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/demo.png` & `isilon_hadoop_tools-5.0.1/demo.png`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/setup.py` & `isilon_hadoop_tools-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/__init__.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/_scripts.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/_scripts.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/cli.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/cli.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/directories.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/directories.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,32 +167,34 @@
             "/user/hue/.cloudera_manager_hive_metastore_canary", "hue", "hue", 0o777
         ),
         HDFSDirectory("/user/impala", "impala", "impala", 0o775),
         HDFSDirectory("/user/livy", "livy", "livy", 0o775),
         HDFSDirectory("/user/oozie", "oozie", "oozie", 0o775),
         HDFSDirectory("/user/spark", "spark", "spark", 0o751),
         HDFSDirectory("/user/spark/applicationHistory", "spark", "spark", 0o1777),
+        HDFSDirectory("/user/spark/spark3ApplicationHistory", "spark", "spark", 0o1777),
         HDFSDirectory("/user/spark/driverLogs", "spark", "spark", 0o1777),
+        HDFSDirectory("/user/spark/driver3Logs", "spark", "spark", 0o1777),
         HDFSDirectory("/user/sqoop", "sqoop", "sqoop", 0o775),
         HDFSDirectory("/user/sqoop2", "sqoop2", "sqoop", 0o775),
         HDFSDirectory("/user/tez", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/user/yarn", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/user/yarn/mapreduce", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/user/yarn/mapreduce/mr-framework", "yarn", "hadoop", 0o775),
         HDFSDirectory("/user/yarn/services", "hdfs", "supergroup", 0o775),
-        HDFSDirectory(
-            "/user/yarn/services/service-framework", "hdfs", "supergroup", 0o775
-        ),
+        HDFSDirectory("/user/yarn/services/service-framework", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/user/zeppelin", "zeppelin", "zeppelin", 0o775),
         HDFSDirectory("/warehouse", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/warehouse/tablespace", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/warehouse/tablespace/external", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/warehouse/tablespace/managed", "hdfs", "supergroup", 0o775),
         HDFSDirectory("/warehouse/tablespace/external/hive", "hive", "hive", 0o1775),
         HDFSDirectory("/warehouse/tablespace/managed/hive", "hive", "hive", 0o1775),
+        HDFSDirectory("/yarn", "yarn", "yarn", 0o700),
+        HDFSDirectory("/yarn/node-labels", "yarn", "yarn", 0o700),
     ]
     if identity_suffix:
         for directory in directories:
             directory.apply_identity_suffix(identity_suffix)
     return directories
```

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/identities.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/identities.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools/onefs.py` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools/onefs.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/PKG-INFO` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isilon-hadoop-tools
-Version: 5.0.0
+Version: 5.0.1
 Summary: Tools for Using Hadoop with OneFS
 Home-page: https://github.com/isilon/isilon_hadoop_tools
 Maintainer: Isilon
 Maintainer-email: support@isilon.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isilon_hadoop_tools-5.0.0/src/isilon_hadoop_tools.egg-info/SOURCES.txt` & `isilon_hadoop_tools-5.0.1/src/isilon_hadoop_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/conftest.py` & `isilon_hadoop_tools-5.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/test__scripts.py` & `isilon_hadoop_tools-5.0.1/tests/test__scripts.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/test_cli.py` & `isilon_hadoop_tools-5.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/test_directories.py` & `isilon_hadoop_tools-5.0.1/tests/test_directories.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/test_identities.py` & `isilon_hadoop_tools-5.0.1/tests/test_identities.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tests/test_onefs.py` & `isilon_hadoop_tools-5.0.1/tests/test_onefs.py`

 * *Files identical despite different names*

### Comparing `isilon_hadoop_tools-5.0.0/tox.ini` & `isilon_hadoop_tools-5.0.1/tox.ini`

 * *Files identical despite different names*

