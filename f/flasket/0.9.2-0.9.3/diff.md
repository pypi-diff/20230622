# Comparing `tmp/flasket-0.9.2.tar.gz` & `tmp/flasket-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flasket-0.9.2.tar", last modified: Sun Jan 29 23:22:45 2023, max compression
+gzip compressed data, was "flasket-0.9.3.tar", last modified: Mon Jan 30 08:29:25 2023, max compression
```

## Comparing `flasket-0.9.2.tar` & `flasket-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.008103 flasket-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-01-29 23:21:53.000000 flasket-0.9.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-01-29 23:21:53.000000 flasket-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2491 2023-01-29 23:22:45.008103 flasket-0.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-01-29 23:21:53.000000 flasket-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:44.997102 flasket-0.9.2/flasket/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.003103 flasket-0.9.2/flasket/api/
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/api/openapi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/api/x-responses.yml
--rw-rw-rw-   0 root         (0) root         (0)     4056 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/api/x-schemas.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.006103 flasket-0.9.2/flasket/backends/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/backends/_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5638 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/backends/api.py
--rw-rw-rw-   0 root         (0) root         (0)     5157 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/backends/dash.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/backends/static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.006103 flasket-0.9.2/flasket/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.007103 flasket-0.9.2/flasket/ext/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/ext/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10140 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/flasket.py
--rw-rw-rw-   0 root         (0) root         (0)     2496 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.008103 flasket-0.9.2/flasket/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/middleware/gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     4196 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/properties.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2023-01-29 23:21:53.000000 flasket-0.9.2/flasket/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 23:22:45.001103 flasket-0.9.2/flasket.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2491 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      781 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 23:22:44.000000 flasket-0.9.2/flasket.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     6739 2023-01-29 23:21:53.000000 flasket-0.9.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-29 23:21:53.000000 flasket-0.9.2/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-01-29 23:22:44.000000 flasket-0.9.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-29 23:22:45.008103 flasket-0.9.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1078 2023-01-29 23:21:53.000000 flasket-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.802744 flasket-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-01-30 08:28:38.000000 flasket-0.9.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-01-30 08:28:38.000000 flasket-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-01-30 08:29:25.802744 flasket-0.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-01-30 08:28:38.000000 flasket-0.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.794763 flasket-0.9.3/flasket/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.798753 flasket-0.9.3/flasket/api/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/api/openapi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/api/x-responses.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/api/x-schemas.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.800749 flasket-0.9.3/flasket/backends/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/backends/_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5638 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/backends/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/backends/dash.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/backends/static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.800749 flasket-0.9.3/flasket/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.801746 flasket-0.9.3/flasket/ext/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/ext/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10140 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/flasket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.802744 flasket-0.9.3/flasket/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/middleware/gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     4196 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2023-01-30 08:28:38.000000 flasket-0.9.3/flasket/templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 08:29:25.797756 flasket-0.9.3/flasket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      781 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 08:29:25.000000 flasket-0.9.3/flasket.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     6739 2023-01-30 08:28:38.000000 flasket-0.9.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-30 08:28:38.000000 flasket-0.9.3/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-01-30 08:29:25.000000 flasket-0.9.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-30 08:29:25.802744 flasket-0.9.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1078 2023-01-30 08:28:38.000000 flasket-0.9.3/setup.py
```

### Comparing `flasket-0.9.2/LICENSE` & `flasket-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/PKG-INFO` & `flasket-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasket
-Version: 0.9.2
+Version: 0.9.3
 Summary: A flask + connexion + dash ensemble to quickly deploy an app.
 Author-email: Julien Lecomte <julien@lecomte.at>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/jlecomte/python/flasket
 Project-URL: Documentation, https://jlecomte.gitlab.io/python/flasket/
 Project-URL: Source code, https://gitlab.com/jlecomte/python/flasket
 Project-URL: Bug tracker, https://gitlab.com/jlecomte/python/flasket/-/issues
```

### Comparing `flasket-0.9.2/README.md` & `flasket-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/_utils.py` & `flasket-0.9.3/flasket/_utils.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/api/x-responses.yml` & `flasket-0.9.3/flasket/api/x-responses.yml`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/api/x-schemas.yml` & `flasket-0.9.3/flasket/api/x-schemas.yml`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/backends/_backend.py` & `flasket-0.9.3/flasket/backends/_backend.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/backends/api.py` & `flasket-0.9.3/flasket/backends/api.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/backends/dash.py` & `flasket-0.9.3/flasket/backends/dash.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,47 +2,46 @@
 import typing as t
 
 from boltons.fileutils import iter_find_files
 from dash import Dash, html
 from dash import register_page as dash_register_page
 
 from ._backend import Backend
