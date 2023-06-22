# Comparing `tmp/tipg-0.1.0.tar.gz` & `tmp/tipg-0.2.0.tar.gz`

## Comparing `tipg-0.1.0.tar` & `tipg-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/db.py
--rw-r--r--   0        0        0    32258 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/dbmodel.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/errors.py
--rw-r--r--   0        0        0    73268 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/logger.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/main.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/middleware.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/model.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/resources/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/resources/enums.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/resources/response.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/collection.html
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/collections.html
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/header.html
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/item.html
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/items.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/landing.html
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/map.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/tileset.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.1.0/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.1.0/LICENSE
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.1.0/README.md
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 tipg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 tipg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/__init__.py
+-rw-r--r--   0        0        0    32494 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/collections.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/database.py
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/errors.py
+-rw-r--r--   0        0        0    73270 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/logger.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/main.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/middleware.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/model.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/enums.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/response.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/collections.html
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/header.html
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/item.html
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/items.html
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/landing.html
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/map.html
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.2.0/README.md
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 tipg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 tipg-0.2.0/PKG-INFO
```

### Comparing `tipg-0.1.0/tipg/db.py` & `tipg-0.2.0/tipg/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """tipg.db: database events."""
 
 import pathlib
-from typing import Any, List, Optional
+from typing import List, Optional
 
 import orjson
 from buildpg import asyncpg
 
-from tipg.dbmodel import get_collection_index
 from tipg.logger import logger
 from tipg.settings import PostgresSettings
 
 from fastapi import FastAPI
 
 try:
     from importlib.resources import files as resources_files  # type: ignore
@@ -88,15 +87,10 @@
         max_queries=settings.db_max_queries,
         max_inactive_connection_lifetime=settings.db_max_inactive_conn_lifetime,
         init=con_init,
         **kwargs,
     )
 
 
-async def register_collection_catalog(app: FastAPI, **kwargs: Any) -> None:
-    """Register Table catalog."""
-    app.state.collection_catalog = await get_collection_index(app.state.pool, **kwargs)
-
-
 async def close_db_connection(app: FastAPI) -> None:
     """Close connection."""
     await app.state.pool.close()
```

### Comparing `tipg-0.1.0/tipg/dbmodel.py` & `tipg-0.2.0/tipg/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 )
 from tipg.filter.evaluate import to_filter
 from tipg.filter.filters import bbox_to_wkt
 from tipg.logger import logger
 from tipg.model import Extent
 from tipg.settings import FeaturesSettings, MVTSettings, TableSettings
 
+from fastapi import FastAPI
+
 mvt_settings = MVTSettings()
 features_settings = FeaturesSettings()
 
 
 def debug_query(q, *p):
     """Utility to print raw statement to use for debugging."""
 
@@ -870,16 +872,16 @@
             for col in self.properties
             if col.name not in geoms
         }
 
         return {**geoms, **props}
 
 
