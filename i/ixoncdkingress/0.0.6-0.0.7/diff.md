# Comparing `tmp/ixoncdkingress-0.0.6.tar.gz` & `tmp/ixoncdkingress-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixoncdkingress-0.0.6.tar", last modified: Thu Apr 13 13:38:45 2023, max compression
+gzip compressed data, was "ixoncdkingress-0.0.7.tar", last modified: Thu Jun 22 09:01:13 2023, max compression
```

## Comparing `ixoncdkingress-0.0.6.tar` & `ixoncdkingress-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.040094 ixoncdkingress-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-13 13:38:45.040094 ixoncdkingress-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-13 13:38:11.000000 ixoncdkingress-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.028094 ixoncdkingress-0.0.6/ixoncdkingress/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.032094 ixoncdkingress-0.0.6/ixoncdkingress/cbc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/cbc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/cbc/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/cbc/caller.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/cbc/context.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.040094 ixoncdkingress-0.0.6/ixoncdkingress/webserver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6027 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6398 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/servlet.py
--rw-rw-rw-   0 root         (0) root         (0)     5362 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/ixoncdkingress/webserver/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.028094 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-13 13:38:44.000000 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      683 2023-04-13 13:38:45.000000 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:38:44.000000 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-13 13:38:44.000000 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 13:38:44.000000 ixoncdkingress-0.0.6/ixoncdkingress.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:38:45.040094 ixoncdkingress-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-04-13 13:38:44.000000 ixoncdkingress-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:38:45.040094 ixoncdkingress-0.0.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/tests/test___main__.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-13 09:55:32.000000 ixoncdkingress-0.0.6/tests/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/cbc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/caller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2547 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/context.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/webserver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4208 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7398 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4445 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/servlet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test___main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test_utils.py
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/__main__.py` & `ixoncdkingress-0.0.7/ixoncdkingress/__main__.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/cbc/api_client.py` & `ixoncdkingress-0.0.7/ixoncdkingress/cbc/api_client.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/cbc/context.py` & `ixoncdkingress-0.0.7/ixoncdkingress/cbc/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """
 Context.
 """
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Set
 
 from ixoncdkingress.cbc.api_client import ApiClient
 
 class CbcIxapiResource:
     """
     Describes an IXAPI resource.
     """
     public_id: str
     name: str
     custom_properties: Dict[str, Any]
+    permissions: Optional[Set[str]]
 
-    def __init__(self, public_id: str, name: str, custom_properties: Dict[str, Any]) -> None:
+    def __init__(
+            self,
+            public_id: str,
+            name: str,
+            custom_properties: Dict[str, Any],
+            permissions: Optional[Set[str]]
+        ) -> None:
         self.public_id = public_id
         self.name = name
         self.custom_properties = custom_properties
+        self.permissions = permissions
 
     def __repr__(self) -> str:
         return (
             '<CbcResource'
             f' public_id={self.public_id},'
             f' name={self.name},'
             f' custom_properties={repr(self.custom_properties)},'
+            f' permissions={repr(self.permissions)},'
             f'>'
         )
 
 class CbcContext:
     """
     The context for a backend component.
     """
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/types.py` & `ixoncdkingress-0.0.7/ixoncdkingress/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,12 +37,13 @@
     """
     HTTP response codes to return
     """
     OK = 200
     NO_CONTENT = 204
     BAD_REQUEST = 400
     METHOD_NOT_ALLOWED = 405
+    INTERNAL_ERROR = 500
     NOT_AVAILABLE = 503
 
     def status_line(self) -> str:
         """Produces a HTTP status line: <status-code> <message>"""
         return f"{self.value} {self.name.replace('_', ' ')}"
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/webserver/config.py` & `ixoncdkingress-0.0.7/ixoncdkingress/webserver/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,35 +51,28 @@
 
         res.version = load_str_file(environ.get('VERSION_PATH'), 'dev')
 
         res.cbc_path = environ.get('CBC_PATH', '/user_scripts')
 
         res.api_client_base_url = environ.get('API_CLIENT_BASE_URL', 'https://api.ayayot.com/')
 
-        res.context_config = {}
-        if not res.production_mode:
-            res.context_config = load_json_file(
-                environ.get('CONTEXT_CONFIG_PATH', './context_config.json'), {}
-            )
-
         return res
 
     production_mode: bool
 
     http_server_bind: str
     http_server_port: int
     wsgi_provider: WsgiProvider
 
     logger_log_level: Union[int, str]
     logger_format: str
 
     version: str
     cbc_path: str
     api_client_base_url: str
