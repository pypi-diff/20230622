# Comparing `tmp/scrappeycom-0.3.5.tar.gz` & `tmp/scrappeycom-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.5.tar", last modified: Thu Jun 22 08:31:55 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.6.tar", last modified: Thu Jun 22 08:32:44 2023, max compression
```

## Comparing `scrappeycom-0.3.5.tar` & `scrappeycom-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:31:55.741181 scrappeycom-0.3.5/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0     6333 2023-06-22 08:31:55.741181 scrappeycom-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 08:31:55.719180 scrappeycom-0.3.5/scrappeycom/
--rw-rw-rw-   0        0        0     1346 2023-06-22 08:26:36.000000 scrappeycom-0.3.5/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0     1898 2023-06-22 08:30:49.000000 scrappeycom-0.3.5/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:31:55.740179 scrappeycom-0.3.5/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     6333 2023-06-22 08:31:55.000000 scrappeycom-0.3.5/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-22 08:31:55.000000 scrappeycom-0.3.5/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:31:55.000000 scrappeycom-0.3.5/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 08:31:55.000000 scrappeycom-0.3.5/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 08:31:55.000000 scrappeycom-0.3.5/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 08:31:55.746184 scrappeycom-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-22 08:31:25.000000 scrappeycom-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.925320 scrappeycom-0.3.6/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     7499 2023-06-22 08:32:44.925320 scrappeycom-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6344 2023-06-22 08:32:33.000000 scrappeycom-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.907321 scrappeycom-0.3.6/scrappeycom/
+-rw-rw-rw-   0        0        0     1346 2023-06-22 08:26:36.000000 scrappeycom-0.3.6/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0     1898 2023-06-22 08:30:49.000000 scrappeycom-0.3.6/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.923320 scrappeycom-0.3.6/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     7499 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 08:32:44.927319 scrappeycom-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-22 08:32:40.000000 scrappeycom-0.3.6/setup.py
```

### Comparing `scrappeycom-0.3.5/LICENSE.txt` & `scrappeycom-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.5/PKG-INFO` & `scrappeycom-0.3.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,99 +1,111 @@
-Metadata-Version: 2.1
-Name: scrappeycom
-Version: 0.3.5
-Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
-Home-page: https://github.com/pim97/scrappey-wrapper-python
-Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
-Author: dormic97
-Author-email: crozz-boy@hotmail.com
-License: MIT
-Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# 🤖 Scrappey Wrapper - Data Extraction Made Easy
 
