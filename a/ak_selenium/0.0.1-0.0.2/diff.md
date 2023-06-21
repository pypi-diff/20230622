# Comparing `tmp/ak_selenium-0.0.1.tar.gz` & `tmp/ak_selenium-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_selenium-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ak_selenium-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ak_selenium-0.0.1.tar` & `ak_selenium-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      653 2023-06-21 07:45:53.041694 ak_selenium-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     2003 2023-06-21 08:31:27.810982 ak_selenium-0.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2023-06-21 07:45:53.041694 ak_selenium-0.0.1/LICENSE
--rw-r--r--   0        0        0     3277 2023-06-21 08:03:13.628399 ak_selenium-0.0.1/README.md
--rw-r--r--   0        0        0      532 2023-06-21 07:46:43.251725 ak_selenium-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      145 2023-06-21 08:04:45.600157 ak_selenium-0.0.1/src/ak_selenium/__init__.py
--rw-r--r--   0        0        0     6400 2023-06-21 07:57:23.668256 ak_selenium-0.0.1/src/ak_selenium/browser.py
--rw-r--r--   0        0        0        0 2023-06-21 07:45:53.042694 ak_selenium-0.0.1/src/tests/__init__.py
--rw-r--r--   0        0        0     1572 2023-06-21 07:45:53.042694 ak_selenium-0.0.1/src/tests/test_browser.py
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 ak_selenium-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      694 2023-06-21 15:27:04.024515 ak_selenium-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2003 2023-06-21 08:31:27.810982 ak_selenium-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1100 2023-06-21 07:45:53.041694 ak_selenium-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2980 2023-06-21 15:23:54.097594 ak_selenium-0.0.2/README.md
+-rw-r--r--   0        0        0    46704 2023-06-21 09:05:19.849182 ak_selenium-0.0.2/assets/Addl_Options.png
+-rw-r--r--   0        0        0    80746 2023-06-21 08:59:29.420231 ak_selenium-0.0.2/assets/usage.png
+-rw-r--r--   0        0        0      578 2023-06-21 08:36:54.049853 ak_selenium-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-06-21 23:49:54.241562 ak_selenium-0.0.2/src/ak_selenium/__init__.py
+-rw-r--r--   0        0        0     7171 2023-06-21 18:14:28.539445 ak_selenium-0.0.2/src/ak_selenium/browser.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:45:53.042694 ak_selenium-0.0.2/src/tests/__init__.py
+-rw-r--r--   0        0        0     1260 2023-06-21 08:45:02.471607 ak_selenium-0.0.2/src/tests/test_browser.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 ak_selenium-0.0.2/PKG-INFO
```

### Comparing `ak_selenium-0.0.1/.github/workflows/test.yml` & `ak_selenium-0.0.2/.github/workflows/test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 name: tests
 
 on: [push]
 
 jobs:
   build:
-
     runs-on: ${{ matrix.os }}
