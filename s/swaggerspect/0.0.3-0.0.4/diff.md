# Comparing `tmp/swaggerspect-0.0.3.tar.gz` & `tmp/swaggerspect-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swaggerspect-0.0.3.tar", last modified: Thu Jun 15 13:56:13 2023, max compression
+gzip compressed data, was "dist/swaggerspect-0.0.4.tar", last modified: Thu Jun 22 10:57:23 2023, max compression
```

## Comparing `swaggerspect-0.0.3.tar` & `swaggerspect-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      513 2023-06-15 13:55:40.000000 swaggerspect-0.0.3/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.3/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    10488 2023-06-15 13:02:50.000000 swaggerspect-0.0.3/swaggerspect/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 12:42:58.000000 swaggerspect-0.0.3/swaggerspect/test.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        9 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      251 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1498 2023-06-15 07:56:31.000000 swaggerspect-0.0.3/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      513 2023-06-22 10:56:43.000000 swaggerspect-0.0.4/setup.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.4/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/setup.cfg
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    11895 2023-06-22 10:56:14.000000 swaggerspect-0.0.4/swaggerspect/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 12:42:58.000000 swaggerspect-0.0.4/swaggerspect/test.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        9 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      251 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2037 2023-06-16 07:24:49.000000 swaggerspect-0.0.4/README.md
```

### Comparing `swaggerspect-0.0.3/setup.py` & `swaggerspect-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name='swaggerspect',
-    version='0.0.3',
+    version='0.0.4',
     description='',
     long_description="""Introspects python classes and functions and generates swagger style documentation objects.""",
     long_description_content_type="text/markdown",
     author='Egil Moeller',
     author_email='em@emrld.no',
     url='https://github.com/emerald-geomodelling/swaggerspect',
     packages=setuptools.find_packages(),
```

### Comparing `swaggerspect-0.0.3/LICENSE` & `swaggerspect-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swaggerspect-0.0.3/swaggerspect/__init__.py` & `swaggerspect-0.0.4/swaggerspect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import numpydoc.docscrape
 import ast
 import typing
+import types
 import importlib.metadata
 
 def _get_name(obj):
     if obj is None: return None
     if obj is typing.Any: return 'typing.Any'
     return obj.__module__ + "." + obj.__name__
 
@@ -28,34 +29,46 @@
 }
 
 def typeof(v):
     if v is None: return None
     if v is inspect._empty: return None
     return type(v)
 
-def make_type_schema(*typenames):
+def make_type_schema(*typenames, hasdefault=False):
     for typename in typenames:
-        orig = repr(typename)
         if typename is inspect._empty:
             continue
         if typename is None:
             continue
+
+        orig = repr(typename)
+        schema = {}
         args = None
         metadatas = None
         if not isinstance(typename, str):
             if isinstance(typename, typing._AnnotatedAlias):
                 metadatas = typename.__metadata__
                 typename = typename.__args__[0]
-            args = typing.get_args(typename)
-            typename = _get_name(typename)
+            if isinstance(typename, typing._LiteralGenericAlias):
+                schema["enum"] = list(typing.get_args(typename))
+                typename = _get_name(type(schema["enum"][0]))
+            else:
+                if hasattr(typename, "json_schema"):
+                    metadatas = [typename]
+                args = typing.get_args(typename)
+                typename = _get_name(typename)
 
         pytypename = typename
-        typename = typemap.get(typename, "object")
+        typename = typemap.get(typename)
 
-        schema = {}
+        if typename is None:
+            typename = "object"
+            if typeof(hasdefault) is not None:
+                schema["hide"] = True
+        
         if typename is not None:
             schema["type"] = typename
             schema["x-python-type"] = pytypename
             #schema["x-python-orig"] = orig
             if schema["type"] == "array" and args:
                 schema["items"] = make_type_schema(args[0])
             elif schema["type"] == "object" and args:
@@ -74,15 +87,15 @@
 
 def make_value_schema(*values):
     for value in values:
         if value is inspect._empty:
             continue
         if value is None:
             continue
-        if isinstance(value, (int, str, dict, list, bool)):
+        if isinstance(value, (int, str, float, dict, list, bool)):
             return {"default": value}
     return {}
 
 def _merge_list(a, b):
     akeys = [p["name"] for p in a]
     bkeys = [p["name"] for p in b]
     params = merge({p["name"]: p for p in a}, {p["name"]: p for p in b})
@@ -131,102 +144,103 @@
 
     return propdocs
 
 def get_class_api_parameters_comments(cls):
     return [{"name": n, "in": "query", "description": v} for n, v in _get_class_property_comments(cls).items()]
 
 def get_class_api_parameters_inspect(cls):
