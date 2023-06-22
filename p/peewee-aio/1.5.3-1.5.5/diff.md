# Comparing `tmp/peewee_aio-1.5.3.tar.gz` & `tmp/peewee_aio-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.5.3.tar", max compression
+gzip compressed data, was "peewee_aio-1.5.5.tar", max compression
```

## Comparing `peewee_aio-1.5.3.tar` & `peewee_aio-1.5.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4681 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/README.md
--rw-r--r--   0        0        0      132 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/fields.py
--rw-r--r--   0        0        0    15580 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/manager.py
--rw-r--r--   0        0        0    16604 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/types.py
--rw-r--r--   0        0        0     2585 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 peewee_aio-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/README.md
+-rw-r--r--   0        0        0      132 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15580 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/manager.py
+-rw-r--r--   0        0        0    16639 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/peewee_aio/types.py
+-rw-r--r--   0        0        0     2622 2023-06-22 07:57:30.614358 peewee_aio-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.5.5/PKG-INFO
```

### Comparing `peewee_aio-1.5.3/README.md` & `peewee_aio-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.3/peewee_aio/databases.py` & `peewee_aio-1.5.5/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.3/peewee_aio/fields.py` & `peewee_aio-1.5.5/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.3/peewee_aio/manager.py` & `peewee_aio-1.5.5/peewee_aio/manager.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.3/peewee_aio/model.py` & `peewee_aio-1.5.5/peewee_aio/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,36 +433,36 @@
             )
         return res
 
     if TYPE_CHECKING:
         _limit: Optional[int]
         _offset: Optional[int]
 
-        with_cte: Callable[..., Self]
-        where: Callable[..., Self]
-        filter: Callable[..., Self]
-        orwhere: Callable[..., Self]
-        order_by: Callable[..., Self]
-        order_by_extend: Callable[..., Self]
-        limit: Callable[[Union[int, None]], Self]
-        offset: Callable[[int], Self]
-        paginate: Callable[..., Self]
-
         columns: Callable[..., Self]
-        select_extend: Callable[..., Self]
+        distinct: Callable[..., Self]
+        filter: Callable[..., Self]
+        for_update: Callable[..., Self]
         from_: Callable[..., Self]
-        join: Callable[..., Self]
-        join_from: Callable[..., Self]
         group_by: Callable[..., Self]
         having: Callable[..., Self]
-        distinct: Callable[..., Self]
-        window: Callable[..., Self]
-        for_update: Callable[..., Self]
+        join: Callable[..., Self]
+        join_from: Callable[..., Self]
         lateral: Callable[..., Self]
+        limit: Callable[[Union[int, None]], Self]
         objects: Callable[..., Self]
+        offset: Callable[[int], Self]
+        order_by: Callable[..., Self]
+        order_by_extend: Callable[..., Self]
+        orwhere: Callable[..., Self]
+        paginate: Callable[..., Self]
+        select_extend: Callable[..., Self]
+        switch: Callable[..., Self]
+        where: Callable[..., Self]
+        window: Callable[..., Self]
+        with_cte: Callable[..., Self]
 
         def __await__(self) -> Generator[Any, None, List[TVAIOModel]]:
             return self.manager.run(self).__await__()
 
 
 class AIOModelCompoundSelectQuery(BaseModelSelect[TVAIOModel], ModelCompoundSelectQuery):
     if TYPE_CHECKING:
```

### Comparing `peewee_aio-1.5.3/pyproject.toml` & `peewee_aio-1.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.5.3"
+version = "1.5.5"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Framework :: AsyncIO",
-    "Framework :: Trio",
-]
-packages = [
-    { include = "peewee_aio" },
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Framework :: AsyncIO",
+  "Framework :: Trio",
 ]
+packages = [{ include = "peewee_aio" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 peewee = "^3"
 aio-databases = "^0"
-typing-extensions = {version = "*", python = "<3.11"}
+typing-extensions = { version = "*", python = "<3.11" }
 
 # Optional dependencies
-asyncpg = {version = "*", optional = true}
-aiopg = {version = "*", optional = true}
-aiomysql = {version = "*", optional = true}
-aiosqlite = {version = "*", optional = true}
-triopg = {version = "*", optional = true}
-trio_mysql = {version = "*", optional = true}
+asyncpg = { version = "*", optional = true }
+aiopg = { version = "*", optional = true }
+aiomysql = { version = "*", optional = true }
+aiosqlite = { version = "*", optional = true }
+triopg = { version = "*", optional = true }
+trio_mysql = { version = "*", optional = true }
 
 [tool.poetry.extras]
 asyncpg = ["asyncpg"]
 aiopg = ["aiopg"]
 aiomysql = ["aiomysql"]
 aiosqlite = ["aiosqlite"]
 triopg = ["triopg"]
 trio_mysql = ["trio_mysql"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pytest-mypy = "*"
-pytest-aio = {version = "*", extras = ["trio"]}
+pytest-aio = { version = "*", extras = ["trio"] }
 trio_asyncio = "*"
-aio-databases = {version = "*", extras = [ "aiopg", "aiomysql", "aiosqlite", "asyncpg", "trio_mysql", "triopg"] }
+aio-databases = { version = "*", extras = [
+  "aiopg",
+  "aiomysql",
+  "aiosqlite",
+  "asyncpg",
+  "trio_mysql",
+  "triopg",
+] }
 ruff = "*"
 black = "*"
 pre-commit = "*"
 
 [tool.pytest.ini_options]
 addopts = "-xsv"
 log_cli = true
@@ -83,15 +88,32 @@
 """
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
 select = ["ALL"]
-ignore = ["ARG", "D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003", "COM812"]
+ignore = [
+  "ARG",
+  "D",
+  "UP",
+  "ANN",
+  "DJ",
+  "EM",
+  "RSE",
+  "SLF",
+  "RET",
+  "S101",
+  "PLR2004",
+  "PLR0912",
+  "N804",
+  "A003",
+  "TRY003",
+  "COM812",
+]
 
 [tool.black]
 line-length = 100
 target-version = ["py38", "py39", "py310", "py311"]
 preview = true
 
 [build-system]
```

### Comparing `peewee_aio-1.5.3/PKG-INFO` & `peewee_aio-1.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.5.3
+Version: 1.5.5
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: aiomysql
 Provides-Extra: aiopg
 Provides-Extra: aiosqlite
 Provides-Extra: asyncpg
 Provides-Extra: trio-mysql
 Provides-Extra: triopg
 Requires-Dist: aio-databases (>=0,<1)
```

