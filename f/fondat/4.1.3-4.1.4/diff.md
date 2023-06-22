# Comparing `tmp/fondat-4.1.3.tar.gz` & `tmp/fondat-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.3.tar", max compression
+gzip compressed data, was "fondat-4.1.4.tar", max compression
```

## Comparing `fondat-4.1.3.tar` & `fondat-4.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.3/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.3/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.3/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.3/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.3/fondat/cache.py
--rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.3/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.3/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.3/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.3/fondat/data.py
--rw-r--r--   0        0        0     2444 2022-09-25 17:46:57.851193 fondat-4.1.3/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.3/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.3/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.3/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.3/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.3/fondat/monitor.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.3/fondat/openapi.py
--rw-r--r--   0        0        0     2592 2022-10-17 23:26:39.100935 fondat-4.1.3/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.3/fondat/patch.py
--rw-r--r--   0        0        0    11398 2023-05-28 15:08:56.067124 fondat-4.1.3/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.3/fondat/security.py
--rw-r--r--   0        0        0    27754 2022-10-26 17:21:16.900572 fondat-4.1.3/fondat/sql.py
--rw-r--r--   0        0        0    10988 2023-02-01 23:37:21.447708 fondat-4.1.3/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.3/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.3/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.3/fondat/types.py
--rw-r--r--   0        0        0    10948 2022-09-30 06:16:57.338274 fondat-4.1.3/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-05-28 15:11:00.657172 fondat-4.1.3/pyproject.toml
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.4/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.4/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.4/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.4/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/cache.py
+-rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.4/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.4/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.4/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/data.py
+-rw-r--r--   0        0        0     2444 2022-09-25 17:46:57.851193 fondat-4.1.4/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.4/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.4/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.4/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.4/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.4/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.4/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.4/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.4/fondat/patch.py
+-rw-r--r--   0        0        0    11398 2023-05-28 15:08:56.067124 fondat-4.1.4/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.4/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.4/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.4/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.4/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.4/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.4/fondat/types.py
+-rw-r--r--   0        0        0    10948 2022-09-30 06:16:57.338274 fondat-4.1.4/fondat/validation.py
+-rw-r--r--   0        0        0     1172 2023-06-22 07:22:32.061609 fondat-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.4/PKG-INFO
```

### Comparing `fondat-4.1.3/LICENSE` & `fondat-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/README.md` & `fondat-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/annotation.py` & `fondat-4.1.4/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/asgi.py` & `fondat-4.1.4/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/cache.py` & `fondat-4.1.4/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/codec.py` & `fondat-4.1.4/fondat/codec.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/context.py` & `fondat-4.1.4/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/csv.py` & `fondat-4.1.4/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/data.py` & `fondat-4.1.4/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/error.py` & `fondat-4.1.4/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/file.py` & `fondat-4.1.4/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/http.py` & `fondat-4.1.4/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/lazy.py` & `fondat-4.1.4/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/memory.py` & `fondat-4.1.4/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/monitor.py` & `fondat-4.1.4/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/openapi.py` & `fondat-4.1.4/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/pagination.py` & `fondat-4.1.4/fondat/pagination.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 An operation should establish a reasonable limit of items it would return in each page. If
 appropriate, the operation can also expose a `limit` parameter, which allows a caller to
 request a number of items to be returned in the page. Regardless of how many items are
 requested, the operation should be free to decide how many items to actually return.
 """
 
-from collections.abc import AsyncGenerator, Callable, Coroutine, Iterable
+from collections.abc import AsyncIterable, Callable, Coroutine, Iterable
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
 
 class PaginationError(Exception):
     """
     Error raised if pagination could not be performed.
@@ -49,15 +49,15 @@
 
     items: Iterable[Item]
     cursor: Cursor = None
 
 
 async def paginate(
     operation: Callable[..., Coroutine[Any, Any, Page[Item]]], /, **kwargs
-) -> AsyncGenerator[Item, None]:
+) -> AsyncIterable[Item]:
     """
     Wraps a paginated resource operation with an asynchronous generator that iterates through
     all items. The wrapped resource operation must return a page dataclass and accept a
     `cursor` parameter.
 
     Parameters:
     • operation: resource operation to wrap with generator
```

### Comparing `fondat-4.1.3/fondat/patch.py` & `fondat-4.1.4/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/resource.py` & `fondat-4.1.4/fondat/resource.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/security.py` & `fondat-4.1.4/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/sql.py` & `fondat-4.1.4/fondat/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 
 _logger = logging.getLogger(__name__)
 
 
 # type variables
 Item = TypeVar("Item")  # item type variable
-PK = TypeVar("PK")  # primary key type variable
-R = TypeVar("R")  # row type variable
+Schema = TypeVar("Schema")  # table schema type variable
 T = TypeVar("T")  # generic type variable
 
 
 @dataclass
 class Param:
     """
     A parameterized value to include in an expression.