-# ðŸ¤– Scrappey Wrapper - Data Extraction Made Easy
-
-Introducing Scrappey, your comprehensive website scraping solution provided by Scrappey.com. With Scrappey's powerful and user-friendly API, you can effortlessly retrieve data from websites, including those protected by Cloudflare. Join Scrappey today and revolutionize your data extraction process. ðŸš€
+Introducing Scrappey, your comprehensive website scraping solution provided by Scrappey.com. With Scrappey's powerful and user-friendly API, you can effortlessly retrieve data from websites, including those protected by Cloudflare. Join Scrappey today and revolutionize your data extraction process. 🚀
 
 **Disclaimer: Please ensure that your web scraping activities comply with the website's terms of service and legal regulations. Scrappey is not responsible for any misuse or unethical use of the library. Use it responsibly and respect the website's policies.**
 
 Website: https://scrappey.com/
 
 ## Topics
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Example](#example)
 - [License](#license)
 
 ## Installation
 
-Use pip to install the Scrappey library. ðŸ’»
+Use pip to install the Scrappey library. 💻
 
 ```shell
 pip install scrappeycom
 ```
 
 ## Usage
 
-Import the Scrappey library in your code. ðŸ“¦
+Import the Scrappey library in your code. 📦
 
 ```python
 from scrappeycom.scrappey import Scrappey
 ```
 
-Create an instance of Scrappey by providing your Scrappey API key. ðŸ”‘
+Create an instance of Scrappey by providing your Scrappey API key. 🔑
 
 ```python
 api_key = 'YOUR_API_KEY'
 scrappey_instance = scrappey.Scrappey(api_key)
 ```
 
 ### Example
 
-Here's an example of how to use Scrappey. ðŸš€
+Here's an example of how to use Scrappey. 🚀
 
 ```python
-from scrappeycom.scrappey import Scrappey
+from scrappey import Scrappey
+import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
-        session = scrappey.create_session()
-        print(session)
-
-        get_request_result = scrappey.get_request('https://httpbin.rs/get', session['session'])
+        sessionData = {
+            'session': str(uuid.uuid4()), #uuid is also optional, otherwise default uuid will be used
+            #'proxy': 'http://username:password@ip:port' #proxy is optional, otherwise default proxy will be used
+        }
+        session = scrappey.create_session(sessionData)
+        print('Session created:', session['session'])
+
+        # View all the options here with the request builder
+        # https://app.scrappey.com/#/builder
+        # Just copy paste it below, example
+        #
+        #    {
+        #       "cmd":  "request.get",
+        #       "url":  "https://httpbin.rs/get"
+        #    }
+
+        get_request_result = scrappey.request({
+            "cmd":  "request.get",
+            'session': session['session'],
+            'url': 'https://httpbin.rs/get',
+        })
         print('GET Request Result:', get_request_result)
 
-        post_data = {'username': 'user123', 'password': 'pass456'}
-        post_request_result = scrappey.post_request('https://httpbin.rs/post', post_data, session['session'])
+        post_request_result = scrappey.request({
+            "cmd": "request.post",
+            "url": "https://httpbin.rs/post",
+            "postData": "test=test&test2=test2"
+        })
         print('POST Request Result:', post_request_result)
 
-        scrappey.destroy_session(session['session'])
-        print('Session destroyed.')
+        # JSON request example
+        post_request_result_json = scrappey.request({
+            "cmd": "request.post",
+            "url": "https://backend.scrappey.com/api/auth/login",
+            "postData": "{\"email\":\"email\",\"password\":\"password\"}",
+            "customHeaders": {
+                "content-type": "application/json"
+            }
+        })
+        print('POST Request Result:', post_request_result_json)
+
+        sessionDestroyed = scrappey.destroy_session(sessionData)
+        print('Session destroyed:', sessionDestroyed)
     except Exception as error:
         print(error)
 
 run_test()
+
 ```
 
-For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). ðŸ“š
+For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). 📚
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Additional Tags
 
 cloudflare anti bot bypass, cloudflare solver, scraper, scraping, cloudflare scraper, cloudflare turnstile solver, turnstile solver, data extraction, web scraping, website scraping, data scraping, scraping tool, API scraping, scraping solution, web data extraction, website data extraction, web scraping library, website scraping library, cloudflare bypass, scraping API, web scraping API, cloudflare protection, data scraping tool, scraping service, cloudflare challenge solver, web scraping solution, web scraping service, cloudflare scraping, cloudflare bot protection, scraping framework, scraping library, cloudflare bypass tool, cloudflare anti-bot, cloudflare protection bypass, cloudflare solver tool, web scraping tool, data extraction library, website scraping tool, cloudflare turnstile bypass, cloudflare anti-bot solver, turnstile solver tool, cloudflare scraping solution, website data scraper, cloudflare challenge bypass, web scraping framework, cloudflare challenge solver tool, web data scraping, data scraper, scraping data from websites, SEO, data mining,
 
