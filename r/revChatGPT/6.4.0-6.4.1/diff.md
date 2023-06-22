# Comparing `tmp/revChatGPT-6.4.0.tar.gz` & `tmp/revChatGPT-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.4.0.tar", last modified: Tue Jun 20 05:14:34 2023, max compression
+gzip compressed data, was "revChatGPT-6.4.1.tar", last modified: Thu Jun 22 03:55:44 2023, max compression
```

## Comparing `revChatGPT-6.4.0.tar` & `revChatGPT-6.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.896348 revChatGPT-6.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.896348 revChatGPT-6.4.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58782 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.744142 revChatGPT-6.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58782 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.4.0/LICENSE` & `revChatGPT-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/PKG-INFO` & `revChatGPT-6.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.0
+Version: 6.4.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.0/README.md` & `revChatGPT-6.4.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/setup.py` & `revChatGPT-6.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.4.0",
+    version="6.4.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.4.0/src/revChatGPT/V1.py` & `revChatGPT-6.4.1/src/revChatGPT/V1.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT/V3.py` & `revChatGPT-6.4.1/src/revChatGPT/V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,16 @@
                 if not line:
                     continue
                 # Remove "data: "
                 line = line[6:]
                 if line == "[DONE]":
                     break
                 resp: dict = json.loads(line)
+                if 'error' in resp:
+                    raise t.ResponseError(f"{resp['error']}")
                 choices = resp.get("choices")
                 if not choices:
                     continue
                 delta: dict[str, str] = choices[0].get("delta")
                 if not delta:
                     continue
                 if "role" in delta:
```

### Comparing `revChatGPT-6.4.0/src/revChatGPT/__init__.py` & `revChatGPT-6.4.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT/__main__.py` & `revChatGPT-6.4.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.4.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT/typings.py` & `revChatGPT-6.4.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT/utils.py` & `revChatGPT-6.4.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.4.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.0
+Version: 6.4.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.0/tests/test_recipient.py` & `revChatGPT-6.4.1/tests/test_recipient.py`

 * *Files identical despite different names*

