# Comparing `tmp/league-0.0.1.tar.gz` & `tmp/league-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "league-0.0.1.tar", last modified: Thu Jun 22 07:58:11 2023, max compression
+gzip compressed data, was "league-0.0.2.tar", last modified: Thu Jun 22 08:20:13 2023, max compression
```

## Comparing `league-0.0.1.tar` & `league-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:58:11.081046 league-0.0.1/
--rw-rw-rw-   0        0        0     1081 2023-06-22 01:34:20.000000 league-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      894 2023-06-22 07:58:11.079051 league-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-06-22 01:34:20.000000 league-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:58:11.022817 league-0.0.1/league/
--rw-rw-rw-   0        0        0      194 2023-06-22 07:35:40.000000 league-0.0.1/league/__init__.py
--rw-rw-rw-   0        0        0     3757 2023-06-22 07:35:40.000000 league-0.0.1/league/client.py
--rw-rw-rw-   0        0        0     1679 2023-06-22 07:35:40.000000 league-0.0.1/league/handler.py
--rw-rw-rw-   0        0        0     2783 2023-06-22 07:35:40.000000 league-0.0.1/league/lexicon.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:58:11.074065 league-0.0.1/league/objects/
--rw-rw-rw-   0        0        0      202 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/__init__.py
--rw-rw-rw-   0        0        0       75 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/account.py
--rw-rw-rw-   0        0        0      386 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/cache.py
--rw-rw-rw-   0        0        0      180 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/character.py
--rw-rw-rw-   0        0        0      191 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/item.py
--rw-rw-rw-   0        0        0      175 2023-06-22 07:35:40.000000 league-0.0.1/league/objects/spell.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:58:11.048749 league-0.0.1/league.egg-info/
--rw-rw-rw-   0        0        0      894 2023-06-22 07:58:10.000000 league-0.0.1/league.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-22 07:58:10.000000 league-0.0.1/league.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:58:10.000000 league-0.0.1/league.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 07:48:20.000000 league-0.0.1/league.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-22 07:58:10.000000 league-0.0.1/league.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:58:11.081046 league-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      958 2023-06-22 07:56:50.000000 league-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:20:13.047437 league-0.0.2/
+-rw-rw-rw-   0        0        0     1081 2023-06-22 01:34:20.000000 league-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      917 2023-06-22 08:20:13.046429 league-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-06-22 01:34:20.000000 league-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:20:12.995772 league-0.0.2/league/
+-rw-rw-rw-   0        0        0      194 2023-06-22 08:19:47.000000 league-0.0.2/league/__init__.py
+-rw-rw-rw-   0        0        0     3757 2023-06-22 07:35:40.000000 league-0.0.2/league/client.py
+-rw-rw-rw-   0        0        0     1679 2023-06-22 07:35:40.000000 league-0.0.2/league/handler.py
+-rw-rw-rw-   0        0        0     2783 2023-06-22 07:35:40.000000 league-0.0.2/league/lexicon.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:20:13.043436 league-0.0.2/league/objects/
+-rw-rw-rw-   0        0        0      202 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/account.py
+-rw-rw-rw-   0        0        0      386 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/cache.py
+-rw-rw-rw-   0        0        0      180 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/character.py
+-rw-rw-rw-   0        0        0      191 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/item.py
+-rw-rw-rw-   0        0        0      175 2023-06-22 07:35:40.000000 league-0.0.2/league/objects/spell.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:20:13.017328 league-0.0.2/league.egg-info/
+-rw-rw-rw-   0        0        0      917 2023-06-22 08:20:12.000000 league-0.0.2/league.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-22 08:20:12.000000 league-0.0.2/league.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:20:12.000000 league-0.0.2/league.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 07:48:20.000000 league-0.0.2/league.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-22 08:20:12.000000 league-0.0.2/league.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:20:13.048424 league-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-06-22 08:17:30.000000 league-0.0.2/setup.py
```

### Comparing `league-0.0.1/LICENSE` & `league-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `league-0.0.1/PKG-INFO` & `league-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: league
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial Python interface for the League of Legends API!
 Home-page: https://github.com/timothyckl/league.py
 Author: timothyckl
 License: MIT
 Project-URL: Source Code, https://github.com/timothyckl/league.py
 Project-URL: Pull Requests, https://github.com/timothyckl/league.py/pulls
 Project-URL: Issue Tracker, https://github.com/timothyckl/league.py/issues
@@ -15,9 +15,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<_io.TextIOWrapper name='README.md' mode='r' encoding='cp1252'>
+```league.py``` is an unofficial Python wrapper for Riot Games' League of Legends API.
```

### Comparing `league-0.0.1/league/client.py` & `league-0.0.2/league/client.py`

 * *Files identical despite different names*

### Comparing `league-0.0.1/league/handler.py` & `league-0.0.2/league/handler.py`

 * *Files identical despite different names*

### Comparing `league-0.0.1/league/lexicon.py` & `league-0.0.2/league/lexicon.py`

 * *Files identical despite different names*

### Comparing `league-0.0.1/league.egg-info/PKG-INFO` & `league-0.0.2/league.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: league
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial Python interface for the League of Legends API!
 Home-page: https://github.com/timothyckl/league.py
 Author: timothyckl
 License: MIT
 Project-URL: Source Code, https://github.com/timothyckl/league.py
 Project-URL: Pull Requests, https://github.com/timothyckl/league.py/pulls
 Project-URL: Issue Tracker, https://github.com/timothyckl/league.py/issues
@@ -15,9 +15,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<_io.TextIOWrapper name='README.md' mode='r' encoding='cp1252'>
+```league.py``` is an unofficial Python wrapper for Riot Games' League of Legends API.
```

### Comparing `league-0.0.1/setup.py` & `league-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     url=url,
     project_urls={
         "Source Code": url,
         "Pull Requests": url + "/pulls",
         "Issue Tracker": url + "/issues",
     },
 
-    long_description=readme,
+    long_description=long_description,
     long_description_content_type="text/markdown",
 
     python_requires=">=3.8.0",
     zip_safe=False,
     packages=['league', 'league.objects'],
 
     classifiers=[
```

