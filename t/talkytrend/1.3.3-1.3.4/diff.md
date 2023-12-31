# Comparing `tmp/talkytrend-1.3.3.tar.gz` & `tmp/talkytrend-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.3.3.tar", max compression
+gzip compressed data, was "talkytrend-1.3.4.tar", max compression
```

## Comparing `talkytrend-1.3.3.tar` & `talkytrend-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-21 21:00:37.315259 talkytrend-1.3.3/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-21 21:00:37.315259 talkytrend-1.3.3/README.md
--rw-r--r--   0        0        0     2178 2023-06-21 21:00:38.159267 talkytrend-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-21 21:00:38.159267 talkytrend-1.3.3/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-21 21:00:37.315259 talkytrend-1.3.3/talkytrend/config.py
--rw-r--r--   0        0        0      932 2023-06-21 21:00:37.315259 talkytrend-1.3.3/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6121 2023-06-21 21:00:37.319259 talkytrend-1.3.3/talkytrend/main.py
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-22 07:48:01.032185 talkytrend-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-22 07:48:01.032185 talkytrend-1.3.4/README.md
+-rw-r--r--   0        0        0     2178 2023-06-22 07:48:01.736192 talkytrend-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-22 07:48:01.736192 talkytrend-1.3.4/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-22 07:48:01.032185 talkytrend-1.3.4/talkytrend/config.py
+-rw-r--r--   0        0        0      932 2023-06-22 07:48:01.032185 talkytrend-1.3.4/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6121 2023-06-22 07:48:01.032185 talkytrend-1.3.4/talkytrend/main.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.3.4/PKG-INFO
```

### Comparing `talkytrend-1.3.3/LICENSE` & `talkytrend-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.3/README.md` & `talkytrend-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.3/pyproject.toml` & `talkytrend-1.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.3.3"
+version = "1.3.4"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.3.3/talkytrend/config.py` & `talkytrend-1.3.4/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.3/talkytrend/default_settings.toml` & `talkytrend-1.3.4/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.3/talkytrend/main.py` & `talkytrend-1.3.4/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.3/PKG-INFO` & `talkytrend-1.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.3.3
+Version: 1.3.4
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

