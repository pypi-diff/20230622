# Comparing `tmp/pytest_gitconfig-0.1.1.tar.gz` & `tmp/pytest_gitconfig-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_gitconfig-0.1.1.tar", last modified: Sat Jun 17 01:12:59 2023, max compression
+gzip compressed data, was "pytest_gitconfig-0.2.0.tar", last modified: Thu Jun 22 09:18:16 2023, max compression
```

## Comparing `pytest_gitconfig-0.1.1.tar` & `pytest_gitconfig-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-06-16 09:32:31.548634 pytest_gitconfig-0.1.1/LICENSE
--rw-r--r--   0        0        0      823 2023-06-16 13:23:04.119535 pytest_gitconfig-0.1.1/README.md
--rw-r--r--   0        0        0     3479 2023-06-17 01:12:59.043561 pytest_gitconfig-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-16 09:32:31.539634 pytest_gitconfig-0.1.1/src/pytest_gitconfig/__init__.py
--rw-r--r--   0        0        0       62 2023-06-16 13:18:04.260801 pytest_gitconfig-0.1.1/src/pytest_gitconfig/_version.py
--rw-r--r--   0        0        0     2863 2023-06-16 13:21:58.308562 pytest_gitconfig-0.1.1/src/pytest_gitconfig/plugin.py
--rw-r--r--   0        0        0        0 2023-06-16 09:32:31.537634 pytest_gitconfig-0.1.1/src/pytest_gitconfig/py.typed
--rw-r--r--   0        0        0       64 2023-06-16 13:10:10.760439 pytest_gitconfig-0.1.1/tests/conftests.py
--rw-r--r--   0        0        0      633 2023-06-16 13:11:36.083976 pytest_gitconfig-0.1.1/tests/test_override_defaults.py
--rw-r--r--   0        0        0      788 2023-06-16 13:11:35.517979 pytest_gitconfig-0.1.1/tests/test_pytest_gitconfig.py
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 pytest_gitconfig-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-16 09:32:31.548634 pytest_gitconfig-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2092 2023-06-22 09:14:34.535563 pytest_gitconfig-0.2.0/README.md
+-rw-r--r--   0        0        0     3697 2023-06-22 09:18:16.469405 pytest_gitconfig-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-06-22 09:14:09.418841 pytest_gitconfig-0.2.0/src/pytest_gitconfig/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-16 13:18:04.260801 pytest_gitconfig-0.2.0/src/pytest_gitconfig/_version.py
+-rw-r--r--   0        0        0     2648 2023-06-22 09:10:07.835012 pytest_gitconfig-0.2.0/src/pytest_gitconfig/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:32:31.537634 pytest_gitconfig-0.2.0/src/pytest_gitconfig/py.typed
+-rw-r--r--   0        0        0       64 2023-06-16 13:10:10.760439 pytest_gitconfig-0.2.0/tests/conftests.py
+-rw-r--r--   0        0        0      826 2023-06-22 08:57:18.934341 pytest_gitconfig-0.2.0/tests/test_override_defaults.py
+-rw-r--r--   0        0        0      788 2023-06-16 13:11:35.517979 pytest_gitconfig-0.2.0/tests/test_pytest_gitconfig.py
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 pytest_gitconfig-0.2.0/PKG-INFO
```

### Comparing `pytest_gitconfig-0.1.1/LICENSE` & `pytest_gitconfig-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.1/pyproject.toml` & `pytest_gitconfig-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
     "pytest>=7.1.2",
 ]
-version = "0.1.1"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/noirbizarre/pytest-gitconfig"
 Documentation = "https://github.com/noirbizarre/pytest-gitconfig#readme"
@@ -48,15 +48,15 @@
 source = "scm"
 write_to = "src/pytest_gitconfig/_version.py"
 write_template = "__version__ = \"{}\""
 
 [tool.pdm.dev-dependencies]
 test = [
     "pytest-sugar>=0.9.5",
-    "pytest-cov>=3.0.0",
+    "coverage[toml]>=4",
 ]
 lint = [
     "black>=23.3.0",
     "mypy>=1.3.0",
     "ruff>=0.0.270",
 ]
 tox = [
@@ -90,17 +90,23 @@
 [tool.pdm.scripts.typing]
 help = "Full typing linting (includes imported packages and uncommmited files)"
 cmd = "mypy src tests --warn-unused-ignores"
 
 [tool.pdm.scripts.cover]
 help = "Run the test suite with coverage"
 composite = [
-    "  test\n    --cov\n    --cov-report=term\n    --cov-report=html:reports/coverage\n    --cov-report=xml:reports/coverage.xml\n    --no-cov-on-fail\n    --junitxml=reports/tests.xml\n  ",
+    "coverage run --append -m pytest {args} --junitxml=reports/tests.xml",
+    "coverage report",
+    "coverage html -d reports/coverage",
+    "coverage xml -o reports/coverage.xml",
 ]
 
+[tool.pdm.scripts.cover.env]
+COV_CORE_SOURCE = "src"
+
 [tool.pdm.scripts."cover:all"]
 help = "Run the test suite against all supported Python version"
 cmd = "tox --parallel"
 
 [tool.pdm.scripts.changelog]
 help = "Update the changelog"
 cmd = "cz changelog"
@@ -124,21 +130,28 @@
 testpaths = [
     "src/",
     "tests/",
 ]
 
 [tool.coverage.run]
 source = [
-    "src",
+    "src/",
 ]
 branch = true
 omit = [
     "tests/*",
 ]
 
+[tool.coverage.report]
+exclude_also = [
+    "def __repr__",
+    "if TYPE_CHECKING:",
+]
+ignore_errors = true
+
 [tool.black]
 line-length = 100
 
 [tool.ruff]
 line-length = 110
 respect-gitignore = true
 select = [
@@ -150,14 +163,19 @@
     "I001",
 ]
 src = [
     "src",
     "tests",
 ]
 
+[tool.ruff.per-file-ignores]
+"__init__.py" = [
+    "F401",
+]
+
 [tool.ruff.isort]
 known-first-party = [
     "pytest_gitconfig",
 ]
 known-third-party = [
     "pytest",
 ]
```

### Comparing `pytest_gitconfig-0.1.1/src/pytest_gitconfig/plugin.py` & `pytest_gitconfig-0.2.0/src/pytest_gitconfig/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from __future__ import annotations
 
 import os
-import shlex
-import subprocess
 
 from configparser import ConfigParser
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Iterator
 
 import pytest
 
-DEFAULT_GIT_USER_NAME = "John Doe"
-DEFAULT_GIT_USER_EMAIL = "john.doe@local.dev"
+DEFAULT_GIT_USER_NAME = "Pytest"
+DEFAULT_GIT_USER_EMAIL = "pytest@local.dev"
 DEFAULT_GIT_BRANCH = "main"
 
 
-def run(cmd: str, *args, **kwargs) -> subprocess.CompletedProcess[str]:
-    real_args = [cmd, *args] if args else shlex.split(cmd)
-    return subprocess.run(real_args, **kwargs)
-
-
 @pytest.fixture(scope="session")
 def sessionpatch() -> Iterator[pytest.MonkeyPatch]:
     with pytest.MonkeyPatch.context() as mp:
         yield mp
 
 
 @pytest.fixture(scope="session")
```

### Comparing `pytest_gitconfig-0.1.1/tests/test_pytest_gitconfig.py` & `pytest_gitconfig-0.2.0/tests/test_pytest_gitconfig.py`

 * *Files identical despite different names*

