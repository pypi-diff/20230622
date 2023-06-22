# Comparing `tmp/fastapi_swagger2-0.0.1b4.tar.gz` & `tmp/fastapi_swagger2-0.0.1b5.tar.gz`

## Comparing `fastapi_swagger2-0.0.1b4.tar` & `fastapi_swagger2-0.0.1b5.tar`

### file list

```diff
@@ -1,26 +1,34 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/.update-informer
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/10fbfe993ec4be0d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/1abeadf52d9572ab
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/8cf332caaea8e79b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/a8a883be09c5919b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/c180a20ea5e70786
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/f16744491f37c6f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/f885759af04f4f9e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/fbcf51701267e364
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/build.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/clean.sh
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/format.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/lint.sh
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/publish.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/test.sh
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/constants.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/models.py
--rw-r--r--   0        0        0    18659 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/utils.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/LICENSE
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/README.md
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/requirements-dev.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/requirements.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/.update-informer
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/10fbfe993ec4be0d
+-rw-r--r--   0        0        0    19350 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/1a84b0002c6f63c3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/1abeadf52d9572ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/26e89fbd03286482
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/2d87409254dbc080
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/3bf02553ad62c3bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/6d5e270589f4c84f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/8cf332caaea8e79b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/91433f946dd52c35
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/a8a883be09c5919b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/c180a20ea5e70786
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/f16744491f37c6f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/f885759af04f4f9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.ruff_cache/content/fbcf51701267e364
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/build.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/clean.sh
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/format.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/lint.sh
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/publish.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/scripts/test.sh
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/constants.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/models.py
+-rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/LICENSE
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/README.md
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b5/PKG-INFO
```

### Comparing `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/__init__.py` & `fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1b4"
+__version__ = "0.0.1b5"
 
 from typing import Any, Dict, List, Optional, TypeVar
 
 from fastapi import FastAPI
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
@@ -130,14 +130,15 @@
     def swagger2(self) -> Dict[str, Any]:
         if not self.app.swagger2_schema:
             self.app.swagger2_schema = get_swagger2(
                 title=self.app.title,
                 version=self.app.version,
                 swagger2_version=self.app.swagger2_version,
                 description=self.app.description,
+                server=str(self.app.servers[0]) if self.app.servers else None,
                 terms_of_service=self.app.terms_of_service,
                 contact=self.app.contact,
                 license_info=self.app.license_info,
                 routes=self.app.routes,
                 tags=self.app.swagger2_tags,
             )
```

### Comparing `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/models.py` & `fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/utils.py` & `fastapi_swagger2-0.0.1b5/src/fastapi_swagger2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import http.client
 import inspect
 from enum import Enum
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
+from urllib.parse import ParseResult, urlparse
 
 from fastapi import routing
 from fastapi.datastructures import DefaultPlaceholder
 from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_flat_dependant, get_flat_params
 from fastapi.encoders import jsonable_encoder
 from fastapi.logger import logger
@@ -360,18 +361,16 @@
                         or "Additional Response"
                     )
                     deep_dict_update(openapi_response, process_response)
                     openapi_response["description"] = description
 
             http422 = str(HTTP_422_UNPROCESSABLE_ENTITY)
             if (all_route_params or route.body_field) and not any(
-                [
-                    status in operation["responses"]
-                    for status in [http422, "4XX", "default"]
-                ]
+                status in operation["responses"]
+                for status in [http422, "4XX", "default"]
             ):
                 operation["responses"][http422] = {
                     "description": "Validation Error",
                     "schema": {"$ref": REF_PREFIX + "HTTPValidationError"},
                 }
                 if "ValidationError" not in definitions:
                     definitions.update(
@@ -391,14 +390,15 @@
     *,
     title: str,
     version: str,
     swagger2_version: str = "2.0",
     description: Optional[str] = None,
     routes: Sequence[BaseRoute],
     tags: Optional[List[Dict[str, Any]]] = None,
+    server: Optional[str] = None,
     terms_of_service: Optional[str] = None,
     contact: Optional[Dict[str, Union[str, Any]]] = None,
     license_info: Optional[Dict[str, Union[str, Any]]] = None,
 ) -> Dict[str, Any]:
     info: Dict[str, Any] = {"title": title, "version": version}
     if description:
         info["description"] = description
@@ -407,14 +407,20 @@
     if contact:
         info["contact"] = contact
     if license_info:
         info["license"] = license_info
 
     output: Dict[str, Any] = {"swagger": swagger2_version, "info": info}
 
+    if server:
+        pr: ParseResult = urlparse(server)
+        output["host"] = pr.netloc
+        output["basePath"] = pr.path or "/"
+        output.setdefault("schemes", []).append(pr.scheme)
+
     paths: Dict[str, Dict[str, Any]] = {}
     operation_ids: Set[str] = set()
 
     flat_models = get_flat_models_from_routes(routes)
     model_name_map = get_model_name_map(flat_models)
     definitions = get_model_definitions(
         flat_models=flat_models, model_name_map=model_name_map
```

### Comparing `fastapi_swagger2-0.0.1b4/.gitignore` & `fastapi_swagger2-0.0.1b5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b4/LICENSE` & `fastapi_swagger2-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b4/README.md` & `fastapi_swagger2-0.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b4/pyproject.toml` & `fastapi_swagger2-0.0.1b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b4/PKG-INFO` & `fastapi_swagger2-0.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_swagger2
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Swagger2 support for FastAPI framework
 Project-URL: Homepage, https://github.com/virajkanwade/fastapi_swagger2
 Project-URL: Documentation, https://github.com/virajkanwade/fastapi_swagger2
 Author-email: Viraj Kanwade <virajk.oib@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Viraj Kanwade
```

