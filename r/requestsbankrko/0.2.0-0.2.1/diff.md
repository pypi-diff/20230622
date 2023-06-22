# Comparing `tmp/requestsbankrko-0.2.0.tar.gz` & `tmp/requestsbankrko-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.0.tar", last modified: Thu May  4 09:22:58 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.1.tar", last modified: Thu Jun 22 14:41:56 2023, max compression
```

## Comparing `requestsbankrko-0.2.0.tar` & `requestsbankrko-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:22:58.937464 requestsbankrko-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 09:22:58.937464 requestsbankrko-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:22:58.937464 requestsbankrko-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:22:58.933463 requestsbankrko-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:22:58.937464 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 09:22:58.000000 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 09:22:58.000000 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:22:58.000000 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 09:22:58.000000 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 09:22:58.000000 requestsbankrko-0.2.0/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:22:58.937464 requestsbankrko-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    51653 2023-05-04 09:22:34.000000 requestsbankrko-0.2.0/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.0/LICENSE` & `requestsbankrko-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.0/PKG-INFO` & `requestsbankrko-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.0
+Version: 0.2.1
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.0/pyproject.toml` & `requestsbankrko-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.0"
+version = "0.2.1"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.0/src/bank_methods.py` & `requestsbankrko-0.2.1/src/bank_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -813,7 +813,32 @@
 
         elif 'errors' in self.response_json:
             if 'message' in self.response_json['errors']:
                 if self.response_json['errors']['message'] == 'inn: В системе найден дубликат.':
                     self.success = True
                     return inn_busy
 
+class RosBankLead(RequestsGarant):
+    def __init__(self, json):
+        super().__init__()
+        self.url = 'https://api.rosbank.ru/private-person/agent-pro-request/request/index'
+        self.method = 'post'
+        self.json = json
+        self.headers = {
+            'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36',
+            'Referer': "https://www.rosbank.ru/",
+            'Accept': 'application/json, text/plain, */*',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Language': 'ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,es;q=0.6,ja;q=0.5',
+            'Content-Type': "application/json;",
+            'Origin': "https://www.rosbank.ru",
+            'Sec-Fetch-Dest': "empty",
+            'Sec-Fetch-Mode': "cors",
+            'Sec-Fetch-Site': "same-site",
+
+        }
+
+    def do_json(self):
+        if 'success' in self.response_json:
+            if 'id' in self.response_json:
+                self.success = True
+                return self.response_json['id']
```

### Comparing `requestsbankrko-0.2.0/src/open_methods.py` & `requestsbankrko-0.2.1/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.0/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.1/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.0
+Version: 0.2.1
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.0/src/zip_functions.py` & `requestsbankrko-0.2.1/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.0/tests/test_bank_methods.py` & `requestsbankrko-0.2.1/tests/test_bank_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1236,8 +1236,31 @@
         def f(*args):
             print(args)
 
         args = ()
         f(*args)
 
 
+class RosBankLeadTestCase(TestCase):
+    def test_test(self):
+        json = {
+            'inn': '7751252660',
+            'contact_comment': 'тест',
+            'contact_name': 'ТЕСТОВА ТЕСТА ТЕСТОВНА',
+            'phone': '+79167819499',
+            'is_registered_inn': True,
+            'is_accept_info': True,
+            'mgm_code': 'K10X5D1',
+            # 'webmaster_id': '',
+            'region_code': '77',
+            'google_id': '777.777',
+        }
+        obj = RosBankLead(json)
+        obj.get_rezult()
+        print(obj.response.request.headers)
+        print(obj.response.text)
+        print(obj.response.content)
+        print(obj.response.json())
+#         {"success":true,"id":2192696}
+
+
```

