# Comparing `tmp/asphalt-redis-4.0.0.tar.gz` & `tmp/asphalt-redis-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphalt-redis-4.0.0.tar", last modified: Thu Apr 14 15:31:53 2022, max compression
+gzip compressed data, was "asphalt-redis-4.1.0.tar", last modified: Thu Jun 22 14:34:12 2023, max compression
```

## Comparing `asphalt-redis-4.0.0.tar` & `asphalt-redis-4.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.286465 asphalt-redis-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-04-14 15:31:53.286465 asphalt-redis-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/modules/component.rst
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 15:31:53.286465 asphalt-redis-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/src/asphalt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.282465 asphalt-redis-4.0.0/src/asphalt/redis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/src/asphalt/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/src/asphalt/redis/component.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/src/asphalt/redis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.286465 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-04-14 15:31:52.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-04-14 15:31:53.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 15:31:52.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-14 15:31:52.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-04-14 15:31:53.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-14 15:31:53.000000 asphalt-redis-4.0.0/src/asphalt_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 15:31:53.286465 asphalt-redis-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-04-14 15:31:35.000000 asphalt-redis-4.0.0/tests/test_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.525233 asphalt-redis-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.525233 asphalt-redis-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.525233 asphalt-redis-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/modules/component.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.525233 asphalt-redis-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.525233 asphalt-redis-4.1.0/src/asphalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/src/asphalt/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/src/asphalt/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/src/asphalt/redis/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/src/asphalt/redis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 14:34:12.000000 asphalt-redis-4.1.0/src/asphalt_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:12.529233 asphalt-redis-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-22 14:33:53.000000 asphalt-redis-4.1.0/tests/test_component.py
```

### Comparing `asphalt-redis-4.0.0/.github/workflows/publish.yml` & `asphalt-redis-4.1.0/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 name: Publish packages to PyPI
 
 on:
   push:
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
+      - "[0-9]+.[0-9]+.[0-9]+.post[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+[a-b][0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+rc[0-9]+"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
-      run: python -m build -s -w .
+      run: python -m build
     - name: Upload packages
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_password }}
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `asphalt-redis-4.0.0/.github/workflows/test.yml` & `asphalt-redis-4.1.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-name: Run the test suite
+name: test suite
 
 on:
   push:
     branches: [master]
   pull_request:
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.10", "3.11-dev", "pypy-3.8"]
+        python-version: ["3.7", "3.10", "3.11", "3.12", "pypy-3.10"]
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    - uses: actions/cache@v2
-      with:
-        path: ~/.cache/pip
-        key: pip-test-${{ matrix.python-version }}-${{ matrix.os }}
+        allow-prereleases: true
+        cache: pip
+        cache-dependency-path: pyproject.toml
     - name: Start external services
       run: docker-compose up -d
     - name: Install dependencies
-      run: pip install .[test] coveralls
+      run: pip install .[test] coverage
     - name: Test with pytest
-      run: coverage run -m pytest
+      run: |
+        coverage run -m pytest
+        coverage xml
     - name: Upload Coverage
-      run: coveralls --service=github
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
-        COVERALLS_PARALLEL: true
+      uses: coverallsapp/github-action@v2
+      with:
+        parallel: true
+        file: coverage.xml
 
   coveralls:
     name: Finish Coveralls
     needs: test
     runs-on: ubuntu-latest
-    container: python:3-slim
     steps:
     - name: Finished
-      run: |
-        pip install coveralls
-        coveralls --service=github --finish
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      uses: coverallsapp/github-action@v2
+      with:
+        parallel-finished: true
```

### Comparing `asphalt-redis-4.0.0/.pre-commit-config.yaml` & `asphalt-redis-4.1.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,35 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.274
     hooks:
-      - id: pyupgrade
-        args: [ "--py37-plus", "--keep-runtime-typing" ]
+      - id: ruff
+        args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/csachs/pyproject-flake8
-    rev: v0.0.1a4
-    hooks:
-      - id: pyproject-flake8
-
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.942
+    rev: v1.3.0
     hooks:
       - id: mypy
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
+        additional_dependencies:
+          - asphalt
+          - pytest
```

### Comparing `asphalt-redis-4.0.0/LICENSE` & `asphalt-redis-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asphalt-redis-4.0.0/PKG-INFO` & `asphalt-redis-4.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: asphalt-redis
-Version: 4.0.0
+Version: 4.1.0
 Summary: Redis integration component for the Asphalt framework
