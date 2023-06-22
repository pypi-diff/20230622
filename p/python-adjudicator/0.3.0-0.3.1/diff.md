# Comparing `tmp/python_adjudicator-0.3.0.tar.gz` & `tmp/python_adjudicator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.3.0.tar", max compression
+gzip compressed data, was "python_adjudicator-0.3.1.tar", max compression
```

## Comparing `python_adjudicator-0.3.0.tar` & `python_adjudicator-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,31 @@
--rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.3.0/LICENSE
--rw-r--r--   0        0        0     3862 2023-06-21 23:01:08.385844 python_adjudicator-0.3.0/README.md
--rw-r--r--   0        0        0     2048 2023-06-21 23:01:41.788080 python_adjudicator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2119 2023-06-21 22:55:41.840466 python_adjudicator-0.3.0/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3214 2023-06-21 22:55:41.841814 python_adjudicator-0.3.0/src/adjudicator/Executor.py
--rw-r--r--   0        0        0     1530 2023-06-21 22:55:41.842426 python_adjudicator-0.3.0/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     7246 2023-06-21 22:55:41.842936 python_adjudicator-0.3.0/src/adjudicator/Params.py
--rw-r--r--   0        0        0     1054 2023-06-21 22:55:41.843369 python_adjudicator-0.3.0/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     5978 2023-06-21 22:55:41.844148 python_adjudicator-0.3.0/src/adjudicator/RuleEngine.py
--rw-r--r--   0        0        0     2741 2023-06-21 22:55:41.844722 python_adjudicator-0.3.0/src/adjudicator/RuleEngine_test.py
--rw-r--r--   0        0        0     5460 2023-06-21 22:55:41.845250 python_adjudicator-0.3.0/src/adjudicator/RuleGraph.py
--rw-r--r--   0        0        0     3932 2023-06-21 22:55:41.845569 python_adjudicator-0.3.0/src/adjudicator/RuleGraph_test.py
--rw-r--r--   0        0        0      426 2023-06-21 22:55:41.847616 python_adjudicator-0.3.0/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      800 2023-06-21 23:01:41.788376 python_adjudicator-0.3.0/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1462 2023-06-21 22:55:41.848771 python_adjudicator-0.3.0/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-06-21 22:55:41.849105 python_adjudicator-0.3.0/src/adjudicator/py.typed
--rw-r--r--   0        0        0     6856 2023-06-21 22:56:10.537884 python_adjudicator-0.3.0/src/adjudicator/rule.py
--rw-r--r--   0        0        0      824 2023-06-21 22:56:15.991531 python_adjudicator-0.3.0/src/adjudicator/rule_test.py
--rw-r--r--   0        0        0     4609 1970-01-01 00:00:00.000000 python_adjudicator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5517 2023-06-22 09:40:19.907406 python_adjudicator-0.3.1/README.md
+-rw-r--r--   0        0        0     2063 2023-06-22 09:40:48.863984 python_adjudicator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2119 2023-06-21 22:55:41.840466 python_adjudicator-0.3.1/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3214 2023-06-21 22:55:41.841814 python_adjudicator-0.3.1/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-06-21 22:55:41.842426 python_adjudicator-0.3.1/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     7246 2023-06-21 22:55:41.842936 python_adjudicator-0.3.1/src/adjudicator/Params.py
+-rw-r--r--   0        0        0     1054 2023-06-21 22:55:41.843369 python_adjudicator-0.3.1/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     5978 2023-06-21 22:55:41.844148 python_adjudicator-0.3.1/src/adjudicator/RuleEngine.py
+-rw-r--r--   0        0        0     2741 2023-06-21 22:55:41.844722 python_adjudicator-0.3.1/src/adjudicator/RuleEngine_test.py
+-rw-r--r--   0        0        0     5460 2023-06-21 22:55:41.845250 python_adjudicator-0.3.1/src/adjudicator/RuleGraph.py
+-rw-r--r--   0        0        0     3932 2023-06-21 22:55:41.845569 python_adjudicator-0.3.1/src/adjudicator/RuleGraph_test.py
+-rw-r--r--   0        0        0      426 2023-06-21 22:55:41.847616 python_adjudicator-0.3.1/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      800 2023-06-22 09:40:48.864130 python_adjudicator-0.3.1/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-21 22:55:41.848771 python_adjudicator-0.3.1/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:42:08.569908 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-22 09:40:16.485223 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/__main__.py
+-rw-r--r--   0        0        0      427 2023-06-22 08:56:18.386086 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/context.py
+-rw-r--r--   0        0        0        5 2023-06-22 09:37:17.112389 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/__init__.py
+-rw-r--r--   0        0        0      984 2023-06-22 08:56:18.831781 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/generic.py
+-rw-r--r--   0        0        0     2359 2023-06-22 08:56:18.835613 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/include.py
+-rw-r--r--   0        0        0     2187 2023-06-22 09:36:35.218361 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/parser.py
+-rw-r--r--   0        0        0     1931 2023-06-22 09:17:26.944389 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/runcmd.py
+-rw-r--r--   0        0        0     1754 2023-06-22 09:38:53.088581 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/directives/toc.py
+-rw-r--r--   0        0        0      994 2023-06-22 09:14:20.231315 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/goals.py
+-rw-r--r--   0        0        0      330 2023-06-22 08:57:06.993692 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/readfile.py
+-rw-r--r--   0        0        0     1063 2023-06-22 08:56:39.404224 python_adjudicator-0.3.1/src/adjudicator/examples/readmesync/targets.py
+-rw-r--r--   0        0        0        0 2023-06-21 22:55:41.849105 python_adjudicator-0.3.1/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     6856 2023-06-21 22:56:10.537884 python_adjudicator-0.3.1/src/adjudicator/rule.py
+-rw-r--r--   0        0        0      824 2023-06-21 22:56:15.991531 python_adjudicator-0.3.1/src/adjudicator/rule_test.py
+-rw-r--r--   0        0        0     6264 1970-01-01 00:00:00.000000 python_adjudicator-0.3.1/PKG-INFO
```

### Comparing `python_adjudicator-0.3.0/LICENSE` & `python_adjudicator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/README.md` & `python_adjudicator-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 __Table of Contents__
 
 <!-- table of contents -->
 * [Quickstart](#quickstart)
 * [Installation](#installation)
 * [Future Extensions](#future-extensions)
+* [Add-on: ReadmeSync](#add-on-readmesync)
+  * [Synopsis](#synopsis)
 <!-- end table of contents -->
 
 ## Quickstart
 
 The following example shows how to use Adjudicator to implement a simple "Hello World" application. The rule engine
 invokes the `say_hello()` production rule because a `HelloResponse` is requested and a `HelloRequest` is provided,
 which matches the rule's signature.
@@ -58,18 +60,18 @@
 engine = RuleEngine()
 engine.load_module(__name__)
 response = engine.get(HelloResponse, Params(HelloRequest(name="World")))
 print(response.greeting)
 ```
 <!-- end include -->
 
-A more complex example can be found in the [examples/update_readme.py](examples/update_readme.py) file. That script
-is actually used to keep this README file up to date with the example and the table of contents above. It demonstrates
-how to use the rule engine to generate a file based on a set of rules, leveraging union memberships and rule result
-caching.
+A more complex example can be found in [src/adjudicator/examples/readmesync](src/adjudicator/examples/readmesync)
+directory. That script is actually used to keep this README file up to date with the example and the table of contents
+above. It demonstrates how to use the rule engine to generate a file based on a set of rules, leveraging union
+memberships and rule result caching.
 
 ## Installation
 
 Adjudicator is available on PyPI. You need at least Python 3.10.
 
 ```bash
 pip install python-adjudicator
@@ -77,7 +79,43 @@
 
 ## Future Extensions
 
 * Currently the rule graph stores rules as connections between types and rules on edges. A more efficient
   representation would be the one illustrated above, where types are connected to rules which are connected to types.
 * The ability to mark facts as required to be consumed. If such a fact is not consumed during the execution of a
   request, an error will be raised.
+
+## Add-on: ReadmeSync
+
+The `python-adjudicator` package includes functionality to keep the content of a `README.md` file up to date by
+placing inline comments into the file that follow a certain syntax. In fact, the same utility is used to keep this
+readme file up to date with the example code and the table of contents.
+
+### Synopsis
+
+<!-- runcmd code: python -m adjudicator.examples.readmesync --help -->
+```
+usage: python -m adjudicator.examples.readmesync [-h] [--preview] [--verbose]
+                                                 [file]
+
+ReadmeSync is a utility that allows you to place comments into a Markdown file that represent
+directives for content to be included in their place. The following types of directives are
+supported:
+
+- `<!-- include <path> -->`: Include the contents of the file at the given path. A `code:<lang>`
+    option can be added to the directive to wrap the content in a code block using the specified
+    language name (can be empty).
+- `<!-- runcmd <command> -->`: Run the given command and include the output in the document. A
+    `code:<lang>` option can be added to the directive to wrap the output in a code block using
+    the specified language name (can be empty).
+- `<!-- table of contents -->`: Include a table of contents for the document for all Markdown
+    headers following the directive.
+
+positional arguments:
+  file           [default: README.md]
+
+options:
+  -h, --help     show this help message and exit
+  --preview, -p  run in preview mode
+  --verbose, -v  enable verbose logging
+```
+<!-- end runcmd -->
```

### Comparing `python_adjudicator-0.3.0/pyproject.toml` & `python_adjudicator-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
@@ -50,15 +50,20 @@
 isort  = "isort --check-only examples/ src/ tests/ --extend-skip examples/hello.py"
 mypy   = "dmypy run examples/ src/"
 pycln  = "pycln examples/ src/ tests/ --check"
 pytest = "pytest src/ tests/ -vv --doctest-modules"
 
 [tool.slap.run]
 "docs:build" = ">&2 echo 'Not implemented' && exit 1"
-fmt          = "pycln src/ tests/ examples/ && black src/ tests/ examples/ --exclude examples/hello.py && isort src/ tests/ examples/ --extend-skip examples/hello.py && python examples/update_readme.py"
+fmt          = """
+pycln src/ tests/ examples/ &&
+black src/ tests/ examples/ --exclude examples/hello.py &&
+isort src/ tests/ examples/ --extend-skip examples/hello.py &&
+python -m adjudicator.examples.readmesync
+"""
 
 [tool.mypy]
 python_version = "3.10"
 explicit_package_bases = true
 mypy_path = ["src"]
 namespace_packages = true
 pretty = true
```

### Comparing `python_adjudicator-0.3.0/src/adjudicator/Cache.py` & `python_adjudicator-0.3.1/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/Executor.py` & `python_adjudicator-0.3.1/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/HashSupport.py` & `python_adjudicator-0.3.1/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/Params.py` & `python_adjudicator-0.3.1/src/adjudicator/Params.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/Params_test.py` & `python_adjudicator-0.3.1/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/RuleEngine.py` & `python_adjudicator-0.3.1/src/adjudicator/RuleEngine.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/RuleEngine_test.py` & `python_adjudicator-0.3.1/src/adjudicator/RuleEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/RuleGraph.py` & `python_adjudicator-0.3.1/src/adjudicator/RuleGraph.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/RuleGraph_test.py` & `python_adjudicator-0.3.1/src/adjudicator/RuleGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/__init__.py` & `python_adjudicator-0.3.1/src/adjudicator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     "RuleGraph",
     "RuleResolveError",
     "union_rule",
     "union",
     "UnionRule",
 ]
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `python_adjudicator-0.3.0/src/adjudicator/errors.py` & `python_adjudicator-0.3.1/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/rule.py` & `python_adjudicator-0.3.1/src/adjudicator/rule.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/src/adjudicator/rule_test.py` & `python_adjudicator-0.3.1/src/adjudicator/rule_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.0/PKG-INFO` & `python_adjudicator-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -45,14 +45,16 @@
 
 __Table of Contents__
 
 <!-- table of contents -->
 * [Quickstart](#quickstart)
 * [Installation](#installation)
 * [Future Extensions](#future-extensions)
+* [Add-on: ReadmeSync](#add-on-readmesync)
+  * [Synopsis](#synopsis)
 <!-- end table of contents -->
 
 ## Quickstart
 
 The following example shows how to use Adjudicator to implement a simple "Hello World" application. The rule engine
 invokes the `say_hello()` production rule because a `HelloResponse` is requested and a `HelloRequest` is provided,
 which matches the rule's signature.
@@ -77,18 +79,18 @@
 engine = RuleEngine()
 engine.load_module(__name__)
 response = engine.get(HelloResponse, Params(HelloRequest(name="World")))
 print(response.greeting)
 ```
 <!-- end include -->
 
-A more complex example can be found in the [examples/update_readme.py](examples/update_readme.py) file. That script
-is actually used to keep this README file up to date with the example and the table of contents above. It demonstrates
-how to use the rule engine to generate a file based on a set of rules, leveraging union memberships and rule result
-caching.
+A more complex example can be found in [src/adjudicator/examples/readmesync](src/adjudicator/examples/readmesync)
+directory. That script is actually used to keep this README file up to date with the example and the table of contents
+above. It demonstrates how to use the rule engine to generate a file based on a set of rules, leveraging union
+memberships and rule result caching.
 
 ## Installation
 
 Adjudicator is available on PyPI. You need at least Python 3.10.
 
 ```bash
 pip install python-adjudicator
@@ -97,7 +99,43 @@
 ## Future Extensions
 
 * Currently the rule graph stores rules as connections between types and rules on edges. A more efficient
   representation would be the one illustrated above, where types are connected to rules which are connected to types.
 * The ability to mark facts as required to be consumed. If such a fact is not consumed during the execution of a
   request, an error will be raised.
 
+## Add-on: ReadmeSync
+
+The `python-adjudicator` package includes functionality to keep the content of a `README.md` file up to date by
+placing inline comments into the file that follow a certain syntax. In fact, the same utility is used to keep this
+readme file up to date with the example code and the table of contents.
+
+### Synopsis
+
+<!-- runcmd code: python -m adjudicator.examples.readmesync --help -->
+```
+usage: python -m adjudicator.examples.readmesync [-h] [--preview] [--verbose]
+                                                 [file]
+
+ReadmeSync is a utility that allows you to place comments into a Markdown file that represent
+directives for content to be included in their place. The following types of directives are
+supported:
+
+- `<!-- include <path> -->`: Include the contents of the file at the given path. A `code:<lang>`
+    option can be added to the directive to wrap the content in a code block using the specified
+    language name (can be empty).
+- `<!-- runcmd <command> -->`: Run the given command and include the output in the document. A
+    `code:<lang>` option can be added to the directive to wrap the output in a code block using
+    the specified language name (can be empty).
+- `<!-- table of contents -->`: Include a table of contents for the document for all Markdown
+    headers following the directive.
+
+positional arguments:
+  file           [default: README.md]
+
+options:
+  -h, --help     show this help message and exit
+  --preview, -p  run in preview mode
+  --verbose, -v  enable verbose logging
+```
+<!-- end runcmd -->
+
```

