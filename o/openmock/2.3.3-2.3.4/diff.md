# Comparing `tmp/openmock-2.3.3.tar.gz` & `tmp/openmock-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmock-2.3.3.tar", max compression
+gzip compressed data, was "openmock-2.3.4.tar", max compression
```

## Comparing `openmock-2.3.3.tar` & `openmock-2.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-06-21 14:12:04.681585 openmock-2.3.3/LICENSE
--rw-r--r--   0        0        0     4946 2023-06-21 14:12:04.681585 openmock-2.3.3/README.md
--rw-r--r--   0        0        0      830 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/__init__.py
--rw-r--r--   0        0        0      121 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/behaviour/__init__.py
--rw-r--r--   0        0        0      475 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/behaviour/server_failure.py
--rw-r--r--   0        0        0     1100 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_cluster.py
--rw-r--r--   0        0        0     1179 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_indices.py
--rw-r--r--   0        0        0    40327 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_opensearch.py
--rw-r--r--   0        0        0     2154 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/normalize_hosts.py
--rw-r--r--   0        0        0      732 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/utilities/__init__.py
--rw-r--r--   0        0        0      451 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/utilities/decorator.py
--rw-r--r--   0        0        0     2302 2023-06-21 14:12:04.681585 openmock-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-22 18:20:37.913266 openmock-2.3.4/LICENSE
+-rw-r--r--   0        0        0     4946 2023-06-22 18:20:37.917266 openmock-2.3.4/README.md
+-rw-r--r--   0        0        0      830 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/behaviour/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/behaviour/server_failure.py
+-rw-r--r--   0        0        0     1100 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/fake_cluster.py
+-rw-r--r--   0        0        0     1179 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/fake_indices.py
+-rw-r--r--   0        0        0    40503 2023-06-22 18:21:15.781716 openmock-2.3.4/openmock/fake_opensearch.py
+-rw-r--r--   0        0        0     2154 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/normalize_hosts.py
+-rw-r--r--   0        0        0      732 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/utilities/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-22 18:20:37.917266 openmock-2.3.4/openmock/utilities/decorator.py
+-rw-r--r--   0        0        0     2302 2023-06-22 18:20:37.917266 openmock-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.4/PKG-INFO
```

### Comparing `openmock-2.3.3/LICENSE` & `openmock-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/README.md` & `openmock-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/openmock/__init__.py` & `openmock-2.3.4/openmock/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/openmock/fake_cluster.py` & `openmock-2.3.4/openmock/fake_cluster.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/openmock/fake_indices.py` & `openmock-2.3.4/openmock/fake_indices.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/openmock/fake_opensearch.py` & `openmock-2.3.4/openmock/fake_opensearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,17 @@
     def _compare_value_for_field(self, doc_source, field, value, ignore_case):
         if ignore_case and isinstance(value, str):
             value = value.lower()
 
         doc_val = doc_source
         # Remove boosting
         field, *_ = field.split("*")
+        # Remove ".keyword"
+        exact_search = field.lower().endswith(".keyword")
+        field = field[: -len(".keyword")] if exact_search else field
         for k in field.split("."):
             if hasattr(doc_val, k):
                 doc_val = getattr(doc_val, k)
             elif k in doc_val:
                 doc_val = doc_val[k]
             else:
                 return False
@@ -335,15 +338,15 @@
             if not isinstance(val, (int, float, complex)) or val is None:
                 val = str(val)
                 if ignore_case:
                     val = val.lower()
 
             if value == val:
                 return True
-            if isinstance(val, str) and str(value) in val:
+            if isinstance(val, str) and str(value) in val and not exact_search:
                 return True
 
         return False
 
 
 @for_all_methods([server_failure])
 class FakeOpenSearch(OpenSearch):
```

### Comparing `openmock-2.3.3/openmock/normalize_hosts.py` & `openmock-2.3.4/openmock/normalize_hosts.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/openmock/utilities/__init__.py` & `openmock-2.3.4/openmock/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.3/pyproject.toml` & `openmock-2.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmock"
-version = "2.3.3"
+version = "2.3.4"
 description = "Python OpenSearch Mock for test purposes"
 authors = ["Marcos Cardoso",
     "Mathew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["opensearch", "mocking", "testing"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matthewdeanmartin/openmock"
```

### Comparing `openmock-2.3.3/PKG-INFO` & `openmock-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmock
-Version: 2.3.3
+Version: 2.3.4
 Summary: Python OpenSearch Mock for test purposes
 Home-page: https://github.com/matthewdeanmartin/openmock
 License: MIT
 Keywords: opensearch,mocking,testing
 Author: Marcos Cardoso
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
```

