# Comparing `tmp/py_jokes_py-1.0.1.tar.gz` & `tmp/py_jokes_py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_jokes_py-1.0.1.tar", max compression
+gzip compressed data, was "py_jokes_py-1.1.1.tar", max compression
```

## Comparing `py_jokes_py-1.0.1.tar` & `py_jokes_py-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-06 15:44:39.537549 py_jokes_py-1.0.1/LICENSE
--rw-r--r--   0        0        0      158 2023-06-22 11:47:45.369484 py_jokes_py-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-06 09:37:15.914283 py_jokes_py-1.0.1/jokes/__init__.py
--rw-r--r--   0        0        0     1735 2023-06-22 08:12:36.991867 py_jokes_py-1.0.1/jokes/jokes.py
--rw-r--r--   0        0        0     2152 2023-06-22 12:05:50.095754 py_jokes_py-1.0.1/jokes/jokesv2.py
--rw-r--r--   0        0        0      885 2023-06-22 12:08:00.454776 py_jokes_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 py_jokes_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/LICENSE
+-rw-r--r--   0        0        0      158 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/jokes/__init__.py
+-rw-r--r--   0        0        0     4519 2023-06-22 13:34:18.699884 py_jokes_py-1.1.1/jokes/jokes.py
+-rw-r--r--   0        0        0     5262 2023-06-22 13:47:46.200233 py_jokes_py-1.1.1/jokes/jokesv2.py
+-rw-r--r--   0        0        0      886 2023-06-22 13:56:00.940498 py_jokes_py-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 py_jokes_py-1.1.1/PKG-INFO
```

### Comparing `py_jokes_py-1.0.1/LICENSE` & `py_jokes_py-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.0.1/pyproject.toml` & `py_jokes_py-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "py-jokes-py"
-version = "1.0.1"
-description = "Python wrapper for the dad jokes API provided by icanhazdadjokes.com"
+version = "1.1.1"
+description = "Python wrapper for jokes APIs provided by icanhazdadjokes.com and jokeapi.dev"
 authors = ["Freedom Loisa <kitakayaloisa@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jokes"}]
-homepage = "https://github.com/LoisaKitakaya/dad-jokes"
-documentation = "https://github.com/LoisaKitakaya/dad-jokes#readme"
+homepage = "https://github.com/LoisaKitakaya/Jokes"
+documentation = "https://github.com/LoisaKitakaya/Jokes#readme"
 keywords = ["python", "jokes", "api", "dad jokes"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
-pytest = "^7.3.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_jokes_py-1.0.1/PKG-INFO` & `py_jokes_py-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: py-jokes-py
-Version: 1.0.1
-Summary: Python wrapper for the dad jokes API provided by icanhazdadjokes.com
-Home-page: https://github.com/LoisaKitakaya/dad-jokes
+Version: 1.1.1
+Summary: Python wrapper for jokes APIs provided by icanhazdadjokes.com and jokeapi.dev
+Home-page: https://github.com/LoisaKitakaya/Jokes
 Keywords: python,jokes,api,dad jokes
 Author: Freedom Loisa
 Author-email: kitakayaloisa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://github.com/LoisaKitakaya/dad-jokes#readme
+Project-URL: Documentation, https://github.com/LoisaKitakaya/Jokes#readme
 Description-Content-Type: text/markdown
 
 # dad_jokes
 
 Python wrapper for the jokes APIs provided by:
 
 - [icanhazdadjokes.com](https://icanhazdadjoke.com/)
```