-    context_config: Dict[str, str]
 
     _logger: Optional[Logger]
 
     def __init__(self) -> None:
         self._logger = None
 
     def get_logger(self) -> Logger:
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/webserver/form.py` & `ixoncdkingress-0.0.7/ixoncdkingress/webserver/form.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 HTML form generator
 """
-from typing import Optional, Dict, Tuple, TYPE_CHECKING
+from typing import Optional, Dict, Set, Tuple, TYPE_CHECKING
 from urllib.parse import parse_qs
 
 from ixoncdkingress.cbc.api_client import ApiClient
 from ixoncdkingress.cbc.context import CbcContext, CbcIxapiResource
 from ixoncdkingress.types import FunctionLocation, FunctionArguments
 from ixoncdkingress.webserver.config import Config
 from ixoncdkingress.webserver.utils import parse_function_location
@@ -49,24 +49,24 @@
                        value=pre_fill.get('function'))
             with div(class_name='arguments'):
                 h3('Function input')
                 _custom_properties(pre_fill, prefix='function_args__')
 
             with div(class_name='resource'):
                 h3('User')
-                _resource(pre_fill, prefix='user__')
+                _resource(pre_fill, prefix='user__', show_permission=False)
             with div(class_name='resource'):
                 h3('Company')
-                _resource(pre_fill, prefix='company__')
+                _resource(pre_fill, prefix='company__', show_permission=True)
             with div(class_name='resource'):
                 h3('Asset')
-                _resource(pre_fill, prefix='asset__')
+                _resource(pre_fill, prefix='asset__', show_permission=True)
             with div(class_name='resource'):
                 h3('Agent')
-                _resource(pre_fill, prefix='agent__')
+                _resource(pre_fill, prefix='agent__', show_permission=True)
 
             input_(type='submit', value='Run function')
             input_(type='reset', value='Clear form')
 
         h3('Function output')
         textarea(form_output or 'Function output goes here', rows='10', cols='80')
 
@@ -88,15 +88,30 @@
                     td(input_(type='text', name=f'{prefix}key{i}', id=f'{prefix}key{i}',
                               size='16', value=pre_fill.get(f'{prefix}key{i}')))
                     td(input_(type='text', name=f'{prefix}value{i}', id=f'{prefix}value{i}',
                               size='32', value=pre_fill.get(f'{prefix}value{i}')))
 
     return table_tag
 
-def _resource(pre_fill: Dict[str, str], prefix: str) -> 'tags.html_tag':
+def _permissions(pre_fill: Dict[str, str], prefix: str) -> 'tags.html_tag':
+    """
+    Generates a form fragment for permissions.
+    """
+    table_tag = table()
+
+    with table_tag:
+        with tbody():
+            for i in range(0, 9):
+                with tr():
+                    td(input_(type='text', name=f'{prefix}value{i}', id=f'{prefix}value{i}',
+                              size='32', value=pre_fill.get(f'{prefix}value{i}')))
+
+    return table_tag
+
+def _resource(pre_fill: Dict[str, str], prefix: str, show_permission: bool) -> 'tags.html_tag':
     """
     Generates a form fragment for a context resource.
     """
     table_tag = table()
 
     with table_tag:
         with tbody():
@@ -108,33 +123,38 @@
                 td(label('Name', _for=f'{prefix}name'))
                 td(input_(type='text', id=f'{prefix}name', name=f'{prefix}name', size='32',
                           value=pre_fill.get(f'{prefix}name')))
             with tr():
                 td('Custom properties')
                 td(_custom_properties(pre_fill, f'{prefix}custom_properties__'))
 
+            if show_permission:
+                td('Permissions')
+                td(_permissions(pre_fill, f'{prefix}permissions__'))
+
     return table_tag
 
 def parse_form_input(
         config: Config,
+        context_config: Dict[str, str],
         body: str) -> Tuple[CbcContext, FunctionLocation, FunctionArguments]:
     """
     Parses an application/x-www-form-urlencoded request body string into a context, function
     location and function arguments.
     """
 
     in_put = parse_qs(body)
 
     context = CbcContext(
-        config.context_config,
+        context_config,
         api_client=ApiClient(config.api_client_base_url),
-        user=_parse_resource('user__', in_put),
-        company=_parse_resource('company__', in_put),
-        asset=_parse_resource('asset__', in_put),
-        agent=_parse_resource('agent__', in_put)
+        user=_parse_resource('user__', in_put, False),
+        company=_parse_resource('company__', in_put, True),
+        asset=_parse_resource('asset__', in_put, True),
+        agent=_parse_resource('agent__', in_put, True)
     )
 
     function_location = parse_function_location(in_put.get('function', [''])[0])
     function_arguments = _parse_function_args(in_put)
 
     return context, function_location, function_arguments
 
@@ -144,24 +164,40 @@
     while in_put.get(f'function_args__key{i}') and in_put.get(f'function_args__value{i}'):
         function_arguments[in_put[f'function_args__key{i}'][0]] = \
             in_put[f'function_args__value{i}'][0]
         i += 1
 
     return function_arguments
 
-def _parse_resource(prefix: str, in_put: dict[str, list[str]]) -> Optional[CbcIxapiResource]:
+def _parse_resource(
+        prefix: str,
+        in_put: dict[str, list[str]],
+        has_permissions: bool
+    ) -> Optional[CbcIxapiResource]:
     """
     Reads a resource description from the in_put and returns it as a CbcResource.
     """
     props = {}
+    permissions: Optional[Set[str]] = None
     if not in_put.get(f'{prefix}public_id') or not in_put.get(f'{prefix}name'):
         return None
 
-    i = 0
+    prop_iterator = 0
     prop_prefix = f'{prefix}custom_properties__'
-    while in_put.get(f'{prop_prefix}key{i}') and in_put.get(f'{prop_prefix}value{i}'):
-        props[in_put[f'{prop_prefix}key{i}'][0]] = in_put[f'{prop_prefix}value{i}'][0]
-        i += 1
+    while (in_put.get(f'{prop_prefix}key{prop_iterator}')
+           and in_put.get(f'{prop_prefix}value{prop_iterator}')):
+        permission = in_put[f'{prop_prefix}value{prop_iterator}'][0]
+        props[in_put[f'{prop_prefix}key{prop_iterator}'][0]] = permission
+        prop_iterator += 1
+
+    if has_permissions:
+        permissions = set()
+        permission_iterator = 0
+        permission_prefix = f'{prefix}permissions__'
+        while in_put.get(f'{permission_prefix}value{permission_iterator}'):
+            permissions.add(in_put[f'{permission_prefix}value{permission_iterator}'][0])
+            permission_iterator += 1
 
     return CbcIxapiResource(in_put[f'{prefix}public_id'][0],
                             in_put[f'{prefix}name'][0],
-                            props)
+                            props,
+                            permissions)
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/webserver/servlet.py` & `ixoncdkingress-0.0.7/ixoncdkingress/webserver/servlet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,25 @@
 """CBC servlet module."""
-from http.cookies import SimpleCookie
-from typing import Tuple, Optional, Dict, Any, Iterable, TYPE_CHECKING
+from typing import Tuple, Dict
 
+import os
 import json
-from urllib.parse import parse_qs
 
+from ixoncdkingress.utils import handle_exception
 from ixoncdkingress.cbc.caller import call_cbc
+from ixoncdkingress.webserver.config import load_json_file
 from ixoncdkingress.cbc.context import CbcContext
+from ixoncdkingress.webserver.config import Config
 from ixoncdkingress.webserver.form import generate_form, parse_form_input
+from ixoncdkingress.webserver.response import Response
+from ixoncdkingress.webserver.request import Request
 from ixoncdkingress.webserver.utils import read_qs_as_dict, parse_json_input
 
-from ixoncdkingress.types import ResponseCode, ContentType, FunctionLocation, FunctionArguments, \
-    RequestMethod
-
-from ixoncdkingress.webserver.config import Config
-
-if TYPE_CHECKING:
-    # pylint: disable=E0401,E0611
-    from _typeshed.wsgi import WSGIEnvironment, StartResponse
-
-class Request:
-    """
-    Represents an HTTP request, containing headers and optionally a body
-    """
-    body: Optional[Dict[str, Any]]
-    config: Config
-    content_type: Optional[ContentType]
-    cookies: Optional[SimpleCookie[str]]
-    request_body: bytes
-    request_method: RequestMethod
-
-    def __init__(self, config: Config, environ: 'WSGIEnvironment') -> None:
-        self.config = config
-        self.request_method = RequestMethod(environ['REQUEST_METHOD'])
-        self.body = None
-
-        if cookies_env := environ.get('HTTP_COOKIE'):
-            self.cookies = SimpleCookie(cookies_env)
-        else:
-            self.cookies = None
-
-        try:
-            request_body_size = int(environ.get('CONTENT_LENGTH', 0))
-            self.request_body = environ['wsgi.input'].read(request_body_size)
-        except ValueError:
-            self.request_body = b''
-
-        try:
-            self.content_type = ContentType(environ['CONTENT_TYPE'])
-        except (KeyError, ValueError):
-            self.content_type = None
-
-    def parse_body(self) -> None:
-        """
-        Parses the request body according to the `content_type`.
-
-        Must only be called once.
-        """
-        assert self.body is None
-
-        if ContentType.FORM == self.content_type:
-            self.body = parse_qs(self.request_body.decode('utf-8'))
-        elif ContentType.JSON == self.content_type:
-            self.body = json.loads(self.request_body)
-        else:
-            raise NotImplementedError()
-
-class Response:
-    """
-    Represents an HTTP response, containing headers and a body
-    """
-    body: Optional[bytes]
-    content_type: Optional[ContentType]
-    cookie: dict[str, str]
-    headers: list[tuple[str, str]]
-    start_response: 'StartResponse'
-    status_code: ResponseCode
-
-    def __init__(self, start_response: 'StartResponse') -> None:
-        self.body = None
-        self.content_type = None
-        self.cookie = {}
-        self.headers = []
-        self.start_response = start_response
-        self.status_code = ResponseCode.OK
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Iterable[bytes]:
-        headers = [*self.headers, *[('Set-Cookie', f'{k}={v}') for (k,v) in self.cookie.items()]]
-
-        if self.content_type:
-            headers.insert(0, ('Content-Type', f'{self.content_type.value}; charset=utf-8'))
-
-        self.start_response(self.status_code.status_line(), headers)
-
-        if self.body:
-            return [self.body]
+from ixoncdkingress.types import ResponseCode, ContentType, FunctionLocation, FunctionArguments
 
-        return []
-
-    def set_body(self, body: bytes) -> None:
-        """
-        Sets the body of the response
-        """
-        self.body = body
 
 class Servlet:
     """Servlet handling CBC calls."""
     config: Config
 
     def __init__(self, config: Config) -> None:
         self.config = config
@@ -145,24 +58,44 @@
         response.set_body(bytes(generate_form(pre_fill), 'utf-8'))
 
     def do_post(self, request: Request, response: Response) -> None:
         """
         Handle a POST request
         """
         available_content_types = [ContentType.JSON]
+
+        context_config = {}
+
         if not self.config.production_mode:
             # Only JSON requests are allowed in production mode
             available_content_types.append(ContentType.FORM)
+            try:
+                context_config = load_json_file(
+                    os.environ.get('CONTEXT_CONFIG_PATH', './context_config.json'), {}
+                )
+            except json.JSONDecodeError as exception:
+                handle_exception(exception, response)
+                return
+
+            logger = self.config.get_logger()
+            logger.info(
+                'Default context.config: %s', context_config
+            )
 
         if request.content_type not in available_content_types:
             raise NotImplementedError()
 
         out_put = call_cbc(
-            self.config,
-            *(self._parse_body(request.request_body, request.content_type)))
+                self.config,
+                *(self._parse_body(request.request_body, request.content_type, context_config)),
+                response
+            )
+
+        if response.status_code == ResponseCode.INTERNAL_ERROR:
+            return
 
         if ContentType.FORM == request.content_type:
             pre_fill = read_qs_as_dict(request.request_body)
             response.set_body(
                 bytes(generate_form(pre_fill, json.dumps(out_put, indent=4)), 'utf-8')
             )
             response.content_type = ContentType.HTML
@@ -171,21 +104,22 @@
             response.set_body(bytes(json.dumps(out_put), 'utf-8'))
             response.content_type = request.content_type
             response.headers.append(('Access-Control-Allow-Origin', '*'))
 
     def _parse_body(
         self,
         in_put: bytes,
-        content_type: ContentType
+        content_type: ContentType,
+        context_config: Dict[str, str],
     ) -> Tuple[CbcContext, FunctionLocation, FunctionArguments]:
         """
         Parses the request body to a key-value dictionary.
         """
         body = in_put.decode('utf-8')
 
         if content_type == ContentType.FORM:
-            return parse_form_input(self.config, body)
+            return parse_form_input(self.config, context_config, body)
 
         if content_type == ContentType.JSON:
-            return parse_json_input(self.config, body)
+            return parse_json_input(self.config, context_config, body)
 
         raise NotImplementedError()
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/webserver/utils.py` & `ixoncdkingress-0.0.7/ixoncdkingress/webserver/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,39 +54,47 @@
 
         # accessToken is not a CbcIxapiResource because it doesn't have
         # a publicId, name and custom field.
         if context_name == 'accessToken':
             context_values[context_name] = context_resource.get('headerValue')
             continue
 
+        permissions = None
+        if context_name in ['company', 'agent', 'asset']:
+            permissions = set()
+            if 'permissions' in context_resource:
+                permissions.update(context_resource['permissions'])
+
         context_values[context_name] = CbcIxapiResource(
             context_resource['publicId'],
             context_resource['name'],
             context_resource['custom'],
+            permissions,
         )
 
     return context_values
 
 def parse_json_input(
         config: Config,
+        context_config: Dict[str, str],
         body: str
     ) -> Tuple[CbcContext, FunctionLocation, FunctionArguments]:
     """
     Parses an application/json request body string into a context, function
     location and function arguments.
     """
     in_put = json.loads(body)
 
     function_location = parse_function_location(in_put.get('name', ''))
 
     # Get all context values, may be overwritten if a custom apiApplication is set
     # however this is then still needed for getting authentication values
     context_values = _parse_context_values(in_put.get('context', {}))
 
-    context_config = config.context_config | {
+    context_config = context_config | {
         config_name: str(config_value)
         for config_name, config_value in in_put.get('config', {}).items()
     }
 
     api_client_kwargs = {}
 
     if api_application_res := context_values.get('apiApplication'):
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress/webserver/wsgi.py` & `ixoncdkingress-0.0.7/ixoncdkingress/webserver/wsgi.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 """
 from typing import TYPE_CHECKING, Any, Iterable
 
 import functools, signal
 
 from ixoncdkingress.types import ResponseCode, RequestMethod
 from ixoncdkingress.webserver.config import Config, WsgiProvider