-
-
-def app_layout(layout):
-    if DashBackend._dash:
-        DashBackend._dash.layout = layout
-        DashBackend.layout = layout
-    else:
-        DashBackend.layout = layout
-
-
-def callback(*args, **kwargs):
-    def wrapper(fn):
-        DashBackend._callbacks += [(fn, args, kwargs)]
-
-    if DashBackend._dash:
-        print("Setting callback on live dash app xxx")
-    else:
-        print("Setting callback on empty dash app xxx")
-    return wrapper
-
-
-def register_page(*args, **kwargs):
-    # Nuke the app prefix
-    # prefix = DashBackend._prefix()
-    # path = kwargs["path"]
-    # path = path[len(prefix):]
-    # kwargs["path"] = path
-    DashBackend._registered_pages += [(args, kwargs)]
-
+###
+###
+###def app_layout(layout):
+###    if DashBackend._dash:
+###        DashBackend._dash.layout = layout
+###        DashBackend.layout = layout
+###    else:
+###        DashBackend.layout = layout
+###
+###
+###def callback(*args, **kwargs):
+###    def wrapper(fn):
+###        DashBackend._callbacks += [(fn, args, kwargs)]
+###
+###    if DashBackend._dash:
+###        print("Setting callback on live dash app xxx")
+###    else:
+###        print("Setting callback on empty dash app xxx")
+###    return wrapper
+###
+###
+###def register_page(*args, **kwargs):
+###    # Nuke the app prefix
+###    # prefix = DashBackend._prefix()
+###    # path = kwargs["path"]
+###    # path = path[len(prefix):]
+###    # kwargs["path"] = path
+###    DashBackend._registered_pages += [(args, kwargs)]
+###
+dash = None
 
 class DashBackend(Backend):
-    layout = html.Div()
-    _dash = None
     _callbacks = []
     _registered_pages = []
 
     @staticmethod
     def init_app(flasket, rootpath, options=None) -> "DashBackend":
         return DashBackend(flasket, rootpath, options)
 
@@ -78,15 +77,16 @@
         # Some settings can't be used together
         use_pages = options.get("use_pages", False)
         if use_pages:
             pages_folder = options.get("pages", "")
         else:
             pages_folder = None
 
-        self._dash = Dash(
+        global dash
+        dash = Dash(
             __name__,
             # url_base_pathname="/app/",
             # requests_pathname_prefix="/app/",
             routes_pathname_prefix="/app/",
             #
             assets_external_path=options.get("assets_external_path"),
             # assets_folder='assets',
@@ -108,18 +108,16 @@
             # server=True,
             # show_undo_redo=False,
             suppress_callback_exceptions=options.get("suppress_callback_exceptions", False),
             title=options.get("title", "Flasket"),
             update_title=options.get("update_title", ""),
             use_pages=use_pages,
         )
-        DashBackend._dash = self._dash
-        DashBackend._dash.layout = DashBackend.layout
 
-        self._flask = self._dash.server
+        self._flask = dash.server
         self.logger.info(f"Aplication is available at: {self.flasket.sitename}/app/")
 
     def _init_app_files(self) -> None:
         files = iter_find_files(self._rootpath, "*.py")
         files = sorted(set(files))
 
         # TODO: Load __init__.py only once, that means
@@ -133,17 +131,17 @@
             file = file[:-3]
             file = file.replace("/", ".")
             file = dirname + "." + file
             modules += [file]
 
         for module in modules:
             __import__(module, globals(), locals())
-            assert callable(
-                app_layout,
-            ), f"error: app_layout was set to a variable in module '{module}'. Use it as a function: app_layout(html...)"
+            ###assert callable(
+            ###    app_layout,
+            ###), f"error: app_layout was set to a variable in module '{module}'. Use it as a function: app_layout(html...)"
 
     def _init_decorators(self):
         def callback_wrapper(cb_fn, cb_args, cb_kwargs):
             @self._dash.callback(*cb_args, **cb_kwargs)
             def wrapper(*args, **kwargs):
                 print("Setting callback on saved dash app")
                 return cb_fn(*args, **kwargs)
```

### Comparing `flasket-0.9.2/flasket/backends/static.py` & `flasket-0.9.3/flasket/backends/static.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/clients/__init__.py` & `flasket-0.9.3/flasket/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/exceptions.py` & `flasket-0.9.3/flasket/exceptions.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/ext/celery.py` & `flasket-0.9.3/flasket/ext/celery.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/flasket.py` & `flasket-0.9.3/flasket/flasket.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/logger.py` & `flasket-0.9.3/flasket/logger.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/middleware/gunicorn.py` & `flasket-0.9.3/flasket/middleware/gunicorn.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/properties.py` & `flasket-0.9.3/flasket/properties.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket/templates.py` & `flasket-0.9.3/flasket/templates.py`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/flasket.egg-info/PKG-INFO` & `flasket-0.9.3/flasket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasket
-Version: 0.9.2
+Version: 0.9.3
 Summary: A flask + connexion + dash ensemble to quickly deploy an app.
 Author-email: Julien Lecomte <julien@lecomte.at>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/jlecomte/python/flasket
 Project-URL: Documentation, https://jlecomte.gitlab.io/python/flasket/
 Project-URL: Source code, https://gitlab.com/jlecomte/python/flasket
 Project-URL: Bug tracker, https://gitlab.com/jlecomte/python/flasket/-/issues
```

### Comparing `flasket-0.9.2/flasket.egg-info/SOURCES.txt` & `flasket-0.9.3/flasket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flasket-0.9.2/pyproject.toml` & `flasket-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # ------------------------------------------------------------------------------
 # Setup
 # ------------------------------------------------------------------------------
 [project]
 dynamic = ["dependencies"]
 
 name = "flasket"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   {name = "Julien Lecomte", email = "julien@lecomte.at"}
 ]
 readme  = "README.md"
 license = {text = "MIT"}
 description = "A flask + connexion + dash ensemble to quickly deploy an app."
```

### Comparing `flasket-0.9.2/setup.py` & `flasket-0.9.3/setup.py`

 * *Files identical despite different names*