-Home-page: https://github.com/asphalt-framework/asphalt-redis
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/asphalt-framework/asphalt-redis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/asphalt-framework/asphalt-redis/actions/workflows/test.yml/badge.svg
@@ -40,9 +40,7 @@
 Project links
 -------------
 
 * `Documentation <http://asphalt-redis.readthedocs.org/en/latest/>`_
 * `Help and support <https://github.com/asphalt-framework/asphalt/wiki/Help-and-support>`_
 * `Source code <https://github.com/asphalt-framework/asphalt-redis>`_
 * `Issue tracker <https://github.com/asphalt-framework/asphalt-redis/issues>`_
-
-
```

### Comparing `asphalt-redis-4.0.0/README.rst` & `asphalt-redis-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `asphalt-redis-4.0.0/docs/conf.py` & `asphalt-redis-4.1.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx_autodoc_typehints",
-    "sphinxcontrib.asyncio",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "asphalt-redis"
 author = "Alex Grönholm"
 copyright = "2016, " + author
 
 v = parse(version(project))
 version = v.base_version
 release = v.public
 
-language = None
+language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 highlight_language = "python3"
 todo_include_todos = False
 
 html_theme = "sphinx_rtd_theme"
-html_static_path = ["_static"]
 htmlhelp_basename = project.replace("-", "") + "doc"
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "asphalt": ("https://asphalt.readthedocs.org/en/latest/", None),
     "redis": ("https://redis.readthedocs.org/en/latest/", None),
 }
```

### Comparing `asphalt-redis-4.0.0/docs/configuration.rst` & `asphalt-redis-4.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `asphalt-redis-4.0.0/docs/usage.rst` & `asphalt-redis-4.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asphalt-redis-4.0.0/docs/versionhistory.rst` & `asphalt-redis-4.1.0/docs/versionhistory.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
+**4.1.0** (2023-06-22)
+
+- Removed explicit run-time argument type checks and the ``typeguard`` dependency
+
 **4.0.0** (2022-04-14)
 
 - **BACKWARD INCOMPATIBLE** Upgraded Asphalt dependency to ~4.7
 - **BACKWARD INCOMPATIBLE** Switched backing library from aioredis to the official
   redis-py (which now has asyncio support)
 - **BACKWARD INCOMPATIBLE** Refactored component to only provide a single Redis client
   (you will have to add two components to get two clients)
```

### Comparing `asphalt-redis-4.0.0/pyproject.toml` & `asphalt-redis-4.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools >= 61",
+    "setuptools >= 64",
     "setuptools_scm[toml] >= 6.4"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asphalt-redis"
 description = "Redis integration component for the Asphalt framework"
@@ -12,83 +12,88 @@
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Database",
+    "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">= 3.7"
 dependencies = [
     "asphalt ~= 4.7",
     "redis >= 4.2.0",
-    "typeguard ~= 2.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/asphalt-framework/asphalt-redis"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-asyncio",
 ]
 doc = [
-    "Sphinx >= 1.5",
-    "sphinx_rtd_theme",
-    "sphinx-autodoc-typehints >= 1.0.5",
-    "sphinxcontrib-asyncio >= 0.2.0",
+    "Sphinx >= 6.0",
+    "sphinx_rtd_theme >= 1.2.0",
+    "sphinx-autodoc-typehints >= 1.22",
 ]
 
 [project.entry-points."asphalt.components"]
 redis = "asphalt.redis.component:RedisComponent"
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
-[tool.isort]
-src_paths = ["src"]
-skip_gitignore = true
-profile = "black"
+[tool.ruff]
+line-length = 99
+select = [
+    "E", "F", "W",  # default flake-8
+    "I",            # isort
+    "PGH",          # pygrep-hooks
+    "UP",           # pyupgrade
+]
+target-version = "py37"
 
-[tool.flake8]
-max-line-length = 99
+[tool.ruff.isort]
+known-first-party = ["asphalt.redis"]
 
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short"
 asyncio_mode = "strict"
 testpaths = ["tests"]
 
 [tool.mypy]
 python_version = "3.7"
-ignore_missing_imports = true
+strict = true
 
 [tool.coverage.run]
 source = ["asphalt.redis"]
 relative_files = true
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37, py38, py39, py310, py311, pypy3
+envlist = py37, py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
-isolated_build = true
+minversion = 4.0
 
 [testenv]
 extras = test
 commands = python -m pytest {posargs}
 
 [testenv:docs]
 extras = doc
