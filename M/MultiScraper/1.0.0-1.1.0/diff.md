# Comparing `tmp/MultiScraper-1.0.0.tar.gz` & `tmp/MultiScraper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultiScraper-1.0.0.tar", last modified: Sat Jun 10 14:35:21 2023, max compression
+gzip compressed data, was "MultiScraper-1.1.0.tar", last modified: Fri Jun 16 19:25:56 2023, max compression
```

## Comparing `MultiScraper-1.0.0.tar` & `MultiScraper-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 14:35:21.066046 MultiScraper-1.0.0/
--rw-rw-rw-   0        0        0     1339 2023-06-10 13:55:24.000000 MultiScraper-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-10 14:35:21.031512 MultiScraper-1.0.0/MultiScraper/
--rw-rw-rw-   0        0        0      489 2023-06-10 14:07:40.000000 MultiScraper-1.0.0/MultiScraper/Aiohttp.py
--rw-rw-rw-   0        0        0      354 2023-06-10 09:01:10.000000 MultiScraper-1.0.0/MultiScraper/CloudScraper.py
--rw-rw-rw-   0        0        0      679 2023-06-10 09:01:11.000000 MultiScraper-1.0.0/MultiScraper/HttpClient.py
--rw-rw-rw-   0        0        0     2805 2023-06-10 08:50:31.000000 MultiScraper-1.0.0/MultiScraper/LxmlSoup.py
--rw-rw-rw-   0        0        0     1870 2023-06-07 17:31:29.000000 MultiScraper-1.0.0/MultiScraper/Regular.py
--rw-rw-rw-   0        0        0     1030 2023-06-10 09:01:10.000000 MultiScraper-1.0.0/MultiScraper/Requests.py
--rw-rw-rw-   0        0        0      954 2023-06-07 17:37:31.000000 MultiScraper-1.0.0/MultiScraper/ResponseHandler.py
--rw-rw-rw-   0        0        0      899 2023-06-10 09:01:10.000000 MultiScraper-1.0.0/MultiScraper/Selenium.py
--rw-rw-rw-   0        0        0      356 2023-06-10 09:01:10.000000 MultiScraper-1.0.0/MultiScraper/Urllib.py
--rw-rw-rw-   0        0        0      551 2023-06-08 18:16:01.000000 MultiScraper-1.0.0/MultiScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:35:21.061783 MultiScraper-1.0.0/MultiScraper.egg-info/
--rw-rw-rw-   0        0        0     1950 2023-06-10 14:35:20.000000 MultiScraper-1.0.0/MultiScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-10 14:35:20.000000 MultiScraper-1.0.0/MultiScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 14:35:20.000000 MultiScraper-1.0.0/MultiScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-10 14:35:20.000000 MultiScraper-1.0.0/MultiScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 14:35:20.000000 MultiScraper-1.0.0/MultiScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1950 2023-06-10 14:35:21.066046 MultiScraper-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2023-06-10 14:17:56.000000 MultiScraper-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 14:35:21.078901 MultiScraper-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-06-10 14:17:56.000000 MultiScraper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:56.757610 MultiScraper-1.1.0/
+-rw-rw-rw-   0        0        0     1354 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:56.726336 MultiScraper-1.1.0/MultiScraper/
+-rw-rw-rw-   0        0        0      489 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/Aiohttp.py
+-rw-rw-rw-   0        0        0      354 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/CloudScraper.py
+-rw-rw-rw-   0        0        0      679 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/HttpClient.py
+-rw-rw-rw-   0        0        0     4373 2023-06-16 19:18:28.000000 MultiScraper-1.1.0/MultiScraper/LxmlSoup.py
+-rw-rw-rw-   0        0        0     1870 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/Regular.py
+-rw-rw-rw-   0        0        0     1195 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/Requests.py
+-rw-rw-rw-   0        0        0      954 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/ResponseHandler.py
+-rw-rw-rw-   0        0        0      899 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/Selenium.py
+-rw-rw-rw-   0        0        0      356 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/Urllib.py
+-rw-rw-rw-   0        0        0      551 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/MultiScraper/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:56.757610 MultiScraper-1.1.0/MultiScraper.egg-info/
+-rw-rw-rw-   0        0        0     1934 2023-06-16 19:25:56.000000 MultiScraper-1.1.0/MultiScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-06-16 19:25:56.000000 MultiScraper-1.1.0/MultiScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:25:56.000000 MultiScraper-1.1.0/MultiScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-16 19:25:56.000000 MultiScraper-1.1.0/MultiScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 19:25:56.000000 MultiScraper-1.1.0/MultiScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1934 2023-06-16 19:25:56.757610 MultiScraper-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1483 2023-06-16 16:56:58.000000 MultiScraper-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:25:56.769613 MultiScraper-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-06-16 19:25:44.000000 MultiScraper-1.1.0/setup.py
```

### Comparing `MultiScraper-1.0.0/LICENSE` & `MultiScraper-1.1.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MultiScraper is made available under the MIT license:
 
- Copyright (c) Alexander Gladkih
+ Copyright (c) Alexander Gladkih (gladkihaa-38)
 
  Permission is hereby granted, free of charge, to any person obtaining
  a copy of this software and associated documentation files (the
  "Software"), to deal in the Software without restriction, including
  without limitation the rights to use, copy, modify, merge, publish,
  distribute, sublicense, and/or sell copies of the Software, and to
  permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `MultiScraper-1.0.0/MultiScraper/HttpClient.py` & `MultiScraper-1.1.0/MultiScraper/HttpClient.py`

 * *Files identical despite different names*

