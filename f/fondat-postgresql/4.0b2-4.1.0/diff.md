# Comparing `tmp/fondat-postgresql-4.0b2.tar.gz` & `tmp/fondat_postgresql-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-postgresql-4.0b2.tar", max compression
+gzip compressed data, was "fondat_postgresql-4.1.0.tar", max compression
```

## Comparing `fondat-postgresql-4.0b2.tar` & `fondat_postgresql-4.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1063 2022-01-09 19:33:17.668378 fondat-postgresql-4.0b2/LICENSE
--rw-r--r--   0        0        0      847 2021-12-13 05:19:58.616855 fondat-postgresql-4.0b2/README.md
--rw-r--r--   0        0        0    12594 2022-09-30 20:51:21.618450 fondat-postgresql-4.0b2/fondat/postgresql.py
--rw-r--r--   0        0        0     1126 2022-10-05 22:22:40.860623 fondat-postgresql-4.0b2/pyproject.toml
--rw-r--r--   0        0        0     1545 2022-10-05 22:23:11.925315 fondat-postgresql-4.0b2/setup.py
--rw-r--r--   0        0        0     1630 2022-10-05 22:23:11.925484 fondat-postgresql-4.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-01-09 19:33:17.668378 fondat_postgresql-4.1.0/LICENSE
+-rw-r--r--   0        0        0      853 2022-10-11 02:33:22.679172 fondat_postgresql-4.1.0/README.md
+-rw-r--r--   0        0        0    17507 2023-06-22 07:27:11.439705 fondat_postgresql-4.1.0/fondat/postgresql.py
+-rw-r--r--   0        0        0     1143 2023-06-22 07:27:45.283201 fondat_postgresql-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 fondat_postgresql-4.1.0/PKG-INFO
```

### Comparing `fondat-postgresql-4.0b2/LICENSE` & `fondat_postgresql-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-postgresql-4.0b2/README.md` & `fondat_postgresql-4.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # fondat-postgresql
 
 [![PyPI](https://badge.fury.io/py/fondat-postgresql.svg)](https://badge.fury.io/py/fondat-postgresql)
-[![Python](https://img.shields.io/pypi/pyversions/fondat-core)](https://python.org/)
+[![Python](https://img.shields.io/pypi/pyversions/fondat-postgresql)](https://python.org/)
 [![GitHub](https://img.shields.io/badge/github-main-blue.svg)](https://github.com/fondat/fondat-postgresql/)
 [![Test](https://github.com/fondat/fondat-postgresql/workflows/test/badge.svg)](https://github.com/fondat/fondat-postgresql/actions?query=workflow/test)
 [![License](https://img.shields.io/github/license/fondat/fondat-postgresql.svg)](https://github.com/fondat/fondat-postgresql/blob/main/LICENSE)
 [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 
 Fondat module for PostgreSQL.
```

### Comparing `fondat-postgresql-4.0b2/fondat/postgresql.py` & `fondat_postgresql-4.1.0/fondat/postgresql.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,85 +11,168 @@
 import logging
 import types
 import typing
 import uuid
 
 from collections.abc import AsyncIterator, Iterable, Mapping, Sequence
 from contextlib import asynccontextmanager
+from dataclasses import dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from fondat.codec import Codec, DecodeError, JSONCodec
 from fondat.data import datacls
-from fondat.sql import Expression
+from fondat.sql import Expression, Param
 from fondat.types import is_optional, is_subclass, literal_values, strip_annotations
-from fondat.validation import validate_arguments
+from fondat.validation import validate, validate_arguments
 from types import NoneType
-from typing import Annotated, Any, Literal, TypeVar, get_args, get_origin
+from typing import Annotated, Any, Generic, Literal, TypeVar, get_args, get_origin
 from uuid import UUID
 
 
 _logger = logging.getLogger(__name__)
 
 
-PT = TypeVar("PT")
-ST = TypeVar("ST")
+PT = TypeVar("PT")  # python type
+ST = TypeVar("ST")  # sql type
+
+
+Schema = TypeVar("Schema")
+T = TypeVar("T")
 
 
 class PostgreSQLCodec(Codec[PT, Any]):
     """Base class for PostgreSQL codecs."""
 
     _cache = {}
 
 
-class PassthroughCodec(PostgreSQLCodec[PT]):
+class _PassthroughCodec(Generic[PT]):
     """..."""
 
-    sql_types = {
-        str: "TEXT",
-        bool: "BOOLEAN",
-        int: "BIGINT",
-        float: "DOUBLE PRECISION",
-        bytes: "BYTEA",
-        bytearray: "BYTEA",
-        UUID: "UUID",
-        Decimal: "NUMERIC",
-        datetime: "TIMESTAMP WITH TIME ZONE",
-        date: "DATE",
-    }
-
-    @classmethod
-    def handles(cls, python_type: Any) -> bool:
-        python_type = strip_annotations(python_type)
-        return python_type in cls.sql_types.keys()
-
-    def __init__(self, python_type: Any):
-        super().__init__(python_type)
-        self.sql_type = self.sql_types[strip_annotations(python_type)]
-
     @validate_arguments
     def encode(self, value: PT) -> PT:
         return value
 
     @validate_arguments
     def decode(self, value: PT) -> PT:
         return value
 
 
+class StrCodec(_PassthroughCodec[str], PostgreSQLCodec[str]):
+    sql_type = "TEXT"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, str)
+
+
+class FloatCodec(_PassthroughCodec[float], PostgreSQLCodec[float]):
+    sql_type = "DOUBLE PRECISION"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, float)
+
+
+class DecimalCodec(_PassthroughCodec[Decimal], PostgreSQLCodec[Decimal]):
+    sql_type = "NUMERIC"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, Decimal)
+
+
+class BytesCodec(_PassthroughCodec[bytes], PostgreSQLCodec[bytes]):
+    sql_type = "BYTEA"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, bytes)
+
+
+class BytearrayCodec(_PassthroughCodec[bytearray], PostgreSQLCodec[bytearray]):
+    sql_type = "BYTEA"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, bytearray)
+
+    @validate_arguments
+    def decode(self, value: bytes | bytearray) -> bytearray:
+        return value if isinstance(value, bytearray) else bytearray(value)
+
+
+class IntCodec(_PassthroughCodec[int], PostgreSQLCodec[int]):
+    sql_type = "BIGINT"
+
+    @staticmethod
+    def handles(python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, int) and not is_subclass(python_type, bool)
+
+
+class BoolCodec(_PassthroughCodec[bool], PostgreSQLCodec[bool]):
+    sql_type = "BOOLEAN"
+
+    @classmethod
+    def handles(cls, python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, bool)
+
+    @validate_arguments
+    def decode(self, value: int | bool) -> bool:
+        return bool(value)
+
+
+class DateCodec(_PassthroughCodec[date], PostgreSQLCodec[date]):
+    sql_type = "DATE"
+
+    @classmethod
+    def handles(cls, python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, date) and not is_subclass(python_type, datetime)
+
+
+class DatetimeCodec(_PassthroughCodec[datetime], PostgreSQLCodec[datetime]):
+    sql_type = "TIMESTAMP WITH TIME ZONE"
+
+    @classmethod
+    def handles(cls, python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, datetime)
+
+
+class UUIDCodec(_PassthroughCodec[UUID], PostgreSQLCodec[UUID]):
+    sql_type = "UUID"
+
+    @classmethod
+    def handles(cls, python_type: Any) -> bool:
+        python_type = strip_annotations(python_type)
+        return is_subclass(python_type, UUID)
+
+
 class ArrayCodec(PostgreSQLCodec[PT]):
     """..."""
 
     _AVOID = str | bytes | bytearray | Mapping | tuple
 
     @classmethod
     def handles(cls, python_type: Any) -> bool:
         python_type = strip_annotations(python_type)
         origin = get_origin(python_type) or python_type
         args = get_args(python_type)
         return (
-            is_subclass(origin, Iterable) and is_subclass(origin, cls._AVOID) and len(args) == 1
+            is_subclass(origin, Iterable)
+            and not is_subclass(origin, cls._AVOID)
+            and len(args) == 1
         )
 
     def __init__(self, python_type: Any):
         super().__init__(python_type)
         python_type = strip_annotations(python_type)
         self.codec = PostgreSQLCodec.get(get_args(python_type)[0])
         self.sql_type = f"{self.codec.sql_type}[]"
@@ -192,42 +275,44 @@
     def encode(self, value: PT) -> Any:
         return json.dumps(self.codec.encode(value))
 
     def decode(self, value: Any) -> PT:
         return self.codec.decode(json.loads(value))
 
 
-class _Results(AsyncIterator[Any]):
-
+class _Results(AsyncIterator[T]):
     __slots__ = {"statement", "result", "rows", "codecs"}
 
     def __init__(self, statement, result, rows):
         self.statement = statement
         self.result = result
         self.rows = rows
         self.codecs = {
             k: PostgreSQLCodec.get(t)
             for k, t in typing.get_type_hints(result, include_extras=True).items()
         }
 
     def __aiter__(self):
         return self
 
-    async def __anext__(self):
-        row = await self.rows.__anext__()
-        result = {}
+    async def __anext__(self) -> T:
+        row = await anext(self.rows)
+        build = {}
         for key in self.codecs:
             with DecodeError.path_on_error(key):
-                result[key] = self.codecs[key].decode(row[key])
-        return self.result(**result)
+                build[key] = self.codecs[key].decode(row[key])
+        result = self.result(**build)
+        validate(result, self.result)
+        return result
 
 
 # fmt: off
 @datacls
 class Config:
+    """PostgreSQL connection pool configuration."""
     dsn: Annotated[str | None, "connection arguments in libpg connection URI format"]
     min_size: Annotated[int | None, "number of connections to initialize pool with"]
     max_size: Annotated[int | None, "maximum number of connections in the pool"]
     max_queries: Annotated[int | None, "number of queries before connection is replaced"]
     max_inactive_connection_lifetime: Annotated[float | None, "seconds after inactive connection closed"]
     host: Annotated[str | None, "database host address"]
     port: Annotated[int | None, "port number to connect to"]
@@ -245,53 +330,80 @@
     yield
 
 
 class Database(fondat.sql.Database):
     """
     Manages access to a PostgreSQL database.
 
-    Supplied configuration can be a Config dataclass instance, or a function or coroutine
-    function that returns a Config dataclass instance.
+    Parameters:
+    • config: connection pool configuration
+
+    The connection pool will be initialized on the first connection request, or it can be
+    explicitly initialized using the `init` method.
     """
 
-    @classmethod
-    async def create(cls, config: Config):
-        self = cls()
-        kwargs = {k: v for k, v in dataclasses.asdict(config).items() if v is not None}
+    def __init__(self, config: Config):
         self._config = config
-        self._pool = await asyncpg.create_pool(**kwargs)
         self._conn = contextvars.ContextVar("fondat_postgresql_conn", default=None)
         self._txn = contextvars.ContextVar("fondat_postgresql_txn", default=None)
         self._task = contextvars.ContextVar("fondat_postgresql_task", default=None)
+        self._pool = None
+
+    @classmethod
+    async def new(cls, config: Config) -> "Database":
+        """Deprecated."""
+        self = cls(config)
+        await self.init()
         return self
 
-    async def close(self):
-        """Close all database connections."""
+    @classmethod
+    async def create(cls, config: Config) -> "Database":
+        """Deprecated."""
+        self = cls(config)
+        await self.init()
+        return self
+
+    async def init(self) -> None:
+        """Create database connection pool."""
+        if not self._pool:
+            _logger.debug("create connection pool")
+            self._pool = await asyncpg.create_pool(
+                **{k: v for k, v in dataclasses.asdict(self._config).items() if v is not None}
+            )
+
+    async def close(self) -> None:
+        """Close database connection pool."""
         if self._pool:
             await self._pool.close()
         self._pool = None
 
     @asynccontextmanager
-    async def connection(self) -> None:
+    async def connection(self) -> AsyncIterator[None]:
         task = asyncio.current_task()
         if self._conn.get() and self._task.get() is task:
             yield  # connection already established
             return
-        _logger.debug("open connection")
+        await self.init()
+        _logger.debug("acquire connection from pool")
         self._task.set(task)
         async with self._pool.acquire(timeout=self._config.timeout) as connection:
             self._conn.set(connection)
             try:
                 yield
             finally:
-                _logger.debug("close connection")
+                _logger.debug("release connection to pool")
                 self._conn.set(None)
 
     @asynccontextmanager
-    async def transaction(self) -> None:
+    async def transaction(self) -> AsyncIterator[None]:
+        """
+        Return an asynchronous context manager, which scopes a transaction in which
+        statement(s) are executed. Upon exit of the context, if an exception was raised,
+        changes will be rolled back; otherwise changes will be committed.
+        """
         txid = uuid.uuid4().hex
         _logger.debug("transaction begin %s", txid)
         token = self._txn.set(txid)
         async with self.connection():
             connection = self._conn.get()
             transaction = connection.transaction()
             await transaction.start()
@@ -315,16 +427,29 @@
                 await commit()
             finally:
                 self._txn.reset(token)
 
     async def execute(
         self,
         statement: Expression,
-        result: type = None,
-    ) -> AsyncIterator[Any] | None:
+        result: type[T] = None,
+    ) -> AsyncIterator[T] | None:
+        """
+        Execute a SQL statement.
+
+        Parameters:
+        • statement: SQL statement to excute
+        • result: the type to return a query result row
+
+        If the statement is a query that generates results, each row can be returned in
+        a dataclass or TypedDict object, whose type is specifed in the `result` parameter.
+        Rows are provided via a returned asynchronous iterator.
+
+        Must be called within a database transaction context.
+        """
         if not self._txn.get():
             raise RuntimeError("transaction context required to execute statement")
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(str(statement))
         text = []
         args = []
         for fragment in statement:
@@ -333,55 +458,84 @@
             else:
                 args.append(PostgreSQLCodec.get(fragment.type).encode(fragment.value))
                 text.append(f"${len(args)}")
         text = "".join(text)
         conn = self._conn.get()
         if result is None:
             await conn.execute(text, *args)
-        else:  # expecting a result
+        else:  # expecting results
             return _Results(statement, result, conn.cursor(text, *args).__aiter__())
 
     def sql_type(self, type: Any) -> str:
+        """Return the SQL type string that corresponds with the specified Python type."""
         return PostgreSQLCodec.get(type).sql_type
 
 
+class Table(fondat.sql.Table[Schema]):
+    """..."""
+
+    async def upsert(self, value: Schema):
+        """
+        Upsert table row. Must be called within a database transaction context.
+        """
+        stmt = Expression(
+            f"INSERT INTO {self.name} (",
+            ", ".join(self.columns),
+            ") VALUES (",
+            Expression.join(
+                (
+                    Param(getattr(value, name), python_type)
+                    for name, python_type in self.columns.items()
+                ),
+                ", ",
+            ),
+            f") ON CONFLICT ({self.pk}) DO UPDATE SET ",
+            Expression.join(
+                (
+                    Expression(f"{name} = ", Param(getattr(value, name), python_type))
+                    for name, python_type in self.columns.items()
+                    if name != self.pk
+                ),
+                ", ",
+            ),
+            ";",
+        )
+        await self.database.execute(stmt)
+
+
+@dataclass
 class Index(fondat.sql.Index):
     """
     Represents an index on a table in a PostgreSQL database.
 
     Parameters:
     • name: name of index
     • table: table that the index defined for
     • keys: index keys (typically column names with optional order)
     • unique: is index unique
     • method: indexing method
     """
 
-    __slots__ = ("method",)
+    method: str | None = None
 
-    def __init__(
-        self,
-        name: str,
-        table: fondat.sql.Table,
-        keys: Sequence[str],
-        unique: bool = False,
-        method: str | None = None,
-    ):
-        super().__init__(name, table, keys, unique)
-        self.method = method
+    async def create(self, execute: bool = True) -> Expression:
+        """
+        Generate statement to create index in database.
 
-    def __repr__(self):
-        result = f"Index(name={self.name}, table={self.table}, keys={self.keys}, unique={self.unique} method={self.method})"
+        Parameters:
+        • execute: execute statement
 
-    async def create(self):
-        """Create index in database."""
+        Statement must be executed within a database transaction context.
+        """
         stmt = Expression()
         stmt += "CREATE "
         if self.unique:
             stmt += "UNIQUE "
         stmt += f"INDEX {self.name} ON {self.table.name} "
         if self.method:
             stmt += f"USING {self.method} "
         stmt += "("
         stmt += ", ".join(self.keys)
         stmt += ");"
-        await self.table.database.execute(stmt)
+        if execute:
+            await self.table.database.execute(stmt)
+        return stmt
```

### Comparing `fondat-postgresql-4.0b2/pyproject.toml` & `fondat_postgresql-4.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat-postgresql"
-version = "4.0b2"
-description = "Fondat PostgreSQL module."
+version = "4.1.0"
+description = "Fondat module for PostgreSQL."
 readme = "README.md"
 authors = ["fondat-postgresql authors"]
 homepage = "https://github.com/fondat/fondat-postgresql/"
 documentation = "https://github.com/fondat/fondat-postgresql/wiki"
 license = "MIT"
 keywords = ["asgi", "framework", "resource", "openapi"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fondat = "^4.0b4"
+fondat = "^4.1.4"
 asyncpg = "^0.26"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8"
+black = "^22.10"
 isort = "^5.10"
 pre-commit = "^2.20"
 pytest = "^7.1"
 pytest-asyncio = "^0.19"
 pytest-cov = "^3.0"
 
 [tool.isort]
```

### Comparing `fondat-postgresql-4.0b2/setup.py` & `fondat_postgresql-4.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fondat-postgresql
+Version: 4.1.0
+Summary: Fondat module for PostgreSQL.
+Home-page: https://github.com/fondat/fondat-postgresql/
+License: MIT
+Keywords: asgi,framework,resource,openapi
+Author: fondat-postgresql authors
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Dist: asyncpg (>=0.26,<0.27)
+Requires-Dist: fondat (>=4.1.4,<5.0.0)
+Project-URL: Documentation, https://github.com/fondat/fondat-postgresql/wiki
+Description-Content-Type: text/markdown
+
+# fondat-postgresql
+
+[![PyPI](https://badge.fury.io/py/fondat-postgresql.svg)](https://badge.fury.io/py/fondat-postgresql)
+[![Python](https://img.shields.io/pypi/pyversions/fondat-postgresql)](https://python.org/)
+[![GitHub](https://img.shields.io/badge/github-main-blue.svg)](https://github.com/fondat/fondat-postgresql/)
+[![Test](https://github.com/fondat/fondat-postgresql/workflows/test/badge.svg)](https://github.com/fondat/fondat-postgresql/actions?query=workflow/test)
+[![License](https://img.shields.io/github/license/fondat/fondat-postgresql.svg)](https://github.com/fondat/fondat-postgresql/blob/main/LICENSE)
+[![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+
+Fondat module for PostgreSQL.
+
+## Develop
+
+```
+poetry install
+poetry run pre-commit install
+```
+
+## Test
+
+```
+poetry run pytest
+```
 
-packages = \
-['fondat']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['asyncpg>=0.26,<0.27', 'fondat>=4.0b4,<5.0']
-
-setup_kwargs = {
-    'name': 'fondat-postgresql',
-    'version': '4.0b2',
-    'description': 'Fondat PostgreSQL module.',
-    'long_description': '# fondat-postgresql\n\n[![PyPI](https://badge.fury.io/py/fondat-postgresql.svg)](https://badge.fury.io/py/fondat-postgresql)\n[![Python](https://img.shields.io/pypi/pyversions/fondat-core)](https://python.org/)\n[![GitHub](https://img.shields.io/badge/github-main-blue.svg)](https://github.com/fondat/fondat-postgresql/)\n[![Test](https://github.com/fondat/fondat-postgresql/workflows/test/badge.svg)](https://github.com/fondat/fondat-postgresql/actions?query=workflow/test)\n[![License](https://img.shields.io/github/license/fondat/fondat-postgresql.svg)](https://github.com/fondat/fondat-postgresql/blob/main/LICENSE)\n[![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n\nFondat module for PostgreSQL.\n\n## Develop\n\n```\npoetry install\npoetry run pre-commit install\n```\n\n## Test\n\n```\npoetry run pytest\n```\n',
-    'author': 'fondat-postgresql authors',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/fondat/fondat-postgresql/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

