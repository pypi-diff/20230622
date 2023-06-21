# Comparing `tmp/pymongocrypt-1.6.0.tar.gz` & `tmp/pymongocrypt-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongocrypt-1.6.0.tar", last modified: Wed May 10 18:44:23 2023, max compression
+gzip compressed data, was "pymongocrypt-1.6.1.tar", last modified: Wed Jun 21 21:23:53 2023, max compression
```

## Comparing `pymongocrypt-1.6.0.tar` & `pymongocrypt-1.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.959134 pymongocrypt-1.6.0/
--rw-r--r--   0 mci        (500) admin       (80)    11357 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/LICENSE
--rw-r--r--   0 mci        (500) admin       (80)     8580 2023-05-10 18:44:23.958857 pymongocrypt-1.6.0/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)     7362 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/README.rst
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.956191 pymongocrypt-1.6.0/pymongocrypt/
--rw-r--r--   0 mci        (500) admin       (80)      687 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/__init__.py
--rw-r--r--   0 mci        (500) admin       (80)     2053 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/auto_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)     3156 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/binary.py
--rw-r--r--   0 mci        (500) admin       (80)    55615 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/binding.py
--rw-r--r--   0 mci        (500) admin       (80)     1027 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/compat.py
--rw-r--r--   0 mci        (500) admin       (80)     5119 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/credentials.py
--rw-r--r--   0 mci        (500) admin       (80)     6157 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/crypto.py
--rw-r--r--   0 mci        (500) admin       (80)     1393 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/errors.py
--rw-r--r--   0 mci        (500) admin       (80)    11125 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/explicit_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)    32003 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/mongocrypt.py
--rw-r--r--   0 mci        (500) admin       (80)     4850 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/state_machine.py
--rw-r--r--   0 mci        (500) admin       (80)      642 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/version.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.957777 pymongocrypt-1.6.0/pymongocrypt.egg-info/
--rw-r--r--   0 mci        (500) admin       (80)     8580 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)      622 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/SOURCES.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/dependency_links.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/not-zip-safe
--rw-r--r--   0 mci        (500) admin       (80)      148 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/requires.txt
--rw-r--r--   0 mci        (500) admin       (80)       13 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/top_level.txt
--rw-r--r--   0 mci        (500) admin       (80)       38 2023-05-10 18:44:23.959192 pymongocrypt-1.6.0/setup.cfg
--rw-r--r--   0 mci        (500) admin       (80)     3439 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/setup.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.958539 pymongocrypt-1.6.0/test/
--rw-r--r--   0 mci        (500) admin       (80)     2398 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_binding.py
--rw-r--r--   0 mci        (500) admin       (80)     3479 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_crypto.py
--rw-r--r--   0 mci        (500) admin       (80)    35736 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_mongocrypt.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-06-21 21:23:53.997512 pymongocrypt-1.6.1/
+-rw-r--r--   0 mci        (500) admin       (80)    11357 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/LICENSE
+-rw-r--r--   0 mci        (500) admin       (80)     8580 2023-06-21 21:23:53.997290 pymongocrypt-1.6.1/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)     7362 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/README.rst
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-06-21 21:23:53.995082 pymongocrypt-1.6.1/pymongocrypt/
+-rw-r--r--   0 mci        (500) admin       (80)      687 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/__init__.py
+-rw-r--r--   0 mci        (500) admin       (80)     2053 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/auto_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)     3156 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/binary.py
+-rw-r--r--   0 mci        (500) admin       (80)    55615 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     1027 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/compat.py
+-rw-r--r--   0 mci        (500) admin       (80)     5119 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/credentials.py
+-rw-r--r--   0 mci        (500) admin       (80)     6157 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)     1393 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/errors.py
+-rw-r--r--   0 mci        (500) admin       (80)    11125 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/explicit_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)    32003 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/mongocrypt.py
+-rw-r--r--   0 mci        (500) admin       (80)     4850 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/state_machine.py
+-rw-r--r--   0 mci        (500) admin       (80)      642 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/pymongocrypt/version.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-06-21 21:23:53.996348 pymongocrypt-1.6.1/pymongocrypt.egg-info/
+-rw-r--r--   0 mci        (500) admin       (80)     8580 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)      622 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/not-zip-safe
+-rw-r--r--   0 mci        (500) admin       (80)      148 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/requires.txt
+-rw-r--r--   0 mci        (500) admin       (80)       13 2023-06-21 21:23:53.000000 pymongocrypt-1.6.1/pymongocrypt.egg-info/top_level.txt
+-rw-r--r--   0 mci        (500) admin       (80)       38 2023-06-21 21:23:53.997565 pymongocrypt-1.6.1/setup.cfg
+-rw-r--r--   0 mci        (500) admin       (80)     3439 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/setup.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-06-21 21:23:53.996987 pymongocrypt-1.6.1/test/
+-rw-r--r--   0 mci        (500) admin       (80)     2398 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/test/test_binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     3479 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/test/test_crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)    35736 2023-06-21 21:23:50.000000 pymongocrypt-1.6.1/test/test_mongocrypt.py
```

### Comparing `pymongocrypt-1.6.0/LICENSE` & `pymongocrypt-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/PKG-INFO` & `pymongocrypt-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymongocrypt-1.6.0/README.rst` & `pymongocrypt-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/__init__.py` & `pymongocrypt-1.6.1/pymongocrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/auto_encrypter.py` & `pymongocrypt-1.6.1/pymongocrypt/auto_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/binary.py` & `pymongocrypt-1.6.1/pymongocrypt/binary.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/binding.py` & `pymongocrypt-1.6.1/pymongocrypt/binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/compat.py` & `pymongocrypt-1.6.1/pymongocrypt/compat.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/credentials.py` & `pymongocrypt-1.6.1/pymongocrypt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/crypto.py` & `pymongocrypt-1.6.1/pymongocrypt/crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/errors.py` & `pymongocrypt-1.6.1/pymongocrypt/errors.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/explicit_encrypter.py` & `pymongocrypt-1.6.1/pymongocrypt/explicit_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/mongocrypt.py` & `pymongocrypt-1.6.1/pymongocrypt/mongocrypt.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/state_machine.py` & `pymongocrypt-1.6.1/pymongocrypt/state_machine.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/pymongocrypt/version.py` & `pymongocrypt-1.6.1/pymongocrypt/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 
 _MIN_LIBMONGOCRYPT_VERSION = '1.8.0'
```

### Comparing `pymongocrypt-1.6.0/pymongocrypt.egg-info/PKG-INFO` & `pymongocrypt-1.6.1/pymongocrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymongocrypt-1.6.0/pymongocrypt.egg-info/SOURCES.txt` & `pymongocrypt-1.6.1/pymongocrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/setup.py` & `pymongocrypt-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/test/test_binding.py` & `pymongocrypt-1.6.1/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/test/test_crypto.py` & `pymongocrypt-1.6.1/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.6.0/test/test_mongocrypt.py` & `pymongocrypt-1.6.1/test/test_mongocrypt.py`

 * *Files identical despite different names*