- data harvesting, data crawling, web scraping software, website scraping tool, web scraping framework, data extraction tool, web data scraper, data scraping service, scraping automation, scraping tutorial, scraping code, scraping techniques, scraping best practices, scraping scripts, scraping tutorial, scraping examples, scraping challenges, scraping tricks, scraping tips, scraping tricks, scraping strategies, scraping methods, cloudflare protection bypass, cloudflare security bypass, web scraping Python, web scraping JavaScript, web scraping PHP, web scraping Ruby, web scraping Java, web scraping C#, web scraping Node.js, web scraping BeautifulSoup, web scraping Selenium, web scraping Scrapy, web scraping Puppeteer, web scraping requests, web scraping headless browser, web scraping dynamic content, web scraping AJAX, web scraping pagination, web scraping authentication, web scraping cookies, web scraping session management, web scraping data parsing, web scraping data cleaning, web scraping data analysis, web scraping data visualization, web scraping legal issues, web scraping ethics, web scraping compliance, web scraping regulations, web scraping IP blocking, web scraping anti-scraping measures, web scraping proxy, web scraping CAPTCHA solving, web scraping IP rotation, web scraping rate limiting, web scraping data privacy, web scraping consent, web scraping terms of service, web scraping robots.txt, web scraping data storage, web scraping database integration, web scraping data integration, web scraping API integration, web scraping data export, web scraping data processing, web scraping data transformation, web scraping data enrichment, web scraping data validation, web scraping error handling, web scraping scalability, web scraping performance optimization, web scraping distributed scraping, web scraping cloud-based scraping, web scraping serverless scraping.
+ data harvesting, data crawling, web scraping software, website scraping tool, web scraping framework, data extraction tool, web data scraper, data scraping service, scraping automation, scraping tutorial, scraping code, scraping techniques, scraping best practices, scraping scripts, scraping tutorial, scraping examples, scraping challenges, scraping tricks, scraping tips, scraping tricks, scraping strategies, scraping methods, cloudflare protection bypass, cloudflare security bypass, web scraping Python, web scraping JavaScript, web scraping PHP, web scraping Ruby, web scraping Java, web scraping C#, web scraping Node.js, web scraping BeautifulSoup, web scraping Selenium, web scraping Scrapy, web scraping Puppeteer, web scraping requests, web scraping headless browser, web scraping dynamic content, web scraping AJAX, web scraping pagination, web scraping authentication, web scraping cookies, web scraping session management, web scraping data parsing, web scraping data cleaning, web scraping data analysis, web scraping data visualization, web scraping legal issues, web scraping ethics, web scraping compliance, web scraping regulations, web scraping IP blocking, web scraping anti-scraping measures, web scraping proxy, web scraping CAPTCHA solving, web scraping IP rotation, web scraping rate limiting, web scraping data privacy, web scraping consent, web scraping terms of service, web scraping robots.txt, web scraping data storage, web scraping database integration, web scraping data integration, web scraping API integration, web scraping data export, web scraping data processing, web scraping data transformation, web scraping data enrichment, web scraping data validation, web scraping error handling, web scraping scalability, web scraping performance optimization, web scraping distributed scraping, web scraping cloud-based scraping, web scraping serverless scraping.
```

### Comparing `scrappeycom-0.3.5/scrappeycom/scrappey.py` & `scrappeycom-0.3.6/scrappeycom/scrappey.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.5/scrappeycom/test.py` & `scrappeycom-0.3.6/scrappeycom/test.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.5/scrappeycom.egg-info/PKG-INFO` & `scrappeycom-0.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.5
+Version: 0.3.6
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
@@ -58,36 +58,69 @@
 ```
 
 ### Example
 
 Here's an example of how to use Scrappey. ðŸš€
 
 ```python
-from scrappeycom.scrappey import Scrappey
+from scrappey import Scrappey
+import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
-        session = scrappey.create_session()
-        print(session)
-
-        get_request_result = scrappey.get_request('https://httpbin.rs/get', session['session'])
+        sessionData = {
+            'session': str(uuid.uuid4()), #uuid is also optional, otherwise default uuid will be used
+            #'proxy': 'http://username:password@ip:port' #proxy is optional, otherwise default proxy will be used
+        }
+        session = scrappey.create_session(sessionData)
+        print('Session created:', session['session'])
+
+        # View all the options here with the request builder
+        # https://app.scrappey.com/#/builder
+        # Just copy paste it below, example
+        #
+        #    {
+        #       "cmd":  "request.get",
+        #       "url":  "https://httpbin.rs/get"
+        #    }
+
+        get_request_result = scrappey.request({
+            "cmd":  "request.get",
+            'session': session['session'],
+            'url': 'https://httpbin.rs/get',
+        })
         print('GET Request Result:', get_request_result)
 
-        post_data = {'username': 'user123', 'password': 'pass456'}
-        post_request_result = scrappey.post_request('https://httpbin.rs/post', post_data, session['session'])
+        post_request_result = scrappey.request({
+            "cmd": "request.post",
+            "url": "https://httpbin.rs/post",
+            "postData": "test=test&test2=test2"
+        })
         print('POST Request Result:', post_request_result)
 
-        scrappey.destroy_session(session['session'])
-        print('Session destroyed.')
+        # JSON request example
+        post_request_result_json = scrappey.request({
+            "cmd": "request.post",
+            "url": "https://backend.scrappey.com/api/auth/login",
+            "postData": "{\"email\":\"email\",\"password\":\"password\"}",
+            "customHeaders": {
+                "content-type": "application/json"
+            }
+        })
+        print('POST Request Result:', post_request_result_json)
+
+        sessionDestroyed = scrappey.destroy_session(sessionData)
+        print('Session destroyed:', sessionDestroyed)
     except Exception as error:
         print(error)
 
 run_test()
+
 ```
 
 For more information, please visit the [official Scrappey documentation](https://wiki.scrappey.com/getting-started). ðŸ“š
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `scrappeycom-0.3.5/setup.py` & `scrappeycom-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3.5',      # Start with a small number and increase it with every change you make
+  version = '0.3.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
```

