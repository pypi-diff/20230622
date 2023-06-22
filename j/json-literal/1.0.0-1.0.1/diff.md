# Comparing `tmp/json_literal-1.0.0.tar.gz` & `tmp/json_literal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_literal-1.0.0.tar", max compression
+gzip compressed data, was "json_literal-1.0.1.tar", max compression
```

## Comparing `json_literal-1.0.0.tar` & `json_literal-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-22 00:25:55.912255 json_literal-1.0.0/README.md
--rw-r--r--   0        0        0      464 2023-06-22 00:25:55.912255 json_literal-1.0.0/json_literal/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-22 00:25:55.912255 json_literal-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 json_literal-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      344 2023-06-22 00:32:39.725506 json_literal-1.0.1/README.md
+-rw-r--r--   0        0        0      464 2023-06-22 00:32:39.725506 json_literal-1.0.1/json_literal/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-22 00:32:39.725506 json_literal-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 json_literal-1.0.1/PKG-INFO
```

### Comparing `json_literal-1.0.0/pyproject.toml` & `json_literal-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-literal"
-version = "1.0.0"
+version = "1.0.1"
 description = "Definition of literal values for compatibility with JSON data."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "json_literal" }]
 license = "BSD-3-Clause"
 classifiers = [
     "Development Status :: 4 - Beta",
```

