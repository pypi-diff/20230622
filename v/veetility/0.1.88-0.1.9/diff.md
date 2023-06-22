# Comparing `tmp/veetility-0.1.88.tar.gz` & `tmp/veetility-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.88.tar", last modified: Thu Jun 22 10:12:28 2023, max compression
+gzip compressed data, was "veetility-0.1.9.tar", last modified: Fri Jan 27 12:16:41 2023, max compression
```

## Comparing `veetility-0.1.88.tar` & `veetility-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-22 10:12:28.763238 veetility-0.1.88/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-22 10:12:28.763053 veetility-0.1.88/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.88/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-22 10:12:28.763300 veetility-0.1.88/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-22 10:11:05.000000 veetility-0.1.88/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-22 10:12:28.757844 veetility-0.1.88/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.88/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.88/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.88/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-22 10:12:28.761736 veetility-0.1.88/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.88/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-12 11:29:12.000000 veetility-0.1.88/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.88/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.88/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    30394 2023-06-22 10:10:14.000000 veetility-0.1.88/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.88/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-12 19:20:06.000000 veetility-0.1.88/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.88/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.88/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-22 10:12:28.762789 veetility-0.1.88/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-22 10:12:28.000000 veetility-0.1.88/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-22 10:12:28.000000 veetility-0.1.88/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-22 10:12:28.000000 veetility-0.1.88/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-22 10:12:28.000000 veetility-0.1.88/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-22 10:12:28.000000 veetility-0.1.88/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.142082 veetility-0.1.9/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:41.141929 veetility-0.1.9/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      166 2023-01-04 11:21:38.000000 veetility-0.1.9/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-01-27 12:16:41.142139 veetility-0.1.9/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1424 2023-01-27 12:16:27.000000 veetility-0.1.9/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.140419 veetility-0.1.9/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-16 18:08:11.000000 veetility-0.1.9/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    32811 2023-01-27 12:11:54.000000 veetility-0.1.9/veetility/utility_functions.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.141660 veetility-0.1.9/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      235 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       90 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.88/setup.py` & `veetility-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.88",
+    version="0.1.9",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
@@ -32,12 +32,12 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["veetility"],
     include_package_data=True,
-    install_requires=["fuzzywuzzy", 'gspread',
-                        "gspread_dataframe", "numpy",
-                        "pandas", "psycopg2-binary", "regex",
-                        "requests", "SQLAlchemy", "tqdm"]
+    install_requires=["fuzzywuzzy",'gspread',
+                        "gspread_dataframe","numpy",
+                        "pandas","psycopg2","regex",
+                        "requests","SQLAlchemy","tqdm"]
 )
```