+    paths-ignore:
+      - '**/README.md'
     strategy:
       matrix:
         python-version: ["3.9", "3.10"]
         os: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `ak_selenium-0.0.1/.gitignore` & `ak_selenium-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ak_selenium-0.0.1/LICENSE` & `ak_selenium-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_selenium-0.0.1/README.md` & `ak_selenium-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 <!--- Heading --->
 <div align="center">
   <h1>ak_selenium</h1>
   <p>
     Selenium package with requests integration and anti-bot detection measures
   </p>
 <h4>
-    <a href="https://github.com/rpakishore/ak_selenium/">View Demo</a>
-  <span> · </span>
     <a href="https://github.com/rpakishore/ak_selenium">Documentation</a>
   <span> · </span>
     <a href="https://github.com/rpakishore/ak_selenium/issues/">Report Bug</a>
   <span> · </span>
     <a href="https://github.com/rpakishore/ak_selenium/issues/">Request Feature</a>
   </h4>
 </div>
 <br />
 
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/rpakishore/ak_selenium)
 ![GitHub last commit](https://img.shields.io/github/last-commit/rpakishore/ak_selenium)
+[![tests](https://github.com/rpakishore/ak_selenium/actions/workflows/test.yml/badge.svg)](https://github.com/rpakishore/ak_selenium/actions/workflows/test.yml)
+
 <!-- Table of Contents -->
 <h2>Table of Contents</h2>
 
 - [1. About the Project](#1-about-the-project)
   - [1.1. Features](#11-features)
 - [2. Getting Started](#2-getting-started)
   - [2.1. Dependencies](#21-dependencies)
   - [2.3. Installation](#23-installation)
     - [2.3.1. Production](#231-production)
     - [2.3.2. Development](#232-development)
 - [3. Usage](#3-usage)
+  - [Additional Options](#additional-options)
 - [4. Roadmap](#4-roadmap)
 - [5. License](#5-license)
 - [6. Contact](#6-contact)
 - [7. Acknowledgements](#7-acknowledgements)
 
 <!-- About the Project -->
 ## 1. About the Project
@@ -84,39 +85,19 @@
 ```bash
   flit install --pth-file
 ```
 
 <!-- Usage -->
 ## 3. Usage
 
-```python
-from ak_selenium import Chrome
-chrome = Chrome(
-    headless=False, 
-    Chrome_userdata_path=r"Path\to\User Data",
-    half_screen=True,
-)
-
-#Get Chromedriver
-driver = chrome.init_chrome()
-
-#Get the website
-driver.get("https://example.com")
-
-By, Keys = chrome.get_By_and_Keys()
-
-#Wait for elements to load
-locator = (By.TAG_NAME, "h1")
-chrome.Wait_for_locator(locator)
-
-#Get Requests Session
-s = chrome.update_req_headers_cookies()
-s.get('https://www.iana.org/domains/reserved')
-```
+![Usage](assets/usage.png)
+
+### Additional Options
 
+![Additional Options](assets/Addl_Options.png)
 <!-- Roadmap -->
 ## 4. Roadmap
 
 - [ ] Add beautifulsoup integration
 - [ ] Proxy
 
 <!-- License -->
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
                            ****** ak_selenium ******
   Selenium package with requests integration and anti-bot detection measures
-   *** View_Demo  Â·  Documentation  Â·  Report_Bug  Â·  Request_Feature ***
+          *** Documentation  Â·  Report_Bug  Â·  Request_Feature ***
 
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/
 rpakishore/ak_selenium) ![GitHub last commit](https://img.shields.io/github/
-last-commit/rpakishore/ak_selenium)
+last-commit/rpakishore/ak_selenium) [![tests](https://github.com/rpakishore/
+ak_selenium/actions/workflows/test.yml/badge.svg)](https://github.com/
+rpakishore/ak_selenium/actions/workflows/test.yml)
 ***** Table of Contents *****
 - [1. About the Project](#1-about-the-project) - [1.1. Features](#11-features)
 - [2. Getting Started](#2-getting-started) - [2.1. Dependencies](#21-
 dependencies) - [2.3. Installation](#23-installation) - [2.3.1. Production]
 (#231-production) - [2.3.2. Development](#232-development) - [3. Usage](#3-
-usage) - [4. Roadmap](#4-roadmap) - [5. License](#5-license) - [6. Contact](#6-
-contact) - [7. Acknowledgements](#7-acknowledgements)  ## 1. About the Project
-### 1.1. Features - Launch Selenium with custom options - Automatically try to
-add Chrome UserData - Add anti-bot detection measures - Pass selenium headers/
-cookies to requests library  ## 2. Getting Started ### 2.1. Dependencies Create
-the virutual environment and install dependencies ```bash python -m venv .venv
-.venv\Scripts\activate.bat pip install flit ```  ### 2.3. Installation ####
-2.3.1. Production Install with flit ```bash flit install --deps production ```
-Alternatively, you can use pip ```bash pip install ak_selenium ``` #### 2.3.2.
-Development Install with flit ```bash flit install --pth-file ```  ## 3. Usage
-```python from ak_selenium import Chrome chrome = Chrome( headless=False,
-Chrome_userdata_path=r"Path\to\User Data", half_screen=True, ) #Get
-Chromedriver driver = chrome.init_chrome() #Get the website driver.get("https:/
-/example.com") By, Keys = chrome.get_By_and_Keys() #Wait for elements to load
-locator = (By.TAG_NAME, "h1") chrome.Wait_for_locator(locator) #Get Requests
-Session s = chrome.update_req_headers_cookies() s.get('https://www.iana.org/
-domains/reserved') ```  ## 4. Roadmap - [ ] Add beautifulsoup integration - [ ]
-Proxy  ## 5. License See LICENSE.txt for more information.  ## 6. Contact Arun
-Kishore - [@rpakishore](mailto:pypi@rpakishore.co.in) Project Link: [https://
-github.com/rpakishore/ak_selenium](https://github.com/rpakishore/ak_selenium)
-## 7. Acknowledgements - [Awesome README Template](https://github.com/
-Louis3797/awesome-readme-template/blob/main/README-WITHOUT-EMOJI.md) - [Banner
-Maker](https://banner.godori.dev/) - [Shields.io](https://shields.io/) -
-[Carbon](https://carbon.now.sh/)
+usage) - [Additional Options](#additional-options) - [4. Roadmap](#4-roadmap) -
+[5. License](#5-license) - [6. Contact](#6-contact) - [7. Acknowledgements](#7-
+acknowledgements)  ## 1. About the Project  ### 1.1. Features - Launch Selenium
+with custom options - Automatically try to add Chrome UserData - Add anti-bot
+detection measures - Pass selenium headers/cookies to requests library  ## 2.
+Getting Started ### 2.1. Dependencies Create the virutual environment and
+install dependencies ```bash python -m venv .venv .venv\Scripts\activate.bat
+pip install flit ```  ### 2.3. Installation #### 2.3.1. Production Install with
+flit ```bash flit install --deps production ``` Alternatively, you can use pip
+```bash pip install ak_selenium ``` #### 2.3.2. Development Install with flit
+```bash flit install --pth-file ```  ## 3. Usage ![Usage](assets/usage.png) ###
+Additional Options ![Additional Options](assets/Addl_Options.png)  ## 4.
+Roadmap - [ ] Add beautifulsoup integration - [ ] Proxy  ## 5. License See
+LICENSE.txt for more information.  ## 6. Contact Arun Kishore - [@rpakishore]
+(mailto:pypi@rpakishore.co.in) Project Link: [https://github.com/rpakishore/
+ak_selenium](https://github.com/rpakishore/ak_selenium)  ## 7. Acknowledgements
+- [Awesome README Template](https://github.com/Louis3797/awesome-readme-
+template/blob/main/README-WITHOUT-EMOJI.md) - [Banner Maker](https://
+banner.godori.dev/) - [Shields.io](https://shields.io/) - [Carbon](https://
+carbon.now.sh/)
```

### Comparing `ak_selenium-0.0.1/pyproject.toml` & `ak_selenium-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 00000050: 696c 6461 7069 220d 0a0d 0a5b 7072 6f6a  ildapi"....[proj
 00000060: 6563 745d 0d0a 6e61 6d65 203d 2022 616b  ect]..name = "ak
 00000070: 5f73 656c 656e 6975 6d22 0d0a 6175 7468  _selenium"..auth
 00000080: 6f72 7320 3d20 5b7b 6e61 6d65 203d 2022  ors = [{name = "
 00000090: 4172 756e 204b 6973 686f 7265 222c 2065  Arun Kishore", e
 000000a0: 6d61 696c 203d 2022 7079 7069 4072 7061  mail = "pypi@rpa
 000000b0: 6b69 7368 6f72 652e 636f 2e69 6e22 7d5d  kishore.co.in"}]
-000000c0: 0d0a 6c69 6365 6e73 6520 3d20 7b66 696c  ..license = {fil
-000000d0: 6520 3d20 224c 4943 454e 5345 227d 0d0a  e = "LICENSE"}..
-000000e0: 636c 6173 7369 6669 6572 7320 3d20 5b22  classifiers = ["
-000000f0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000100: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000110: 6963 656e 7365 225d 0d0a 6479 6e61 6d69  icense"]..dynami
-00000120: 6320 3d20 5b22 7665 7273 696f 6e22 2c20  c = ["version", 
-00000130: 2264 6573 6372 6970 7469 6f6e 225d 0d0a  "description"]..
-00000140: 6465 7065 6e64 656e 6369 6573 3d5b 2273  dependencies=["s
-00000150: 656c 656e 6975 6d22 2c20 2277 6562 6472  elenium", "webdr
-00000160: 6976 6572 2d6d 616e 6167 6572 222c 2022  iver-manager", "
-00000170: 7265 7175 6573 7473 225d 0d0a 0d0a 5b70  requests"]....[p
-00000180: 726f 6a65 6374 2e6f 7074 696f 6e61 6c2d  roject.optional-
-00000190: 6465 7065 6e64 656e 6369 6573 5d0d 0a74  dependencies]..t
-000001a0: 6573 7420 3d20 5b0d 0a20 2020 2022 7079  est = [..    "py
-000001b0: 7465 7374 222c 0d0a 2020 2020 2269 7079  test",..    "ipy
-000001c0: 6b65 726e 656c 220d 0a5d 0d0a 0d0a 0d0a  kernel"..]......
-000001d0: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
-000001e0: 486f 6d65 203d 2022 6874 7470 733a 2f2f  Home = "https://
-000001f0: 6769 7468 7562 2e63 6f6d 2f72 7061 6b69  github.com/rpaki
-00000200: 7368 6f72 652f 616b 5f73 656c 656e 6975  shore/ak_seleniu
-00000210: 6d22 0d0a                                m"..
+000000c0: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
+000000d0: 4d45 2e6d 6422 0d0a 6c69 6365 6e73 6520  ME.md"..license 
+000000e0: 3d20 7b66 696c 6520 3d20 224c 4943 454e  = {file = "LICEN
+000000f0: 5345 227d 0d0a 636c 6173 7369 6669 6572  SE"}..classifier
+00000100: 7320 3d20 5b22 4c69 6365 6e73 6520 3a3a  s = ["License ::
+00000110: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000120: 204d 4954 204c 6963 656e 7365 225d 0d0a   MIT License"]..
+00000130: 6479 6e61 6d69 6320 3d20 5b22 7665 7273  dynamic = ["vers
+00000140: 696f 6e22 2c20 2264 6573 6372 6970 7469  ion", "descripti
+00000150: 6f6e 225d 0d0a 6465 7065 6e64 656e 6369  on"]..dependenci
+00000160: 6573 3d5b 0d0a 2020 2020 2273 656c 656e  es=[..    "selen
+00000170: 6975 6d22 2c20 0d0a 2020 2020 2277 6562  ium", ..    "web
+00000180: 6472 6976 6572 2d6d 616e 6167 6572 222c  driver-manager",
+00000190: 200d 0a20 2020 2022 7265 7175 6573 7473   ..    "requests
+000001a0: 220d 0a20 2020 205d 0d0a 0d0a 5b70 726f  "..    ]....[pro
+000001b0: 6a65 6374 2e6f 7074 696f 6e61 6c2d 6465  ject.optional-de
+000001c0: 7065 6e64 656e 6369 6573 5d0d 0a74 6573  pendencies]..tes
+000001d0: 7420 3d20 5b0d 0a20 2020 2022 7079 7465  t = [..    "pyte
+000001e0: 7374 222c 0d0a 2020 2020 2269 7079 6b65  st",..    "ipyke
+000001f0: 726e 656c 220d 0a5d 0d0a 0d0a 0d0a 5b70  rnel"..]......[p
+00000200: 726f 6a65 6374 2e75 726c 735d 0d0a 486f  roject.urls]..Ho
+00000210: 6d65 203d 2022 6874 7470 733a 2f2f 6769  me = "https://gi
+00000220: 7468 7562 2e63 6f6d 2f72 7061 6b69 7368  thub.com/rpakish
+00000230: 6f72 652f 616b 5f73 656c 656e 6975 6d22  ore/ak_selenium"
+00000240: 0d0a                                     ..
```

### Comparing `ak_selenium-0.0.1/src/ak_selenium/browser.py` & `ak_selenium-0.0.2/src/ak_selenium/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
 
 
+from selenium.webdriver.remote.webelement import WebElement
+
+
 from webdriver_manager.chrome import ChromeDriverManager
 
 from pathlib import Path
 import sys
 
 class Chrome:
     USERAGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) \
@@ -145,15 +148,25 @@
             "User-Agent": driver.execute_script("return window.navigator.userAgent;"),
             "Connection": "keep-alive"
         })
         self.s = s
         return s
     
     @staticmethod
-    def find_element_by_text(elements, text):
+    def find_element_by_text(elements:list[WebElement], text: str) -> WebElement:
+        """
+        Finds a WebElement from a list based on its text content.
+
+        Args:
+            elements (List[WebElement]): The list of WebElements to search through.
+            text (str): The text to match against the elements' text content.
+
+        Returns:
+            WebElement or None: The first WebElement that matches the provided text, or None if no match is found.
+        """
         for element in elements:
             if element.text.strip() == text:
                 return element
         return None
     
 
 def _ram_optimization_browser_options(options: Options) -> Options:
@@ -163,8 +176,12 @@
     options.add_argument("--no-sandbox")
     options.add_argument("--disable-extensions")
     options.add_argument("--no-sandbox")
     options.add_argument("--disable-application-cache")
     options.add_argument("--disable-gpu")
     options.add_argument("--disable-dev-shm-usage")
     options.add_argument("--lang=en-US")
+    
+    # Based on https://stackoverflow.com/questions/59514049/unable-to-sign-into-google-with-selenium-automation-because-of-this-browser-or
+    options.add_argument("--allow-running-insecure-content")
+    options.add_argument("--disable-web-security")
     return options
```

### Comparing `ak_selenium-0.0.1/src/tests/test_browser.py` & `ak_selenium-0.0.2/src/tests/test_browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 import pytest
 from ak_selenium import Chrome
 
-
 @pytest.fixture(scope="module")
 def chrome_instance():
     chrome = Chrome(headless=True)
     yield chrome
     del chrome
 
-
 def test_init_chrome(chrome_instance):
     assert chrome_instance.init_chrome()
 
-
 def test_implicitly_wait_time(chrome_instance):
     assert chrome_instance.IMPLICITLY_WAIT_TIME == 3
 
-
 def test_max_wait_time(chrome_instance):
     assert chrome_instance.MAX_WAIT_TIME == 5
 
-
 def test_chrome_user_agent(chrome_instance):
     assert chrome_instance.USERAGENT == 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) \
                 AppleWebKit/537.36 (KHTML, like Gecko) \
                 Chrome/83.0.4103.53 Safari/537.36'
 
-
 def test_half_screen(chrome_instance):
-    assert chrome_instance.half_screen == True
-
-
-def test_Chrome_userdata_path(chrome_instance):
-    assert chrome_instance.Chrome_userdata_path == None
-
+    assert chrome_instance.half_screen is True
 
 def test_str_method(chrome_instance):
     assert str(chrome_instance) == f"""
         Chrome.Object
         UserAgent:{chrome_instance.USERAGENT}
         Implicit Wait Time: {chrome_instance.IMPLICITLY_WAIT_TIME:.2f}s
         Max Wait Time: {chrome_instance.MAX_WAIT_TIME:.2f}s
         Headless: {chrome_instance.headless}
         Chrome Userdata Path: {chrome_instance.Chrome_userdata_path}
         Half Screen View: {chrome_instance.half_screen}
-        """
-
-
-def test_repr_method(chrome_instance):
-    assert repr(chrome_instance) == "Chrome(headless=True,\
-                Chrome_userdata_path=None,\
-                half_screen=True)"
+        """
```