### Comparing `MultiScraper-1.0.0/MultiScraper/Regular.py` & `MultiScraper-1.1.0/MultiScraper/Regular.py`

 * *Files identical despite different names*

### Comparing `MultiScraper-1.0.0/MultiScraper/Requests.py` & `MultiScraper-1.1.0/MultiScraper/Requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,13 +17,18 @@
     return soup
 
 def parse_post_html(url, json={}, data={}):
     response = requests.post(url, json=json, data=data)
     return response.text
 
 
-def parse_auth(url, user, password):
+def parse_auth_soup(url, user, password):
     basic = HTTPBasicAuth(user, password)
     response = requests.get(url, auth=basic)
     soup = BeautifulSoup(response.text, 'lxml')
     return soup
 
+def parse_auth_html(url, user, password):
+    basic = HTTPBasicAuth(user, password)
+    response = requests.get(url, auth=basic)
+    return response.text
+
```

### Comparing `MultiScraper-1.0.0/MultiScraper/ResponseHandler.py` & `MultiScraper-1.1.0/MultiScraper/ResponseHandler.py`

 * *Files identical despite different names*

### Comparing `MultiScraper-1.0.0/MultiScraper/Selenium.py` & `MultiScraper-1.1.0/MultiScraper/Selenium.py`

 * *Files identical despite different names*

### Comparing `MultiScraper-1.0.0/MultiScraper/__init__.py` & `MultiScraper-1.1.0/MultiScraper/__init__.py`

 * *Files identical despite different names*

### Comparing `MultiScraper-1.0.0/MultiScraper.egg-info/PKG-INFO` & `MultiScraper-1.1.0/MultiScraper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: MultiScraper
-Version: 1.0.0
+Version: 1.1.0
 Summary: Multi Scraper is a set of tools for fast and easy parsing
 Author: Alexander554
 Author-email: gaa.280811@gmail.com
 Keywords: MultiScraper
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-MultiScraper
-============
-
+# MultiScraper
 MultiScraper is a set of tools for fast and easy parsing. It includes methods for extracting html and soup objects from modules such as: requests, cloudscraper, Selenium, http.client, Aiohttp, urllib3. It also has 2 assistants. The first one is Regular, it contains ready-made, useful for parsing regular expressions. The second one is ResponseHandler, will help you figure out what the status code means to you. The most important thing is Lxmlsoup. This is an analogue of BeautifulSoup containing the most basic and necessary methods. Its speed exceeds bs4 by 2 times. The syntax is the same.
 
 ```
 0.7749056816101074 - LxmlSoup
 1.4368107318878174 - BeautifulSoup
 ```
 ## Installation
@@ -54,8 +52,7 @@
     soup = LxmlSoup.LxmlSoup(html)  
     title = soup.find('h1').text()
     print(title)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
-
```

### Comparing `MultiScraper-1.0.0/PKG-INFO` & `MultiScraper-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: MultiScraper
-Version: 1.0.0
+Version: 1.1.0
 Summary: Multi Scraper is a set of tools for fast and easy parsing
 Author: Alexander554
 Author-email: gaa.280811@gmail.com
 Keywords: MultiScraper
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-MultiScraper
-============
-
+# MultiScraper
 MultiScraper is a set of tools for fast and easy parsing. It includes methods for extracting html and soup objects from modules such as: requests, cloudscraper, Selenium, http.client, Aiohttp, urllib3. It also has 2 assistants. The first one is Regular, it contains ready-made, useful for parsing regular expressions. The second one is ResponseHandler, will help you figure out what the status code means to you. The most important thing is Lxmlsoup. This is an analogue of BeautifulSoup containing the most basic and necessary methods. Its speed exceeds bs4 by 2 times. The syntax is the same.
 
 ```
 0.7749056816101074 - LxmlSoup
 1.4368107318878174 - BeautifulSoup
 ```
 ## Installation
@@ -54,8 +52,7 @@
     soup = LxmlSoup.LxmlSoup(html)  
     title = soup.find('h1').text()
     print(title)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
-
```

### Comparing `MultiScraper-1.0.0/README.md` & `MultiScraper-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-MultiScraper
-============
-
+# MultiScraper
 MultiScraper is a set of tools for fast and easy parsing. It includes methods for extracting html and soup objects from modules such as: requests, cloudscraper, Selenium, http.client, Aiohttp, urllib3. It also has 2 assistants. The first one is Regular, it contains ready-made, useful for parsing regular expressions. The second one is ResponseHandler, will help you figure out what the status code means to you. The most important thing is Lxmlsoup. This is an analogue of BeautifulSoup containing the most basic and necessary methods. Its speed exceeds bs4 by 2 times. The syntax is the same.
 
 ```
 0.7749056816101074 - LxmlSoup
 1.4368107318878174 - BeautifulSoup
 ```
 ## Installation
@@ -40,8 +38,7 @@
     soup = LxmlSoup.LxmlSoup(html)  
     title = soup.find('h1').text()
     print(title)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
-
```

### Comparing `MultiScraper-1.0.0/setup.py` & `MultiScraper-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='MultiScraper',
-  version='1.0.0',
+  version='1.1.0',
   author='Alexander554',
   author_email='gaa.280811@gmail.com',
   description='Multi Scraper is a set of tools for fast and easy parsing',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
-  install_requires=['requests', 'lxml', 'bs4', 'aiohttp', 'cloudscraper', 'selenium', 'urllib3'],
+  install_requires=['requests', 'lxml', 'bs4', 'aiohttp', 'cloudscraper', 'selenium', 'urllib3', 'cssselect'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='MultiScraper',
   python_requires='>=3.7'
```