-from ixoncdkingress.webserver.servlet import Servlet, Request, Response
+from ixoncdkingress.webserver.servlet import Servlet
+from ixoncdkingress.webserver.response import Response
+from ixoncdkingress.webserver.request import Request
 
 if TYPE_CHECKING:
     # pylint: disable=E0401,E0611
     from _typeshed.wsgi import WSGIApplication, WSGIEnvironment, StartResponse
 
 def restapi_wsgi(
         config: Config,
@@ -101,17 +103,14 @@
             'wsgiref listening on http://%s:%s/',
             config.http_server_bind,
             config.http_server_port
         )
         logger.info(
             'CBC_PATH: %s', config.cbc_path
         )
-        logger.info(
-            'config.context_config: %s', config.context_config
-        )
         try:
             httpd.serve_forever()
         except KeyboardInterrupt:
             logger.info('Caught keyboard interrupt')
             httpd.shutdown()
```

### Comparing `ixoncdkingress-0.0.6/ixoncdkingress.egg-info/SOURCES.txt` & `ixoncdkingress-0.0.7/ixoncdkingress.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 README.md
 setup.py
 ixoncdkingress/__init__.py
 ixoncdkingress/__main__.py
 ixoncdkingress/py.typed
 ixoncdkingress/types.py
+ixoncdkingress/utils.py
 ixoncdkingress.egg-info/PKG-INFO
 ixoncdkingress.egg-info/SOURCES.txt
 ixoncdkingress.egg-info/dependency_links.txt
 ixoncdkingress.egg-info/requires.txt
 ixoncdkingress.egg-info/top_level.txt
 ixoncdkingress/cbc/__init__.py
 ixoncdkingress/cbc/api_client.py
 ixoncdkingress/cbc/caller.py
 ixoncdkingress/cbc/context.py
 ixoncdkingress/webserver/__init__.py
 ixoncdkingress/webserver/config.py
 ixoncdkingress/webserver/form.py
+ixoncdkingress/webserver/request.py
+ixoncdkingress/webserver/response.py
 ixoncdkingress/webserver/servlet.py
 ixoncdkingress/webserver/utils.py
 ixoncdkingress/webserver/wsgi.py
 tests/test___main__.py
-tests/test_types.py
+tests/test_types.py
+tests/test_utils.py
```

### Comparing `ixoncdkingress-0.0.6/setup.py` & `ixoncdkingress-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'pytest-mock==3.8.2',
     'types-requests>=2.28.11.5',
     'wouter==0.0.3',
 ]
 
 setup(
     name='ixoncdkingress',
-    version='0.0.6',
+    version='0.0.7',
     description='IXON CDK Ingress used in Custom Backend Components(CBC) for the IXON Cloud',
     author='IXON',
     author_email='development@ixon.cloud',
     url='https://www.ixon.cloud/',
     packages=find_packages(exclude=['tests*', ]),
     package_data={
         '': ['py.typed', 'assets/*'],
```

### Comparing `ixoncdkingress-0.0.6/tests/test___main__.py` & `ixoncdkingress-0.0.7/tests/test___main__.py`

 * *Files identical despite different names*