```

### Comparing `asphalt-redis-4.0.0/src/asphalt/redis/component.py` & `asphalt-redis-4.1.0/src/asphalt/redis/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
-
-from typeguard import check_argument_types
+from collections.abc import AsyncGenerator
+from typing import Any
 
 from asphalt.core import Component, Context, context_teardown
+
 from redis.asyncio import Redis
 
 logger = logging.getLogger(__name__)
 
 
 class RedisComponent(Component):
     """
@@ -21,23 +22,22 @@
     """
 
     def __init__(
         self,
         *,
         resource_name: str = "default",
         validate_connection: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ):
-        check_argument_types()
         self.resource_name = resource_name
         self.validate_connection = validate_connection
         self.client = Redis(**kwargs)
 
     @context_teardown
-    async def start(self, ctx: Context) -> None:
+    async def start(self, ctx: Context) -> AsyncGenerator[None, Exception | None]:
         async with self.client:
             if self.validate_connection:
                 await self.client.ping()
 
             ctx.add_resource(self.client, self.resource_name)
 
             connection_kwargs = self.client.connection_pool.connection_kwargs
```

### Comparing `asphalt-redis-4.0.0/src/asphalt_redis.egg-info/PKG-INFO` & `asphalt-redis-4.1.0/src/asphalt_redis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: asphalt-redis
-Version: 4.0.0
+Version: 4.1.0
 Summary: Redis integration component for the Asphalt framework
-Home-page: https://github.com/asphalt-framework/asphalt-redis
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/asphalt-framework/asphalt-redis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/asphalt-framework/asphalt-redis/actions/workflows/test.yml/badge.svg
@@ -40,9 +40,7 @@
 Project links
 -------------
 
 * `Documentation <http://asphalt-redis.readthedocs.org/en/latest/>`_
 * `Help and support <https://github.com/asphalt-framework/asphalt/wiki/Help-and-support>`_
 * `Source code <https://github.com/asphalt-framework/asphalt-redis>`_
 * `Issue tracker <https://github.com/asphalt-framework/asphalt-redis/issues>`_
-
-
```

### Comparing `asphalt-redis-4.0.0/src/asphalt_redis.egg-info/SOURCES.txt` & `asphalt-redis-4.1.0/src/asphalt_redis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 docker-compose.yml
 pyproject.toml
-setup.cfg
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/conf.py
 docs/configuration.rst
 docs/index.rst
 docs/usage.rst
 docs/versionhistory.rst
```

### Comparing `asphalt-redis-4.0.0/tests/test_component.py` & `asphalt-redis-4.1.0/tests/test_component.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 
 import pytest
+from _pytest.logging import LogCaptureFixture
 from asphalt.core.context import Context
 from redis.asyncio import Redis
 
 from asphalt.redis.component import RedisComponent
 
 
 @pytest.mark.asyncio
-async def test_default_connection(caplog):
+async def test_default_connection(caplog: LogCaptureFixture) -> None:
     """Test that the default connection is started and is available on the context."""
     caplog.set_level(logging.INFO)
     async with Context() as context:
         await RedisComponent(port=63790).start(context)
         context.require_resource(Redis)
 
     records = [
@@ -24,35 +25,35 @@
     assert records[0].message == (
         "Configured Redis client (default; host='localhost', port=63790)"
     )
     assert records[1].message == "Redis client (default) shut down"
 
 
 @pytest.mark.asyncio
-async def test_unix_socket_connection(caplog):
+async def test_unix_socket_connection(caplog: LogCaptureFixture) -> None:
     """Test that the default connection is started and is available on the context."""
     caplog.set_level(logging.INFO)
     async with Context() as context:
-        component = RedisComponent(unix_socket_path='/tmp/foo', validate_connection=False)
+        component = RedisComponent(
+            unix_socket_path="/tmp/foo", validate_connection=False
+        )
         await component.start(context)
         context.require_resource(Redis)
 
     records = [
         record for record in caplog.records if record.name == "asphalt.redis.component"
     ]
     records.sort(key=lambda r: r.message)
     assert len(records) == 2
-    assert records[0].message == (
-        "Configured Redis client (default; path='/tmp/foo')"
-    )
+    assert records[0].message == ("Configured Redis client (default; path='/tmp/foo')")
     assert records[1].message == "Redis client (default) shut down"
 
 
 @pytest.mark.asyncio
-async def test_create_remove_key():
+async def test_create_remove_key() -> None:
     """Test the client against a real Redis server."""
     async with Context() as context:
         component = RedisComponent(
             host=os.getenv("REDIS_HOST", "localhost"),
             port=os.getenv("REDIS_PORT", 63790),
         )
         await component.start(context)
```

