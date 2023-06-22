# Comparing `tmp/hotjar-data-wrapper-0.1.4.tar.gz` & `tmp/hotjar-data-wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotjar-data-wrapper-0.1.4.tar", last modified: Tue Jun 13 13:08:08 2023, max compression
+gzip compressed data, was "hotjar-data-wrapper-0.1.5.tar", last modified: Thu Jun 22 06:36:49 2023, max compression
```

## Comparing `hotjar-data-wrapper-0.1.4.tar` & `hotjar-data-wrapper-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.770820 hotjar-data-wrapper-0.1.4/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.4/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1923 2023-06-13 13:08:08.771067 hotjar-data-wrapper-0.1.4/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1579 2023-06-02 19:34:25.000000 hotjar-data-wrapper-0.1.4/README.md
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.765394 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:33:47.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/hotjar_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.769715 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1923 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      274 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       20 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      504 2023-06-13 13:08:08.774797 hotjar-data-wrapper-0.1.4/setup.cfg
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:33:47.000000 hotjar-data-wrapper-0.1.4/setup.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:36:49.220291 hotjar-data-wrapper-0.1.5/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       91 2023-05-21 20:51:57.000000 hotjar-data-wrapper-0.1.5/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.5/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.5/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      878 2023-06-22 06:22:08.000000 hotjar-data-wrapper-0.1.5/Makefile
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3158 2023-06-22 06:36:49.219170 hotjar-data-wrapper-0.1.5/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1579 2023-06-02 19:34:25.000000 hotjar-data-wrapper-0.1.5/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      925 2023-06-22 06:25:58.000000 hotjar-data-wrapper-0.1.5/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      764 2023-06-22 06:31:03.000000 hotjar-data-wrapper-0.1.5/pyproject.toml
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:36:49.202011 hotjar-data-wrapper-0.1.5/requirements/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3368 2023-06-22 06:25:21.000000 hotjar-data-wrapper-0.1.5/requirements/dev.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      432 2023-06-22 06:25:00.000000 hotjar-data-wrapper-0.1.5/requirements/main.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-06-22 06:36:49.220529 hotjar-data-wrapper-0.1.5/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:36:49.188813 hotjar-data-wrapper-0.1.5/src/
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:36:49.204061 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:33:47.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6078 2023-06-22 06:28:56.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper/hotjar_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-22 06:36:49.217502 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3158 2023-06-22 06:36:49.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      425 2023-06-22 06:36:49.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-22 06:36:49.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       75 2023-06-22 06:36:49.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/requires.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       20 2023-06-22 06:36:49.000000 hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper.egg-info/top_level.txt
```

### Comparing `hotjar-data-wrapper-0.1.4/LICENSE` & `hotjar-data-wrapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.4/PKG-INFO` & `hotjar-data-wrapper-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: hotjar-data-wrapper
-Version: 0.1.4
-Summary: a wrapper for using Hotjar APIs
-Home-page: https://github.com/navikt/hotjar-data-wrapper
-Author: Tobias McVey
-Author-email: tobias.mcvey@nav.no
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hotjar Data Wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for Hotjar APIs to let you login and download survey data and metadata for your account.
 
 ## Supported APIs and docs
@@ -63,8 +51,8 @@
 hot.get_all_surveys_metadata(
     path="data/hotjar surveys",
     surveys_list=ids,
     site_id=site_id,
     username=username,
     password=password,
 )
-```
+```
```

### Comparing `hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/hotjar_api.py` & `hotjar-data-wrapper-0.1.5/src/hotjar_data_wrapper/hotjar_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # %%
 import json
 import requests
 
+
 # %%
 def login_hotjar(username: str, password: str):
     """
     Log into Hotjar
     """
     session = requests.Session()
     login_url = "https://insights.hotjar.com/api/v2/users"
```

