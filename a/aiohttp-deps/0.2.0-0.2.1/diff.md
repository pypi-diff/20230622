# Comparing `tmp/aiohttp_deps-0.2.0.tar.gz` & `tmp/aiohttp_deps-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.2.0.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.2.1.tar", max compression
```

## Comparing `aiohttp_deps-0.2.0.tar` & `aiohttp_deps-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/LICENSE
--rw-r--r--   0        0        0     7669 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/README.md
--rw-r--r--   0        0        0      497 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3202 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     9363 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/swagger.py
--rw-r--r--   0        0        0     9138 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1317 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1763 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 aiohttp_deps-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8540 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/README.md
+-rw-r--r--   0        0        0      497 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0     9363 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0     9138 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1385 2023-06-22 13:26:41.636729 aiohttp_deps-0.2.1/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1763 2023-06-22 13:26:41.636729 aiohttp_deps-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9652 1970-01-01 00:00:00.000000 aiohttp_deps-0.2.1/PKG-INFO
```

### Comparing `aiohttp_deps-0.2.0/LICENSE` & `aiohttp_deps-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.0/README.md` & `aiohttp_deps-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -310,7 +310,39 @@
 
 
 @router.get("/view/{var}")
 async def my_handler(var: str = Depends(Path())):
     return web.json_response({"var": var})
 
 ```
+
+
+## Overridiing dependencies
+
+Sometimes for tests you don't want to calculate actual functions
+and you want to pass another functions instead.
+
+To do so, you can add "dependency_overrides" key to the aplication.
+It's a dict that is passed as additional context to dependency resolvers.
+
+Here's an example.
+
+```python
+def original_dep() -> int:
+    return 1
+
+class MyView(View):
+    async def get(self, num: int = Depends(original_dep)):
+        """Nothing."""
+        return web.json_response({"request": num})
+```
+
+Imagine you have a handler that depends on some function,
+but instead of `1` you want to have `2` in your tests.
+
+To do it, jsut add `dependency_overrides` somewhere,
+where you create your application. And make sure that keys
+of that dict are actual function that are being replaced.
+
+```python
+    my_app["dependency_overrides"] = {original_dep: 2}
+```
```

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/initializer.py` & `aiohttp_deps-0.2.1/aiohttp_deps/initializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         :param request: current request.
         :return: response.
         """
         async with self.graph.async_ctx(
             {
                 web.Request: request,
                 web.Application: request.app,
+                **request.app.get("dependency_overrides", {}),
             },
         ) as resolver:
             return await self.original_handler(**(await resolver.resolve_kwargs()))
 
 
 class InjectableViewHandler:
     """
```

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/router.py` & `aiohttp_deps-0.2.1/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/router.pyi` & `aiohttp_deps-0.2.1/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/swagger.py` & `aiohttp_deps-0.2.1/aiohttp_deps/swagger.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/utils.py` & `aiohttp_deps-0.2.1/aiohttp_deps/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.0/aiohttp_deps/view.py` & `aiohttp_deps-0.2.1/aiohttp_deps/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,10 +39,11 @@
         )
         if method is None:
             self._raise_allowed_methods()
         async with self._graph_map[self.request.method.lower()].async_ctx(
             {
                 web.Request: self.request,
                 web.Application: self.request.app,
+                **self.request.app.get("dependency_overrides", {}),
             },
         ) as ctx:
             return await method(**(await ctx.resolve_kwargs()))  # type: ignore
```

### Comparing `aiohttp_deps-0.2.0/pyproject.toml` & `aiohttp_deps-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aiohttp_deps-0.2.0/PKG-INFO` & `aiohttp_deps-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
@@ -341,7 +341,39 @@
 
 @router.get("/view/{var}")
 async def my_handler(var: str = Depends(Path())):
     return web.json_response({"var": var})
 
 ```
 
+
+## Overridiing dependencies
+
+Sometimes for tests you don't want to calculate actual functions
+and you want to pass another functions instead.
+
+To do so, you can add "dependency_overrides" key to the aplication.
+It's a dict that is passed as additional context to dependency resolvers.
+
+Here's an example.
+
+```python
+def original_dep() -> int:
+    return 1
+
+class MyView(View):
+    async def get(self, num: int = Depends(original_dep)):
+        """Nothing."""
+        return web.json_response({"request": num})
+```
+
+Imagine you have a handler that depends on some function,
+but instead of `1` you want to have `2` in your tests.
+
+To do it, jsut add `dependency_overrides` somewhere,
+where you create your application. And make sure that keys
+of that dict are actual function that are being replaced.
+
+```python
+    my_app["dependency_overrides"] = {original_dep: 2}
+```
+
```