@@ -140,22 +139,20 @@
     return re.sub(r"[^A-Za-z_]", "_", value)
 
 
 class Database:
     """Base class for a SQL database."""
 
     async def execute(
-        self,
-        statement: Expression | str,
-        result: type[T] | None = None,
+        self, statement: Expression | str, result: type[T] | None = None
     ) -> AsyncIterator[T] | None:
         """
         Execute a SQL statement.
 
-        Parameter:
+        Parameters:
         • statement: SQL statement to excute
         • result: the type to return a query result row
 
         If the statement is a query that generates results, each row can be returned in
         a dataclass or TypedDict object, whose type is specifed in the `result` parameter.
         Rows are provided via a returned asynchronous iterator.
 
@@ -172,15 +169,15 @@
         raise NotImplementedError
 
     def sql_type(self, python_type: Any) -> str:
         """Return the SQL type string that corresponds with the specified Python type."""
         raise NotImplementedError
 
 
-class Table(Generic[R, PK]):
+class Table(Generic[Schema]):
     """
     Represents a table in a SQL database.
 
     Parameters and attributes:
     • name: name of database table
     • database: database where table is managed
     • schema: dataclass representing the table schema
@@ -188,15 +185,15 @@
 
     Attributes:
     • columns: mapping of column names to ther associated types
     """
 
     __slots__ = {"name", "database", "schema", "columns", "pk"}
 
-    def __init__(self, name: str, database: Database, schema: type[R], pk: str):
+    def __init__(self, name: str, database: Database, schema: type[Schema], pk: str):
         self.name = name
         self.database = database
         schema = fondat.types.strip_annotations(schema)
         if not is_dataclass(schema):
             raise TypeError("table schema must be a dataclass")
         self.schema = schema
         self.columns = typing.get_type_hints(schema, include_extras=True)
@@ -302,15 +299,15 @@
         stmt = Expression(f"SELECT COUNT(*) AS count FROM {self.name}")
         if where:
             stmt += Expression(" WHERE ", where)
         stmt += ";"
         result = await self.database.execute(stmt, TypedDict("Result", {"count": int}))
         return (await anext(result))["count"]
 
-    async def insert(self, value: R):
+    async def insert(self, value: Schema):
         """
         Insert table row. Must be called within a database transaction context.
         """
         stmt = Expression(
             f"INSERT INTO {self.name} (",
             ", ".join(self.columns),
             ") VALUES (",
@@ -321,32 +318,32 @@
                 ),
                 ", ",
             ),
             ");",
         )
         await self.database.execute(stmt)
 
-    async def read(self, pk: PK) -> R:
+    async def read(self, pk: Any) -> Schema:
         """
-        Return a table row, or None if not found. Must be called within a database transaction
-        context.
+        Return table row that has the specified primary key, or `None` if not found. Must be
+        called within a database transaction context.
         """
         try:
             return self.schema(
                 **await anext(
                     self.select(
                         where=Expression(f"{self.pk} = ", Param(pk, self.columns[self.pk])),
                         limit=1,
                     )
                 )
             )
         except StopAsyncIteration:
             return None
 
-    async def update(self, value: R):
+    async def update(self, value: Schema):
         """
         Update table row. Must be called within a database transaction context.
         """
         await self.database.execute(
             Expression(
                 f"UPDATE {self.name} SET ",
                 Expression.join(
@@ -358,30 +355,31 @@
                 ),
                 f" WHERE {self.pk} = ",
                 Param(getattr(value, self.pk), self.columns[self.pk]),
                 ";",
             )
         )
 
-    async def delete(self, pk: PK):
+    async def delete(self, pk: Any):
         """
         Delete table row. Must be called within a database transaction context.
         """
         await self.database.execute(
             Expression(
                 f"DELETE FROM {self.name} WHERE {self.pk} = ",
                 Param(pk, self.columns[self.pk]),
                 ";",
             )
         )
 
-    async def upsert(self, value: R):
+    async def upsert(self, value: Schema):
         """
