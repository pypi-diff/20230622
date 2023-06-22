# Comparing `tmp/engorgio-0.2.0.tar.gz` & `tmp/engorgio-0.3.0.tar.gz`

## Comparing `engorgio-0.2.0.tar` & `engorgio-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.2.0/.pydantic-typer-copier-answers.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 engorgio-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 engorgio-0.2.0/docs/tutorial.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/__about__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/condense.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/decorator.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/expand.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/person.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/person_cli.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/models.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_expand.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_hero.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_no_model.py
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_person.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.2.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 engorgio-0.2.0/README.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 engorgio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 engorgio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.3.0/.pydantic-typer-copier-answers.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 engorgio-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 engorgio-0.3.0/docs/tutorial.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 engorgio-0.3.0/engorgio/__about__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 engorgio-0.3.0/engorgio/__init__.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 engorgio-0.3.0/engorgio/condense.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 engorgio-0.3.0/engorgio/decorator.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 engorgio-0.3.0/engorgio/expand.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.3.0/examples/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 engorgio-0.3.0/examples/person.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 engorgio-0.3.0/examples/person_cli.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/models.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/test_expand.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/test_hero.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/test_no_model.py
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 engorgio-0.3.0/tests/test_person.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 engorgio-0.3.0/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 engorgio-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 engorgio-0.3.0/PKG-INFO
```

### Comparing `engorgio-0.2.0/docs/tutorial.md` & `engorgio-0.3.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/engorgio/condense.py` & `engorgio-0.3.0/engorgio/condense.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 
 def get_kwargs_for_param(
     param: inspect.Parameter,
     kwargs: Dict,
     model_separator: str = "__",
 ):
     """Get kwargs for the param from the dict of kwargs."""
-    param_kwargs = {}
     min_kwargs = 2
     model_kwargs = {k: v for k, v in kwargs.items() if len(k.split("__")) >= min_kwargs}
-    param_kwargs = {
+    return {
         k.split(model_separator)[-1]: v
         for k, v in model_kwargs.items()
         if k.split(model_separator)[-2] == param.name
     }
-    return param_kwargs
 
 
 def expand_param(
     param: inspect.Parameter,
     kwargs: Dict[str, Any],
     models: Optional[Dict[str, str]] = None,
     model_separator: str = "__",
```

### Comparing `engorgio-0.2.0/engorgio/decorator.py` & `engorgio-0.3.0/engorgio/decorator.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/engorgio/expand.py` & `engorgio-0.3.0/engorgio/expand.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     return None
 
 
 def get_more_args(
     func: Callable,
     model_separator: str = "__",
     *,
-    include_parent_model: bool = None,
+    include_parent_model: Optional[bool] = None,
     more_args: Optional[Dict] = None,
 ) -> Dict:
     """Get the more_args dict."""
     if more_args is None:
         more_args = {}
     more_args, parents = init_more_args(
         func=func,
```

### Comparing `engorgio-0.2.0/examples/person_cli.py` & `engorgio-0.3.0/examples/person_cli.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/tests/models.py` & `engorgio-0.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/tests/test_expand.py` & `engorgio-0.3.0/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/tests/test_hero.py` & `engorgio-0.3.0/tests/test_hero.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/tests/test_no_model.py` & `engorgio-0.3.0/tests/test_no_model.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/tests/test_person.py` & `engorgio-0.3.0/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/.gitignore` & `engorgio-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/LICENSE.txt` & `engorgio-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/README.md` & `engorgio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `engorgio-0.2.0/pyproject.toml` & `engorgio-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+  "black",
   "rich",
   "textual",
   "typer",
   "pydantic",
   "anyconfig"
 ]
 dynamic = ["version"]
```

### Comparing `engorgio-0.2.0/PKG-INFO` & `engorgio-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engorgio
-Version: 0.2.0
+Version: 0.3.0
 Summary: Expand pydantic function arguments by casting the engorgio decorator
 Project-URL: Documentation, https://github.com/waylonwalker/engorgio#readme
 Project-URL: Issues, https://github.com/waylonwalker/engorgio/issues
 Project-URL: Source, https://github.com/waylonwalker/engorgio
 Project-URL: Changelog, https://github.com/WaylonWalker/engorgio/blob/main/CHANGELOG.md
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: anyconfig
+Requires-Dist: black
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: textual
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # engorgio
```

