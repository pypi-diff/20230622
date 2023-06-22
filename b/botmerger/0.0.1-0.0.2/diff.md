# Comparing `tmp/botmerger-0.0.1.tar.gz` & `tmp/botmerger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botmerger-0.0.1.tar", max compression
+gzip compressed data, was "botmerger-0.0.2.tar", max compression
```

## Comparing `botmerger-0.0.1.tar` & `botmerger-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1079 2023-05-20 19:54:52.435984 botmerger-0.0.1/LICENSE
--rw-r--r--   0        0        0     2088 2023-06-22 06:28:22.493013 botmerger-0.0.1/README.md
--rw-r--r--   0        0        0      533 2023-06-20 18:36:34.559558 botmerger-0.0.1/botmerger/__init__.py
--rw-r--r--   0        0        0    10173 2023-06-20 18:36:34.560532 botmerger-0.0.1/botmerger/base.py
--rw-r--r--   0        0        0    11578 2023-06-20 18:36:34.561088 botmerger-0.0.1/botmerger/core.py
--rw-r--r--   0        0        0     1017 2023-06-20 18:36:34.561493 botmerger-0.0.1/botmerger/errors.py
--rw-r--r--   0        0        0        0 2023-06-20 18:36:34.561562 botmerger-0.0.1/botmerger/experimental/__init__.py
--rw-r--r--   0        0        0      464 2023-06-20 18:36:34.562351 botmerger-0.0.1/botmerger/experimental/inquiry_bot.py
--rw-r--r--   0        0        0        0 2023-06-20 18:36:34.562427 botmerger-0.0.1/botmerger/ext/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-20 18:58:55.311347 botmerger-0.0.1/botmerger/ext/discord_integration.py
--rw-r--r--   0        0        0     5921 2023-06-20 18:36:34.563650 botmerger-0.0.1/botmerger/models.py
--rw-r--r--   0        0        0      507 2023-06-20 18:36:34.564717 botmerger-0.0.1/botmerger/utils.py
--rw-r--r--   0        0        0      644 2023-06-20 18:36:34.567970 botmerger-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 botmerger-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-20 19:54:52.435984 botmerger-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2088 2023-06-22 06:28:22.493013 botmerger-0.0.2/README.md
+-rw-r--r--   0        0        0      533 2023-06-20 18:36:34.559558 botmerger-0.0.2/botmerger/__init__.py
+-rw-r--r--   0        0        0    10173 2023-06-20 18:36:34.560532 botmerger-0.0.2/botmerger/base.py
+-rw-r--r--   0        0        0    11578 2023-06-20 18:36:34.561088 botmerger-0.0.2/botmerger/core.py
+-rw-r--r--   0        0        0     1017 2023-06-20 18:36:34.561493 botmerger-0.0.2/botmerger/errors.py
+-rw-r--r--   0        0        0        0 2023-06-20 18:36:34.561562 botmerger-0.0.2/botmerger/experimental/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-20 18:54:31.461740 botmerger-0.0.2/botmerger/experimental/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1077 2023-06-20 18:54:31.464345 botmerger-0.0.2/botmerger/experimental/__pycache__/inquiry_bot.cpython-311.pyc
+-rw-r--r--   0        0        0      464 2023-06-20 18:36:34.562351 botmerger-0.0.2/botmerger/experimental/inquiry_bot.py
+-rw-r--r--   0        0        0        0 2023-06-20 18:36:34.562427 botmerger-0.0.2/botmerger/ext/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-20 18:54:31.465977 botmerger-0.0.2/botmerger/ext/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4679 2023-06-20 19:12:41.813523 botmerger-0.0.2/botmerger/ext/__pycache__/discord_integration.cpython-311.pyc
+-rw-r--r--   0        0        0     3456 2023-06-20 18:58:55.311347 botmerger-0.0.2/botmerger/ext/discord_integration.py
+-rw-r--r--   0        0        0     5921 2023-06-20 18:36:34.563650 botmerger-0.0.2/botmerger/models.py
+-rw-r--r--   0        0        0      507 2023-06-20 18:36:34.564717 botmerger-0.0.2/botmerger/utils.py
+-rw-r--r--   0        0        0      673 2023-06-22 08:15:51.645087 botmerger-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 botmerger-0.0.2/PKG-INFO
```

### Comparing `botmerger-0.0.1/LICENSE` & `botmerger-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/README.md` & `botmerger-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/__init__.py` & `botmerger-0.0.2/botmerger/__init__.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/base.py` & `botmerger-0.0.2/botmerger/base.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/core.py` & `botmerger-0.0.2/botmerger/core.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/errors.py` & `botmerger-0.0.2/botmerger/errors.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/ext/discord_integration.py` & `botmerger-0.0.2/botmerger/ext/discord_integration.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/botmerger/models.py` & `botmerger-0.0.2/botmerger/models.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.1/pyproject.toml` & `botmerger-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "botmerger"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 readme = "README.md"
+include = ["botmerger/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"  # TODO extend this to older versions too
 pydantic = "^1"
 
 [tool.poetry.dev-dependencies]
 black = "*"
```

### Comparing `botmerger-0.0.1/PKG-INFO` & `botmerger-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botmerger
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
```

