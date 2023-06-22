# Comparing `tmp/python-runit-0.2.1.tar.gz` & `tmp/python-runit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-runit-0.2.1.tar", last modified: Tue Jun 20 01:06:17 2023, max compression
+gzip compressed data, was "python-runit-0.2.2.tar", last modified: Thu Jun 22 17:28:49 2023, max compression
```

## Comparing `python-runit-0.2.1.tar` & `python-runit-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.164562 python-runit-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4703 2023-06-20 01:06:17.162564 python-runit-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.690956 python-runit-0.2.1/python_runit.egg-info/
--rw-rw-rw-   0        0        0     4703 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 01:06:16.000000 python-runit-0.2.1/python_runit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.784490 python-runit-0.2.1/runit/
--rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/Request.py
--rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.2.1/runit/__init__.py
--rw-rw-rw-   0        0        0    12750 2023-06-19 19:13:54.000000 python-runit-0.2.1/runit/cli.py
--rw-rw-rw-   0        0        0     2066 2023-06-19 19:21:40.000000 python-runit-0.2.1/runit/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.854528 python-runit-0.2.1/runit/languages/
--rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/languages/__init__.py
--rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/languages/javascript.py
--rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/languages/multi.py
--rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/languages/php.py
--rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/languages/python.py
--rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/languages/runtime.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.883736 python-runit-0.2.1/runit/modules/
--rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/modules/__init__.py
--rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/modules/account.py
--rw-rw-rw-   0        0        0    13030 2023-06-19 19:13:55.000000 python-runit-0.2.1/runit/runit.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.924167 python-runit-0.2.1/runit/templates/
--rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/.runitignore
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/404.html
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.944340 python-runit-0.2.1/runit/templates/javascript/
--rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.2.1/runit/templates/javascript/.env
--rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/javascript/main.js
--rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/javascript/package.json
--rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/javascript/runit.json
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.074567 python-runit-0.2.1/runit/templates/multi/
--rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/application.py
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/composer.json
--rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/index.php
--rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/main.js
--rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/package.json
--rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/request.php
--rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/requirements.txt
--rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/multi/test.php
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.094563 python-runit-0.2.1/runit/templates/php/
--rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.2.1/runit/templates/php/.env
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/php/composer.json
--rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/php/index.php
--rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/php/runit.json
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.133566 python-runit-0.2.1/runit/templates/python/
--rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.2.1/runit/templates/python/.env
--rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/python/application.py
--rw-rw-rw-   0        0        0      363 2023-06-19 19:13:55.000000 python-runit-0.2.1/runit/templates/python/requirements.txt
--rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/python/runit.json
--rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/templates/request.php
--rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/templates/runit.json
--rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/test.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:16.634430 python-runit-0.2.1/runit/tools/
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.142562 python-runit-0.2.1/runit/tools/javascript/
--rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.2.1/runit/tools/javascript/loader.js
--rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.2.1/runit/tools/javascript/runner.js
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.150561 python-runit-0.2.1/runit/tools/php/
--rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/tools/php/loader.php
--rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/tools/php/runner.php
-drwxrwxrwx   0        0        0        0 2023-06-20 01:06:17.158567 python-runit-0.2.1/runit/tools/python/
--rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/tools/python/loader.py
--rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.2.1/runit/tools/python/runner.py
--rw-rw-rw-   0        0        0       42 2023-06-20 01:06:17.165565 python-runit-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-06-19 19:21:28.000000 python-runit-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.961460 python-runit-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4703 2023-06-22 17:28:49.959507 python-runit-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.880047 python-runit-0.2.2/python_runit.egg-info/
+-rw-rw-rw-   0        0        0     4703 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1528 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.982051 python-runit-0.2.2/runit/
+-rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/Request.py
+-rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.2.2/runit/__init__.py
+-rw-rw-rw-   0        0        0    13015 2023-06-22 17:24:28.000000 python-runit-0.2.2/runit/cli.py
+-rw-rw-rw-   0        0        0     2037 2023-06-22 17:25:15.000000 python-runit-0.2.2/runit/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.041050 python-runit-0.2.2/runit/languages/
+-rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/__init__.py
+-rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/javascript.py
+-rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/multi.py
+-rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/php.py
+-rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/python.py
+-rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/runtime.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.060052 python-runit-0.2.2/runit/modules/
+-rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/modules/__init__.py
+-rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/modules/account.py
+-rw-rw-rw-   0        0        0    13030 2023-06-19 19:13:55.000000 python-runit-0.2.2/runit/runit.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.254048 python-runit-0.2.2/runit/templates/
+-rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/.runitignore
+-rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/404.html
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.344827 python-runit-0.2.2/runit/templates/javascript/
+-rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/javascript/.env
+-rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/javascript/main.js
+-rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/javascript/package.json
+-rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/javascript/runit.json
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.540388 python-runit-0.2.2/runit/templates/multi/
+-rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/application.py
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/composer.json
+-rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/index.php
+-rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/main.js
+-rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/package.json
+-rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/request.php
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/requirements.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/test.php
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.578665 python-runit-0.2.2/runit/templates/php/
+-rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/php/.env
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/php/composer.json
+-rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/php/index.php
+-rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/php/runit.json
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.659243 python-runit-0.2.2/runit/templates/python/
+-rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/python/.env
+-rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/python/application.py
+-rw-rw-rw-   0        0        0      363 2023-06-19 19:13:55.000000 python-runit-0.2.2/runit/templates/python/requirements.txt
+-rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/python/runit.json
+-rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/request.php
+-rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/runit.json
+-rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.821245 python-runit-0.2.2/runit/tools/
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.814464 python-runit-0.2.2/runit/tools/javascript/
+-rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.2.2/runit/tools/javascript/loader.js
+-rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/tools/javascript/runner.js
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.947460 python-runit-0.2.2/runit/tools/php/
+-rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/php/loader.php
+-rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/php/runner.php
+drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.955462 python-runit-0.2.2/runit/tools/python/
+-rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/python/loader.py
+-rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/python/runner.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:28:49.962465 python-runit-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-06-22 17:25:23.000000 python-runit-0.2.2/setup.py
```

### Comparing `python-runit-0.2.1/LICENSE` & `python-runit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/PKG-INFO` & `python-runit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-runit-0.2.1/README.md` & `python-runit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/python_runit.egg-info/PKG-INFO` & `python-runit-0.2.2/python_runit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-runit-0.2.1/python_runit.egg-info/SOURCES.txt` & `python-runit-0.2.2/python_runit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/Request.py` & `python-runit-0.2.2/runit/Request.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/cli.py` & `python-runit-0.2.2/runit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dotenv import load_dotenv, set_key, find_dotenv, dotenv_values
 
 from .languages import LanguageParser
 from .modules import Account
 from .runit import RunIt
 
 from .constants import VERSION, CURRENT_PROJECT, CURRENT_PROJECT_DIR, EXT_TO_RUNTIME, \
