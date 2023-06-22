# Comparing `tmp/scrappeycom-0.3.7.tar.gz` & `tmp/scrappeycom-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.7.tar", last modified: Thu Jun 22 08:37:27 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.8.tar", last modified: Thu Jun 22 10:55:40 2023, max compression
```

## Comparing `scrappeycom-0.3.7.tar` & `scrappeycom-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.868874 scrappeycom-0.3.7/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0     7511 2023-06-22 08:37:27.869874 scrappeycom-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     6356 2023-06-22 08:37:06.000000 scrappeycom-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.852874 scrappeycom-0.3.7/scrappeycom/
--rw-rw-rw-   0        0        0     1346 2023-06-22 08:26:36.000000 scrappeycom-0.3.7/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0     1910 2023-06-22 08:36:48.000000 scrappeycom-0.3.7/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.867873 scrappeycom-0.3.7/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     7511 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 08:37:27.870873 scrappeycom-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-22 08:37:23.000000 scrappeycom-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:55:40.920463 scrappeycom-0.3.8/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     7395 2023-06-22 10:55:40.920463 scrappeycom-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6240 2023-06-22 10:53:54.000000 scrappeycom-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 10:55:40.892463 scrappeycom-0.3.8/scrappeycom/
+-rw-rw-rw-   0        0        0     1719 2023-06-22 10:53:19.000000 scrappeycom-0.3.8/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0     1833 2023-06-22 10:54:30.000000 scrappeycom-0.3.8/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:55:40.919462 scrappeycom-0.3.8/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     7395 2023-06-22 10:55:40.000000 scrappeycom-0.3.8/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-22 10:55:40.000000 scrappeycom-0.3.8/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:55:40.000000 scrappeycom-0.3.8/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 10:55:40.000000 scrappeycom-0.3.8/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 10:55:40.000000 scrappeycom-0.3.8/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 10:55:40.925461 scrappeycom-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-22 10:55:38.000000 scrappeycom-0.3.8/setup.py
```

### Comparing `scrappeycom-0.3.7/LICENSE.txt` & `scrappeycom-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.7/PKG-INFO` & `scrappeycom-0.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.7
+Version: 0.3.8
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
@@ -81,31 +81,28 @@
         # Just copy paste it below, example
         #
         #    {
         #       "cmd":  "request.get",
         #       "url":  "https://httpbin.rs/get"
         #    }
 
