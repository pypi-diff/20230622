# Comparing `tmp/scrapy-manipulate-request-0.0.1.tar.gz` & `tmp/scrapy-manipulate-request-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-manipulate-request-0.0.1.tar", last modified: Wed Jun 21 14:57:37 2023, max compression
+gzip compressed data, was "scrapy-manipulate-request-0.0.2.tar", last modified: Wed Jun 21 23:27:03 2023, max compression
```

## Comparing `scrapy-manipulate-request-0.0.1.tar` & `scrapy-manipulate-request-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:57:37.146624 scrapy-manipulate-request-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6564 2023-06-21 14:57:37.145624 scrapy-manipulate-request-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5488 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 14:57:37.143194 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/
--rw-rw-rw-   0        0        0       72 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/__init__.py
--rw-rw-rw-   0        0        0      411 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/__version__.py
--rw-rw-rw-   0        0        0     5205 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/downloadermiddlewares.py
--rw-rw-rw-   0        0        0       39 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/exception.py
--rw-rw-rw-   0        0        0        8 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:57:37.145624 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/
--rw-rw-rw-   0        0        0     6564 2023-06-21 14:57:37.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-06-21 14:57:37.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:57:37.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 14:57:37.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-21 14:57:37.000000 scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 14:57:37.146624 scrapy-manipulate-request-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1744 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:57:37.145624 scrapy-manipulate-request-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      384 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6564 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5488 2023-06-21 22:52:14.000000 scrapy-manipulate-request-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/
+-rw-rw-rw-   0        0        0       72 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-06-21 23:25:40.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/__version__.py
+-rw-rw-rw-   0        0        0     5207 2023-06-21 23:16:41.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/downloadermiddlewares.py
+-rw-rw-rw-   0        0        0       39 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/exception.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/
+-rw-rw-rw-   0        0        0     6564 2023-06-21 23:27:03.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-21 23:27:03.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 23:27:03.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 23:27:03.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-21 23:27:03.000000 scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:27:03.667909 scrapy-manipulate-request-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      384 2023-06-21 14:56:07.000000 scrapy-manipulate-request-0.0.2/tests/test.py
```

### Comparing `scrapy-manipulate-request-0.0.1/LICENSE` & `scrapy-manipulate-request-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-manipulate-request-0.0.1/PKG-INFO` & `scrapy-manipulate-request-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-manipulate-request
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async scrapy request downloader middleware, support random request and response manipulation.
 Home-page: https://github.com/dylankeepon/ScrapyManipulateRequestMiddleware
 Author: Dylan Chen
 Author-email: dylankeep@163.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -63,15 +63,15 @@
 ```python
 import scrapy
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
     
         # return None, the requesst will be ignored
         # return scrapy.http.HtmlResponse or scrapy.http.TextResponse object,
         # the process of handle response will be started.
@@ -90,15 +90,15 @@
 import tls_client
 from scrapy.http import TextResponse
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         url = request.url
         headers = request.headers.to_unicode_dict()
         tls_session = tls_client.Session(
             client_identifier='chrome_112',
@@ -128,15 +128,15 @@
 from scrapy.http import HtmlResponse
 from seleniumwire import undetected_chromedriver as uc
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         chrome_options = uc.ChromeOptions()
         chrome_options.add_experimental_option()
         chrome_options.add_argument()
         chrome_options.add_extension()
```

### Comparing `scrapy-manipulate-request-0.0.1/README.md` & `scrapy-manipulate-request-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ```python
 import scrapy
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
     
         # return None, the requesst will be ignored
         # return scrapy.http.HtmlResponse or scrapy.http.TextResponse object,
         # the process of handle response will be started.
@@ -65,15 +65,15 @@
 import tls_client
 from scrapy.http import TextResponse
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         url = request.url
         headers = request.headers.to_unicode_dict()
         tls_session = tls_client.Session(
             client_identifier='chrome_112',
@@ -103,15 +103,15 @@
 from scrapy.http import HtmlResponse
 from seleniumwire import undetected_chromedriver as uc
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         chrome_options = uc.ChromeOptions()
         chrome_options.add_experimental_option()
         chrome_options.add_argument()
         chrome_options.add_extension()
```

### Comparing `scrapy-manipulate-request-0.0.1/scrapy_manipulate_request/downloadermiddlewares.py` & `scrapy-manipulate-request-0.0.2/scrapy_manipulate_request/downloadermiddlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,17 @@
             raise TypeError(f'manipulate_request should be a function, but {type(request)} received')
         try:
             response = manipulate_request(request, spider)
         except Exception as e:
             return None
         if response is None:
             raise IgnoreRequest
-        if not isinstance(response, HtmlResponse) or not isinstance(response, TextResponse):
+        if not isinstance(response, HtmlResponse) and not isinstance(response, TextResponse):
             raise TypeError(f'response should be a HtmlResponse or TextResponse object,\
-                                    but {type(request)} received')
+                                    but {type(response)} received')
         return response
 
     def process_request(self, request, spider):
         logger.debug('manipulate_process function process request %s', request)
         return deferToThread(self._process_request, request, spider)
 
     def process_response(self, request, response, spider):
```

### Comparing `scrapy-manipulate-request-0.0.1/scrapy_manipulate_request.egg-info/PKG-INFO` & `scrapy-manipulate-request-0.0.2/scrapy_manipulate_request.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-manipulate-request
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async scrapy request downloader middleware, support random request and response manipulation.
 Home-page: https://github.com/dylankeepon/ScrapyManipulateRequestMiddleware
 Author: Dylan Chen
 Author-email: dylankeep@163.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -63,15 +63,15 @@
 ```python
 import scrapy
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
     
         # return None, the requesst will be ignored
         # return scrapy.http.HtmlResponse or scrapy.http.TextResponse object,
         # the process of handle response will be started.
@@ -90,15 +90,15 @@
 import tls_client
 from scrapy.http import TextResponse
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         url = request.url
         headers = request.headers.to_unicode_dict()
         tls_session = tls_client.Session(
             client_identifier='chrome_112',
@@ -128,15 +128,15 @@
 from scrapy.http import HtmlResponse
 from seleniumwire import undetected_chromedriver as uc
 
 class TestSpider(scrapy.Spider):
     name = "test"
 
     def start_requests(self,):
-        meta_data = {'manipulate_request', self.manipulate_request}
+        meta_data = {'manipulate_request': self.manipulate_request}
         yield scrapy.Request(url="https://tls.browserleaks.com/json", meta=meta_data)
     
     def manipulate_request(self, request, spider):
         chrome_options = uc.ChromeOptions()
         chrome_options.add_experimental_option()
         chrome_options.add_argument()
         chrome_options.add_extension()
```

### Comparing `scrapy-manipulate-request-0.0.1/setup.py` & `scrapy-manipulate-request-0.0.2/setup.py`

 * *Files identical despite different names*

