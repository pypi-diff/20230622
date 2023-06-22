# Comparing `tmp/acct-8.5.2.tar.gz` & `tmp/acct-8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acct-8.5.2.tar", last modified: Wed Feb 15 23:52:08 2023, max compression
+gzip compressed data, was "acct-8.6.0.tar", last modified: Thu Jun 22 15:33:28 2023, max compression
```

## Comparing `acct-8.5.2.tar` & `acct-8.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.026079 acct-8.5.2/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-02-15 23:51:52.000000 acct-8.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-15 23:52:08.026079 acct-8.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3088 2023-02-15 23:51:52.000000 acct-8.5.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct/acct/backend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct/acct/backend/contracts/
--rw-r--r--   0 root         (0) root         (0)       39 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/backend/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/backend/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct/acct/contracts/
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)    12558 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.026079 acct-8.5.2/acct/acct/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.026079 acct-8.5.2/acct/acct/metadata/contracts/
--rw-r--r--   0 root         (0) root         (0)      259 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/metadata/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-02-15 23:51:52.000000 acct-8.5.2/acct/acct/metadata/init.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-02-15 23:51:52.000000 acct-8.5.2/acct/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.026079 acct-8.5.2/acct/crypto/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-15 23:51:52.000000 acct-8.5.2/acct/crypto/aesgcm256.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.026079 acct-8.5.2/acct/crypto/contracts/
--rw-r--r--   0 root         (0) root         (0)      256 2023-02-15 23:51:52.000000 acct-8.5.2/acct/crypto/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      495 2023-02-15 23:51:52.000000 acct-8.5.2/acct/crypto/fernet.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-02-15 23:51:52.000000 acct-8.5.2/acct/crypto/init.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-02-15 23:51:52.000000 acct-8.5.2/acct/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-15 23:52:07.000000 acct-8.5.2/acct/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 23:52:08.025080 acct-8.5.2/acct.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-15 23:52:07.000000 acct-8.5.2/acct.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      255 2023-02-15 23:51:52.000000 acct-8.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 23:52:08.026079 acct-8.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2750 2023-02-15 23:51:52.000000 acct-8.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-06-22 15:33:15.000000 acct-8.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-06-22 15:33:28.880938 acct-8.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-22 15:33:15.000000 acct-8.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/backend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/backend/contracts/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/backend/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/backend/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/contracts/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/acct/metadata/contracts/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/metadata/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-22 15:33:15.000000 acct-8.6.0/acct/acct/metadata/init.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-06-22 15:33:15.000000 acct-8.6.0/acct/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/crypto/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-22 15:33:15.000000 acct-8.6.0/acct/crypto/aesgcm256.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct/crypto/contracts/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-22 15:33:15.000000 acct-8.6.0/acct/crypto/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-22 15:33:15.000000 acct-8.6.0/acct/crypto/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-06-22 15:33:15.000000 acct-8.6.0/acct/crypto/init.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-22 15:33:15.000000 acct-8.6.0/acct/scripts.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-22 15:33:28.000000 acct-8.6.0/acct/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:33:28.880938 acct-8.6.0/acct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 15:33:28.000000 acct-8.6.0/acct.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-22 15:33:15.000000 acct-8.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:33:28.880938 acct-8.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2801 2023-06-22 15:33:15.000000 acct-8.6.0/setup.py
```

### Comparing `acct-8.5.2/LICENSE` & `acct-8.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/PKG-INFO` & `acct-8.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: acct
-Version: 8.5.2
+Version: 8.6.0
 Summary: Simple, secure, account and credential management
 Home-page: https://saltstack.com
 Author: Thomas S Hatch
 Author-email: thatch@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====
 acct
```

### Comparing `acct-8.5.2/README.rst` & `acct-8.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/acct/backend/init.py` & `acct-8.6.0/acct/acct/backend/init.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/acct/init.py` & `acct-8.6.0/acct/acct/init.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/acct/metadata/init.py` & `acct-8.6.0/acct/acct/metadata/init.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/conf.py` & `acct-8.6.0/acct/conf.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/crypto/aesgcm256.py` & `acct-8.6.0/acct/crypto/aesgcm256.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct/crypto/init.py` & `acct-8.6.0/acct/crypto/init.py`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/acct.egg-info/PKG-INFO` & `acct-8.6.0/acct.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: acct
-Version: 8.5.2
+Version: 8.6.0
 Summary: Simple, secure, account and credential management
 Home-page: https://saltstack.com
 Author: Thomas S Hatch
 Author-email: thatch@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====
 acct
```

### Comparing `acct-8.5.2/acct.egg-info/SOURCES.txt` & `acct-8.6.0/acct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acct-8.5.2/setup.py` & `acct-8.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,18 @@
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
     python_requires=">=3.6",
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={
         "console_scripts": [
             "acct = acct.scripts:start",
         ],
```

