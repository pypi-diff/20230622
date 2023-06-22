# Comparing `tmp/dbami-0.1.0.tar.gz` & `tmp/dbami-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbami-0.1.0.tar", last modified: Wed May 24 20:57:43 2023, max compression
+gzip compressed data, was "dbami-0.2.0.tar", last modified: Thu Jun 22 20:30:24 2023, max compression
```

## Comparing `dbami-0.1.0.tar` & `dbami-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.487099 dbami-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 20:57:31.000000 dbami-0.1.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.483099 dbami-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.487099 dbami-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-24 20:57:31.000000 dbami-0.1.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-24 20:57:31.000000 dbami-0.1.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-24 20:57:31.000000 dbami-0.1.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-24 20:57:31.000000 dbami-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-24 20:57:31.000000 dbami-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 20:57:31.000000 dbami-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-24 20:57:31.000000 dbami-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-24 20:57:31.000000 dbami-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 20:57:43.487099 dbami-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 20:57:31.000000 dbami-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-24 20:57:31.000000 dbami-0.1.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-24 20:57:31.000000 dbami-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 20:57:31.000000 dbami-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:57:43.487099 dbami-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.483099 dbami-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.487099 dbami-0.1.0/src/dbami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/pg_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 20:57:31.000000 dbami-0.1.0/src/dbami/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.487099 dbami-0.1.0/src/dbami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 20:57:43.000000 dbami-0.1.0/src/dbami.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:43.487099 dbami-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_find_next_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_pg_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-24 20:57:31.000000 dbami-0.1.0/tests/test_sqlfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-22 20:30:14.000000 dbami-0.2.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.890576 dbami-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.894576 dbami-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-22 20:30:14.000000 dbami-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-22 20:30:14.000000 dbami-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-22 20:30:14.000000 dbami-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-22 20:30:14.000000 dbami-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 20:30:14.000000 dbami-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:30:24.898576 dbami-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 20:30:14.000000 dbami-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 20:30:14.000000 dbami-0.2.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 20:30:14.000000 dbami-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-22 20:30:14.000000 dbami-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:30:24.898576 dbami-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.890576 dbami-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.894576 dbami-0.2.0/src/dbami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/pg_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/src/dbami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_find_next_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_pg_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_sqlfile.py
```

### Comparing `dbami-0.1.0/.github/workflows/python-publish.yaml` & `dbami-0.2.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/.github/workflows/python-test.yml` & `dbami-0.2.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/.github/workflows/snyk-scan.yml` & `dbami-0.2.0/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/.gitignore` & `dbami-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/.pre-commit-config.yaml` & `dbami-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/CONTRIBUTING.md` & `dbami-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/LICENSE` & `dbami-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/PKG-INFO` & `dbami-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbami
-Version: 0.1.0
+Version: 0.2.0
 Summary: Lightweight, Python-based, framework-agnostic async PostgreSQL migration tool
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,migration,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: snyk
 License-File: LICENSE
 
 # `dbami`: The database friend you didn't know you needed
 
 A lightweight, Python-based, framework-agnostic, async-compatible PostgreSQL
```

### Comparing `dbami-0.1.0/README.md` & `dbami-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/pyproject.toml` & `dbami-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 snyk = [
     "typing-extensions",
 ]
 
 [tool.setuptools_scm]
 
 [tool.setuptools.dynamic]
-readme = {file = "README.md"}
+readme = {file = "README.md", content-type = "text/markdown"}
 
 [[tool.mypy.overrides]]
 module = [
     "asyncpg",
     "buildpg",
 ]
 ignore_missing_imports = true
```

### Comparing `dbami-0.1.0/src/dbami/cli.py` & `dbami-0.2.0/src/dbami/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,37 +99,55 @@
             action=EnvDefault,
             envvars=[f"{cls.env_prefix}_PG_DUMP"],
             default="pg_dump",
             help=("path to pg_dump executable or name to lookup on path"),
         )
 
     @classmethod
