# Comparing `tmp/swoop.db-0.1.3.tar.gz` & `tmp/swoop.db-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-0.1.3.tar", last modified: Fri Jun  9 13:21:24 2023, max compression
+gzip compressed data, was "swoop.db-2.0.0.tar", last modified: Thu Jun 22 21:40:37 2023, max compression
```

## Comparing `swoop.db-0.1.3.tar` & `swoop.db-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 13:21:11.000000 swoop.db-0.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-09 13:21:11.000000 swoop.db-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 13:21:11.000000 swoop.db-0.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-09 13:21:11.000000 swoop.db-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-09 13:21:24.411055 swoop.db-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 13:21:11.000000 swoop.db-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-09 13:21:11.000000 swoop.db-0.1.3/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-09 13:21:11.000000 swoop.db-0.1.3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 13:21:11.000000 swoop.db-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 13:21:11.000000 swoop.db-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:21:24.411055 swoop.db-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_item_inserts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.550473 swoop.db-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-22 21:40:19.000000 swoop.db-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 21:40:19.000000 swoop.db-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 21:40:19.000000 swoop.db-2.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 21:40:19.000000 swoop.db-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-22 21:40:37.558473 swoop.db-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-22 21:40:19.000000 swoop.db-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 21:40:19.000000 swoop.db-2.0.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-22 21:40:19.000000 swoop.db-2.0.0/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 21:40:19.000000 swoop.db-2.0.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 21:40:19.000000 swoop.db-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 21:40:19.000000 swoop.db-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:40:37.558473 swoop.db-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00001_version.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_item_inserts.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/test_database.py
```

### Comparing `swoop.db-0.1.3/.github/workflows/publish-image.yml` & `swoop.db-2.0.0/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/.github/workflows/python-test.yml` & `swoop.db-2.0.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/.github/workflows/snyk-scan.yml` & `swoop.db-2.0.0/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/.gitignore` & `swoop.db-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/.pre-commit-config.yaml` & `swoop.db-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/.snyk` & `swoop.db-2.0.0/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/CONTRIBUTING.md` & `swoop.db-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/Dockerfile` & `swoop.db-2.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/LICENSE` & `swoop.db-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/PKG-INFO` & `swoop.db-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.3
+Version: 2.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.3/README.md` & `swoop.db-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/RELEASE.md` & `swoop.db-2.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/docker-compose.yml` & `swoop.db-2.0.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/pyproject.toml` & `swoop.db-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "asyncpg >=0.27.0",
-    "dbami >=0.1.0",
+    "dbami >=0.2.0",
 ]
 dynamic = [
   "version",
   "readme",
 ]
 
 [project.scripts]
```

### Comparing `swoop.db-0.1.3/src/swoop/db/cli.py` & `swoop.db-2.0.0/src/swoop/db/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import argparse
+import json
+from importlib import metadata
 
 import dbami.cli as dbcli
 
 from swoop.db import SwoopDB
 
 SWOOP_DB_ENV_PREFIX = "SWOOP_DB"
 
@@ -39,13 +41,28 @@
 
 # maybe this is indicative of an issue, but mypy doesn't like
 # this monkey patching, so we explicitly ignore the type errors
 dbcli.Arguments = SwoopArgs  # type: ignore
 dbcli.DbamiCommand = SwoopCommand  # type: ignore
 
 
+def is_editable_install(pkg_name: str) -> bool:
+    dist = metadata.distribution(pkg_name)
+    return (
+        json.loads(dist.read_text("direct_url.json") or "{}")
+        .get("dir_info", {})
+        .get("editable", False)
+    )
+
+
 def get_cli() -> dbcli.DbamiCLI:
+    # by definition swoop.db has a project, we don't want init
     dbcli.DbamiCLI.commands.pop("init")