-class Database(TypedDict):
-    """Database."""
+class Catalog(TypedDict):
+    """Collection Catalog."""
 
     collections: Dict[str, Collection]
     last_updated: datetime.datetime
 
 
 async def get_collection_index(  # noqa: C901
     db_pool: asyncpg.BuildPgPool,
@@ -887,15 +889,15 @@
     tables: Optional[List[str]] = None,
     exclude_tables: Optional[List[str]] = None,
     exclude_table_schemas: Optional[List[str]] = None,
     functions: Optional[List[str]] = None,
     exclude_functions: Optional[List[str]] = None,
     exclude_function_schemas: Optional[List[str]] = None,
     spatial: bool = True,
-) -> Database:
+) -> Catalog:
     """Fetch Table and Functions index."""
     schemas = schemas or ["public"]
 
     query = """
         SELECT pg_temp.tipg_catalog(
             :schemas,
             :tables,
@@ -977,8 +979,13 @@
                 id_column=id_column,
                 properties=properties,
                 datetime_column=datetime_column,
                 geometry_column=geometry_column,
                 parameters=table.get("parameters", []),
             )
 
-        return Database(collections=catalog, last_updated=datetime.datetime.now())
+        return Catalog(collections=catalog, last_updated=datetime.datetime.now())
+
+
+async def register_collection_catalog(app: FastAPI, **kwargs: Any) -> None:
+    """Register Table catalog."""
+    app.state.collection_catalog = await get_collection_index(app.state.pool, **kwargs)
```

### Comparing `tipg-0.1.0/tipg/dependencies.py` & `tipg-0.2.0/tipg/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from morecantile import Tile
 from morecantile import tms as default_tms
 from pygeofilter.ast import AstType
 from pygeofilter.parsers.cql2_json import parse as cql2_json_parser
 from pygeofilter.parsers.cql2_text import parse as cql2_text_parser
 
-from tipg.dbmodel import Collection, Database
+from tipg.collections import Catalog, Collection
 from tipg.errors import InvalidBBox, MissingCollectionCatalog, MissingFunctionParameter
 from tipg.resources import enums
 from tipg.settings import TMSSettings
 
 from fastapi import Depends, HTTPException, Path, Query
 
 from starlette.requests import Request
@@ -40,17 +40,15 @@
         raise HTTPException(
             status_code=422, detail=f"Invalid Collection format '{collectionId}'."
         )
 
     assert collection_pattern.groupdict()["schema"]
     assert collection_pattern.groupdict()["collection"]
 
-    collection_catalog: Database = getattr(
-        request.app.state, "collection_catalog", None
-    )
+    collection_catalog: Catalog = getattr(request.app.state, "collection_catalog", None)
     if not collection_catalog:
         raise MissingCollectionCatalog("Could not find collections catalog.")
 
     if collectionId in collection_catalog["collections"]:
         return collection_catalog["collections"][collectionId]
 
     raise HTTPException(
```

### Comparing `tipg-0.1.0/tipg/errors.py` & `tipg-0.2.0/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/factory.py` & `tipg-0.2.0/tipg/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ciso8601 import parse_rfc3339
 from morecantile import Tile, TileMatrixSet
 from morecantile import tms as default_tms
 from morecantile.defaults import TileMatrixSets
 from pygeofilter.ast import AstType
 
 from tipg import model
-from tipg.dbmodel import Collection, Database
+from tipg.collections import Catalog, Collection
 from tipg.dependencies import (
     CollectionParams,
     ItemsOutputType,
     OutputType,
     TileParams,
     bbox_query,
     datetime_query,
@@ -457,15 +457,15 @@
                     ge=0,
                     description="Starts the response at an offset.",
                 ),
             ] = None,
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
         ):
             """List of collections."""
-            collection_catalog: Database = getattr(
+            collection_catalog: Catalog = getattr(
                 request.app.state, "collection_catalog", None
             )
             if not collection_catalog:
                 raise MissingCollectionCatalog("Could not find collections catalog.")
 
             collections_list = list(collection_catalog["collections"].values())
```

### Comparing `tipg-0.1.0/tipg/main.py` & `tipg-0.2.0/tipg/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from contextlib import asynccontextmanager
 from typing import Any, List
 
 import jinja2
 
 from tipg import __version__ as tipg_version
-from tipg.db import close_db_connection, connect_to_db, register_collection_catalog
+from tipg.collections import register_collection_catalog
+from tipg.database import close_db_connection, connect_to_db
 from tipg.errors import DEFAULT_STATUS_CODES, add_exception_handlers
 from tipg.factory import Endpoints
 from tipg.middleware import CacheControlMiddleware, CatalogUpdateMiddleware
 from tipg.settings import (
     APISettings,
     CustomSQLSettings,
     DatabaseSettings,
@@ -62,15 +63,14 @@
 app = FastAPI(
     title=settings.name,
     version=tipg_version,
     openapi_url="/api",
     docs_url="/api.html",
     lifespan=lifespan,
 )
-app.state.db_settings = db_settings
 
 # custom template directory
 templates_location: List[Any] = (
     [jinja2.FileSystemLoader(settings.template_directory)]
     if settings.template_directory
     else []
 )
```

### Comparing `tipg-0.1.0/tipg/middleware.py` & `tipg-0.2.0/tipg/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """tipg middlewares."""
 
 import re
 from datetime import datetime, timedelta
 from typing import Any, Optional, Set
 
-from tipg.db import register_collection_catalog
+from tipg.collections import register_collection_catalog
 from tipg.logger import logger
 
 from starlette.background import BackgroundTask
 from starlette.datastructures import MutableHeaders
 from starlette.requests import Request
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
```

### Comparing `tipg-0.1.0/tipg/model.py` & `tipg-0.2.0/tipg/model.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/settings.py` & `tipg-0.2.0/tipg/settings.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/filter/evaluate.py` & `tipg-0.2.0/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/filter/filters.py` & `tipg-0.2.0/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/resources/enums.py` & `tipg-0.2.0/tipg/resources/enums.py`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/sql/dbcatalog.sql` & `tipg-0.2.0/tipg/sql/dbcatalog.sql`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/collection.html` & `tipg-0.2.0/tipg/templates/collection.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/collections.html` & `tipg-0.2.0/tipg/templates/collections.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/conformance.html` & `tipg-0.2.0/tipg/templates/conformance.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/header.html` & `tipg-0.2.0/tipg/templates/header.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/item.html` & `tipg-0.2.0/tipg/templates/item.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/items.html` & `tipg-0.2.0/tipg/templates/items.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/landing.html` & `tipg-0.2.0/tipg/templates/landing.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/map.html` & `tipg-0.2.0/tipg/templates/map.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/queryables.html` & `tipg-0.2.0/tipg/templates/queryables.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/tilematrixset.html` & `tipg-0.2.0/tipg/templates/tilematrixset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/tilematrixsets.html` & `tipg-0.2.0/tipg/templates/tilematrixsets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/tileset.html` & `tipg-0.2.0/tipg/templates/tileset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/tipg/templates/tilesets.html` & `tipg-0.2.0/tipg/templates/tilesets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/.gitignore` & `tipg-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/LICENSE` & `tipg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/README.md` & `tipg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/pyproject.toml` & `tipg-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tipg-0.1.0/PKG-INFO` & `tipg-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tipg Version: 0.1.0 Summary: Simple and Fast
+Metadata-Version: 2.1 Name: tipg Version: 0.2.0 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
```

