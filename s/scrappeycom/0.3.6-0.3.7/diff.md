# Comparing `tmp/scrappeycom-0.3.6.tar.gz` & `tmp/scrappeycom-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.6.tar", last modified: Thu Jun 22 08:32:44 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.7.tar", last modified: Thu Jun 22 08:37:27 2023, max compression
```

## Comparing `scrappeycom-0.3.6.tar` & `scrappeycom-0.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.925320 scrappeycom-0.3.6/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0     7499 2023-06-22 08:32:44.925320 scrappeycom-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     6344 2023-06-22 08:32:33.000000 scrappeycom-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.907321 scrappeycom-0.3.6/scrappeycom/
--rw-rw-rw-   0        0        0     1346 2023-06-22 08:26:36.000000 scrappeycom-0.3.6/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0     1898 2023-06-22 08:30:49.000000 scrappeycom-0.3.6/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:32:44.923320 scrappeycom-0.3.6/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     7499 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 08:32:44.000000 scrappeycom-0.3.6/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 08:32:44.927319 scrappeycom-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-22 08:32:40.000000 scrappeycom-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.868874 scrappeycom-0.3.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     7511 2023-06-22 08:37:27.869874 scrappeycom-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6356 2023-06-22 08:37:06.000000 scrappeycom-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.852874 scrappeycom-0.3.7/scrappeycom/
+-rw-rw-rw-   0        0        0     1346 2023-06-22 08:26:36.000000 scrappeycom-0.3.7/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0     1910 2023-06-22 08:36:48.000000 scrappeycom-0.3.7/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:37:27.867873 scrappeycom-0.3.7/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     7511 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 08:37:27.000000 scrappeycom-0.3.7/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 08:37:27.870873 scrappeycom-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-22 08:37:23.000000 scrappeycom-0.3.7/setup.py
```

### Comparing `scrappeycom-0.3.6/LICENSE.txt` & `scrappeycom-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.6/PKG-INFO` & `scrappeycom-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.6
+Version: 0.3.7
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
@@ -58,15 +58,15 @@
 ```
 
 ### Example
 
 Here's an example of how to use Scrappey. ðŸš€
 
 ```python
-from scrappey import Scrappey
+from scrappeycom.scrappey import Scrappey
 import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
         sessionData = {
```

### Comparing `scrappeycom-0.3.6/README.md` & `scrappeycom-0.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ```
 
 ### Example
 
 Here's an example of how to use Scrappey. 🚀
 
 ```python
-from scrappey import Scrappey
+from scrappeycom.scrappey import Scrappey
 import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
         sessionData = {
```

### Comparing `scrappeycom-0.3.6/scrappeycom/scrappey.py` & `scrappeycom-0.3.7/scrappeycom/scrappey.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.6/scrappeycom/test.py` & `scrappeycom-0.3.7/scrappeycom/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from scrappey import Scrappey
+from scrappeycom.scrappey import Scrappey
 import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
         sessionData = {
```

### Comparing `scrappeycom-0.3.6/scrappeycom.egg-info/PKG-INFO` & `scrappeycom-0.3.7/scrappeycom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.6
+Version: 0.3.7
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
@@ -58,15 +58,15 @@
 ```
 
 ### Example
 
 Here's an example of how to use Scrappey. ðŸš€
 
 ```python
-from scrappey import Scrappey
+from scrappeycom.scrappey import Scrappey
 import uuid
 
 scrappey = Scrappey('API_KEY')
 
 def run_test():
     try:
         sessionData = {
```

### Comparing `scrappeycom-0.3.6/setup.py` & `scrappeycom-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3.6',      # Start with a small number and increase it with every change you make
+  version = '0.3.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
```

