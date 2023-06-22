# Comparing `tmp/hipal_mixin_scrud-1.0.2.tar.gz` & `tmp/hipal_mixin_scrud-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hipal_mixin_scrud-1.0.2.tar", last modified: Tue Jun 20 21:31:49 2023, max compression
+gzip compressed data, was "dist\hipal_mixin_scrud-1.0.3.tar", last modified: Thu Jun 22 18:20:27 2023, max compression
```

## Comparing `hipal_mixin_scrud-1.0.2.tar` & `hipal_mixin_scrud-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.935236 hipal_mixin_scrud-1.0.2/
--rw-rw-rw-   0        0        0      316 2023-06-20 21:31:49.935236 hipal_mixin_scrud-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.903237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.924238 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/__init__.py
--rw-rw-rw-   0        0        0     5725 2023-06-20 21:25:12.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/generator.py
--rw-rw-rw-   0        0        0     3112 2023-06-20 21:25:07.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/mixin_list.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.929238 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/__init__.py
--rw-rw-rw-   0        0        0      165 2023-06-20 18:14:02.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/operators.py
--rw-rw-rw-   0        0        0       82 2023-06-20 17:19:07.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/sorts.py
--rw-rw-rw-   0        0        0     3432 2023-06-20 21:25:59.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/mixin.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.933237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/__init__.py
--rw-rw-rw-   0        0        0      396 2023-06-20 21:24:58.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/paginate_params.py
--rw-rw-rw-   0        0        0      364 2023-06-15 00:38:39.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/pagination_base.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.919237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/
--rw-rw-rw-   0        0        0      316 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 21:31:49.937237 hipal_mixin_scrud-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      483 2023-06-20 21:31:45.000000 hipal_mixin_scrud-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.075886 hipal_mixin_scrud-1.0.3/
+-rw-rw-rw-   0        0        0     4613 2023-06-22 18:20:27.074885 hipal_mixin_scrud-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3264 2023-06-22 18:16:36.000000 hipal_mixin_scrud-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.041888 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.060886 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/__init__.py
+-rw-rw-rw-   0        0        0     5808 2023-06-22 17:44:55.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/generator.py
+-rw-rw-rw-   0        0        0     3366 2023-06-22 17:45:00.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/mixin_list.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.067886 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/operators.py
+-rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/sorts.py
+-rw-rw-rw-   0        0        0     4691 2023-06-22 17:44:49.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.072887 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-06-22 17:45:08.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/paginate_params.py
+-rw-rw-rw-   0        0        0      364 2023-06-22 17:45:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/pagination_base.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.055889 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/
+-rw-rw-rw-   0        0        0     4613 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 18:20:27.077886 hipal_mixin_scrud-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-06-22 18:18:21.000000 hipal_mixin_scrud-1.0.3/setup.py
```

### Comparing `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/generator.py` & `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,24 @@
     def schema_factory(
         self, schema_cls: Type[T], pk_field_name: str = "id", name: str = "Create"
     ) -> Type[T]:
         """
         Is used to create a CreateSchema which does not contain pk
         """
 
+        exclude_fields = [
+            "created_at",
+            "updated_at",
+            pk_field_name,
+        ]
+
         fields = {
             f.name: (f.type_, ...)
             for f in schema_cls.__fields__.values()
-            if f.name != pk_field_name
+            if f.name not in exclude_fields
         }
 
         name = schema_cls.__name__ + name
         schema: Type[T] = create_model(__model_name=name, **fields)  # type: ignore
         return schema
 
     def __init__(
@@ -118,15 +124,14 @@
             )
 
         if has_delete_one:
             self._add_api_route(
                 "/{item_id}",
                 self._delete_one(),
                 methods=["DELETE"],
-                response_model=self.schema,
                 summary="Delete One",
                 dependencies=[],
             )
 
     def _add_api_route(
         self,
         path: str,
```

### Comparing `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/mixin_list.py` & `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/mixin_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from fastapi import HTTPException
 from typing import Type
 from pydantic import BaseModel
-from sqlalchemy import String, cast
+from sqlalchemy import String, cast, or_
 from sqlalchemy.orm import Session
 from sqlalchemy.orm import Query
 from sqlalchemy.orm import declarative_base
 
 from hipal_mixin_scrud.schemas.paginate_params import PaginateParams
 
 
@@ -43,19 +43,31 @@
         order_by = getattr(model, "created_at")
         order_by = order_by.desc()
 
         if paginate_params.sort:
             order_by = getattr(model, paginate_params.sort_field)
             order_by = getattr(order_by, paginate_params.sort.value)()
 
-        if paginate_params.search_field and paginate_params.search_value:
-            field = getattr(model, paginate_params.search_field)
-            search_value = paginate_params.search_value
-            filter = cast(field, String).ilike(f"%{search_value}%")
-            query = query.filter(filter)
+        if paginate_params.search:
+            SEPARATOR = ";"
+            OPERATOR = "="
+
+            filters = paginate_params.search.split(SEPARATOR)
+            filters_sql = []
+
+            for filter in filters:
+                field = filter.split(OPERATOR)[0]
+                field = getattr(model, field)
+                search_value = filter.split(OPERATOR)[1]
+
+                filter = cast(field, String).ilike(f"%{search_value}%")
+
+                filters_sql.append(filter)
+
+            query = query.filter(or_(*filters_sql))
 
         query = query.order_by(order_by)
         paginate_model = query.limit(paginate_params.limit).offset(
             paginate_params.offset
         )
         total_pages = math.ceil(query.count() / paginate_params.limit)
         total_items = query.count()
```

### Comparing `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/SOURCES.txt` & `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 hipal_mixin_scrud/__init__.py
 hipal_mixin_scrud/mixin.py
 hipal_mixin_scrud.egg-info/PKG-INFO
 hipal_mixin_scrud.egg-info/SOURCES.txt
 hipal_mixin_scrud.egg-info/dependency_links.txt
 hipal_mixin_scrud.egg-info/requires.txt
```