-        Upsert table row. Must be called within a database transaction context.
-        Default is inefficient; database-specific implementations should override.
+        Upsert table row. Must be called within a database transaction context. Default is
+        inefficient; database-specific instances should override with a more efficient
+        implementation.
         """
         if await self.read(getattr(value, self.pk)) is None:
             await self.insert(value)
         else:
             await self.update(value)
 
 
@@ -435,32 +433,40 @@
         stmt = Expression(f"DROP INDEX {self.name};")
         if execute:
             await self.table.database.execute(stmt)
         return stmt
 
 
 @resource
-class TableResource(Generic[R, PK]):
+class TableResource(Generic[Schema]):
+    """
+    A resource representation of a SQL table.
+
+    Parameters:
+    • table: table object being represented by resource
+    • cache: resource to cache rows
+    """
+
     def __init__(
         self,
-        table: Table,
+        table: Table[Schema],
         cache: CacheResource | None = None,
     ):
         self.table = table
         self.cache = cache
 
-    def __getitem__(self, pk: PK) -> RowResource[R, PK]:
+    def __getitem__(self, pk: Any) -> RowResource[Schema]:
         return RowResource(table=self.table, pk=pk, cache=self.cache)
 
     @operation
     async def get(
         self,
         limit: Annotated[int, MinValue(1)] = 1000,
         cursor: bytes | None = None,
-    ) -> Page[T]:
+    ) -> Page[Schema]:
         """Get paginated list of rows, ordered by primary key."""
         pk_type = self.table.columns[self.table.pk]
         cursor_codec = BinaryCodec.get(pk_type)
         if cursor is not None:
             where = Expression(
                 f"{self.table.pk} > ", Param(cursor_codec.decode(cursor), pk_type)
             )
@@ -498,15 +504,15 @@
                     await self[pk].patch({k: v for k, v in doc.items() if k != self.table.pk})
                 except NotFoundError:
                     new = JSONCodec.get(self.table.schema).decode(doc)
                     validate(new, self.table.schema)
                     await self.table.insert(new)
 
     @query
-    async def find_pks(self, pks: set[PK]) -> list[R]:
+    async def find_pks(self, pks: set[Any]) -> list[Schema]:
         """Return rows corresponding to the specified set of primary keys."""
         if not pks:
             return []
         async with self.table.database.transaction():
             return [
                 self.table.schema(**row)
                 async for row in self.table.select(
@@ -518,25 +524,25 @@
                         ")",
                     )
                 )
             ]
 
 
 @resource
-class RowResource(Generic[R, PK]):
+class RowResource(Generic[Schema]):
     """
     Resource that represents a row in a database table.
 
     Parameters:
     • table: table where row is located
-    • pk: primary key of row
+    • pk: primary key value of row
     • cache: resource to cache rows
     """
 
-    def __init__(self, table: Table[R, PK], pk: PK, cache: CacheResource | None = None):
+    def __init__(self, table: Table[Schema], pk: Any, cache: CacheResource | None = None):
         self.table = table
         self.pk = pk
         self._cache_entry = (
             cache[
                 hash_json(
                     {
                         "database": self.table.database.__class__.__qualname__,
@@ -546,29 +552,29 @@
                 )
             ]
             if cache
             else None
         )
 
     @operation
-    async def get(self) -> R:
+    async def get(self) -> Schema:
         """Get row from table."""
         if self._cache_entry:
             with suppress(NotFoundError):
                 return await self._cache_entry.get()
         async with self.table.database.transaction():
             row = await self.table.read(self.pk)
         if not row:
             raise NotFoundError
         if self._cache_entry:
             await self._cache_entry.put(row)
         return row
 
     @operation
-    async def put(self, value: R):
+    async def put(self, value: Schema):
         """Insert or update (upsert) row."""
         if getattr(value, self.table.pk) != self.pk:
             raise ValidationError("primary key mismatch")
         async with self.table.database.transaction():
             await self.table.upsert(value)
         if self._cache_entry:
             await self._cache_entry.put(value)
```

### Comparing `fondat-4.1.3/fondat/sqlite.py` & `fondat-4.1.4/fondat/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 from typing import Any, Literal, TypeVar
 
 
 _logger = logging.getLogger(__name__)
 
 
 T = TypeVar("T")  # generic
-R = TypeVar("R")  # row type
+Schema = TypeVar("Schema")  # row type
 PT = TypeVar("PT")  # Python type
 ST = TypeVar("ST")  # SQL type
-PK = TypeVar("PK")  # primary key type
 
 
 class SQLiteCodec(Codec[PT, ST]):
     """Base class for SQLite codecs."""
 
     _cache = {}
 
@@ -310,18 +309,18 @@
         if result is not None:  # expecting a result
             return _Results[T](statement, result, aiter(results))
 
     def sql_type(self, type: Any) -> str:
         return SQLiteCodec.get(type).sql_type
 
 
-class Table(fondat.sql.Table[R, PK]):
+class Table(fondat.sql.Table[Schema]):
     """Represents a table in a SQLite database."""
 
-    async def upsert(self, value: R):
+    async def upsert(self, value: Schema):
         """Upsert table row. Must be called within a database transaction context."""
         stmt = Expression(
             f"INSERT INTO {self.name} (",
             ", ".join(self.columns),
             ") VALUES (",
             Expression.join(
                 (
```

### Comparing `fondat-4.1.3/fondat/stream.py` & `fondat-4.1.4/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/string.py` & `fondat-4.1.4/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/types.py` & `fondat-4.1.4/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/fondat/validation.py` & `fondat-4.1.4/fondat/validation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.3/pyproject.toml` & `fondat-4.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.3"
+version = "4.1.4" 
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
```

### Comparing `fondat-4.1.3/PKG-INFO` & `fondat-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.3
+Version: 4.1.4
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

