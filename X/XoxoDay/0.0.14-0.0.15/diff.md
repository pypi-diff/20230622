# Comparing `tmp/XoxoDay-0.0.14.tar.gz` & `tmp/XoxoDay-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.14.tar", last modified: Thu Jun 15 18:04:04 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.15.tar", last modified: Thu Jun 22 09:49:28 2023, max compression
```

## Comparing `XoxoDay-0.0.14.tar` & `XoxoDay-0.0.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-15 18:04:04.234079 XoxoDay-0.0.14/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.14/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-15 18:04:04.233924 XoxoDay-0.0.14/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.14/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-15 18:04:04.230784 XoxoDay-0.0.14/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-15 18:03:54.000000 XoxoDay-0.0.14/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.14/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-15 18:04:04.232142 XoxoDay-0.0.14/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.14/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.14/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.14/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.14/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-15 18:04:04.233565 XoxoDay-0.0.14/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.14/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.14/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.14/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1850 2023-06-15 17:52:44.000000 XoxoDay-0.0.14/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.14/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4588 2023-06-15 17:58:41.000000 XoxoDay-0.0.14/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-15 18:04:04.231561 XoxoDay-0.0.14/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-15 18:04:04.000000 XoxoDay-0.0.14/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-15 18:04:04.000000 XoxoDay-0.0.14/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-15 18:04:04.000000 XoxoDay-0.0.14/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-15 18:04:04.000000 XoxoDay-0.0.14/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-15 18:04:04.000000 XoxoDay-0.0.14/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-15 18:04:04.234129 XoxoDay-0.0.14/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-15 18:03:51.000000 XoxoDay-0.0.14/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.676327 XoxoDay-0.0.15/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.15/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 09:49:28.676194 XoxoDay-0.0.15/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.15/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.673283 XoxoDay-0.0.15/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-22 09:49:17.000000 XoxoDay-0.0.15/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.15/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.674525 XoxoDay-0.0.15/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.15/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.15/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.15/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.15/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.675862 XoxoDay-0.0.15/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.15/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.15/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.15/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1850 2023-06-15 17:52:44.000000 XoxoDay-0.0.15/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.15/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.15/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.674052 XoxoDay-0.0.15/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-22 09:49:28.676368 XoxoDay-0.0.15/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-22 09:49:08.000000 XoxoDay-0.0.15/setup.py
```

### Comparing `XoxoDay-0.0.14/LICENSE` & `XoxoDay-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/PKG-INFO` & `XoxoDay-0.0.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.14
+Version: 0.0.15
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.14/README.md` & `XoxoDay-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/XoxoDay/exception.py` & `XoxoDay-0.0.15/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/XoxoDay/helper/token.py` & `XoxoDay-0.0.15/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/XoxoDay/service/http_service.py` & `XoxoDay-0.0.15/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/XoxoDay/service/token_service.py` & `XoxoDay-0.0.15/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.14/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.15/XoxoDay/service/xoxoday_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         api_url = self.API_DEV_URL if self.environment == 'dev' else self.API_PROD_URL
         payload = {
             "grant_type": kwargs.get('grant_type', 'refresh_token'),
             "refresh_token": self.refresh_token,
             "client_id": self.client_id,
             "client_secret": self.client_secret
         }
-        super().__init__(api_url, **payload)
+        super().__init__(api_url, self.access_token, **payload)
         token = self.token_dict['access_token']
         self.headers = {
             'Authorization': f'Bearer {token}',
             'content-type': 'application/json',
             'accept': 'application/json'
         }
```

### Comparing `XoxoDay-0.0.14/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.15/XoxoDay.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.14
+Version: 0.0.15
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.14/setup.py` & `XoxoDay-0.0.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.14",
+    version="0.0.15",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