-    return [{"name": n, "in": "query", "schema": {} if v is None else merge(make_type_schema(typeof(v)), make_value_schema(v))}
+    return [{"name": n, "in": "query", "schema": {} if v is None else merge(make_type_schema(typeof(v), hasdefault=v), make_value_schema(v))}
             for n, v in inspect.getmembers(cls)
             if (not n.startswith('__')
                 and not inspect.ismethod(v)
                 and not inspect.isfunction(v)
                 and not inspect.isdatadescriptor(v))]
     
 def get_class_api_parameters_typing(cls):
     return [{"name": k, "in": "query", "schema": make_type_schema(t)} for k, t in typing.get_type_hints(cls).items()]
 
 def get_class_api(cls):
-    args = merge(get_class_api_parameters_typing(cls),
-                 merge(get_class_api_parameters_inspect(cls),
-                       get_class_api_parameters_comments(cls)))
+    args = remove_hidden(
+        merge(get_class_api_parameters_typing(cls),
+              merge(get_class_api_parameters_inspect(cls),
+                    get_class_api_parameters_comments(cls))))
     return {
         "operationId": _get_name(cls),
         "description": inspect.getdoc(cls),
         "parameters": args,
         "responses": {"default":
                       {"description": _get_name(cls),
                        "content": {
                            "application/json": {"schema": make_type_schema(cls)}}}}}
 
 def remove_hidden(api):
     return [param for param in api
             if not param.get("schema", {}).get("hide", False)]
     
 def get_function_api_parameters_inspect(fn):
-    return remove_hidden(
-        [remove_empty({"name": k,
-                       "in": "query",
-                       "schema": merge(
-                           make_type_schema(v.annotation, typeof(v.default)),
-                           make_value_schema(v.default))})
-         for k, v in inspect.signature(fn).parameters.items()])
+    return [remove_empty({"name": k,
+                          "in": "query",
+                          "schema": merge(
+                              make_type_schema(v.annotation, typeof(v.default), hasdefault=v.default),
+                              make_value_schema(v.default))})
+            for k, v in inspect.signature(fn).parameters.items()]
 
 def get_function_api_parameters_comments(fn):
     docs = inspect.getdoc(fn)
     if docs is None: return []
     docast = numpydoc.docscrape.NumpyDocString(docs)
     
     return [{"name": p.name,
              "in": "query",
              "description": "\n".join(p.desc),
              "schema": make_type_schema(p.type)}
             for p in docast["Parameters"]]
     
-def get_function_api(fn):
-    args = merge(get_function_api_parameters_inspect(fn),
-                 get_function_api_parameters_comments(fn)) 
+def get_function_api(fn, name = None):
+    args = remove_hidden(
+        merge(get_function_api_parameters_inspect(fn),
+              get_function_api_parameters_comments(fn)))
 
     docs = inspect.getdoc(fn)
     description = _get_name(fn)
     if docs is not None:
         docast = numpydoc.docscrape.NumpyDocString(docs)
         description = "\n".join(docast["Summary"] + docast["Extended Summary"])
 
     returntype = inspect.signature(fn).return_annotation
         
     return {
-        "operationId": _get_name(fn),
+        "operationId": name or _get_name(fn),
         "description": description,
         "parameters": args,
         "responses": {"default":
-                      {"description": _get_name(fn),
+                      {"description": name or _get_name(fn),
                        "content": {
                            "application/json": remove_empty({
                                "schema": make_type_schema(returntype)})}}}}
 
-def get_api(obj):
+def get_api(obj, name = None):
     """Generate a swagger specification fragment for a single function
     call or class instantiation."""
     if type(obj) is type:
         return get_class_api(obj)
     elif inspect.isfunction(obj):
-        return get_function_api(obj)
+        return get_function_api(obj, name=name)
     return None
 
-def get_apis_dict(objs):
+def get_apis_dict(objs, local_names = False):
     return {
         "openapi": '3.0.3',
         "info": {"title": "unknown",
                  "version": "1.0",
                  "description": "unknown"},
         "paths": {
             "/" + k: {"get": v}
             for k, v in
-            [(k, get_api(v))
+            [(k, get_api(v, name = k if local_names else None))
              for k, v in objs.items()]
             if v
         }}
 
 def get_apis_entrypoints(group):
     entrypoints = importlib.metadata.entry_points()
     if group not in entrypoints: return {}
@@ -240,25 +254,45 @@
     
 def get_apis_module(module):
     if isinstance(module, str):
         try:
             module = importlib.import_module(module)
         except:
             return {}
+    if not isinstance(module, types.ModuleType):
+        return {}
     docs = get_apis_dict({name: getattr(module, name)
                          for name in dir(module)
                          if not name.startswith("__")})
     docs["info"] = {"title": module.__name__,
                     "version": "1.0",
                     "description": inspect.getdoc(module) or module.__name__}
     return docs
 
+def get_apis_class(cls):
+    if isinstance(cls, str):
+        try:
+            module, name = cls.rsplit(".", 1)
+            cls = getattr(importlib.import_module(module), name)
+        except:
+            return {}
+    if not isinstance(cls, type):
+        return {}
+    docs = get_apis_dict({name: getattr(cls, name)
+                          for name in dir(cls)
+                          if not name.startswith("__")},
+                         local_names=True)
+    docs["info"] = {"title": _get_name(cls),
+                    "version": "1.0",
+                    "description": inspect.getdoc(cls) or cls.__name__}
+    return docs
+
 def get_apis(objs):
     """Generates a swagger specification for module or entry point group."""
-    return merge(get_apis_module(objs), get_apis_entrypoints(objs))
+    return merge(merge(get_apis_module(objs), get_apis_entrypoints(objs)), get_apis_class(objs))
 
 def swagger_to_json_schema(api, multi = True):
     """Converts a swagger specification into a JSON schema for either
     a single function call serialized as
 
     {"function.name": {"argname1": "value1", ... "argnameN": "valueN"}}
```