-    cli: dbcli.DbamiCLI = dbcli.DbamiCLI(
-        prog="swoop-db", description="Custom dbami cli instance for swoop-db"
+
+    # we don't want to create new migrations in a non-editable install
+    if not is_editable_install(__package__):
+        dbcli.DbamiCLI.commands.pop("new")
+
+    return dbcli.DbamiCLI(
+        prog="swoop-db",
+        description="Custom dbami cli instance for swoop-db",
     )
-    return cli
```

### Comparing `swoop.db-0.1.3/src/swoop/db/fixtures/base_01.sql` & `swoop.db-2.0.0/src/swoop/db/fixtures/base_01.sql`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,19 @@
   NULL
 );
 
 -- payloads
 INSERT INTO swoop.payload_cache (
   payload_uuid,
   payload_hash,
-  workflow_version,
   workflow_name,
   created_at
 ) VALUES (
   'ade69fe7-1d7d-472e-9f36-7242cc2aca77',
   decode('PsqWxdKjAjrV1+BueXnAS1cWIhU=', 'base64'),
-  1,
   'some_workflow',
   '2023-04-28 15:49:00+00'
 );
 
 -- item - payload relations
 INSERT INTO swoop.item_payload (item_uuid, payload_uuid) VALUES (
   'f5db7f4d-7a72-441c-a9e5-ec2d88c66f5c',
@@ -50,43 +48,47 @@
   action_uuid,
   action_type,
   action_name,
   handler_name,
   parent_uuid,
   created_at,
   priority,
-  payload_uuid
+  payload_uuid,
+  workflow_version
 ) VALUES (
   '2595f2da-81a6-423c-84db-935e6791046e',
   'workflow',
   'action_1',
   'handler_foo',
   'cf8ff7f0-ce5d-4de6-8026-4e551787385f',
   '2023-04-28 15:49:00+00',
   100,
-  'ade69fe7-1d7d-472e-9f36-7242cc2aca77'
+  'ade69fe7-1d7d-472e-9f36-7242cc2aca77',
+  1
 );
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   action_name,
   handler_name,
   parent_uuid,
   created_at,
   priority,
-  payload_uuid
+  payload_uuid,
+  workflow_version
 ) VALUES (
   '81842304-0aa9-4609-89f0-1c86819b0752',
   'workflow',
   'action_2',
   'handler_foo',
   '2595f2da-81a6-423c-84db-935e6791046e',
   '2023-04-28 15:49:00+00',
   100,
-  'ade69fe7-1d7d-472e-9f36-7242cc2aca77'
+  'ade69fe7-1d7d-472e-9f36-7242cc2aca77',
+  1
 );
 
 -- threads
 --   created by action insert trigger
 
 -- events
 --     PENDING events created by action insert trigger
```

### Comparing `swoop.db-0.1.3/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-2.0.0/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files 0% similar despite different names*

```diff
@@ -432,16 +432,18 @@
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
-CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
-RETURNS RECORD
+CREATE FUNCTION swoop.check_cache(
+  plhash bytea, wf_version smallint, wf_name text, invalid timestamptz
+)
+RETURNS record
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   rec RECORD;
 BEGIN
     IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
     -- An entry exists in the cache
```

### Comparing `swoop.db-0.1.3/src/swoop/db/schema.sql` & `swoop.db-2.0.0/src/swoop/db/schema.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 CREATE SCHEMA swoop;
 CREATE SCHEMA partman;
 CREATE EXTENSION pg_partman SCHEMA partman;
 
 
-CREATE TABLE swoop.schema_version (
-  version integer,
-  applied_at timestamptz DEFAULT now()
-);
-
-INSERT INTO swoop.schema_version (version) VALUES (0);
-
-
 CREATE TABLE swoop.event_state (
   name text PRIMARY KEY,
   description text NOT NULL
 );
 
 INSERT INTO swoop.event_state (name, description) VALUES
 ('PENDING', 'Action created and waiting to be executed'),
 ('QUEUED', 'Action queued for handler'),
 ('RUNNING', 'Action being run by handler'),
 ('SUCCESSFUL', 'Action successful'),
 ('FAILED', 'Action failed'),
 ('CANCELED', 'Action canceled'),
 ('TIMED_OUT', 'Action did not complete within allowed timeframe'),
-('UNKNOWN', 'Last update was unknown state'),
 ('BACKOFF', 'Transient error, waiting to retry'),
 (
   'INVALID',
   'Action could not be completed successfully due to '
   || 'configuration error or other incompatibility'
 ),
 (
@@ -37,15 +28,14 @@
 ),
 ('INFO', 'Event is informational and does not change thread state');
 
 
 CREATE TABLE swoop.payload_cache (
   payload_uuid uuid DEFAULT gen_random_uuid() PRIMARY KEY,
   payload_hash bytea UNIQUE,
-  workflow_version smallint NOT NULL,
   workflow_name text NOT NULL,
   created_at timestamptz NOT NULL DEFAULT now(),
   invalid_after timestamptz
 );
 
 CREATE INDEX ON swoop.payload_cache (payload_hash);
 
@@ -55,14 +45,15 @@
   action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
   action_name text,
   handler_name text NOT NULL,
   parent_uuid uuid, -- reference omitted, we don't need referential integrity
   created_at timestamptz NOT NULL DEFAULT now(),
   priority smallint DEFAULT 100,
   payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE RESTRICT,
+  workflow_version smallint NOT NULL,
 
   CONSTRAINT workflow_or_callback CHECK (
     CASE
       WHEN action_type = 'callback'
         THEN
           parent_uuid IS NOT NULL
           AND payload_uuid IS NULL
@@ -230,41 +221,33 @@
 
 CREATE FUNCTION swoop.update_thread()
 RETURNS trigger
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   _latest timestamptz;
-  _status text;
   _next_attempt timestamptz;
 BEGIN
   SELECT last_update FROM swoop.thread WHERE action_uuid = NEW.action_uuid INTO _latest;
 
   -- If the event time is older than the last update we don't update the thread
   -- (we can't use a trigger condition to filter this because we don't know the
   -- last update time from the event alone).
   IF _latest IS NOT NULL AND NEW.event_time < _latest THEN
     RETURN NULL;
   END IF;
 
-  -- Coerce status to UNKNOWN if it doesn't match a known status type
-  SELECT name from swoop.event_state WHERE name = NEW.status
-  UNION
-  SELECT 'UNKNOWN'
-  LIMIT 1
-  INTO _status;
-
   -- If we need a next attempt time let's calculate it
   IF NEW.retry_seconds IS NOT NULL THEN
     SELECT NEW.event_time + (NEW.retry_seconds * interval '1 second') INTO _next_attempt;
   END IF;
 
   UPDATE swoop.thread as t SET
     last_update = NEW.event_time,
-    status = _status,
+    status = NEW.status,
     next_attempt_after = _next_attempt,
     error = NEW.error
   WHERE
     t.action_uuid = NEW.action_uuid;
 
   -- We _could_ try to drop the thread lock here, which would be nice for
   -- swoop-conductor so it didn't have to explicitly unlock, but the unlock
@@ -440,70 +423,42 @@
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
-CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
-RETURNS RECORD
+CREATE FUNCTION swoop.find_cached_action_for_payload(plhash bytea, wf_version smallint)
+RETURNS uuid
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
-  rec RECORD;
+  v_status text;
+  n_version smallint;
+  d_invalid timestamptz;
+  v_action_id uuid;
 BEGIN
-    IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
-    -- An entry exists in the cache
-        DECLARE
-            v_status text;
-            v_job_id uuid;
-            v_payload_id uuid;
-        BEGIN
-            SELECT t.status, t.action_uuid, p.payload_uuid
-            INTO v_status, v_job_id, v_payload_id
-            FROM swoop.payload_cache p
-            INNER JOIN swoop.action a
-            ON p.payload_uuid = a.payload_uuid
-            INNER JOIN swoop.thread t
-            ON a.action_uuid = t.action_uuid
-            WHERE p.payload_hash = plhash
-            ORDER BY t.created_at DESC
-			LIMIT 1;
-
-            IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
-            -- Redirect to job details for that workflow, and do not process
-                SELECT FALSE, v_job_id INTO rec;
-            ELSE
-            -- Reprocess payload
-                DECLARE
-                    n_version smallint;
-                    d_invalid timestamptz;
-                BEGIN
-                    SELECT workflow_version, invalid_after
-                    INTO n_version, d_invalid
-                    FROM   swoop.payload_cache
-                    WHERE  payload_hash = plhash;
-
-                    -- Check workflow version and invalidation
-                    IF wf_version > n_version OR d_invalid < NOW() THEN
-                        IF wf_version > n_version AND d_invalid < NOW() THEN
-                            UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
-                        ELSIF wf_version > n_version THEN
-                            UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
-                        ELSE
-                            UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
-                        END IF;
-                    END IF;
-                    -- Reprocess payload with a new action_uuid
-                    SELECT TRUE, v_payload_id, gen_random_uuid() INTO rec;
-                END;
-            END IF;
-        END;
-	ELSE
-        -- Insert a new entry into cache table and process payload with a new action_uuid
-        INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
-        VALUES (plhash, wf_version, wf_name, invalid)
-        RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
-	END IF;
-    RETURN rec;
+  SELECT t.status, a.workflow_version, p.invalid_after, a.action_uuid
+  INTO v_status, n_version, d_invalid, v_action_id
+  FROM swoop.payload_cache p
+  INNER JOIN swoop.action a
+  USING (payload_uuid)
+  INNER JOIN swoop.thread t
+  USING (action_uuid)
+  WHERE p.payload_hash = plhash
+  ORDER BY t.created_at DESC
+  LIMIT 1;
+
+  IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF') THEN
+  -- Redirect to job details for that workflow, and do not process
+    RETURN v_action_id;
+  ELSIF wf_version > n_version THEN
+    RETURN null;
+  ELSIF d_invalid IS NOT NULL and d_invalid < now() THEN
+    RETURN null;
+  ELSIF v_status IN ('SUCCESSFUL', 'INVALID') THEN
+    RETURN v_action_id;
+  ELSE
+    RETURN null;
+  END IF;
 END;
 $$;
```

### Comparing `swoop.db-0.1.3/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-2.0.0/src/swoop.db.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.3
+Version: 2.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.3/tests/conftest.py` & `swoop.db-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/tests/pgtap/test_action.sql` & `swoop.db-2.0.0/tests/pgtap/test_action.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 BEGIN;
 SET search_path = tap, public;
 SELECT plan(13);
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
   payload_hash,
-  workflow_version,
   workflow_name,
   created_at,
   invalid_after
 ) VALUES (
   'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
   decode('123\000456', 'escape'),
-  1,
   'workflow-a',
   '2023-04-14 00:25:07.388012+00'::timestamptz,
   '2023-04-20 00:25:07.388012+00'::timestamptz
 );
 
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   handler_name,
   action_name,
   created_at,
-  payload_uuid
+  payload_uuid,
+  workflow_version
 ) VALUES (
   'b15120b8-b7ab-4180-9b7a-b0384758f468'::uuid,
   'workflow',
   'argo-workflow',
   'workflow-a',
   '2023-04-13 00:25:07.388012+00'::timestamptz,
-  'cdc73916-500c-4501-a658-dd706a943d19'::uuid
+  'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
+  1
 );
 
 -- check event created as expected
 SELECT results_eq(
   $$
     SELECT
       event_time,
```

### Comparing `swoop.db-0.1.3/tests/pgtap/test_item_inserts.sql` & `swoop.db-2.0.0/tests/pgtap/test_item_inserts.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.3/tests/pgtap/test_limit-locking.sql` & `swoop.db-2.0.0/tests/pgtap/test_limit-locking.sql`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 SET search_path = tap, public;
 SELECT plan(3);
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
   payload_hash,
-  workflow_version,
   workflow_name,
   created_at,
   invalid_after
 ) VALUES (
   'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
   decode('123\000456', 'escape'),
-  1,
   'workflow-a',
   '2023-04-14 00:25:07.388012+00'::timestamptz,
   '2023-04-20 00:25:07.388012+00'::timestamptz
 );
 
 DO
 $$
@@ -25,22 +23,24 @@
   FOR i in 1..300 LOOP
     INSERT INTO swoop.action (
       action_uuid,
       action_type,
       handler_name,
       action_name,
       created_at,
-      payload_uuid
+      payload_uuid,
+      workflow_version
     ) VALUES (
       gen_random_uuid(),
       'workflow',
       'argo-workflow',
       'workflow-a',
       now(),
-      'cdc73916-500c-4501-a658-dd706a943d19'::uuid
+      'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
+      1
     );
   END LOOP;
 END;
 $$;
 
 SELECT
   is(
```