-                        LANGUAGE_TO_RUNTIME
+                        LANGUAGE_TO_RUNTIME, RUNIT_HOMEDIR
 
 load_dotenv()
 
 def StartWebserver(project: Type[RunIt], host: str = '127.0.0.1', port: int = 5000):
     app = FastAPI()
     app.secret_key = "fdakfjlfdsaflfkjbasdoiefanckdareafasdfkowadbfakidfadfkj"
     
@@ -27,15 +27,14 @@
     async def serve(func: Optional[str], request: Request):
         if request.method.lower() in ['get', 'post']:
             func = func if func else 'index'
             params = list(request.query_params.values())
             return project.serve(func, params) \
                 if len(params) else project.serve(func)
         return 'MethodNodAllowed'
-
     
     try:
         import uvicorn
         uvicorn.run(app, host=host, port=port)
     except KeyboardInterrupt:
         import sys
         sys.exit(1)
@@ -176,21 +175,27 @@
 def setup_runit(args):
     '''
     Setup Runit server side api
     
     @params args
     @return None
     '''
+    if not find_dotenv():
+        with open(os.path.join(RUNIT_HOMEDIR, '.env'), 'wt') as env_file:
+            pass
+        set_key(find_dotenv(), 'RUNIT_API_ENDPOINT', '')
+        set_key(find_dotenv(), 'RUNIT_PROJECT_ID', '')
+        
     settings = dotenv_values(find_dotenv())
     
     if args.api:
         settings['RUNIT_API_ENDPOINT'] = args.api
     else:
         for key, value in settings.items():
-            new_value = input(f'{key} [{value}]: ')
+            new_value = input(f'{key} [{value}]: ').strip()
             if new_value:
                 settings[key] = new_value 
             else:
                 print(f'{key} cannot be empty')
                 print(f'Setting {key} to default [{value}]')
     
     for key, value in settings.items():
```

### Comparing `python-runit-0.2.1/runit/constants.py` & `python-runit-0.2.2/runit/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = os.path.realpath(os.curdir)
-TOOLS_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'tools')
-PROJECTS_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'projects')
-TEMPLATES_FOLDER = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates')
+RUNIT_HOMEDIR = os.path.dirname(os.path.realpath(__file__))
+TOOLS_DIR = os.path.join(RUNIT_HOMEDIR, 'tools')
+PROJECTS_DIR = os.path.join(RUNIT_HOMEDIR, 'projects')
+TEMPLATES_FOLDER = os.path.join(RUNIT_HOMEDIR, 'templates')
 
 EXT_TO_LOADER = {
     '.py': os.path.join(TOOLS_DIR, 'python', 'loader.py'),
     '.php': os.path.join(TOOLS_DIR, 'php', 'loader.php'),
     '.js': os.path.join(TOOLS_DIR, 'javascript', 'loader.js'),
     '.ts': os.path.join(TOOLS_DIR, 'javascript', 'loader.js'),
 }
```

### Comparing `python-runit-0.2.1/runit/languages/__init__.py` & `python-runit-0.2.2/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/languages/multi.py` & `python-runit-0.2.2/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/languages/runtime.py` & `python-runit-0.2.2/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/modules/account.py` & `python-runit-0.2.2/runit/modules/account.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/runit.py` & `python-runit-0.2.2/runit/runit.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/templates/404.html` & `python-runit-0.2.2/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/templates/multi/application.py` & `python-runit-0.2.2/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/templates/python/application.py` & `python-runit-0.2.2/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/tools/php/runner.php` & `python-runit-0.2.2/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/runit/tools/python/runner.py` & `python-runit-0.2.2/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.1/setup.py` & `python-runit-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='python-runit',
     version=VERSION,
```

