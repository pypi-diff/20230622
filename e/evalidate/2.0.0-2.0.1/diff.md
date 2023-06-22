# Comparing `tmp/evalidate-2.0.0.tar.gz` & `tmp/evalidate-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-2.0.0.tar", last modified: Wed Jun 21 16:19:19 2023, max compression
+gzip compressed data, was "evalidate-2.0.1.tar", last modified: Thu Jun 22 14:47:46 2023, max compression
```

## Comparing `evalidate-2.0.0.tar` & `evalidate-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12056 2023-06-21 16:19:19.914970 evalidate-2.0.0/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     9286 2023-06-21 16:05:39.000000 evalidate-2.0.0/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4103 2023-06-21 15:16:03.000000 evalidate-2.0.0/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 16:18:12.000000 evalidate-2.0.0/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12056 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-2.0.0/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-21 16:19:19.914970 evalidate-2.0.0/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:03:02.000000 evalidate-2.0.0/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12026 2023-06-22 14:47:46.245852 evalidate-2.0.1/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     9256 2023-06-21 21:43:38.000000 evalidate-2.0.1/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/evalidate/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4083 2023-06-22 14:44:37.000000 evalidate-2.0.1/evalidate/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 21:43:38.000000 evalidate-2.0.1/evalidate/security.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/evalidate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12026 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-08-10 17:45:22.000000 evalidate-2.0.1/evalidate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-22 14:47:46.245852 evalidate-2.0.1/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:42:59.000000 evalidate-2.0.1/setup.py
```

### Comparing `evalidate-2.0.0/PKG-INFO` & `evalidate-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 2.0.0
+Version: 2.0.1
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
@@ -59,23 +59,24 @@
         
         
         ## Exceptions
         Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
         inherit from base exception class `EvalException`.
         
         ## Configure validation
-        Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
+        Evalidate is very flexible, depending on security model, same code can either pass validation or raise exception.
         
-        
-        ### EvalModel - using custom security model
-        EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
+        EvalModel is security model class for eval - lists of allowed AST nodes, function calls, attributes and dict of imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
         
         You can create custom empty model (and extend it later):
+        ~~~python
         my_model = evalidate.EvalModel()
-        (nothing is allowed by default, even `1+2` will not be considered as safe code)
+        ~~~
+        
+        (nothing is allowed by default, even `1+2` will not be considered safe)
         
         or you may start from `base_eval_mode` and extend it:
         ~~~python
         from evalidate import Expr, base_eval_model
         
         my_model = base_eval_model.clone()
         my_model.nodes.append('Mult')
@@ -90,19 +91,18 @@
         my_model.allowed_functions.append('int')
         
         Expr('int(36.6)', model=my_model).eval()
         ~~~
         
         Or, to call attributes:
         ~~~python
-        m = evalidate.base_eval_model.clone()
+        m = base_eval_model.clone()
         m.nodes.extend(['Call', 'Attribute'])
         m.attributes.append('startswith')
         
-        
         src = '"abcdef".startswith("abc")'
         r = evalidate.Expr(src, model=m).eval()
         ~~~
         
         But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
```

### Comparing `evalidate-2.0.0/README.md` & `evalidate-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,23 +51,24 @@
 
 
 ## Exceptions
 Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
 inherit from base exception class `EvalException`.
 
 ## Configure validation
-Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
+Evalidate is very flexible, depending on security model, same code can either pass validation or raise exception.
 
-
-### EvalModel - using custom security model
-EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
+EvalModel is security model class for eval - lists of allowed AST nodes, function calls, attributes and dict of imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
 
 You can create custom empty model (and extend it later):
+~~~python
 my_model = evalidate.EvalModel()
-(nothing is allowed by default, even `1+2` will not be considered as safe code)
+~~~
+
+(nothing is allowed by default, even `1+2` will not be considered safe)
 
 or you may start from `base_eval_mode` and extend it:
 ~~~python
 from evalidate import Expr, base_eval_model
 
 my_model = base_eval_model.clone()
 my_model.nodes.append('Mult')
@@ -82,19 +83,18 @@
 my_model.allowed_functions.append('int')
 
 Expr('int(36.6)', model=my_model).eval()
 ~~~
 
 Or, to call attributes:
 ~~~python
-m = evalidate.base_eval_model.clone()
+m = base_eval_model.clone()
 m.nodes.extend(['Call', 'Attribute'])
 m.attributes.append('startswith')
 
-
 src = '"abcdef".startswith("abc")'
 r = evalidate.Expr(src, model=m).eval()
 ~~~
 
 But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
```

### Comparing `evalidate-2.0.0/evalidate/__init__.py` & `evalidate-2.0.1/evalidate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Safe user-supplied python expression evaluation."""
 
 import ast
 import dataclasses
 from typing import Callable
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 
 class EvalException(Exception):
     pass
 
 
 class ValidationException(EvalException):
@@ -30,18 +30,18 @@
         super().__init__(exc)
         self.exc = exc
 
 
 @dataclasses.dataclass
 class EvalModel:
     """ eval security model """
-    nodes: list[str]
-    allowed_functions: list[str] = dataclasses.field(default_factory=list)
-    imported_functions: dict[str] = dataclasses.field(default_factory=dict)
-    attributes: list[str] = dataclasses.field(default_factory=list)
+    nodes: list
+    allowed_functions: list = dataclasses.field(default_factory=list)
+    imported_functions: dict = dataclasses.field(default_factory=dict)
+    attributes: list = dataclasses.field(default_factory=list)
 
     def clone(self):
         return EvalModel(**dataclasses.asdict(self))
 
 
 class SafeAST(ast.NodeVisitor):
```

### Comparing `evalidate-2.0.0/evalidate/security.py` & `evalidate-2.0.1/evalidate/security.py`

 * *Files identical despite different names*

### Comparing `evalidate-2.0.0/evalidate.egg-info/PKG-INFO` & `evalidate-2.0.1/evalidate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 2.0.0
+Version: 2.0.1
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
@@ -59,23 +59,24 @@
         
         
         ## Exceptions
         Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
         inherit from base exception class `EvalException`.
         
         ## Configure validation
-        Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
+        Evalidate is very flexible, depending on security model, same code can either pass validation or raise exception.
         
-        
-        ### EvalModel - using custom security model
-        EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
+        EvalModel is security model class for eval - lists of allowed AST nodes, function calls, attributes and dict of imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
         
         You can create custom empty model (and extend it later):
+        ~~~python
         my_model = evalidate.EvalModel()
-        (nothing is allowed by default, even `1+2` will not be considered as safe code)
+        ~~~
+        
+        (nothing is allowed by default, even `1+2` will not be considered safe)
         
         or you may start from `base_eval_mode` and extend it:
         ~~~python
         from evalidate import Expr, base_eval_model
         
         my_model = base_eval_model.clone()
         my_model.nodes.append('Mult')
@@ -90,19 +91,18 @@
         my_model.allowed_functions.append('int')
         
         Expr('int(36.6)', model=my_model).eval()
         ~~~
         
         Or, to call attributes:
         ~~~python
-        m = evalidate.base_eval_model.clone()
+        m = base_eval_model.clone()
         m.nodes.extend(['Call', 'Attribute'])
         m.attributes.append('startswith')
         
-        
         src = '"abcdef".startswith("abc")'
         r = evalidate.Expr(src, model=m).eval()
         ~~~
         
         But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
```

### Comparing `evalidate-2.0.0/setup.py` & `evalidate-2.0.1/setup.py`

 * *Files identical despite different names*