+    def fixture_path(cls, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument(
+            "--fixture-dir",
+            type=Path,
+            action="append",
+            default=[],
+            dest="fixture_dirs",
+            help=(
+                "directory from which to load sql fixtures; "
+                "later directories take precedence"
+            ),
+        )
+
+    @classmethod
     def process_project(
         cls,
         parser: argparse.ArgumentParser,
         args: argparse.Namespace,
     ) -> None:
         project: Optional[Path] = getattr(args, "project_directory", None)
         svt: str = getattr(
             args,
             "schema_version_table",
             SCHEMA_VERSION_TABLE,
         )
+        fixture_dirs: list[Path] = getattr(args, "fixture_dirs", [])
 
         if project is None:
             args.db = DB
             return
 
         try:
             args.db = DB(project, schema_version_table=svt)
         except FileNotFoundError:
             parser.error(
-                f"Project directoy does not appear to be valid: '{project}'",
+                f"Project directory does not appear to be valid: '{project}'",
             )
 
+        for fixture_dir in fixture_dirs:
+            args.db.add_fixture_dir(fixture_dir)
+
 
 class EnvDefault(argparse.Action):
     def __init__(
         self,
         envvars: Sequence[str],
         required: bool = True,
         default: Optional[Any] = None,
@@ -411,15 +429,15 @@
 
             try:
                 await args.db.migrate(
                     target=target,
                     direction="down",
                     database=args.database,
                 )
-            except exceptions.DirectionError as e:
+            except (exceptions.DirectionError, exceptions.MigrationError) as e:
                 printe(e)
                 return 1
             return 0
 
         return syncrun(run())
 
 
@@ -440,15 +458,15 @@
             try:
                 await args.db.create_database(args.database)
             except asyncpg.DuplicateDatabaseError:
                 pass
 
             try:
                 await args.db.migrate(direction="up", database=args.database)
-            except exceptions.DirectionError as e:
+            except (exceptions.DirectionError, exceptions.MigrationError) as e:
                 printe(e)
                 return 1
             return 0
 
         return syncrun(run())
 
 
@@ -477,14 +495,73 @@
     def __call__(self, args: argparse.Namespace) -> int:
         from dbami.version import __version__
 
         print(f"dbami version: {__version__}")
         return 0
 
 
+class ListFixtures(DbamiCommand):
+    help: str = "List all available fixture files on search path"
+    name: str = "list-fixtures"
+
+    def set_args(
+        self,
+        parser: argparse.ArgumentParser,
+    ) -> None:
+        Arguments.project(parser)
+        Arguments.fixture_path(parser)
+
+    def __call__(self, args: argparse.Namespace) -> int:
+        for name, sqlfile in args.db.fixtures.items():
+            print(f"{name} ({sqlfile.path})")
+        return 0
+
+
+class LoadFixture(DbamiCommand):
+    help: str = "Load a sql fixture into the database"
+    name: str = "load-fixture"
+
+    def set_args(
+        self,
+        parser: argparse.ArgumentParser,
+    ) -> None:
+        Arguments.project(parser)
+        Arguments.fixture_path(parser)
+        Arguments.wait_timeout(parser)
+        Arguments.database(parser)
+        parser.add_argument("fixture_name", help="name of fixture to load")
+
+    def __call__(self, args: argparse.Namespace) -> int:
+        async def run() -> int:
+            await args.db.load_fixture(args.fixture_name, database=args.database)
+            return 0
+
+        return syncrun(run())
+
+
+class ExecuteSql(DbamiCommand):
+    help: str = "Run SQL from stdin against the database"
+    name: str = "execute-sql"
+
+    def set_args(
+        self,
+        parser: argparse.ArgumentParser,
+    ) -> None:
+        Arguments.project(parser)
+        Arguments.wait_timeout(parser)
+        Arguments.database(parser)
+
+    def __call__(self, args: argparse.Namespace) -> int:
+        async def run() -> int:
+            await args.db.execute_sql(sys.stdin.read(), database=args.database)
+            return 0
+
+        return syncrun(run())
+
+
 class CLI(abc.ABC):
     def __init__(
         self,
         prog: str,
         description: str,
     ) -> None:
         self.parser = argparse.ArgumentParser(
@@ -541,14 +618,17 @@
             CurrentSchema(),
             LoadSchema(),
             Migrate(),
             Rollback(),
             Up(),
             Verify(),
             Version(),
+            ListFixtures(),
+            LoadFixture(),
+            ExecuteSql(),
         )
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for cmd in DbamiCLI.commands.values():
             self.add_command(cmd)
```

### Comparing `dbami-0.1.0/src/dbami/db.py` & `dbami-0.2.0/src/dbami/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,17 +158,21 @@
         project: Path,
         schema_version_table: str = SCHEMA_VERSION_TABLE,
     ) -> None:
         self.project_dir = project
         self.validate_project()
         self.schema = SqlFile(self.schema_file)
         self.migrations = migrations_from_dir(self.migrations_dir)
-        self.fixtures = {
-            f.name: f for f in (SqlFile(f) for f in self.fixtures_dir.glob("*.sql"))
-        }
+
+        if not self.migrations:
+            raise FileNotFoundError(
+                "Project is missing base migration file. Try reinitializing."
+            )
+
+        self.fixtures = self.load_fixtures_from_dir(self.fixtures_dir)
         self.schema_version_table = schema_version_table
 
     @classmethod
     def project_schema(cls, project: Path):
         return project.joinpath("schema.sql")
 
     @classmethod
@@ -178,15 +182,17 @@
     @classmethod
     def project_fixtures(cls, project: Path):
         return project.joinpath("fixtures")
 
     @classmethod
     def new_project(cls, directory: Path):
         cls.project_schema(directory).touch()
-        cls.project_migrations(directory).mkdir(exist_ok=True)
+        migrations = cls.project_migrations(directory)
+        migrations.mkdir(exist_ok=True)
+        migrations.joinpath("00000_base.up.sql").touch()
         cls.project_fixtures(directory).mkdir(exist_ok=True)
         return cls(directory)
 
     @property
     def schema_file(self):
         return self.project_schema(self.project_dir)
 
@@ -194,14 +200,21 @@
     def migrations_dir(self):
         return self.project_migrations(self.project_dir)
 
     @property
     def fixtures_dir(self):
         return self.project_fixtures(self.project_dir)
 
+    @staticmethod
+    def load_fixtures_from_dir(directory: Path) -> dict[str, SqlFile]:
+        return {f.name: f for f in (SqlFile(f) for f in directory.glob("*.sql"))}
+
+    def add_fixture_dir(self, directory: Path) -> None:
+        self.fixtures.update(self.load_fixtures_from_dir(directory))
+
     def validate_project(self):
         schema = self.schema_file
         migrations = self.migrations_dir
         fixtures = self.fixtures_dir
 
         if not schema.is_file():
             raise FileNotFoundError(
@@ -269,59 +282,57 @@
             conn = await asyncpg.connect(**kwargs)
             yield conn
         finally:
             if conn:
                 await conn.close()
 
     @classmethod
-    async def create_database(cls, db_name: str, **kwargs) -> None:
+    async def execute_sql(cls, sql: str, *query_params, **kwargs) -> None:
+        if not sql:
+            # asyncpg chokes on an empty string,
+            # so we bail out early on any non-truthy sql
+            return
+
         async with AsyncExitStack() as stack:
-            kwargs["database"] = ""
             conn: asyncpg.Connection = kwargs.get(
-                "conn"
+                "conn",
             ) or await stack.enter_async_context(cls.get_db_connection(**kwargs))
-            await conn.execute(f'CREATE DATABASE "{db_name}";')
+            await conn.execute(sql, *query_params)
+
+    @classmethod
+    async def create_database(cls, db_name: str, **kwargs) -> None:
+        kwargs["database"] = ""
+        await cls.execute_sql(f'CREATE DATABASE "{db_name}";', **kwargs)
 
     @classmethod
     async def drop_database(cls, db_name: str, **kwargs) -> None:
-        async with AsyncExitStack() as stack:
-            kwargs["database"] = ""
-            conn: asyncpg.Connection = kwargs.get(
-                "conn"
-            ) or await stack.enter_async_context(cls.get_db_connection(**kwargs))
-            await conn.execute(f'DROP DATABASE "{db_name}";')
+        kwargs["database"] = ""
+        await cls.execute_sql(f'DROP DATABASE "{db_name}";', **kwargs)
 
     @classmethod
     async def run_sqlfile(cls, sqlfile: SqlFile, **kwargs) -> None:
-        sql = sqlfile.path.read_text()
-
-        if not sql:
-            return
-
-        async with AsyncExitStack() as stack:
-            conn: asyncpg.Connection = kwargs.get(
-                "conn"
-            ) or await stack.enter_async_context(cls.get_db_connection(**kwargs))
-            await conn.execute(sql)
+        await cls.execute_sql(sqlfile.path.read_text(), **kwargs)
 
     async def get_current_version(
         self,
         **kwargs,
     ) -> Optional[int]:
         async with AsyncExitStack() as stack:
             conn: asyncpg.Connection = kwargs.get(
                 "conn"
             ) or await stack.enter_async_context(self.get_db_connection(**kwargs))
 
             query, _ = render(
-                """SELECT
-version
-FROM :version_table
-WHERE applied_at = (SELECT max(applied_at) from :version_table)
-""",
+                """
+                SELECT
+                    version
+                FROM :version_table
+                WHERE
+                    applied_at = (SELECT max(applied_at) from :version_table)
+                """,
                 version_table=V(self.schema_version_table),
             )
 
             try:
                 version = await conn.fetchval(query)
             except asyncpg.UndefinedTableError:
                 return None
@@ -335,16 +346,26 @@
         schema_version = _version if _version is not None else -1
         next_migration = find_next_migration(schema_version, self.migrations)
 
         while next_migration:
             yield next_migration
             next_migration = next_migration.child
 
-    async def load_schema(self, **kwargs):
-        await self.run_sqlfile(self.schema, **kwargs)
+    async def load_schema(self, **kwargs) -> None:
+        async with AsyncExitStack() as stack:
+            conn: asyncpg.Connection = kwargs.pop(
+                "conn",
+                None,
+            ) or await stack.enter_async_context(self.get_db_connection(**kwargs))
+            await stack.enter_async_context(conn.transaction())
+            await self.run_sqlfile(self.schema, conn=conn, **kwargs)
+            await self._update_schema_version(
+                max(self.migrations.keys()),
+                conn,
+            )
 
     async def load_fixture(self, fixture_name: str, **kwargs):
         try:
             fixture = self.fixtures[fixture_name]
         except KeyError:
             raise FileNotFoundError(f"Unknown fixture: '{fixture_name}'")
 
@@ -353,58 +374,62 @@
     async def _update_schema_version(
         self,
         version: int,
         conn,
     ):
         table_sql, _ = render(
             """
-CREATE TABLE IF NOT EXISTS :version_table (
-    version integer,
-    applied_at timestamptz NOT NULL DEFAULT now()
-);
-
-CREATE INDEX ON :version_table (version);
-CREATE INDEX ON :version_table (applied_at);
-""",
+            CREATE TABLE IF NOT EXISTS :version_table (
+                version integer,
+                applied_at timestamptz NOT NULL DEFAULT now()
+            );
+
+            CREATE INDEX ON :version_table (version);
+            CREATE INDEX ON :version_table (applied_at);
+            """,
             version_table=V(self.schema_version_table),
         )
         version_sql, params = render(
             "INSERT INTO :version_table (version) VALUES (:version)",
             version_table=V(self.schema_version_table),
             version=version,
         )
 
         try:
             # use a subtransaction (save point) to prevent this
             # "expected" exception from rolling back the migration
             async with conn.transaction():
-                await conn.execute(table_sql)
+                await self.execute_sql(table_sql, conn=conn)
         except asyncpg.InvalidSchemaNameError:
             schema = self.schema_version_table.split(".")[0]
             schema_sql, _ = render(
                 "CREATE SCHEMA IF NOT EXISTS :schema",
                 schema=V(schema),
             )
-            await conn.execute(schema_sql)
-            await conn.execute(table_sql)
+            await self.execute_sql(schema_sql, conn=conn)
+            await self.execute_sql(table_sql, conn=conn)
 
-        await conn.execute(version_sql, *params)
+        await self.execute_sql(version_sql, *params, conn=conn)
 
     async def migrate(
         self,
         target: Optional[int] = None,
         direction: Union[Literal["up"], Literal["down"], None] = None,
         **kwargs,
     ):
         if not self.migrations:
             return
 
+        min_migration = min(self.migrations.keys())
+
         async with self.get_db_connection(**kwargs) as conn:
             _version = await self.get_current_version(conn=conn)
-            schema_version: int = _version if _version is not None else -1
+            schema_version: int = (
+                _version if _version is not None else min_migration - 1
+            )
 
             if target is None:
                 target = max(self.migrations.keys())
 
                 # if target was not specified then we never want to roll back
                 if schema_version > target:
                     logger.warning(
@@ -413,14 +438,20 @@
                     )
                     return
 
             if schema_version == target:
                 return
 
             if target not in self.migrations:
+                if target < min_migration:
+                    raise exceptions.MigrationError(
+                        f"Target migration ID '{target}' would cause unsupported "
+                        f"rollback of base migration ID '{min_migration}'"
+                    )
+
                 raise exceptions.MigrationError(
                     f"Target migration ID '{target}' has no known migration"
                 )
 
             # moving forward
             if schema_version < target:
                 if direction and direction != "up":
@@ -496,38 +527,34 @@
             "--exclude-table",
             self.schema_version_table,
         ]
 
         async def schema():
             await self.create_database(schema_db)
             await self.load_schema(database=schema_db)
-            version = await self.get_current_version(database=schema_db)
-            rc, dump = await _pg_dump("-d", schema_db, *dump_args, pg_dump=pg_dump)
-            return version, rc, dump
+            return await _pg_dump("-d", schema_db, *dump_args, pg_dump=pg_dump)
 
         async def migrate():
             await self.create_database(migrate_db)
             await self.migrate(database=migrate_db)
-            version = await self.get_current_version(database=migrate_db)
-            rc, dump = await _pg_dump("-d", migrate_db, *dump_args, pg_dump=pg_dump)
-            return version, rc, dump
+            return await _pg_dump("-d", migrate_db, *dump_args, pg_dump=pg_dump)
 
         try:
             results: tuple[
-                tuple[Optional[int], Optional[int], str],
-                tuple[Optional[int], Optional[int], str],
+                tuple[Optional[int], str],
+                tuple[Optional[int], str],
             ] = await asyncio.gather(schema(), migrate())
         finally:
             await self.drop_database(schema_db)
             await self.drop_database(migrate_db)
 
         schema_results, migrate_results = results
 
-        schema_version, schema_rc, schema_dump = schema_results
-        migrate_version, migrate_rc, migrate_dump = migrate_results
+        schema_rc, schema_dump = schema_results
+        migrate_rc, migrate_dump = migrate_results
 
         if schema_rc != 0 or migrate_rc != 0:
             raise RuntimeError("Encoutered an error dumping databases")
 
         is_diff: bool = False
 
         if schema_dump != migrate_dump:
@@ -539,16 +566,8 @@
                     schema_dump.splitlines(keepends=True),
                     migrate_dump.splitlines(keepends=True),
                     fromfile="schema.sql",
                     tofile="combined migrations",
                 )
             )
 
-        if schema_version != migrate_version:
-            is_diff = True
-            print(
-                "Version from schema doesn't match that from migrations: "
-                f"{schema_version} != {migrate_version}",
-                file=output,
-            )
-
         return not is_diff
```

### Comparing `dbami-0.1.0/src/dbami/pg_dump.py` & `dbami-0.2.0/src/dbami/pg_dump.py`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/src/dbami.egg-info/PKG-INFO` & `dbami-0.2.0/src/dbami.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbami
-Version: 0.1.0
+Version: 0.2.0
 Summary: Lightweight, Python-based, framework-agnostic async PostgreSQL migration tool
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,migration,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: snyk
 License-File: LICENSE
 
 # `dbami`: The database friend you didn't know you needed
 
 A lightweight, Python-based, framework-agnostic, async-compatible PostgreSQL
```

### Comparing `dbami-0.1.0/src/dbami.egg-info/SOURCES.txt` & `dbami-0.2.0/src/dbami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/tests/conftest.py` & `dbami-0.2.0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 
 import asyncpg
 import pytest
 
 from dbami.db import DB
-from dbami.util import random_name, syncrun
+from dbami.util import syncrun
 
 
 @pytest.fixture(scope="session")
 def test_db_name_stem() -> str:
     return "dbami_test"
 
 
@@ -29,43 +29,48 @@
 
 @pytest.fixture
 def project(tmp_chdir: Path):
     # create some migrations before instantiating the DB instance
     # to ensure we test the migration load process
     migrations_dir = DB.project_migrations(tmp_chdir)
     migrations_dir.mkdir()
-    migrations_dir.joinpath("00_migration.up.sql").touch()
-    migrations_dir.joinpath("00_migration.down.sql").touch()
+    migrations_dir.joinpath("00000_base.down.sql").touch()
     migrations_dir.joinpath("01_migration.up.sql").touch()
     db: DB = DB.new_project(tmp_chdir)
-    db.schema.path.write_text(
-        """
-CREATE TABLE IF NOT EXISTS schema_version (
-  version integer,
-  applied_at timestamptz NOT NULL DEFAULT now()
-);
-
-CREATE INDEX ON schema_version (version);
-CREATE INDEX ON schema_version (applied_at);
-
-INSERT INTO schema_version (version) VALUES (4);
-"""
-    )
     db.new_migration("migration")
     db.new_migration("migration")
     db.new_migration("migration")
     db.new_fixture("a_fixture")
+    db.fixtures["a_fixture"].path.write_text("select current_database();")
     return db
 
 
 @pytest.fixture
-def tmp_db(test_db_name_stem):
-    db_name = random_name(test_db_name_stem)
+def extra_fixtures(tmp_path: Path) -> Path:
+    tfdir = tmp_path.joinpath("test_fixtures")
+    tfdir.mkdir()
+    # override the fixture in the project fixtures dir
+    tfdir.joinpath("a_fixture.sql").write_text("select current_database();")
+    # add another fixture
+    tfdir.joinpath("b_fixture.sql").write_text("select current_database();")
+    return tfdir
+
+
+@pytest.fixture
+def tmp_db_name(test_db_name_stem: str, request):
+    db_name = (
+        f"{test_db_name_stem}_{request.module.__name__}:{request.function.__name__}"
+    )
 
     try:
-        syncrun(DB.create_database(db_name))
         yield db_name
     finally:
         try:
             syncrun(DB.drop_database(db_name))
         except asyncpg.InvalidCatalogNameError:
             pass
+
+
+@pytest.fixture
+def tmp_db(tmp_db_name: str):
+    syncrun(DB.create_database(tmp_db_name))
+    return tmp_db_name
```

### Comparing `dbami-0.1.0/tests/test_cli.py` & `dbami-0.2.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from pathlib import Path
 from typing import Optional, TextIO
 
 import asyncpg
 import pytest
 
 from dbami import exceptions
-from dbami.cli import get_cli
+from dbami.__main__ import main as cli_main
 from dbami.db import DB
-from dbami.util import random_name, syncrun
+from dbami.util import syncrun
 
 
 @contextlib.contextmanager
 def replace_streams(stdin: Optional[TextIO] = None):
     new_in = io.StringIO() if stdin is None else stdin
     new_out, new_err = io.StringIO(), io.StringIO()
     old_in, old_out, old_err = sys.stdin, sys.stdout, sys.stderr
@@ -25,15 +25,15 @@
         sys.stdin, sys.stdout, sys.stderr = old_in, old_out, old_err
 
 
 def run_cli(*args, stdin: Optional[TextIO] = None):
     rc = None
     with replace_streams(stdin=stdin) as (out, err):
         try:
-            get_cli()(args)
+            cli_main(args)
         except SystemExit as e:
             rc = e.code
 
     out.seek(0)
     err.seek(0)
 
     return rc, out.read(), err.read()
@@ -48,27 +48,14 @@
 
 
 @pytest.fixture
 def project_dir(project: DB) -> Path:
     return project.project_dir
 
 
-@pytest.fixture
-def tmp_db_name():
-    db_name = random_name("dbami_test")
-
-    try:
-        yield db_name
-    finally:
-        try:
-            syncrun(DB.drop_database(db_name))
-        except asyncpg.InvalidCatalogNameError:
-            pass
-
-
 def test_cli():
     rc, out, err = run_cli()
     print(out)
     print(err)
     assert rc == 2
 
 
@@ -318,19 +305,19 @@
 def test_rollback_bad_target(tmp_db, project_dir):
     rc, out, err = run_cli("migrate", "--database", tmp_db)
     print(out)
     print(err)
     assert rc == 0
 
     target = 5
-    with pytest.raises(exceptions.MigrationError) as exc_info:
-        run_cli("rollback", "--target", str(target), "--database", tmp_db)
-    assert (
-        str(exc_info.value) == f"Target migration ID '{target}' has no known migration"
-    )
+    rc, out, err = run_cli("rollback", "--target", str(target), "--database", tmp_db)
+    print(out)
+    print(err)
+    assert rc == 1
+    assert err == f"Target migration ID '{target}' has no known migration\n"
 
 
 def test_rollback_nonint_target(tmp_db, project_dir):
     target = "not-an-int"
     rc, out, err = run_cli("rollback", "--target", str(target), "--database", tmp_db)
     assert rc != 0
 
@@ -347,14 +334,31 @@
     assert rc == 1
     assert (
         err
         == "Target would move version forward and direction is down: can't go 2 -> 4\n"
     )
 
 
+def test_rollback_zero(tmp_db, project_dir):
+    DB(project_dir).migrations[0].down.path.touch()
+    rc, out, err = run_cli("migrate", "--target", "0", "--database", tmp_db)
+    print(out)
+    print(err)
+    assert rc == 0
+
+    rc, out, err = run_cli("rollback", "--database", tmp_db)
+    print(out)
+    print(err)
+    assert rc == 1
+    assert err == (
+        "Target migration ID '-1' would cause unsupported "
+        "rollback of base migration ID '0'\n"
+    )
+
+
 def test_rollback_no_schema(tmp_db, project_dir):
     rc, out, err = run_cli("rollback", "--database", tmp_db)
     print(out)
     print(err)
     assert rc == 1
     assert err == "Cannot rollback: database has no applied schema version\n"
 
@@ -411,23 +415,14 @@
 
 def test_verify_bad_pg_dump(tmp_db, project_dir):
     with pytest.raises(FileNotFoundError) as exc_info:
         run_cli("verify", "--pg-dump", "/bad/path")
     assert str(exc_info.value).startswith("pg_dump could not be located:")
 
 
-def test_verify_wrong_version(tmp_db, project_dir):
-    DB(project_dir).new_migration("new_migration")
-    rc, out, err = run_cli("verify")
-    print(out)
-    print(err)
-    assert rc == 1
-    assert err == "Version from schema doesn't match that from migrations: 4 != 5\n"
-
-
 def test_verify_schema_diff(tmp_db, project_dir):
     DB(project_dir).migrations[4].up.path.write_text(
         "CREATE TABLE test_table (id text NOT NULL);"
     )
     rc, out, err = run_cli("verify")
     print(out)
     print(err)
@@ -439,7 +434,62 @@
     from dbami.version import __version__
 
     rc, out, err = run_cli("version")
     print(out)
     print(err)
     assert rc == 0
     assert out.strip().endswith(str(__version__))
+
+
+def test_list_fixtures(project_dir):
+    rc, out, err = run_cli("list-fixtures")
+    print(out)
+    print(err)
+    assert rc == 0
+    assert len(out.splitlines()) == 1
+    assert out.startswith("a_fixture (")
+
+
+def test_list_fixtures_extra(project_dir, extra_fixtures):
+    rc, out, err = run_cli("list-fixtures", "--fixture-dir", str(extra_fixtures))
+    print(out)
+    print(err)
+    assert rc == 0
+    assert len(out.splitlines()) == 2
+
+
+def test_load_fixture(tmp_db, project_dir):
+    rc, out, err = run_cli("load-fixture", "--database", tmp_db, "a_fixture")
+    print(out)
+    print(err)
+    assert rc == 0
+
+
+def test_load_fixtures_extra(tmp_db, project_dir, extra_fixtures):
+    rc, out, err = run_cli(
+        "load-fixture",
+        "--database",
+        tmp_db,
+        "--fixture-dir",
+        str(extra_fixtures),
+        "b_fixture",
+    )
+    print(out)
+    print(err)
+    assert rc == 0
+
+
+def test_execute_sql(tmp_db, project):
+    stdin = io.StringIO()
+    stdin.write("create table a_table (id int primary key);")
+    stdin.seek(0)
+    rc, out, err = run_cli(
+        "execute-sql",
+        "--database",
+        tmp_db,
+        stdin=stdin,
+    )
+    print(out)
+    print(err)
+    assert rc == 0
+    syncrun(project.execute_sql("select * from a_table", database=tmp_db))
+    assert True
```

### Comparing `dbami-0.1.0/tests/test_db.py` & `dbami-0.2.0/tests/test_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 from pathlib import Path
 from typing import Union
 
 import asyncpg
 import pytest
 
+from dbami import exceptions
 from dbami.db import DB, Migration
 
 
 def test_no_project(tmp_path: Path):
     with pytest.raises(FileNotFoundError) as exc_info:
         DB(tmp_path)
     assert str(exc_info.value).startswith("Schema does not exist or is wrong type:")
@@ -17,23 +18,34 @@
 def test_init(tmp_path: Path):
     db: DB = DB.new_project(tmp_path)
     assert db.fixtures_dir.is_dir()
     assert db.migrations_dir.is_dir()
     assert db.schema_file.is_file()
 
 
+def test_project_no_migrations(tmp_path: Path):
+    db: DB = DB.new_project(tmp_path)
+    db.migrations[0].up.path.unlink()
+    with pytest.raises(FileNotFoundError) as exc_info:
+        DB(tmp_path)
+    assert (
+        str(exc_info.value)
+        == "Project is missing base migration file. Try reinitializing."
+    )
+
+
 def test_new_migration(empty_project):
     migration_name = "a-migration"
     empty_project.new_migration(migration_name)
     new_migration = max(empty_project.migrations.values())
     assert new_migration.name == migration_name
     assert new_migration.up.path.is_file()
     assert new_migration.down.path.is_file()
-    assert new_migration.id == 0
-    assert 0 in empty_project.migrations
+    assert new_migration.id == 1
+    assert 1 in empty_project.migrations
 
 
 def test_new_fixture(empty_project):
     fixture_name = "a_fixture"
     empty_project.new_fixture(fixture_name)
     assert fixture_name in empty_project.fixtures
     fixture = empty_project.fixtures[fixture_name]
@@ -78,14 +90,21 @@
     schema_file.write_text(schema)
     with pytest.raises(asyncpg.UndefinedTableError):
         await project.load_schema(database=tmp_db)
     assert await project.get_current_version(database=tmp_db) is None
 
 
 @pytest.mark.asyncio
+async def test_load_schema_existing_conn(tmp_db, project):
+    async with project.get_db_connection(database=tmp_db) as conn:
+        await project.load_schema(conn=conn)
+    assert await project.get_current_version(database=tmp_db) == 4
+
+
+@pytest.mark.asyncio
 async def test_migrate(tmp_db, project):
     await project.migrate(database=tmp_db)
     assert await project.get_current_version(database=tmp_db) == 4
 
 
 @pytest.mark.asyncio
 async def test_migrate_bad_file(tmp_db, project):
@@ -110,23 +129,43 @@
         await project.migrate(target=2, database=tmp_db)
     assert await project.get_current_version(database=tmp_db) == 3
 
 
 @pytest.mark.asyncio
 async def test_rollback_no_down(tmp_db, project):
     await project.load_schema(database=tmp_db)
-    with pytest.raises(ValueError) as exc_info:
+    with pytest.raises(exceptions.MigrationError) as exc_info:
         await project.migrate(target=1, database=tmp_db)
     assert str(exc_info.value) == (
         "Cannot rollback from version 4 to 1: "
         "one or more migrations do not have down files"
     )
 
 
 @pytest.mark.asyncio
+async def test_rollback_zero(tmp_db, project):
+    project.migrations[0].down.path.touch()
+    await project.migrate(target=0, database=tmp_db)
+    with pytest.raises(exceptions.MigrationError) as exc_info:
+        await project.migrate(target=-1, database=tmp_db)
+    assert str(exc_info.value) == (
+        "Target migration ID '-1' would cause unsupported "
+        "rollback of base migration ID '0'"
+    )
+
+
+@pytest.mark.asyncio
+async def test_migrate_no_migrations(tmp_db, tmp_path) -> None:
+    db = DB.new_project(tmp_path)
+    db.migrations.clear()
+    await db.migrate(database=tmp_db)
+    assert await db.get_current_version(database=tmp_db) is None
+
+
+@pytest.mark.asyncio
 async def test_migrate_no_unapplied_migrations(tmp_db, project):
     await project.load_schema(database=tmp_db)
     await project.migrate(database=tmp_db)
     assert await project.get_current_version(database=tmp_db) == 4
 
 
 @pytest.mark.asyncio
@@ -143,52 +182,46 @@
     await project.migrate(database=tmp_db)
     assert await project.get_current_version(database=tmp_db) == 4
 
 
 @pytest.mark.asyncio
 async def test_migrate_unknown_target(tmp_db, project):
     target = 10
-    with pytest.raises(ValueError) as exc_info:
+    with pytest.raises(exceptions.MigrationError) as exc_info:
         await project.migrate(target, database=tmp_db)
     assert (
         str(exc_info.value) == f"Target migration ID '{target}' has no known migration"
     )
 
 
 @pytest.mark.asyncio
 async def test_migrate_rollback_from_unknown_schema(tmp_db, project):
     target = 3
     await project.migrate(target, database=tmp_db)
     del project.migrations[target]
-    with pytest.raises(ValueError) as exc_info:
+    with pytest.raises(exceptions.MigrationError) as exc_info:
         await project.migrate(0, database=tmp_db)
     assert (
         str(exc_info.value)
         == f"Schema version '{target}' does not have associated migration"
     )
 
 
 @pytest.mark.asyncio
-async def test_migrate_no_migrations(tmp_db, tmp_path) -> None:
-    db = DB.new_project(tmp_path)
-    await db.migrate(database=tmp_db)
-    assert await db.get_current_version(database=tmp_db) is None
-
-
-@pytest.mark.asyncio
 async def test_yield_unapplied_migrations(tmp_db, project) -> None:
     unapplied: list[Migration] = [
         m async for m in project.yield_unapplied_migrations(database=tmp_db)
     ]
     assert len(unapplied) == 5
 
 
 @pytest.mark.asyncio
 async def test_yield_unapplied_migrations_none(tmp_db, tmp_path) -> None:
     db: DB = DB.new_project(tmp_path)
+    await db.migrate(database=tmp_db)
     unapplied: list[Migration] = [
         m async for m in db.yield_unapplied_migrations(database=tmp_db)
     ]
     assert len(unapplied) == 0
 
 
 @pytest.mark.asyncio
@@ -210,40 +243,29 @@
     assert same
 
 
 @pytest.mark.asyncio
 async def test_verify_different_schema(project) -> None:
     project.migrations[4].up.path.write_text(
         """
-CREATE SCHEMA some_schema;
-CREATE TABLE some_schema.some_table (
-    a_col integer PRIMARY KEY,
-    b_col text UNIQUE
-);
-"""
+        CREATE SCHEMA some_schema;
+        CREATE TABLE some_schema.some_table (
+            a_col integer PRIMARY KEY,
+            b_col text UNIQUE
+        );
+        """,
     )
     output = io.StringIO()
     same = await project.verify(output=output)
     assert not same
     output.seek(0)
     outstr = output.read()
     assert outstr.startswith("--- schema.sql")
 
 
-@pytest.mark.asyncio
-async def test_verify_different_version(project) -> None:
-    project.new_migration("migration")
-    output = io.StringIO()
-    same = await project.verify(output=output)
-    assert not same
-    output.seek(0)
-    outstr = output.read()
-    assert outstr == "Version from schema doesn't match that from migrations: 4 != 5\n"
-
-
 def test_load_project_dir(project) -> None:
     expected_migration_count = 5
     project_dir = project.project_dir
     db = DB(project_dir)
     assert len(db.migrations) == expected_migration_count
     assert len(db.fixtures) == 1
 
@@ -251,7 +273,15 @@
     migrations = []
     child: Union[Migration, None] = db.migrations[0]
     while child:
         migrations.append(child)
         child = child.child
 
     assert len(migrations) == expected_migration_count
+
+
+def test_add_fixture_dir(project, extra_fixtures) -> None:
+    project.add_fixture_dir(extra_fixtures)
+
+    assert len(project.fixtures) == 2
+    for fixture in project.fixtures.values():
+        assert fixture.path.parent == extra_fixtures
```

### Comparing `dbami-0.1.0/tests/test_find_next_migration.py` & `dbami-0.2.0/tests/test_find_next_migration.py`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/tests/test_migration.py` & `dbami-0.2.0/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/tests/test_pg_dump.py` & `dbami-0.2.0/tests/test_pg_dump.py`

 * *Files identical despite different names*

### Comparing `dbami-0.1.0/tests/test_sqlfile.py` & `dbami-0.2.0/tests/test_sqlfile.py`

 * *Files identical despite different names*

