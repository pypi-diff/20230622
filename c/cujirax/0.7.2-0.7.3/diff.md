# Comparing `tmp/cujirax-0.7.2.tar.gz` & `tmp/cujirax-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.7.2.tar", last modified: Sat May 20 15:08:32 2023, max compression
+gzip compressed data, was "cujirax-0.7.3.tar", last modified: Thu Jun 22 16:01:29 2023, max compression
```

## Comparing `cujirax-0.7.2.tar` & `cujirax-0.7.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.2/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.2/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.2/README.md
--rw-r--r--   0        0        0    10592 2023-05-20 15:08:26.246966 cujirax-0.7.2/cujirax/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.7.2/cujirax/cucumber.py
--rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.2/cujirax/jira.py
--rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.2/cujirax/xray/__init__.py
--rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.2/cujirax/xray/graphql.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.2/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.2/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.3/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.3/README.md
+-rw-r--r--   0        0        0    10592 2023-06-22 15:59:32.202936 cujirax-0.7.3/cujirax/__init__.py
+-rw-r--r--   0        0        0     2230 2023-06-22 15:57:38.039609 cujirax-0.7.3/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.3/cujirax/jira.py
+-rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.3/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.3/cujirax/xray/graphql.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.3/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.3/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.3/PKG-INFO
```

### Comparing `cujirax-0.7.2/.gitignore` & `cujirax-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/LICENSE` & `cujirax-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/README.md` & `cujirax-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/cujirax/__init__.py` & `cujirax-0.7.3/cujirax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
```

### Comparing `cujirax-0.7.2/cujirax/jira.py` & `cujirax-0.7.3/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/cujirax/xray/__init__.py` & `cujirax-0.7.3/cujirax/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/cujirax/xray/graphql.py` & `cujirax-0.7.3/cujirax/xray/graphql.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/cujirax/xray/import_results.py` & `cujirax-0.7.3/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/cujirax/xray/import_tests.py` & `cujirax-0.7.3/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.2/PKG-INFO` & `cujirax-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.7.2
+Version: 0.7.3
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