-        get_request_result = scrappey.request({
-            "cmd":  "request.get",
+        get_request_result = scrappey.get({
             'session': session['session'],
             'url': 'https://httpbin.rs/get',
         })
         print('GET Request Result:', get_request_result)
 
-        post_request_result = scrappey.request({
-            "cmd": "request.post",
+        post_request_result = scrappey.post({
             "url": "https://httpbin.rs/post",
             "postData": "test=test&test2=test2"
         })
         print('POST Request Result:', post_request_result)
 
         # JSON request example
-        post_request_result_json = scrappey.request({
-            "cmd": "request.post",
+        post_request_result_json = scrappey.post({
             "url": "https://backend.scrappey.com/api/auth/login",
             "postData": "{\"email\":\"email\",\"password\":\"password\"}",
             "customHeaders": {
                 "content-type": "application/json"
             }
         })
         print('POST Request Result:', post_request_result_json)
@@ -113,14 +110,15 @@
         sessionDestroyed = scrappey.destroy_session(sessionData)
         print('Session destroyed:', sessionDestroyed)
     except Exception as error:
         print(error)
 
 run_test()
 
+
 ```
 
 For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). ðŸ“š
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `scrappeycom-0.3.7/README.md` & `scrappeycom-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,31 +60,28 @@
         # Just copy paste it below, example
         #
         #    {
         #       "cmd":  "request.get",
         #       "url":  "https://httpbin.rs/get"
         #    }
 
-        get_request_result = scrappey.request({
-            "cmd":  "request.get",
+        get_request_result = scrappey.get({
             'session': session['session'],
             'url': 'https://httpbin.rs/get',
         })
         print('GET Request Result:', get_request_result)
 
-        post_request_result = scrappey.request({
-            "cmd": "request.post",
+        post_request_result = scrappey.post({
             "url": "https://httpbin.rs/post",
             "postData": "test=test&test2=test2"
         })
         print('POST Request Result:', post_request_result)
 
         # JSON request example
-        post_request_result_json = scrappey.request({
-            "cmd": "request.post",
+        post_request_result_json = scrappey.post({
             "url": "https://backend.scrappey.com/api/auth/login",
             "postData": "{\"email\":\"email\",\"password\":\"password\"}",
             "customHeaders": {
                 "content-type": "application/json"
             }
         })
         print('POST Request Result:', post_request_result_json)
@@ -92,14 +89,15 @@
         sessionDestroyed = scrappey.destroy_session(sessionData)
         print('Session destroyed:', sessionDestroyed)
     except Exception as error:
         print(error)
 
 run_test()
 
+
 ```
 
 For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). 📚
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `scrappeycom-0.3.7/scrappeycom/scrappey.py` & `scrappeycom-0.3.8/scrappeycom/scrappey.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,26 @@
         return self.send_request(endpoint='sessions.create', data=data)
 
     def destroy_session(self, session):
         if session is None:
             raise ValueError('session parameter is required.')
         return self.send_request(endpoint='sessions.destroy', data={'session': session})
 
+    def post(self,data):
+        if data is None:
+            raise ValueError('data parameter is required.')
+
+        return self.send_request(endpoint='request.post', data=data)
+
+    def get(self, data):
+        if data is None:
+            raise ValueError('data parameter is required.')
+
+        return self.send_request(endpoint='request.get', data=data)
+
     def request(self, data):
         if data is None:
             raise ValueError('data parameter is required.')
         
         if data['cmd'] is None:
             raise ValueError('data.cmd parameter is required.')
```

### Comparing `scrappeycom-0.3.7/scrappeycom/test.py` & `scrappeycom-0.3.8/scrappeycom/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from scrappeycom.scrappey import Scrappey
+from scrappey import Scrappey
 import uuid
 
-scrappey = Scrappey('API_KEY')
+scrappey = Scrappey('vQYlEMNSNgA3tNuXy75iFxlVojaKLgNzFtiJnKBKIIeTVfVODC3RpQVYZXPG')
 
 def run_test():
     try:
         sessionData = {
             'session': str(uuid.uuid4()), #uuid is also optional, otherwise default uuid will be used
             #'proxy': 'http://username:password@ip:port' #proxy is optional, otherwise default proxy will be used
         }
@@ -17,31 +17,28 @@
         # Just copy paste it below, example
         #
         #    {
         #       "cmd":  "request.get",
         #       "url":  "https://httpbin.rs/get"
         #    }
 
-        get_request_result = scrappey.request({
-            "cmd":  "request.get",
+        get_request_result = scrappey.get({
             'session': session['session'],
             'url': 'https://httpbin.rs/get',
         })
         print('GET Request Result:', get_request_result)
 
-        post_request_result = scrappey.request({
-            "cmd": "request.post",
+        post_request_result = scrappey.post({
             "url": "https://httpbin.rs/post",
             "postData": "test=test&test2=test2"
         })
         print('POST Request Result:', post_request_result)
 
         # JSON request example
-        post_request_result_json = scrappey.request({
-            "cmd": "request.post",
+        post_request_result_json = scrappey.post({
             "url": "https://backend.scrappey.com/api/auth/login",
             "postData": "{\"email\":\"email\",\"password\":\"password\"}",
             "customHeaders": {
                 "content-type": "application/json"
             }
         })
         print('POST Request Result:', post_request_result_json)
```

### Comparing `scrappeycom-0.3.7/scrappeycom.egg-info/PKG-INFO` & `scrappeycom-0.3.8/scrappeycom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.7
+Version: 0.3.8
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
@@ -81,31 +81,28 @@
         # Just copy paste it below, example
         #
         #    {
         #       "cmd":  "request.get",
         #       "url":  "https://httpbin.rs/get"
         #    }
 
-        get_request_result = scrappey.request({
-            "cmd":  "request.get",
+        get_request_result = scrappey.get({
             'session': session['session'],
             'url': 'https://httpbin.rs/get',
         })
         print('GET Request Result:', get_request_result)
 
-        post_request_result = scrappey.request({
-            "cmd": "request.post",
+        post_request_result = scrappey.post({
             "url": "https://httpbin.rs/post",
             "postData": "test=test&test2=test2"
         })
         print('POST Request Result:', post_request_result)
 
         # JSON request example
-        post_request_result_json = scrappey.request({
-            "cmd": "request.post",
+        post_request_result_json = scrappey.post({
             "url": "https://backend.scrappey.com/api/auth/login",
             "postData": "{\"email\":\"email\",\"password\":\"password\"}",
             "customHeaders": {
                 "content-type": "application/json"
             }
         })
         print('POST Request Result:', post_request_result_json)
@@ -113,14 +110,15 @@
         sessionDestroyed = scrappey.destroy_session(sessionData)
         print('Session destroyed:', sessionDestroyed)
     except Exception as error:
         print(error)
 
 run_test()
 
+
 ```
 
 For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). ðŸ“š
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `scrappeycom-0.3.7/setup.py` & `scrappeycom-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3.7',      # Start with a small number and increase it with every change you make
+  version = '0.3.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
```

