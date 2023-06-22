# Comparing `tmp/taskanalytics-data-wrapper-0.1.6.tar.gz` & `tmp/taskanalytics-data-wrapper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskanalytics-data-wrapper-0.1.6.tar", last modified: Tue Jun 13 13:21:54 2023, max compression
+gzip compressed data, was "taskanalytics-data-wrapper-0.1.7.tar", last modified: Thu Jun 22 06:45:13 2023, max compression
```

## Comparing `taskanalytics-data-wrapper-0.1.6.tar` & `taskanalytics-data-wrapper-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.562163 taskanalytics-data-wrapper-0.1.6/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.6/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3837 2023-06-13 13:21:54.562317 taskanalytics-data-wrapper-0.1.6/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3438 2023-06-02 19:20:01.000000 taskanalytics-data-wrapper-0.1.6/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      559 2023-06-13 13:21:54.563893 taskanalytics-data-wrapper-0.1.6/setup.cfg
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.6/setup.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.558067 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/taskanalytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.561502 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3837 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      323 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       27 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:45:13.892774 taskanalytics-data-wrapper-0.1.7/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       83 2023-05-21 20:49:56.000000 taskanalytics-data-wrapper-0.1.7/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.7/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.7/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      878 2023-06-22 06:42:11.000000 taskanalytics-data-wrapper-0.1.7/Makefile
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5090 2023-06-22 06:45:13.892149 taskanalytics-data-wrapper-0.1.7/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3438 2023-06-02 19:20:01.000000 taskanalytics-data-wrapper-0.1.7/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2255 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.7/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      841 2023-06-22 06:43:02.000000 taskanalytics-data-wrapper-0.1.7/pyproject.toml
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:45:13.864786 taskanalytics-data-wrapper-0.1.7/requirements/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3424 2023-06-22 06:44:13.000000 taskanalytics-data-wrapper-0.1.7/requirements/dev.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      446 2023-06-22 06:43:53.000000 taskanalytics-data-wrapper-0.1.7/requirements/main.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-06-22 06:45:13.892905 taskanalytics-data-wrapper-0.1.7/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:45:13.835986 taskanalytics-data-wrapper-0.1.7/src/
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:45:13.876939 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper/taskanalytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:45:13.890963 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5090 2023-06-22 06:45:13.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      481 2023-06-22 06:45:13.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-22 06:45:13.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       75 2023-06-22 06:45:13.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/requires.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       27 2023-06-22 06:45:13.000000 taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/top_level.txt
```

### Comparing `taskanalytics-data-wrapper-0.1.6/LICENSE` & `taskanalytics-data-wrapper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.6/PKG-INFO` & `taskanalytics-data-wrapper-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: taskanalytics-data-wrapper
-Version: 0.1.6
-Summary: a wrapper for using Task Analytics APIs and downloading survey responses
-Home-page: https://github.com/navikt/taskanalytics-data-wrapper
-Author: Tobias McVey
-Author-email: tobias.mcvey@nav.no
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Task Analytics Data Wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for Task Analytics APIs. You can use it to download survey responses and metadata for each survey.
 
 ## Supported APIs
@@ -120,8 +108,8 @@
 keys = newlist[0].keys()
 
 with open("data/open_survey.csv", "w", encoding="utf-8-sig", newline="") as output_file:
     writer = csv.DictWriter(output_file, fieldnames=keys, delimiter=";")
     writer.writeheader()
     writer.writerows(newlist)
 ```
-</details>
+</details>
```

### Comparing `taskanalytics-data-wrapper-0.1.6/README.md` & `taskanalytics-data-wrapper-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: taskanalytics-data-wrapper
+Version: 0.1.7
+Summary: a wrapper for using Task Analytics APIs and downloading survey responses
+Author-email: Tobias McVey <tobias.mcvey@nav.no>
+License: MIT License
+        
+        Copyright (c) 2022 NAV IT
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/navikt/taskanalytics-data-wrapper
+Keywords: Task Analytics,Top Tasks
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Task Analytics Data Wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for Task Analytics APIs. You can use it to download survey responses and metadata for each survey.
 
 ## Supported APIs
@@ -108,8 +141,8 @@
 keys = newlist[0].keys()
 
 with open("data/open_survey.csv", "w", encoding="utf-8-sig", newline="") as output_file:
     writer = csv.DictWriter(output_file, fieldnames=keys, delimiter=";")
     writer.writeheader()
     writer.writerows(newlist)
 ```
-</details>
+</details>
```

### Comparing `taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/taskanalytics_api.py` & `taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper/taskanalytics_api.py`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/PKG-INFO` & `taskanalytics-data-wrapper-0.1.7/src/taskanalytics_data_wrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 Metadata-Version: 2.1
 Name: taskanalytics-data-wrapper
-Version: 0.1.6
+Version: 0.1.7
 Summary: a wrapper for using Task Analytics APIs and downloading survey responses
-Home-page: https://github.com/navikt/taskanalytics-data-wrapper
-Author: Tobias McVey
-Author-email: tobias.mcvey@nav.no
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+Author-email: Tobias McVey <tobias.mcvey@nav.no>
+License: MIT License
+        
+        Copyright (c) 2022 NAV IT
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/navikt/taskanalytics-data-wrapper
+Keywords: Task Analytics,Top Tasks
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Task Analytics Data Wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for Task Analytics APIs. You can use it to download survey responses and metadata for each survey.
```

