# Comparing `tmp/tblib-1.7.0.tar.gz` & `tmp/tblib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tblib-1.7.0.tar", last modified: Thu Jul 23 23:17:38 2020, max compression
+gzip compressed data, was "tblib-2.0.0.tar", last modified: Thu Jun 22 08:23:57 2023, max compression
```

## Comparing `tblib-1.7.0.tar` & `tblib-2.0.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.794324 tblib-1.7.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2553 2020-03-09 12:14:06.000000 tblib-1.7.0/.appveyor.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      503 2020-07-23 23:17:33.000000 tblib-1.7.0/.bumpversion.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1507 2020-03-09 12:20:21.000000 tblib-1.7.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      173 2020-03-09 12:14:05.000000 tblib-1.7.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      217 2020-03-09 12:14:05.000000 tblib-1.7.0/.editorconfig
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      641 2020-03-09 12:14:05.000000 tblib-1.7.0/.gitignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2020-03-09 12:58:58.000000 tblib-1.7.0/.readthedocs.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1123 2020-03-09 12:14:06.000000 tblib-1.7.0/.travis.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      474 2020-03-09 12:20:06.000000 tblib-1.7.0/AUTHORS.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2233 2020-07-23 23:15:44.000000 tblib-1.7.0/CHANGELOG.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2696 2020-03-09 12:14:05.000000 tblib-1.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1330 2020-03-09 12:20:06.000000 tblib-1.7.0/LICENSE
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      350 2020-03-09 12:14:05.000000 tblib-1.7.0/MANIFEST.in
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    30713 2020-07-23 23:17:38.794324 tblib-1.7.0/PKG-INFO
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    23363 2020-07-23 23:17:33.000000 tblib-1.7.0/README.rst
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.791324 tblib-1.7.0/ci/
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)     3818 2019-10-23 02:58:52.000000 tblib-1.7.0/ci/appveyor-download.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      763 2020-03-09 12:14:05.000000 tblib-1.7.0/ci/appveyor-with-compiler.cmd
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)     2886 2020-03-09 12:14:05.000000 tblib-1.7.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       62 2020-03-09 12:14:05.000000 tblib-1.7.0/ci/requirements.txt
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.791324 tblib-1.7.0/ci/templates/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1708 2020-03-09 12:14:05.000000 tblib-1.7.0/ci/templates/.appveyor.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1014 2020-03-09 12:14:05.000000 tblib-1.7.0/ci/templates/.travis.yml
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.792324 tblib-1.7.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/changelog.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1288 2020-07-23 23:17:33.000000 tblib-1.7.0/docs/conf.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/contributing.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      226 2020-03-09 12:36:16.000000 tblib-1.7.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       85 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/installation.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/readme.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       56 2020-03-09 12:24:07.000000 tblib-1.7.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       62 2020-03-09 12:14:05.000000 tblib-1.7.0/docs/usage.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      587 2020-07-23 23:17:38.795324 tblib-1.7.0/setup.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2951 2020-07-23 23:17:33.000000 tblib-1.7.0/setup.py
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.788324 tblib-1.7.0/src/
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.793324 tblib-1.7.0/src/tblib/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     9433 2020-07-23 23:17:33.000000 tblib-1.7.0/src/tblib/__init__.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2381 2019-05-02 10:11:24.000000 tblib-1.7.0/src/tblib/cpython.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1076 2019-05-02 10:11:24.000000 tblib-1.7.0/src/tblib/decorators.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2917 2019-12-06 20:40:15.000000 tblib-1.7.0/src/tblib/pickling_support.py
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.793324 tblib-1.7.0/src/tblib.egg-info/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    30713 2020-07-23 23:17:38.000000 tblib-1.7.0/src/tblib.egg-info/PKG-INFO
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      933 2020-07-23 23:17:38.000000 tblib-1.7.0/src/tblib.egg-info/SOURCES.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2020-07-23 23:17:38.000000 tblib-1.7.0/src/tblib.egg-info/dependency_links.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2019-05-02 10:17:20.000000 tblib-1.7.0/src/tblib.egg-info/not-zip-safe
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        6 2020-07-23 23:17:38.000000 tblib-1.7.0/src/tblib.egg-info/top_level.txt
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2020-07-23 23:17:38.794324 tblib-1.7.0/tests/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       37 2019-05-02 10:11:24.000000 tblib-1.7.0/tests/badmodule.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       47 2019-05-02 11:23:09.000000 tblib-1.7.0/tests/badsyntax.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      251 2019-05-02 10:11:24.000000 tblib-1.7.0/tests/examples.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      460 2019-10-23 02:58:52.000000 tblib-1.7.0/tests/test_issue30.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2455 2019-12-06 20:40:15.000000 tblib-1.7.0/tests/test_pickle_exception.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     4058 2020-03-09 12:20:06.000000 tblib-1.7.0/tests/test_tblib.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1835 2020-03-09 12:21:02.000000 tblib-1.7.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.693943 tblib-2.0.0/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      734 2023-06-22 08:14:31.000000 tblib-2.0.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1456 2023-06-22 08:14:31.000000 tblib-2.0.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      173 2023-06-22 07:48:51.000000 tblib-2.0.0/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2023-06-22 07:48:51.000000 tblib-2.0.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.688943 tblib-2.0.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.690943 tblib-2.0.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5619 2023-06-22 07:48:51.000000 tblib-2.0.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      678 2023-06-22 07:48:51.000000 tblib-2.0.0/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      703 2023-06-22 08:09:48.000000 tblib-2.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2023-06-22 07:48:51.000000 tblib-2.0.0/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      474 2023-06-22 07:50:17.000000 tblib-2.0.0/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2379 2023-06-22 08:14:18.000000 tblib-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2394 2023-06-22 07:50:17.000000 tblib-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-06-22 07:50:17.000000 tblib-2.0.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      427 2023-06-22 07:48:51.000000 tblib-2.0.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    25057 2023-06-22 08:23:57.692943 tblib-2.0.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    22947 2023-06-22 08:14:31.000000 tblib-2.0.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.690943 tblib-2.0.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2023-06-22 07:56:42.000000 tblib-2.0.0/ci/bootstrap.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2023-06-22 07:48:51.000000 tblib-2.0.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.688943 tblib-2.0.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.688943 tblib-2.0.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.690943 tblib-2.0.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1963 2023-06-22 07:48:51.000000 tblib-2.0.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.691943 tblib-2.0.0/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/changelog.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1197 2023-06-22 08:14:31.000000 tblib-2.0.0/docs/conf.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/contributing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      242 2023-06-22 07:50:17.000000 tblib-2.0.0/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       85 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/installation.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/readme.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       56 2023-06-22 07:50:17.000000 tblib-2.0.0/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       62 2023-06-22 07:48:51.000000 tblib-2.0.0/docs/usage.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1327 2023-06-22 08:07:17.000000 tblib-2.0.0/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      834 2023-06-22 07:50:17.000000 tblib-2.0.0/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2023-06-22 08:23:57.693943 tblib-2.0.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2733 2023-06-22 08:14:31.000000 tblib-2.0.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.688943 tblib-2.0.0/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.691943 tblib-2.0.0/src/tblib/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7236 2023-06-22 08:14:31.000000 tblib-2.0.0/src/tblib/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1068 2023-06-22 07:56:42.000000 tblib-2.0.0/src/tblib/decorators.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2878 2023-06-22 07:56:42.000000 tblib-2.0.0/src/tblib/pickling_support.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.692943 tblib-2.0.0/src/tblib.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    25057 2023-06-22 08:23:57.000000 tblib-2.0.0/src/tblib.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      907 2023-06-22 08:23:57.000000 tblib-2.0.0/src/tblib.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-06-22 08:23:57.000000 tblib-2.0.0/src/tblib.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-06-22 08:23:56.000000 tblib-2.0.0/src/tblib.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        6 2023-06-22 08:23:57.000000 tblib-2.0.0/src/tblib.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-06-22 08:23:57.692943 tblib-2.0.0/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       37 2023-06-22 07:56:42.000000 tblib-2.0.0/tests/badmodule.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       47 2019-05-02 11:23:09.000000 tblib-2.0.0/tests/badsyntax.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      257 2023-06-22 08:06:41.000000 tblib-2.0.0/tests/examples.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      483 2023-06-22 08:03:12.000000 tblib-2.0.0/tests/test_issue30.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2476 2023-06-22 08:08:12.000000 tblib-2.0.0/tests/test_pickle_exception.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4291 2023-06-22 08:03:48.000000 tblib-2.0.0/tests/test_tblib.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1664 2023-06-22 07:48:51.000000 tblib-2.0.0/tox.ini
```

### Comparing `tblib-1.7.0/.gitignore` & `tblib-2.0.0/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 *.py[cod]
 __pycache__
 
+# Temp files
+.*.sw[po]
+*~
+*.bak
+.DS_Store
+
 # C extensions
 *.so
 
-# Packages
+# Build and package files
 *.egg
 *.egg-info
-dist
-build
-eggs
+.bootstrap
+.build
+.cache
 .eggs
-parts
+.env
+.installed.cfg
+.ve
 bin
-var
-sdist
-wheelhouse
+build
 develop-eggs
-.installed.cfg
+dist
+eggs
 lib
 lib64
-venv*/
-pyvenv*/
+parts
 pip-wheel-metadata/
+pyvenv*/
+sdist
+var
+venv*/
+wheelhouse
 
 # Installer logs
 pip-log.txt
 
 # Unit test / coverage reports
+.benchmarks
 .coverage
-.tox
 .coverage.*
+.pytest
 .pytest_cache/
-nosetests.xml
+.tox
 coverage.xml
 htmlcov
+nosetests.xml
 
 # Translations
 *.mo
 
-# Mr Developer
+# Buildout
 .mr.developer.cfg
-.project
-.pydevproject
-.idea
+
+# IDE project files
 *.iml
 *.komodoproject
+.idea
+.project
+.pydevproject
+.vscode
 
 # Complexity
 output/*.html
 output/*/index.html
 
 # Sphinx
 docs/_build
 
-.DS_Store
-*~
-.*.sw[po]
-.build
-.ve
-.env
-.cache
-.pytest
-.benchmarks
-.bootstrap
-.appveyor.token
-*.bak
-
 # Mypy Cache
 .mypy_cache/
```

### Comparing `tblib-1.7.0/CHANGELOG.rst` & `tblib-2.0.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 Changelog
 =========
 
+2.0.0 (2023-06-22)
+~~~~~~~~~~~~~~~~~~
+
+* Removed support for legacy Pythons (2.7 and 3.6) and added Python 3.11 in the test grid.
+* Some cleanups and refactors (mostly from ruff).
+
 1.7.0 (2020-07-24)
 ~~~~~~~~~~~~~~~~~~
 
 * Add more attributes to ``Frame`` and ``Code`` objects for pytest compatibility. Contributed by Ivanq in
   `#58 <https://github.com/ionelmc/python-tblib/pull/58>`_.
 
 1.6.0 (2019-12-07)
@@ -32,15 +38,15 @@
 * Fixed compatibility issue with Twised (``twisted.python.failure.Failure`` expected a ``co_code`` attribute).
 
 1.3.2 (2017-04-09)
 ~~~~~~~~~~~~~~~~~~
 
 * Add support for PyPy3.5-5.7.1-beta. Previously ``AttributeError:
   'Frame' object has no attribute 'clear'``  could be raised. See PyPy
-  issue `#2532 <https://bitbucket.org/pypy/pypy/issues/2532/pypy3-attributeerror-frame-object-has-no>`_.
+  issue `#2532 <https://foss.heptapod.net/pypy/pypy/-/issues/2532>`_.
 
 1.3.1 (2017-03-27)
 ~~~~~~~~~~~~~~~~~~
 
 * Fixed handling for tracebacks due to exceeding the recursion limit.
   Fixes `#15 <https://github.com/ionelmc/python-tblib/issues/15>`_.
```

### Comparing `tblib-1.7.0/CONTRIBUTING.rst` & `tblib-2.0.0/CONTRIBUTING.rst`

 * *Files 19% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 To set up `python-tblib` for local development:
 
 1. Fork `python-tblib <https://github.com/ionelmc/python-tblib>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
-    git clone git@github.com:ionelmc/python-tblib.git
+    git clone git@github.com:YOURGITHUBNAME/python-tblib.git
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
@@ -64,27 +64,24 @@
 Pull Request Guidelines
 -----------------------
 
 If you need some code review or feedback while you're developing the code just make the pull request.
 
 For merging, you should:
 
-1. Include passing tests (run ``tox``) [1]_.
+1. Include passing tests (run ``tox``).
 2. Update documentation when there's new API, functionality etc.
 3. Add a note to ``CHANGELOG.rst`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/ionelmc/python-tblib/pull_requests>`_ for each change you add in the pull request.
 
-       It will be slower though ...
 
 Tips
 ----
 
 To run a subset of tests::
 
     tox -e envname -- pytest -k test_myfeature
 
-To run all the test environments in *parallel* (you need to ``pip install detox``)::
+To run all the test environments in *parallel*::
 
-    detox
+    tox -p auto
```

### Comparing `tblib-1.7.0/LICENSE` & `tblib-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2013-2020, Ionel Cristian Mărieș. All rights reserved.
+Copyright (c) 2013-2022, Ionel Cristian Mărieș. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
 following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
 disclaimer.
```

### Comparing `tblib-1.7.0/PKG-INFO` & `tblib-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,760 +1,768 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tblib
-Version: 1.7.0
+Version: 2.0.0
 Summary: Traceback serialization library.
 Home-page: https://github.com/ionelmc/python-tblib
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-tblib.readthedocs.io/
 Project-URL: Changelog, https://python-tblib.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-tblib/issues
-Description: ========
-        Overview
-        ========
-        
-        
-        
-        Serialization library for Exceptions and Tracebacks.
-        
-        * Free software: BSD license
-        
-        It allows you to:
-        
-        * `Pickle <https://docs.python.org/3/library/pickle.html>`_ tracebacks and raise exceptions
-          with pickled tracebacks in different processes. This allows better error handling when running
-          code over multiple processes (imagine multiprocessing, billiard, futures, celery etc).
-        * Create traceback objects from strings (the ``from_string`` method). *No pickling is used*.
-        * Serialize tracebacks to/from plain dicts (the ``from_dict`` and ``to_dict`` methods). *No pickling is used*.
-        * Raise the tracebacks created from the aforementioned sources.
-        * Pickle an Exception together with its traceback and exception chain
-          (``raise ... from ...``) *(Python 3 only)*
-        
-        **Again, note that using the pickle support is completely optional. You are solely responsible for
-        security problems should you decide to use the pickle support.**
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install tblib
-        
-        Documentation
-        =============
-        
-        .. contents::
-           :local:
-        
-        Pickling tracebacks
-        ~~~~~~~~~~~~~~~~~~~
-        
-        **Note**: The traceback objects that come out are stripped of some attributes (like variables). But you'll be able to raise exceptions with
-        those tracebacks or print them - that should cover 99% of the usecases.
-        
-        ::
-        
-            >>> from tblib import pickling_support
-            >>> pickling_support.install()
-            >>> import pickle, sys
-            >>> def inner_0():
-            ...     raise Exception('fail')
-            ...
-            >>> def inner_1():
-            ...     inner_0()
-            ...
-            >>> def inner_2():
-            ...     inner_1()
-            ...
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s1 = pickle.dumps(sys.exc_info())
-            ...
-            >>> len(s1) > 1
-            True
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s2 = pickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
-            ...
-            >>> len(s2) > 1
-            True
-        
-            >>> try:
-            ...     import cPickle
-            ... except ImportError:
-            ...     import pickle as cPickle
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s3 = cPickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
-            ...
-            >>> len(s3) > 1
-            True
-        
-        Unpickling tracebacks
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            >>> pickle.loads(s1)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-            >>> pickle.loads(s2)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-            >>> pickle.loads(s3)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-        Raising
-        ~~~~~~~
-        
-        ::
-        
-            >>> from six import reraise
-            >>> reraise(*pickle.loads(s1))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-            >>> reraise(*pickle.loads(s2))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-            >>> reraise(*pickle.loads(s3))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        Pickling Exceptions together with their traceback and chain (Python 3 only)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            >>> try:  # doctest: +SKIP
-            ...     try:
-            ...         1 / 0
-            ...     except Exception as e:
-            ...         raise Exception("foo") from e
-            ... except Exception as e:
-            ...     s = pickle.dumps(e)
-            >>> raise pickle.loads(s)  # doctest: +SKIP
-            Traceback (most recent call last):
-              File "<doctest README.rst[16]>", line 3, in <module>
-                1 / 0
-            ZeroDivisionError: division by zero
-        
-            The above exception was the direct cause of the following exception:
-        
-            Traceback (most recent call last):
-              File "<doctest README.rst[17]>", line 1, in <module>
-                raise pickle.loads(s)
-              File "<doctest README.rst[16]>", line 5, in <module>
-                raise Exception("foo") from e
-            Exception: foo
-        
-        BaseException subclasses defined after calling ``pickling_support.install()`` will
-        **not** retain their traceback and exception chain pickling.
-        To cover custom Exceptions, there are three options:
-        
-        1. Use ``@pickling_support.install`` as a decorator for each custom Exception
-        
-            .. code-block:: python
-        
-                >>> from tblib import pickling_support
-                >>> # Declare all imports of your package's dependencies
-                >>> import numpy  # doctest: +SKIP
-        
-                >>> pickling_support.install()  # install for all modules imported so far
-        
-                >>> @pickling_support.install
-                ... class CustomError(Exception):
-                ...     pass
-        
-           Eventual subclasses of ``CustomError`` will need to be decorated again.
-        
-        2. Invoke ``pickling_support.install()`` after all modules have been imported and all
-           Exception subclasses have been declared
-        
-            .. code-block:: python
-        
-                >>> # Declare all imports of your package's dependencies
-                >>> import numpy  # doctest: +SKIP
-                >>> from tblib import pickling_support
-        
-                >>> # Declare your own custom Exceptions
-                >>> class CustomError(Exception):
-                ...     pass
-        
-                >>> # Finally, install tblib
-                >>> pickling_support.install()
-        
-        3. Selectively install tblib for Exception instances just before they are pickled
-        
-            .. code-block:: python
-        
-               pickling_support.install(<Exception instance>, [Exception instance], ...)
-        
-           The above will install tblib pickling for all listed exceptions as well as any other
-           exceptions in their exception chains.
-        
-           For example, one could write a wrapper to be used with
-           `ProcessPoolExecutor <https://docs.python.org/3/library/concurrent.futures.html>`_,
-           `Dask.distributed <https://distributed.dask.org/>`_, or similar libraries:
-        
-        ::
-        
-            >>> from tblib import pickling_support
-            >>> def wrapper(func, *args, **kwargs):
-            ...     try:
-            ...         return func(*args, **kwargs)
-            ...     except Exception as e:
-            ...         pickling_support.install(e)
-            ...         raise
-        
-        What if we have a local stack, does it show correctly ?
-        -------------------------------------------------------
-        
-        Yes it does::
-        
-            >>> exc_info = pickle.loads(s3)
-            >>> def local_0():
-            ...     reraise(*exc_info)
-            ...
-            >>> def local_1():
-            ...     local_0()
-            ...
-            >>> def local_2():
-            ...     local_1()
-            ...
-            >>> local_2()
-            Traceback (most recent call last):
-              File "...doctest.py", line ..., in __run
-                compileflags, 1) in test.globs
-              File "<doctest README.rst[24]>", line 1, in <module>
-                local_2()
-              File "<doctest README.rst[23]>", line 2, in local_2
-                local_1()
-              File "<doctest README.rst[22]>", line 2, in local_1
-                local_0()
-              File "<doctest README.rst[21]>", line 2, in local_0
-                reraise(*exc_info)
-              File "<doctest README.rst[11]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        It also supports more contrived scenarios
-        -----------------------------------------
-        
-        Like tracebacks with syntax errors::
-        
-            >>> from tblib import Traceback
-            >>> from examples import bad_syntax
-            >>> try:
-            ...     bad_syntax()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[58]>", line 1, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[57]>", line 2, in <module>
-                bad_syntax()
-              File "...tests...examples.py", line 18, in bad_syntax
-                import badsyntax
-              File "...tests...badsyntax.py", line 5
-                is very bad
-                 ^
-            SyntaxError: invalid syntax
-        
-        Or other import failures::
-        
-            >>> from examples import bad_module
-            >>> try:
-            ...     bad_module()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[61]>", line 1, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[60]>", line 2, in <module>
-                bad_module()
-              File "...tests...examples.py", line 23, in bad_module
-                import badmodule
-              File "...tests...badmodule.py", line 3, in <module>
-                raise Exception("boom!")
-            Exception: boom!
-        
-        Or a traceback that's caused by exceeding the recursion limit (here we're
-        forcing the type and value to have consistency across platforms)::
-        
-            >>> def f(): f()
-            >>> try:
-            ...    f()
-            ... except RuntimeError:
-            ...    et, ev, tb = sys.exc_info()
-            ...    tb = Traceback(tb)
-            ...
-            >>> reraise(RuntimeError, RuntimeError("maximum recursion depth exceeded"), tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              ...
-            RuntimeError: maximum recursion depth exceeded
-        
-        Reference
-        ~~~~~~~~~
-        
-        tblib.Traceback
-        ---------------
-        
-        It is used by the ``pickling_support``. You can use it too if you want more flexibility::
-        
-            >>> from tblib import Traceback
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[21]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[21]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        tblib.Traceback.to_dict
-        ```````````````````````
-        
-        You can use the ``to_dict`` method and the ``from_dict`` classmethod to
-        convert a Traceback into and from a dictionary serializable by the stdlib
-        json.JSONDecoder::
-        
-            >>> import json
-            >>> from pprint import pprint
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...     tb_dict = tb.to_dict()
-            ...     pprint(tb_dict)
-            {'tb_frame': {'f_code': {'co_filename': '<doctest README.rst[...]>',
-                                     'co_name': '<module>'},
-                          'f_globals': {'__name__': '__main__'},
-                          'f_lineno': 5},
-             'tb_lineno': 2,
-             'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                 'co_name': 'inner_2'},
-                                      'f_globals': {'__name__': '__main__'},
-                                      'f_lineno': 2},
-                         'tb_lineno': 2,
-                         'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                             'co_name': 'inner_1'},
-                                                  'f_globals': {'__name__': '__main__'},
-                                                  'f_lineno': 2},
-                                     'tb_lineno': 2,
-                                     'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                                         'co_name': 'inner_0'},
-                                                              'f_globals': {'__name__': '__main__'},
-                                                              'f_lineno': 2},
-                                                 'tb_lineno': 2,
-                                                 'tb_next': None}}}}
-        
-        tblib.Traceback.from_dict
-        `````````````````````````
-        
-        Building on the previous example::
-        
-            >>> tb_json = json.dumps(tb_dict)
-            >>> tb = Traceback.from_dict(json.loads(tb_json))
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[21]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[21]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        tblib.Traceback.from_string
-        ```````````````````````````
-        
-        ::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "skipped.py", line 123, in func_123
-            ... Traceback (most recent call last):
-            ...   File "tests/examples.py", line 2, in func_a
-            ...     func_b()
-            ...   File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...   File "tests/examples.py", line 10, in func_c
-            ...     func_d()
-            ...   File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """)
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[42]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: fail
-        
-        
-        If you use the ``strict=False`` option then parsing is a bit more lax::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "bogus.py", line 123, in bogus
-            ... Traceback (most recent call last):
-            ...  File "tests/examples.py", line 2, in func_a
-            ...   func_b()
-            ...    File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...    File "tests/examples.py", line 10, in func_c
-            ...   func_d()
-            ...  File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """, strict=False)
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[42]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "bogus.py", line 123, in bogus
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: fail
-        
-        tblib.decorators.return_error
-        -----------------------------
-        
-        ::
-        
-            >>> from tblib.decorators import return_error
-            >>> inner_2r = return_error(inner_2)
-            >>> e = inner_2r()
-            >>> e
-            <tblib.decorators.Error object at ...>
-            >>> e.reraise()
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[26]>", line 1, in <module>
-                e.reraise()
-              File "...tblib...decorators.py", line 19, in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line 25, in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        How's this useful? Imagine you're using multiprocessing like this::
-        
-            # Note that Python 3.4 and later will show the remote traceback (but as a string sadly) so we skip testing this.
-            >>> import traceback
-            >>> from multiprocessing import Pool
-            >>> from examples import func_a
-            >>> pool = Pool()  # doctest: +SKIP
-            >>> try:  # doctest: +SKIP
-            ...     for i in pool.map(func_a, range(5)):
-            ...         print(i)
-            ... except:
-            ...     print(traceback.format_exc())
-            ...
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 2, in <module>
-                for i in pool.map(func_a, range(5)):
-              File "...multiprocessing...pool.py", line ..., in map
-                ...
-              File "...multiprocessing...pool.py", line ..., in get
-                ...
-            Exception: Guessing time !
-            <BLANKLINE>
-            >>> pool.terminate()  # doctest: +SKIP
-        
-        Not very useful is it? Let's sort this out::
-        
-            >>> from tblib.decorators import apply_with_return_error, Error
-            >>> from itertools import repeat
-            >>> pool = Pool()
-            >>> try:
-            ...     for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
-            ...         if isinstance(i, Error):
-            ...             i.reraise()
-            ...         else:
-            ...             print(i)
-            ... except:
-            ...     print(traceback.format_exc())
-            ...
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 4, in <module>
-                i.reraise()
-              File "...tblib...decorators.py", line ..., in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line ..., in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "...tblib...decorators.py", line ..., in apply_with_return_error
-                return args[0](*args[1:])
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: Guessing time !
-            <BLANKLINE>
-            >>> pool.terminate()
-        
-        Much better !
-        
-        What if we have a local call stack ?
-        ````````````````````````````````````
-        
-        ::
-        
-            >>> def local_0():
-            ...     pool = Pool()
-            ...     try:
-            ...         for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
-            ...             if isinstance(i, Error):
-            ...                 i.reraise()
-            ...             else:
-            ...                 print(i)
-            ...     finally:
-            ...         pool.close()
-            ...
-            >>> def local_1():
-            ...     local_0()
-            ...
-            >>> def local_2():
-            ...     local_1()
-            ...
-            >>> try:
-            ...     local_2()
-            ... except:
-            ...     print(traceback.format_exc())
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 2, in <module>
-                local_2()
-              File "<doctest README.rst[...]>", line 2, in local_2
-                local_1()
-              File "<doctest README.rst[...]>", line 2, in local_1
-                local_0()
-              File "<doctest README.rst[...]>", line 6, in local_0
-                i.reraise()
-              File "...tblib...decorators.py", line 20, in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line 27, in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "...tblib...decorators.py", line 47, in apply_with_return_error
-                return args[0](*args[1:])
-              File "...tests...examples.py", line 2, in func_a
-                func_b()
-              File "...tests...examples.py", line 6, in func_b
-                func_c()
-              File "...tests...examples.py", line 10, in func_c
-                func_d()
-              File "...tests...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: Guessing time !
-            <BLANKLINE>
-        
-        Other weird stuff
-        `````````````````
-        
-        Clearing traceback works (Python 3.4 and up)::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "skipped.py", line 123, in func_123
-            ... Traceback (most recent call last):
-            ...   File "tests/examples.py", line 2, in func_a
-            ...     func_b()
-            ...   File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...   File "tests/examples.py", line 10, in func_c
-            ...     func_d()
-            ...   File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """)
-            >>> import traceback, sys
-            >>> if sys.version_info > (3, 4):
-            ...     traceback.clear_frames(tb)
-        
-        Credits
-        =======
-        
-        * `mitsuhiko/jinja2 <https://github.com/mitsuhiko/jinja2>`_ for figuring a way to create traceback objects.
-        
-        
-        Changelog
-        =========
-        
-        1.7.0 (2020-07-24)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Add more attributes to ``Frame`` and ``Code`` objects for pytest compatibility. Contributed by Ivanq in
-          `#58 <https://github.com/ionelmc/python-tblib/pull/58>`_.
-        
-        1.6.0 (2019-12-07)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * When pickling an Exception, also pickle its traceback and the Exception chain
-          (``raise ... from ...``). Contributed by Guido Imperiale in
-          `#53 <https://github.com/ionelmc/python-tblib/issues/53>`_.
-        
-        1.5.0 (2019-10-23)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added support for Python 3.8. Contributed by Victor Stinner in
-          `#42 <https://github.com/ionelmc/python-tblib/issues/42>`_.
-        * Removed support for end of life Python 3.4.
-        * Few CI improvements and fixes.
-        
-        1.4.0 (2019-05-02)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Removed support for end of life Python 3.3.
-        * Fixed tests for Python 3.7. Contributed by Elliott Sales de Andrade in
-          `#36 <https://github.com/ionelmc/python-tblib/issues/36>`_.
-        * Fixed compatibility issue with Twised (``twisted.python.failure.Failure`` expected a ``co_code`` attribute).
-        
-        1.3.2 (2017-04-09)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Add support for PyPy3.5-5.7.1-beta. Previously ``AttributeError:
-          'Frame' object has no attribute 'clear'``  could be raised. See PyPy
-          issue `#2532 <https://bitbucket.org/pypy/pypy/issues/2532/pypy3-attributeerror-frame-object-has-no>`_.
-        
-        1.3.1 (2017-03-27)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Fixed handling for tracebacks due to exceeding the recursion limit.
-          Fixes `#15 <https://github.com/ionelmc/python-tblib/issues/15>`_.
-        
-        1.3.0 (2016-03-08)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added ``Traceback.from_string``.
-        
-        1.2.0 (2015-12-18)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Fixed handling for tracebacks from generators and other internal improvements
-          and optimizations. Contributed by DRayX in `#10 <https://github.com/ionelmc/python-tblib/issues/10>`_
-          and `#11 <https://github.com/ionelmc/python-tblib/pull/11>`_.
-        
-        1.1.0 (2015-07-27)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added support for Python 2.6. Contributed by Arcadiy Ivanov in
-          `#8 <https://github.com/ionelmc/python-tblib/pull/8>`_.
-        
-        1.0.0 (2015-03-30)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added ``to_dict`` method and ``from_dict`` classmethod on Tracebacks.
-          Contributed by beckjake in `#5 <https://github.com/ionelmc/python-tblib/pull/5>`_.
-        
 Keywords: traceback,debugging,exceptions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+Overview
+========
+
+
+
+Serialization library for Exceptions and Tracebacks.
+
+* Free software: BSD license
+
+It allows you to:
+
+* `Pickle <https://docs.python.org/3/library/pickle.html>`_ tracebacks and raise exceptions
+  with pickled tracebacks in different processes. This allows better error handling when running
+  code over multiple processes (imagine multiprocessing, billiard, futures, celery etc).
+* Create traceback objects from strings (the ``from_string`` method). *No pickling is used*.
+* Serialize tracebacks to/from plain dicts (the ``from_dict`` and ``to_dict`` methods). *No pickling is used*.
+* Raise the tracebacks created from the aforementioned sources.
+* Pickle an Exception together with its traceback and exception chain
+  (``raise ... from ...``) *(Python 3 only)*
+
+**Again, note that using the pickle support is completely optional. You are solely responsible for
+security problems should you decide to use the pickle support.**
+
+Installation
+============
+
+::
+
+    pip install tblib
+
+Documentation
+=============
+
+.. contents::
+   :local:
+
+Pickling tracebacks
+~~~~~~~~~~~~~~~~~~~
+
+**Note**: The traceback objects that come out are stripped of some attributes (like variables). But you'll be able to raise exceptions with
+those tracebacks or print them - that should cover 99% of the usecases.
+
+::
+
+    >>> from tblib import pickling_support
+    >>> pickling_support.install()
+    >>> import pickle, sys
+    >>> def inner_0():
+    ...     raise Exception('fail')
+    ...
+    >>> def inner_1():
+    ...     inner_0()
+    ...
+    >>> def inner_2():
+    ...     inner_1()
+    ...
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s1 = pickle.dumps(sys.exc_info())
+    ...
+    >>> len(s1) > 1
+    True
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s2 = pickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
+    ...
+    >>> len(s2) > 1
+    True
+
+    >>> try:
+    ...     import cPickle
+    ... except ImportError:
+    ...     import pickle as cPickle
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s3 = cPickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
+    ...
+    >>> len(s3) > 1
+    True
+
+Unpickling tracebacks
+~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    >>> pickle.loads(s1)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+    >>> pickle.loads(s2)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+    >>> pickle.loads(s3)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+Raising
+~~~~~~~
+
+::
+
+    >>> from six import reraise
+    >>> reraise(*pickle.loads(s1))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+    >>> reraise(*pickle.loads(s2))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+    >>> reraise(*pickle.loads(s3))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+Pickling Exceptions together with their traceback and chain (Python 3 only)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    >>> try:  # doctest: +SKIP
+    ...     try:
+    ...         1 / 0
+    ...     except Exception as e:
+    ...         raise Exception("foo") from e
+    ... except Exception as e:
+    ...     s = pickle.dumps(e)
+    >>> raise pickle.loads(s)  # doctest: +SKIP
+    Traceback (most recent call last):
+      File "<doctest README.rst[16]>", line 3, in <module>
+        1 / 0
+    ZeroDivisionError: division by zero
+
+    The above exception was the direct cause of the following exception:
+
+    Traceback (most recent call last):
+      File "<doctest README.rst[17]>", line 1, in <module>
+        raise pickle.loads(s)
+      File "<doctest README.rst[16]>", line 5, in <module>
+        raise Exception("foo") from e
+    Exception: foo
+
+BaseException subclasses defined after calling ``pickling_support.install()`` will
+**not** retain their traceback and exception chain pickling.
+To cover custom Exceptions, there are three options:
+
+1. Use ``@pickling_support.install`` as a decorator for each custom Exception
+
+    .. code-block:: python
+
+        >>> from tblib import pickling_support
+        >>> # Declare all imports of your package's dependencies
+        >>> import numpy  # doctest: +SKIP
+
+        >>> pickling_support.install()  # install for all modules imported so far
+
+        >>> @pickling_support.install
+        ... class CustomError(Exception):
+        ...     pass
+
+   Eventual subclasses of ``CustomError`` will need to be decorated again.
+
+2. Invoke ``pickling_support.install()`` after all modules have been imported and all
+   Exception subclasses have been declared
+
+    .. code-block:: python
+
+        >>> # Declare all imports of your package's dependencies
+        >>> import numpy  # doctest: +SKIP
+        >>> from tblib import pickling_support
+
+        >>> # Declare your own custom Exceptions
+        >>> class CustomError(Exception):
+        ...     pass
+
+        >>> # Finally, install tblib
+        >>> pickling_support.install()
+
+3. Selectively install tblib for Exception instances just before they are pickled
+
+    .. code-block:: python
+
+       pickling_support.install(<Exception instance>, [Exception instance], ...)
+
+   The above will install tblib pickling for all listed exceptions as well as any other
+   exceptions in their exception chains.
+
+   For example, one could write a wrapper to be used with
+   `ProcessPoolExecutor <https://docs.python.org/3/library/concurrent.futures.html>`_,
+   `Dask.distributed <https://distributed.dask.org/>`_, or similar libraries:
+
+::
+
+    >>> from tblib import pickling_support
+    >>> def wrapper(func, *args, **kwargs):
+    ...     try:
+    ...         return func(*args, **kwargs)
+    ...     except Exception as e:
+    ...         pickling_support.install(e)
+    ...         raise
+
+What if we have a local stack, does it show correctly ?
+-------------------------------------------------------
+
+Yes it does::
+
+    >>> exc_info = pickle.loads(s3)
+    >>> def local_0():
+    ...     reraise(*exc_info)
+    ...
+    >>> def local_1():
+    ...     local_0()
+    ...
+    >>> def local_2():
+    ...     local_1()
+    ...
+    >>> local_2()
+    Traceback (most recent call last):
+      File "...doctest.py", line ..., in __run
+        compileflags, 1) in test.globs
+      File "<doctest README.rst[24]>", line 1, in <module>
+        local_2()
+      File "<doctest README.rst[23]>", line 2, in local_2
+        local_1()
+      File "<doctest README.rst[22]>", line 2, in local_1
+        local_0()
+      File "<doctest README.rst[21]>", line 2, in local_0
+        reraise(*exc_info)
+      File "<doctest README.rst[11]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+It also supports more contrived scenarios
+-----------------------------------------
+
+Like tracebacks with syntax errors::
+
+    >>> from tblib import Traceback
+    >>> from examples import bad_syntax
+    >>> try:
+    ...     bad_syntax()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[58]>", line 1, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[57]>", line 2, in <module>
+        bad_syntax()
+      File "...tests...examples.py", line 18, in bad_syntax
+        import badsyntax
+      File "...tests...badsyntax.py", line 5
+        is very bad
+         ^
+    SyntaxError: invalid syntax
+
+Or other import failures::
+
+    >>> from examples import bad_module
+    >>> try:
+    ...     bad_module()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[61]>", line 1, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[60]>", line 2, in <module>
+        bad_module()
+      File "...tests...examples.py", line 23, in bad_module
+        import badmodule
+      File "...tests...badmodule.py", line 3, in <module>
+        raise Exception("boom!")
+    Exception: boom!
+
+Or a traceback that's caused by exceeding the recursion limit (here we're
+forcing the type and value to have consistency across platforms)::
+
+    >>> def f(): f()
+    >>> try:
+    ...    f()
+    ... except RuntimeError:
+    ...    et, ev, tb = sys.exc_info()
+    ...    tb = Traceback(tb)
+    ...
+    >>> reraise(RuntimeError, RuntimeError("maximum recursion depth exceeded"), tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      ...
+    RuntimeError: maximum recursion depth exceeded
+
+Reference
+~~~~~~~~~
+
+tblib.Traceback
+---------------
+
+It is used by the ``pickling_support``. You can use it too if you want more flexibility::
+
+    >>> from tblib import Traceback
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[21]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[21]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+tblib.Traceback.to_dict
+```````````````````````
+
+You can use the ``to_dict`` method and the ``from_dict`` classmethod to
+convert a Traceback into and from a dictionary serializable by the stdlib
+json.JSONDecoder::
+
+    >>> import json
+    >>> from pprint import pprint
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...     tb_dict = tb.to_dict()
+    ...     pprint(tb_dict)
+    {'tb_frame': {'f_code': {'co_filename': '<doctest README.rst[...]>',
+                             'co_name': '<module>'},
+                  'f_globals': {'__name__': '__main__'},
+                  'f_lineno': 5},
+     'tb_lineno': 2,
+     'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                         'co_name': 'inner_2'},
+                              'f_globals': {'__name__': '__main__'},
+                              'f_lineno': 2},
+                 'tb_lineno': 2,
+                 'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                                     'co_name': 'inner_1'},
+                                          'f_globals': {'__name__': '__main__'},
+                                          'f_lineno': 2},
+                             'tb_lineno': 2,
+                             'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                                                 'co_name': 'inner_0'},
+                                                      'f_globals': {'__name__': '__main__'},
+                                                      'f_lineno': 2},
+                                         'tb_lineno': 2,
+                                         'tb_next': None}}}}
+
+tblib.Traceback.from_dict
+`````````````````````````
+
+Building on the previous example::
+
+    >>> tb_json = json.dumps(tb_dict)
+    >>> tb = Traceback.from_dict(json.loads(tb_json))
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[21]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[21]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+tblib.Traceback.from_string
+```````````````````````````
+
+::
+
+    >>> tb = Traceback.from_string("""
+    ... File "skipped.py", line 123, in func_123
+    ... Traceback (most recent call last):
+    ...   File "tests/examples.py", line 2, in func_a
+    ...     func_b()
+    ...   File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...   File "tests/examples.py", line 10, in func_c
+    ...     func_d()
+    ...   File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """)
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[42]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: fail
+
+
+If you use the ``strict=False`` option then parsing is a bit more lax::
+
+    >>> tb = Traceback.from_string("""
+    ... File "bogus.py", line 123, in bogus
+    ... Traceback (most recent call last):
+    ...  File "tests/examples.py", line 2, in func_a
+    ...   func_b()
+    ...    File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...    File "tests/examples.py", line 10, in func_c
+    ...   func_d()
+    ...  File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """, strict=False)
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[42]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "bogus.py", line 123, in bogus
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: fail
+
+tblib.decorators.return_error
+-----------------------------
+
+::
+
+    >>> from tblib.decorators import return_error
+    >>> inner_2r = return_error(inner_2)
+    >>> e = inner_2r()
+    >>> e
+    <tblib.decorators.Error object at ...>
+    >>> e.reraise()
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[26]>", line 1, in <module>
+        e.reraise()
+      File "...tblib...decorators.py", line 19, in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line 25, in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+How's this useful? Imagine you're using multiprocessing like this::
+
+    # Note that Python 3.4 and later will show the remote traceback (but as a string sadly) so we skip testing this.
+    >>> import traceback
+    >>> from multiprocessing import Pool
+    >>> from examples import func_a
+    >>> pool = Pool()  # doctest: +SKIP
+    >>> try:  # doctest: +SKIP
+    ...     for i in pool.map(func_a, range(5)):
+    ...         print(i)
+    ... except:
+    ...     print(traceback.format_exc())
+    ...
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 2, in <module>
+        for i in pool.map(func_a, range(5)):
+      File "...multiprocessing...pool.py", line ..., in map
+        ...
+      File "...multiprocessing...pool.py", line ..., in get
+        ...
+    Exception: Guessing time !
+    <BLANKLINE>
+    >>> pool.terminate()  # doctest: +SKIP
+
+Not very useful is it? Let's sort this out::
+
+    >>> from tblib.decorators import apply_with_return_error, Error
+    >>> from itertools import repeat
+    >>> pool = Pool()
+    >>> try:
+    ...     for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
+    ...         if isinstance(i, Error):
+    ...             i.reraise()
+    ...         else:
+    ...             print(i)
+    ... except:
+    ...     print(traceback.format_exc())
+    ...
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 4, in <module>
+        i.reraise()
+      File "...tblib...decorators.py", line ..., in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line ..., in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "...tblib...decorators.py", line ..., in apply_with_return_error
+        return args[0](*args[1:])
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: Guessing time !
+    <BLANKLINE>
+    >>> pool.terminate()
+
+Much better !
+
+What if we have a local call stack ?
+````````````````````````````````````
+
+::
+
+    >>> def local_0():
+    ...     pool = Pool()
+    ...     try:
+    ...         for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
+    ...             if isinstance(i, Error):
+    ...                 i.reraise()
+    ...             else:
+    ...                 print(i)
+    ...     finally:
+    ...         pool.close()
+    ...
+    >>> def local_1():
+    ...     local_0()
+    ...
+    >>> def local_2():
+    ...     local_1()
+    ...
+    >>> try:
+    ...     local_2()
+    ... except:
+    ...     print(traceback.format_exc())
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 2, in <module>
+        local_2()
+      File "<doctest README.rst[...]>", line 2, in local_2
+        local_1()
+      File "<doctest README.rst[...]>", line 2, in local_1
+        local_0()
+      File "<doctest README.rst[...]>", line 6, in local_0
+        i.reraise()
+      File "...tblib...decorators.py", line 20, in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line 27, in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "...tblib...decorators.py", line 47, in apply_with_return_error
+        return args[0](*args[1:])
+      File "...tests...examples.py", line 2, in func_a
+        func_b()
+      File "...tests...examples.py", line 6, in func_b
+        func_c()
+      File "...tests...examples.py", line 10, in func_c
+        func_d()
+      File "...tests...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: Guessing time !
+    <BLANKLINE>
+
+Other weird stuff
+`````````````````
+
+Clearing traceback works (Python 3.4 and up)::
+
+    >>> tb = Traceback.from_string("""
+    ... File "skipped.py", line 123, in func_123
+    ... Traceback (most recent call last):
+    ...   File "tests/examples.py", line 2, in func_a
+    ...     func_b()
+    ...   File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...   File "tests/examples.py", line 10, in func_c
+    ...     func_d()
+    ...   File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """)
+    >>> import traceback, sys
+    >>> if sys.version_info > (3, 4):
+    ...     traceback.clear_frames(tb)
+
+Credits
+=======
+
+* `mitsuhiko/jinja2 <https://github.com/mitsuhiko/jinja2>`_ for figuring a way to create traceback objects.
+
+
+Changelog
+=========
+
+2.0.0 (2023-06-22)
+~~~~~~~~~~~~~~~~~~
+
+* Removed support for legacy Pythons (2.7 and 3.6) and added Python 3.11 in the test grid.
+* Some cleanups and refactors (mostly from ruff).
+
+1.7.0 (2020-07-24)
+~~~~~~~~~~~~~~~~~~
+
+* Add more attributes to ``Frame`` and ``Code`` objects for pytest compatibility. Contributed by Ivanq in
+  `#58 <https://github.com/ionelmc/python-tblib/pull/58>`_.
+
+1.6.0 (2019-12-07)
+~~~~~~~~~~~~~~~~~~
+
+* When pickling an Exception, also pickle its traceback and the Exception chain
+  (``raise ... from ...``). Contributed by Guido Imperiale in
+  `#53 <https://github.com/ionelmc/python-tblib/issues/53>`_.
+
+1.5.0 (2019-10-23)
+~~~~~~~~~~~~~~~~~~
+
+* Added support for Python 3.8. Contributed by Victor Stinner in
+  `#42 <https://github.com/ionelmc/python-tblib/issues/42>`_.
+* Removed support for end of life Python 3.4.
+* Few CI improvements and fixes.
+
+1.4.0 (2019-05-02)
+~~~~~~~~~~~~~~~~~~
+
+* Removed support for end of life Python 3.3.
+* Fixed tests for Python 3.7. Contributed by Elliott Sales de Andrade in
+  `#36 <https://github.com/ionelmc/python-tblib/issues/36>`_.
+* Fixed compatibility issue with Twised (``twisted.python.failure.Failure`` expected a ``co_code`` attribute).
+
+1.3.2 (2017-04-09)
+~~~~~~~~~~~~~~~~~~
+
+* Add support for PyPy3.5-5.7.1-beta. Previously ``AttributeError:
+  'Frame' object has no attribute 'clear'``  could be raised. See PyPy
+  issue `#2532 <https://foss.heptapod.net/pypy/pypy/-/issues/2532>`_.
+
+1.3.1 (2017-03-27)
+~~~~~~~~~~~~~~~~~~
+
+* Fixed handling for tracebacks due to exceeding the recursion limit.
+  Fixes `#15 <https://github.com/ionelmc/python-tblib/issues/15>`_.
+
+1.3.0 (2016-03-08)
+~~~~~~~~~~~~~~~~~~
+
+* Added ``Traceback.from_string``.
+
+1.2.0 (2015-12-18)
+~~~~~~~~~~~~~~~~~~
+
+* Fixed handling for tracebacks from generators and other internal improvements
+  and optimizations. Contributed by DRayX in `#10 <https://github.com/ionelmc/python-tblib/issues/10>`_
+  and `#11 <https://github.com/ionelmc/python-tblib/pull/11>`_.
+
+1.1.0 (2015-07-27)
+~~~~~~~~~~~~~~~~~~
+
+* Added support for Python 2.6. Contributed by Arcadiy Ivanov in
+  `#8 <https://github.com/ionelmc/python-tblib/pull/8>`_.
+
+1.0.0 (2015-03-30)
+~~~~~~~~~~~~~~~~~~
+
+* Added ``to_dict`` method and ``from_dict`` classmethod on Tracebacks.
+  Contributed by beckjake in `#5 <https://github.com/ionelmc/python-tblib/pull/5>`_.
```

### Comparing `tblib-1.7.0/README.rst` & `tblib-2.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,39 +6,30 @@
 
 .. list-table::
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - | |travis| |appveyor| |requires|
+      - | |github-actions| |requires|
         | |codecov|
     * - package
       - | |version| |wheel| |supported-versions| |supported-implementations|
         | |commits-since|
-
-.. |docs| image:: https://codecov.io/gh/ionelmc/python-tblib/branch/master/graphs/badge.svg?branch=master
-    :target: https://readthedocs.org/projects/python-tblib
+.. |docs| image:: https://readthedocs.org/projects/python-tblib/badge/?style=flat
+    :target: https://python-tblib.readthedocs.io/
     :alt: Documentation Status
 
-.. |travis| image:: https://api.travis-ci.org/ionelmc/python-tblib.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.org/ionelmc/python-tblib
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/ionelmc/python-tblib?branch=master&svg=true
-    :alt: AppVeyor Build Status
-    :target: https://ci.appveyor.com/project/ionelmc/python-tblib
-
-.. |requires| image:: https://requires.io/github/ionelmc/python-tblib/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/ionelmc/python-tblib/requirements/?branch=master
+.. |github-actions| image:: https://github.com/ionelmc/python-tblib/actions/workflows/github-actions.yml/badge.svg
+    :alt: GitHub Actions Build Status
+    :target: https://github.com/ionelmc/python-tblib/actions
 
-.. |codecov| image:: https://codecov.io/github/ionelmc/python-tblib/coverage.svg?branch=master
+.. |codecov| image:: https://codecov.io/gh/ionelmc/python-tblib/branch/master/graphs/badge.svg?branch=master
     :alt: Coverage Status
-    :target: https://codecov.io/github/ionelmc/python-tblib
+    :target: https://app.codecov.io/github/ionelmc/python-tblib
 
 .. |version| image:: https://img.shields.io/pypi/v/tblib.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/tblib
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/tblib.svg
     :alt: PyPI Wheel
@@ -48,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/tblib
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/tblib.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/tblib
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-tblib/v1.7.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-tblib/v2.0.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-tblib/compare/v1.7.0...master
+    :target: https://github.com/ionelmc/python-tblib/compare/v2.0.0...master
 
 .. end-badges
 
 Serialization library for Exceptions and Tracebacks.
 
 * Free software: BSD license
```

### Comparing `tblib-1.7.0/docs/conf.py` & `tblib-2.0.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-
-import os
+import sphinx_py3doc_enhanced_theme
 
 extensions = [
     'autoapi.extension',
     'sphinx.ext.coverage',
     'sphinx.ext.doctest',
     'sphinx.ext.extlinks',
     'sphinx.ext.ifconfig',
@@ -15,36 +12,35 @@
 ]
 autoapi_type = 'python'
 autoapi_dirs = ['../src']
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'tblib'
-year = '2013-2020'
+year = '2013-2022'
 author = 'Ionel Cristian Mărieș'
-copyright = '{0}, {1}'.format(year, author)
-version = release = '1.7.0'
+copyright = f'{year}, {author}'
+version = release = '2.0.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/ionelmc/python-tblib/issues/%s', '#'),
     'pr': ('https://github.com/ionelmc/python-tblib/pull/%s', 'PR #'),
 }
-import sphinx_py3doc_enhanced_theme
-html_theme = "sphinx_py3doc_enhanced_theme"
+html_theme = 'sphinx_py3doc_enhanced_theme'
 html_theme_path = [sphinx_py3doc_enhanced_theme.get_html_theme_path()]
 html_theme_options = {
-    'githuburl': 'https://github.com/ionelmc/python-tblib/'
+    'githuburl': 'https://github.com/ionelmc/python-tblib/',
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = '%b %d, %Y'
 html_split_index = False
 html_sidebars = {
-   '**': ['searchbox.html', 'globaltoc.html', 'sourcelink.html'],
+    '**': ['searchbox.html', 'globaltoc.html', 'sourcelink.html'],
 }
-html_short_title = '%s-%s' % (project, version)
+html_short_title = f'{project}-{version}'
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
```

### Comparing `tblib-1.7.0/setup.py` & `tblib-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,72 @@
 #!/usr/bin/env python
-# -*- encoding: utf-8 -*-
-from __future__ import absolute_import
-from __future__ import print_function
-
-import io
 import re
-from glob import glob
-from os.path import basename
-from os.path import dirname
-from os.path import join
-from os.path import splitext
+from pathlib import Path
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 def read(*names, **kwargs):
-    with io.open(
-        join(dirname(__file__), *names),
-        encoding=kwargs.get('encoding', 'utf8')
-    ) as fh:
+    with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='tblib',
-    version='1.7.0',
+    version='2.0.0',
     license='BSD-2-Clause',
     description='Traceback serialization library.',
-    long_description='%s\n%s' % (
+    long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
-        re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
+        re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Ionel Cristian Mărieș',
     author_email='contact@ionelmc.ro',
     url='https://github.com/ionelmc/python-tblib',
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
+    py_modules=[path.stem for path in Path('src').glob('*.py')],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: Unix',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         # uncomment if you test on these interpreters:
         # 'Programming Language :: Python :: Implementation :: IronPython',
         # 'Programming Language :: Python :: Implementation :: Jython',
         # 'Programming Language :: Python :: Implementation :: Stackless',
         'Topic :: Utilities',
     ],
     project_urls={
         'Documentation': 'https://python-tblib.readthedocs.io/',
         'Changelog': 'https://python-tblib.readthedocs.io/en/latest/changelog.html',
         'Issue Tracker': 'https://github.com/ionelmc/python-tblib/issues',
     },
     keywords=[
-        'traceback', 'debugging', 'exceptions',
+        'traceback',
+        'debugging',
+        'exceptions',
     ],
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
+    python_requires='>=3.7',
     install_requires=[
         # eg: 'aspectlib==1.1.1', 'six>=1.7',
     ],
     extras_require={
         # eg:
         #   'rst': ['docutils>=0.11'],
         #   ':python_version=="2.6"': ['argparse'],
```

### Comparing `tblib-1.7.0/src/tblib/__init__.py` & `tblib-2.0.0/src/tblib/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,80 @@
 import re
 import sys
 from types import CodeType
-from types import FrameType
-from types import TracebackType
 
-try:
-    from __pypy__ import tproxy
-except ImportError:
-    tproxy = None
-try:
-    from .cpython import tb_set_next
-except ImportError:
-    tb_set_next = None
-
-if not tb_set_next and not tproxy:
-    raise ImportError("Cannot use tblib. Runtime not supported.")
-
-__version__ = '1.7.0'
+__version__ = '2.0.0'
 __all__ = 'Traceback', 'TracebackParseError', 'Frame', 'Code'
 
-PY3 = sys.version_info[0] == 3
 FRAME_RE = re.compile(r'^\s*File "(?P<co_filename>.+)", line (?P<tb_lineno>\d+)(, in (?P<co_name>.+))?$')
 
 
 class _AttrDict(dict):
     __slots__ = ()
 
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError:
-            raise AttributeError(name)
+            raise AttributeError(name) from None
 
 
 # noinspection PyPep8Naming
 class __traceback_maker(Exception):
     pass
 
 
 class TracebackParseError(Exception):
     pass
 
 
-class Code(object):
+class Code:
     """
     Class that replicates just enough of the builtin Code object to enable serialization and traceback rendering.
     """
+
     co_code = None
 
     def __init__(self, code):
         self.co_filename = code.co_filename
         self.co_name = code.co_name
         self.co_argcount = 0
         self.co_kwonlyargcount = 0
         self.co_varnames = ()
         self.co_nlocals = 0
         self.co_stacksize = 0
         self.co_flags = 64
         self.co_firstlineno = 0
 
-    # noinspection SpellCheckingInspection
-    def __tproxy__(self, operation, *args, **kwargs):
-        """
-        Necessary for PyPy's tproxy.
-        """
-        if operation in ('__getattribute__', '__getattr__'):
-            return getattr(self, args[0])
-        else:
-            return getattr(self, operation)(*args, **kwargs)
-
 
-class Frame(object):
+class Frame:
     """
     Class that replicates just enough of the builtin Frame object to enable serialization and traceback rendering.
     """
+
     def __init__(self, frame):
         self.f_locals = {}
-        self.f_globals = {
-            k: v
-            for k, v in frame.f_globals.items()
-            if k in ("__file__", "__name__")
-        }
+        self.f_globals = {k: v for k, v in frame.f_globals.items() if k in ('__file__', '__name__')}
         self.f_code = Code(frame.f_code)
         self.f_lineno = frame.f_lineno
 
     def clear(self):
         """
         For compatibility with PyPy 3.5;
         clear() was added to frame in Python 3.4
         and is called by traceback.clear_frames(), which
         in turn is called by unittest.TestCase.assertRaises
         """
 
-    # noinspection SpellCheckingInspection
-    def __tproxy__(self, operation, *args, **kwargs):
-        """
-        Necessary for PyPy's tproxy.
-        """
-        if operation in ('__getattribute__', '__getattr__'):
-            if args[0] == 'f_code':
-                return tproxy(CodeType, self.f_code.__tproxy__)
-            else:
-                return getattr(self, args[0])
-        else:
-            return getattr(self, operation)(*args, **kwargs)
 
-
-class Traceback(object):
+class Traceback:
     """
     Class that wraps builtin Traceback objects.
     """
+
     tb_next = None
 
     def __init__(self, tb):
         self.tb_frame = Frame(tb.tb_frame)
         # noinspection SpellCheckingInspection
         self.tb_lineno = int(tb.tb_lineno)
 
@@ -129,81 +90,62 @@
             prev_traceback = traceback
             tb = tb.tb_next
 
     def as_traceback(self):
         """
         Convert to a builtin Traceback object that is usable for raising or rendering a stacktrace.
         """
-        if tproxy:
-            return tproxy(TracebackType, self.__tproxy__)
-        if not tb_set_next:
-            raise RuntimeError("Unsupported Python interpreter!")
-
         current = self
         top_tb = None
         tb = None
         while current:
             f_code = current.tb_frame.f_code
             code = compile('\n' * (current.tb_lineno - 1) + 'raise __traceback_maker', current.tb_frame.f_code.co_filename, 'exec')
-            if hasattr(code, "replace"):
+            if hasattr(code, 'replace'):
                 # Python 3.8 and newer
-                code = code.replace(co_argcount=0,
-                                    co_filename=f_code.co_filename, co_name=f_code.co_name,
-                                    co_freevars=(), co_cellvars=())
-            elif PY3:
-                code = CodeType(
-                    0, code.co_kwonlyargcount,
-                    code.co_nlocals, code.co_stacksize, code.co_flags,
-                    code.co_code, code.co_consts, code.co_names, code.co_varnames,
-                    f_code.co_filename, f_code.co_name,
-                    code.co_firstlineno, code.co_lnotab, (), ()
-                )
+                code = code.replace(co_argcount=0, co_filename=f_code.co_filename, co_name=f_code.co_name, co_freevars=(), co_cellvars=())
             else:
                 code = CodeType(
                     0,
-                    code.co_nlocals, code.co_stacksize, code.co_flags,
-                    code.co_code, code.co_consts, code.co_names, code.co_varnames,
-                    f_code.co_filename.encode(), f_code.co_name.encode(),
-                    code.co_firstlineno, code.co_lnotab, (), ()
+                    code.co_kwonlyargcount,
+                    code.co_nlocals,
+                    code.co_stacksize,
+                    code.co_flags,
+                    code.co_code,
+                    code.co_consts,
+                    code.co_names,
+                    code.co_varnames,
+                    f_code.co_filename,
+                    f_code.co_name,
+                    code.co_firstlineno,
+                    code.co_lnotab,
+                    (),
+                    (),
                 )
 
             # noinspection PyBroadException
             try:
-                exec(code, dict(current.tb_frame.f_globals), {})
+                exec(code, dict(current.tb_frame.f_globals), {})  # noqa: S102
             except Exception:
                 next_tb = sys.exc_info()[2].tb_next
                 if top_tb is None:
                     top_tb = next_tb
                 if tb is not None:
-                    tb_set_next(tb, next_tb)
+                    tb.tb_next = next_tb
                 tb = next_tb
                 del next_tb
 
             current = current.tb_next
         try:
             return top_tb
         finally:
             del top_tb
             del tb
-    to_traceback = as_traceback
 
-    # noinspection SpellCheckingInspection
-    def __tproxy__(self, operation, *args, **kwargs):
-        """
-        Necessary for PyPy's tproxy.
-        """
-        if operation in ('__getattribute__', '__getattr__'):
-            if args[0] == 'tb_next':
-                return self.tb_next and self.tb_next.as_traceback()
-            elif args[0] == 'tb_frame':
-                return tproxy(FrameType, self.tb_frame.__tproxy__)
-            else:
-                return getattr(self, args[0])
-        else:
-            return getattr(self, operation)(*args, **kwargs)
+    to_traceback = as_traceback
 
     def as_dict(self):
         """
         Converts to a dictionary representation. You can serialize the result to JSON as it only has
         builtin objects like dicts, lists, ints or strings.
         """
         if self.tb_next is None:
@@ -221,14 +163,15 @@
             'f_lineno': self.tb_frame.f_lineno,
         }
         return {
             'tb_frame': frame,
             'tb_lineno': self.tb_lineno,
             'tb_next': tb_next,
         }
+
     to_dict = as_dict
 
     @classmethod
     def from_dict(cls, dct):
         """
         Creates an instance from a dictionary with the same structure as ``.as_dict()`` returns.
         """
@@ -290,8 +233,8 @@
                         f_code=_AttrDict(frame),
                         f_lineno=int(frame['tb_lineno']),
                     ),
                     tb_next=previous,
                 )
             return cls(previous)
         else:
-            raise TracebackParseError("Could not find any frames in %r." % string)
+            raise TracebackParseError('Could not find any frames in %r.' % string)
```

### Comparing `tblib-1.7.0/src/tblib/decorators.py` & `tblib-2.0.0/src/tblib/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 
 from six import reraise
 
 from . import Traceback
 
 
-class Error(object):
+class Error:
     def __init__(self, exc_type, exc_value, traceback):
         self.exc_type = exc_type
         self.exc_value = exc_value
         self.__traceback = Traceback(traceback)
 
     @property
     def traceback(self):
```

### Comparing `tblib-1.7.0/src/tblib/pickling_support.py` & `tblib-2.0.0/src/tblib/pickling_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     # __reduce_ex__(5) could bring benefits in the unlikely case the exception
     # directly contains buffers, but PickleBuffer objects will cause a crash when
     # running on protocol=4, and there's no clean way to figure out the current
     # protocol from here. Note that any object returned by __reduce_ex__(3) will
     # still be pickled with protocol 5 if pickle.dump() is running with it.
     rv = obj.__reduce_ex__(3)
     if isinstance(rv, str):
-        raise TypeError("str __reduce__ output is not supported")
-    assert isinstance(rv, tuple) and len(rv) >= 2
+        raise TypeError('str __reduce__ output is not supported')
+    assert isinstance(rv, tuple)
+    assert len(rv) >= 2
 
     return (unpickle_exception, rv[:2] + (obj.__cause__, obj.__traceback__)) + rv[2:]
 
 
 def _get_subclasses(cls):
     # Depth-first traversal of all direct and indirect subclasses of cls
     to_visit = [cls]
@@ -77,11 +78,8 @@
                 exc = exc.__cause__
         elif isinstance(exc, type) and issubclass(exc, BaseException):
             copyreg.pickle(exc, pickle_exception)
             # Allow using @install as a decorator for Exception classes
             if len(exc_classes_or_instances) == 1:
                 return exc
         else:
-            raise TypeError(
-                "Expected subclasses or instances of BaseException, got %s"
-                % (type(exc))
-            )
+            raise TypeError('Expected subclasses or instances of BaseException, got %s' % (type(exc)))
```

### Comparing `tblib-1.7.0/src/tblib.egg-info/PKG-INFO` & `tblib-2.0.0/src/tblib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,760 +1,768 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tblib
-Version: 1.7.0
+Version: 2.0.0
 Summary: Traceback serialization library.
 Home-page: https://github.com/ionelmc/python-tblib
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-tblib.readthedocs.io/
 Project-URL: Changelog, https://python-tblib.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-tblib/issues
-Description: ========
-        Overview
-        ========
-        
-        
-        
-        Serialization library for Exceptions and Tracebacks.
-        
-        * Free software: BSD license
-        
-        It allows you to:
-        
-        * `Pickle <https://docs.python.org/3/library/pickle.html>`_ tracebacks and raise exceptions
-          with pickled tracebacks in different processes. This allows better error handling when running
-          code over multiple processes (imagine multiprocessing, billiard, futures, celery etc).
-        * Create traceback objects from strings (the ``from_string`` method). *No pickling is used*.
-        * Serialize tracebacks to/from plain dicts (the ``from_dict`` and ``to_dict`` methods). *No pickling is used*.
-        * Raise the tracebacks created from the aforementioned sources.
-        * Pickle an Exception together with its traceback and exception chain
-          (``raise ... from ...``) *(Python 3 only)*
-        
-        **Again, note that using the pickle support is completely optional. You are solely responsible for
-        security problems should you decide to use the pickle support.**
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install tblib
-        
-        Documentation
-        =============
-        
-        .. contents::
-           :local:
-        
-        Pickling tracebacks
-        ~~~~~~~~~~~~~~~~~~~
-        
-        **Note**: The traceback objects that come out are stripped of some attributes (like variables). But you'll be able to raise exceptions with
-        those tracebacks or print them - that should cover 99% of the usecases.
-        
-        ::
-        
-            >>> from tblib import pickling_support
-            >>> pickling_support.install()
-            >>> import pickle, sys
-            >>> def inner_0():
-            ...     raise Exception('fail')
-            ...
-            >>> def inner_1():
-            ...     inner_0()
-            ...
-            >>> def inner_2():
-            ...     inner_1()
-            ...
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s1 = pickle.dumps(sys.exc_info())
-            ...
-            >>> len(s1) > 1
-            True
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s2 = pickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
-            ...
-            >>> len(s2) > 1
-            True
-        
-            >>> try:
-            ...     import cPickle
-            ... except ImportError:
-            ...     import pickle as cPickle
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     s3 = cPickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
-            ...
-            >>> len(s3) > 1
-            True
-        
-        Unpickling tracebacks
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            >>> pickle.loads(s1)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-            >>> pickle.loads(s2)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-            >>> pickle.loads(s3)
-            (<...Exception'>, Exception('fail'...), <traceback object at ...>)
-        
-        Raising
-        ~~~~~~~
-        
-        ::
-        
-            >>> from six import reraise
-            >>> reraise(*pickle.loads(s1))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-            >>> reraise(*pickle.loads(s2))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-            >>> reraise(*pickle.loads(s3))
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[14]>", line 1, in <module>
-                reraise(*pickle.loads(s2))
-              File "<doctest README.rst[8]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        Pickling Exceptions together with their traceback and chain (Python 3 only)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            >>> try:  # doctest: +SKIP
-            ...     try:
-            ...         1 / 0
-            ...     except Exception as e:
-            ...         raise Exception("foo") from e
-            ... except Exception as e:
-            ...     s = pickle.dumps(e)
-            >>> raise pickle.loads(s)  # doctest: +SKIP
-            Traceback (most recent call last):
-              File "<doctest README.rst[16]>", line 3, in <module>
-                1 / 0
-            ZeroDivisionError: division by zero
-        
-            The above exception was the direct cause of the following exception:
-        
-            Traceback (most recent call last):
-              File "<doctest README.rst[17]>", line 1, in <module>
-                raise pickle.loads(s)
-              File "<doctest README.rst[16]>", line 5, in <module>
-                raise Exception("foo") from e
-            Exception: foo
-        
-        BaseException subclasses defined after calling ``pickling_support.install()`` will
-        **not** retain their traceback and exception chain pickling.
-        To cover custom Exceptions, there are three options:
-        
-        1. Use ``@pickling_support.install`` as a decorator for each custom Exception
-        
-            .. code-block:: python
-        
-                >>> from tblib import pickling_support
-                >>> # Declare all imports of your package's dependencies
-                >>> import numpy  # doctest: +SKIP
-        
-                >>> pickling_support.install()  # install for all modules imported so far
-        
-                >>> @pickling_support.install
-                ... class CustomError(Exception):
-                ...     pass
-        
-           Eventual subclasses of ``CustomError`` will need to be decorated again.
-        
-        2. Invoke ``pickling_support.install()`` after all modules have been imported and all
-           Exception subclasses have been declared
-        
-            .. code-block:: python
-        
-                >>> # Declare all imports of your package's dependencies
-                >>> import numpy  # doctest: +SKIP
-                >>> from tblib import pickling_support
-        
-                >>> # Declare your own custom Exceptions
-                >>> class CustomError(Exception):
-                ...     pass
-        
-                >>> # Finally, install tblib
-                >>> pickling_support.install()
-        
-        3. Selectively install tblib for Exception instances just before they are pickled
-        
-            .. code-block:: python
-        
-               pickling_support.install(<Exception instance>, [Exception instance], ...)
-        
-           The above will install tblib pickling for all listed exceptions as well as any other
-           exceptions in their exception chains.
-        
-           For example, one could write a wrapper to be used with
-           `ProcessPoolExecutor <https://docs.python.org/3/library/concurrent.futures.html>`_,
-           `Dask.distributed <https://distributed.dask.org/>`_, or similar libraries:
-        
-        ::
-        
-            >>> from tblib import pickling_support
-            >>> def wrapper(func, *args, **kwargs):
-            ...     try:
-            ...         return func(*args, **kwargs)
-            ...     except Exception as e:
-            ...         pickling_support.install(e)
-            ...         raise
-        
-        What if we have a local stack, does it show correctly ?
-        -------------------------------------------------------
-        
-        Yes it does::
-        
-            >>> exc_info = pickle.loads(s3)
-            >>> def local_0():
-            ...     reraise(*exc_info)
-            ...
-            >>> def local_1():
-            ...     local_0()
-            ...
-            >>> def local_2():
-            ...     local_1()
-            ...
-            >>> local_2()
-            Traceback (most recent call last):
-              File "...doctest.py", line ..., in __run
-                compileflags, 1) in test.globs
-              File "<doctest README.rst[24]>", line 1, in <module>
-                local_2()
-              File "<doctest README.rst[23]>", line 2, in local_2
-                local_1()
-              File "<doctest README.rst[22]>", line 2, in local_1
-                local_0()
-              File "<doctest README.rst[21]>", line 2, in local_0
-                reraise(*exc_info)
-              File "<doctest README.rst[11]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        It also supports more contrived scenarios
-        -----------------------------------------
-        
-        Like tracebacks with syntax errors::
-        
-            >>> from tblib import Traceback
-            >>> from examples import bad_syntax
-            >>> try:
-            ...     bad_syntax()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[58]>", line 1, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[57]>", line 2, in <module>
-                bad_syntax()
-              File "...tests...examples.py", line 18, in bad_syntax
-                import badsyntax
-              File "...tests...badsyntax.py", line 5
-                is very bad
-                 ^
-            SyntaxError: invalid syntax
-        
-        Or other import failures::
-        
-            >>> from examples import bad_module
-            >>> try:
-            ...     bad_module()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[61]>", line 1, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[60]>", line 2, in <module>
-                bad_module()
-              File "...tests...examples.py", line 23, in bad_module
-                import badmodule
-              File "...tests...badmodule.py", line 3, in <module>
-                raise Exception("boom!")
-            Exception: boom!
-        
-        Or a traceback that's caused by exceeding the recursion limit (here we're
-        forcing the type and value to have consistency across platforms)::
-        
-            >>> def f(): f()
-            >>> try:
-            ...    f()
-            ... except RuntimeError:
-            ...    et, ev, tb = sys.exc_info()
-            ...    tb = Traceback(tb)
-            ...
-            >>> reraise(RuntimeError, RuntimeError("maximum recursion depth exceeded"), tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              File "<doctest README.rst[32]>", line 1, in f
-                def f(): f()
-              ...
-            RuntimeError: maximum recursion depth exceeded
-        
-        Reference
-        ~~~~~~~~~
-        
-        tblib.Traceback
-        ---------------
-        
-        It is used by the ``pickling_support``. You can use it too if you want more flexibility::
-        
-            >>> from tblib import Traceback
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[21]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[21]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        tblib.Traceback.to_dict
-        ```````````````````````
-        
-        You can use the ``to_dict`` method and the ``from_dict`` classmethod to
-        convert a Traceback into and from a dictionary serializable by the stdlib
-        json.JSONDecoder::
-        
-            >>> import json
-            >>> from pprint import pprint
-            >>> try:
-            ...     inner_2()
-            ... except:
-            ...     et, ev, tb = sys.exc_info()
-            ...     tb = Traceback(tb)
-            ...     tb_dict = tb.to_dict()
-            ...     pprint(tb_dict)
-            {'tb_frame': {'f_code': {'co_filename': '<doctest README.rst[...]>',
-                                     'co_name': '<module>'},
-                          'f_globals': {'__name__': '__main__'},
-                          'f_lineno': 5},
-             'tb_lineno': 2,
-             'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                 'co_name': 'inner_2'},
-                                      'f_globals': {'__name__': '__main__'},
-                                      'f_lineno': 2},
-                         'tb_lineno': 2,
-                         'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                             'co_name': 'inner_1'},
-                                                  'f_globals': {'__name__': '__main__'},
-                                                  'f_lineno': 2},
-                                     'tb_lineno': 2,
-                                     'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
-                                                                         'co_name': 'inner_0'},
-                                                              'f_globals': {'__name__': '__main__'},
-                                                              'f_lineno': 2},
-                                                 'tb_lineno': 2,
-                                                 'tb_next': None}}}}
-        
-        tblib.Traceback.from_dict
-        `````````````````````````
-        
-        Building on the previous example::
-        
-            >>> tb_json = json.dumps(tb_dict)
-            >>> tb = Traceback.from_dict(json.loads(tb_json))
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[21]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "<doctest README.rst[21]>", line 2, in <module>
-                inner_2()
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        tblib.Traceback.from_string
-        ```````````````````````````
-        
-        ::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "skipped.py", line 123, in func_123
-            ... Traceback (most recent call last):
-            ...   File "tests/examples.py", line 2, in func_a
-            ...     func_b()
-            ...   File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...   File "tests/examples.py", line 10, in func_c
-            ...     func_d()
-            ...   File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """)
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[42]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: fail
-        
-        
-        If you use the ``strict=False`` option then parsing is a bit more lax::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "bogus.py", line 123, in bogus
-            ... Traceback (most recent call last):
-            ...  File "tests/examples.py", line 2, in func_a
-            ...   func_b()
-            ...    File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...    File "tests/examples.py", line 10, in func_c
-            ...   func_d()
-            ...  File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """, strict=False)
-            >>> reraise(et, ev, tb.as_traceback())
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[42]>", line 6, in <module>
-                reraise(et, ev, tb.as_traceback())
-              File "bogus.py", line 123, in bogus
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: fail
-        
-        tblib.decorators.return_error
-        -----------------------------
-        
-        ::
-        
-            >>> from tblib.decorators import return_error
-            >>> inner_2r = return_error(inner_2)
-            >>> e = inner_2r()
-            >>> e
-            <tblib.decorators.Error object at ...>
-            >>> e.reraise()
-            Traceback (most recent call last):
-              ...
-              File "<doctest README.rst[26]>", line 1, in <module>
-                e.reraise()
-              File "...tblib...decorators.py", line 19, in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line 25, in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "<doctest README.rst[5]>", line 2, in inner_2
-                inner_1()
-              File "<doctest README.rst[4]>", line 2, in inner_1
-                inner_0()
-              File "<doctest README.rst[3]>", line 2, in inner_0
-                raise Exception('fail')
-            Exception: fail
-        
-        How's this useful? Imagine you're using multiprocessing like this::
-        
-            # Note that Python 3.4 and later will show the remote traceback (but as a string sadly) so we skip testing this.
-            >>> import traceback
-            >>> from multiprocessing import Pool
-            >>> from examples import func_a
-            >>> pool = Pool()  # doctest: +SKIP
-            >>> try:  # doctest: +SKIP
-            ...     for i in pool.map(func_a, range(5)):
-            ...         print(i)
-            ... except:
-            ...     print(traceback.format_exc())
-            ...
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 2, in <module>
-                for i in pool.map(func_a, range(5)):
-              File "...multiprocessing...pool.py", line ..., in map
-                ...
-              File "...multiprocessing...pool.py", line ..., in get
-                ...
-            Exception: Guessing time !
-            <BLANKLINE>
-            >>> pool.terminate()  # doctest: +SKIP
-        
-        Not very useful is it? Let's sort this out::
-        
-            >>> from tblib.decorators import apply_with_return_error, Error
-            >>> from itertools import repeat
-            >>> pool = Pool()
-            >>> try:
-            ...     for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
-            ...         if isinstance(i, Error):
-            ...             i.reraise()
-            ...         else:
-            ...             print(i)
-            ... except:
-            ...     print(traceback.format_exc())
-            ...
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 4, in <module>
-                i.reraise()
-              File "...tblib...decorators.py", line ..., in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line ..., in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "...tblib...decorators.py", line ..., in apply_with_return_error
-                return args[0](*args[1:])
-              File "...examples.py", line 2, in func_a
-                func_b()
-              File "...examples.py", line 6, in func_b
-                func_c()
-              File "...examples.py", line 10, in func_c
-                func_d()
-              File "...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: Guessing time !
-            <BLANKLINE>
-            >>> pool.terminate()
-        
-        Much better !
-        
-        What if we have a local call stack ?
-        ````````````````````````````````````
-        
-        ::
-        
-            >>> def local_0():
-            ...     pool = Pool()
-            ...     try:
-            ...         for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
-            ...             if isinstance(i, Error):
-            ...                 i.reraise()
-            ...             else:
-            ...                 print(i)
-            ...     finally:
-            ...         pool.close()
-            ...
-            >>> def local_1():
-            ...     local_0()
-            ...
-            >>> def local_2():
-            ...     local_1()
-            ...
-            >>> try:
-            ...     local_2()
-            ... except:
-            ...     print(traceback.format_exc())
-            Traceback (most recent call last):
-              File "<doctest README.rst[...]>", line 2, in <module>
-                local_2()
-              File "<doctest README.rst[...]>", line 2, in local_2
-                local_1()
-              File "<doctest README.rst[...]>", line 2, in local_1
-                local_0()
-              File "<doctest README.rst[...]>", line 6, in local_0
-                i.reraise()
-              File "...tblib...decorators.py", line 20, in reraise
-                reraise(self.exc_type, self.exc_value, self.traceback)
-              File "...tblib...decorators.py", line 27, in return_exceptions_wrapper
-                return func(*args, **kwargs)
-              File "...tblib...decorators.py", line 47, in apply_with_return_error
-                return args[0](*args[1:])
-              File "...tests...examples.py", line 2, in func_a
-                func_b()
-              File "...tests...examples.py", line 6, in func_b
-                func_c()
-              File "...tests...examples.py", line 10, in func_c
-                func_d()
-              File "...tests...examples.py", line 14, in func_d
-                raise Exception("Guessing time !")
-            Exception: Guessing time !
-            <BLANKLINE>
-        
-        Other weird stuff
-        `````````````````
-        
-        Clearing traceback works (Python 3.4 and up)::
-        
-            >>> tb = Traceback.from_string("""
-            ... File "skipped.py", line 123, in func_123
-            ... Traceback (most recent call last):
-            ...   File "tests/examples.py", line 2, in func_a
-            ...     func_b()
-            ...   File "tests/examples.py", line 6, in func_b
-            ...     func_c()
-            ...   File "tests/examples.py", line 10, in func_c
-            ...     func_d()
-            ...   File "tests/examples.py", line 14, in func_d
-            ... Doesn't: matter
-            ... """)
-            >>> import traceback, sys
-            >>> if sys.version_info > (3, 4):
-            ...     traceback.clear_frames(tb)
-        
-        Credits
-        =======
-        
-        * `mitsuhiko/jinja2 <https://github.com/mitsuhiko/jinja2>`_ for figuring a way to create traceback objects.
-        
-        
-        Changelog
-        =========
-        
-        1.7.0 (2020-07-24)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Add more attributes to ``Frame`` and ``Code`` objects for pytest compatibility. Contributed by Ivanq in
-          `#58 <https://github.com/ionelmc/python-tblib/pull/58>`_.
-        
-        1.6.0 (2019-12-07)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * When pickling an Exception, also pickle its traceback and the Exception chain
-          (``raise ... from ...``). Contributed by Guido Imperiale in
-          `#53 <https://github.com/ionelmc/python-tblib/issues/53>`_.
-        
-        1.5.0 (2019-10-23)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added support for Python 3.8. Contributed by Victor Stinner in
-          `#42 <https://github.com/ionelmc/python-tblib/issues/42>`_.
-        * Removed support for end of life Python 3.4.
-        * Few CI improvements and fixes.
-        
-        1.4.0 (2019-05-02)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Removed support for end of life Python 3.3.
-        * Fixed tests for Python 3.7. Contributed by Elliott Sales de Andrade in
-          `#36 <https://github.com/ionelmc/python-tblib/issues/36>`_.
-        * Fixed compatibility issue with Twised (``twisted.python.failure.Failure`` expected a ``co_code`` attribute).
-        
-        1.3.2 (2017-04-09)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Add support for PyPy3.5-5.7.1-beta. Previously ``AttributeError:
-          'Frame' object has no attribute 'clear'``  could be raised. See PyPy
-          issue `#2532 <https://bitbucket.org/pypy/pypy/issues/2532/pypy3-attributeerror-frame-object-has-no>`_.
-        
-        1.3.1 (2017-03-27)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Fixed handling for tracebacks due to exceeding the recursion limit.
-          Fixes `#15 <https://github.com/ionelmc/python-tblib/issues/15>`_.
-        
-        1.3.0 (2016-03-08)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added ``Traceback.from_string``.
-        
-        1.2.0 (2015-12-18)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Fixed handling for tracebacks from generators and other internal improvements
-          and optimizations. Contributed by DRayX in `#10 <https://github.com/ionelmc/python-tblib/issues/10>`_
-          and `#11 <https://github.com/ionelmc/python-tblib/pull/11>`_.
-        
-        1.1.0 (2015-07-27)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added support for Python 2.6. Contributed by Arcadiy Ivanov in
-          `#8 <https://github.com/ionelmc/python-tblib/pull/8>`_.
-        
-        1.0.0 (2015-03-30)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * Added ``to_dict`` method and ``from_dict`` classmethod on Tracebacks.
-          Contributed by beckjake in `#5 <https://github.com/ionelmc/python-tblib/pull/5>`_.
-        
 Keywords: traceback,debugging,exceptions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+Overview
+========
+
+
+
+Serialization library for Exceptions and Tracebacks.
+
+* Free software: BSD license
+
+It allows you to:
+
+* `Pickle <https://docs.python.org/3/library/pickle.html>`_ tracebacks and raise exceptions
+  with pickled tracebacks in different processes. This allows better error handling when running
+  code over multiple processes (imagine multiprocessing, billiard, futures, celery etc).
+* Create traceback objects from strings (the ``from_string`` method). *No pickling is used*.
+* Serialize tracebacks to/from plain dicts (the ``from_dict`` and ``to_dict`` methods). *No pickling is used*.
+* Raise the tracebacks created from the aforementioned sources.
+* Pickle an Exception together with its traceback and exception chain
+  (``raise ... from ...``) *(Python 3 only)*
+
+**Again, note that using the pickle support is completely optional. You are solely responsible for
+security problems should you decide to use the pickle support.**
+
+Installation
+============
+
+::
+
+    pip install tblib
+
+Documentation
+=============
+
+.. contents::
+   :local:
+
+Pickling tracebacks
+~~~~~~~~~~~~~~~~~~~
+
+**Note**: The traceback objects that come out are stripped of some attributes (like variables). But you'll be able to raise exceptions with
+those tracebacks or print them - that should cover 99% of the usecases.
+
+::
+
+    >>> from tblib import pickling_support
+    >>> pickling_support.install()
+    >>> import pickle, sys
+    >>> def inner_0():
+    ...     raise Exception('fail')
+    ...
+    >>> def inner_1():
+    ...     inner_0()
+    ...
+    >>> def inner_2():
+    ...     inner_1()
+    ...
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s1 = pickle.dumps(sys.exc_info())
+    ...
+    >>> len(s1) > 1
+    True
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s2 = pickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
+    ...
+    >>> len(s2) > 1
+    True
+
+    >>> try:
+    ...     import cPickle
+    ... except ImportError:
+    ...     import pickle as cPickle
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     s3 = cPickle.dumps(sys.exc_info(), protocol=pickle.HIGHEST_PROTOCOL)
+    ...
+    >>> len(s3) > 1
+    True
+
+Unpickling tracebacks
+~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    >>> pickle.loads(s1)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+    >>> pickle.loads(s2)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+    >>> pickle.loads(s3)
+    (<...Exception'>, Exception('fail'...), <traceback object at ...>)
+
+Raising
+~~~~~~~
+
+::
+
+    >>> from six import reraise
+    >>> reraise(*pickle.loads(s1))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+    >>> reraise(*pickle.loads(s2))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+    >>> reraise(*pickle.loads(s3))
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[14]>", line 1, in <module>
+        reraise(*pickle.loads(s2))
+      File "<doctest README.rst[8]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+Pickling Exceptions together with their traceback and chain (Python 3 only)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    >>> try:  # doctest: +SKIP
+    ...     try:
+    ...         1 / 0
+    ...     except Exception as e:
+    ...         raise Exception("foo") from e
+    ... except Exception as e:
+    ...     s = pickle.dumps(e)
+    >>> raise pickle.loads(s)  # doctest: +SKIP
+    Traceback (most recent call last):
+      File "<doctest README.rst[16]>", line 3, in <module>
+        1 / 0
+    ZeroDivisionError: division by zero
+
+    The above exception was the direct cause of the following exception:
+
+    Traceback (most recent call last):
+      File "<doctest README.rst[17]>", line 1, in <module>
+        raise pickle.loads(s)
+      File "<doctest README.rst[16]>", line 5, in <module>
+        raise Exception("foo") from e
+    Exception: foo
+
+BaseException subclasses defined after calling ``pickling_support.install()`` will
+**not** retain their traceback and exception chain pickling.
+To cover custom Exceptions, there are three options:
+
+1. Use ``@pickling_support.install`` as a decorator for each custom Exception
+
+    .. code-block:: python
+
+        >>> from tblib import pickling_support
+        >>> # Declare all imports of your package's dependencies
+        >>> import numpy  # doctest: +SKIP
+
+        >>> pickling_support.install()  # install for all modules imported so far
+
+        >>> @pickling_support.install
+        ... class CustomError(Exception):
+        ...     pass
+
+   Eventual subclasses of ``CustomError`` will need to be decorated again.
+
+2. Invoke ``pickling_support.install()`` after all modules have been imported and all
+   Exception subclasses have been declared
+
+    .. code-block:: python
+
+        >>> # Declare all imports of your package's dependencies
+        >>> import numpy  # doctest: +SKIP
+        >>> from tblib import pickling_support
+
+        >>> # Declare your own custom Exceptions
+        >>> class CustomError(Exception):
+        ...     pass
+
+        >>> # Finally, install tblib
+        >>> pickling_support.install()
+
+3. Selectively install tblib for Exception instances just before they are pickled
+
+    .. code-block:: python
+
+       pickling_support.install(<Exception instance>, [Exception instance], ...)
+
+   The above will install tblib pickling for all listed exceptions as well as any other
+   exceptions in their exception chains.
+
+   For example, one could write a wrapper to be used with
+   `ProcessPoolExecutor <https://docs.python.org/3/library/concurrent.futures.html>`_,
+   `Dask.distributed <https://distributed.dask.org/>`_, or similar libraries:
+
+::
+
+    >>> from tblib import pickling_support
+    >>> def wrapper(func, *args, **kwargs):
+    ...     try:
+    ...         return func(*args, **kwargs)
+    ...     except Exception as e:
+    ...         pickling_support.install(e)
+    ...         raise
+
+What if we have a local stack, does it show correctly ?
+-------------------------------------------------------
+
+Yes it does::
+
+    >>> exc_info = pickle.loads(s3)
+    >>> def local_0():
+    ...     reraise(*exc_info)
+    ...
+    >>> def local_1():
+    ...     local_0()
+    ...
+    >>> def local_2():
+    ...     local_1()
+    ...
+    >>> local_2()
+    Traceback (most recent call last):
+      File "...doctest.py", line ..., in __run
+        compileflags, 1) in test.globs
+      File "<doctest README.rst[24]>", line 1, in <module>
+        local_2()
+      File "<doctest README.rst[23]>", line 2, in local_2
+        local_1()
+      File "<doctest README.rst[22]>", line 2, in local_1
+        local_0()
+      File "<doctest README.rst[21]>", line 2, in local_0
+        reraise(*exc_info)
+      File "<doctest README.rst[11]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+It also supports more contrived scenarios
+-----------------------------------------
+
+Like tracebacks with syntax errors::
+
+    >>> from tblib import Traceback
+    >>> from examples import bad_syntax
+    >>> try:
+    ...     bad_syntax()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[58]>", line 1, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[57]>", line 2, in <module>
+        bad_syntax()
+      File "...tests...examples.py", line 18, in bad_syntax
+        import badsyntax
+      File "...tests...badsyntax.py", line 5
+        is very bad
+         ^
+    SyntaxError: invalid syntax
+
+Or other import failures::
+
+    >>> from examples import bad_module
+    >>> try:
+    ...     bad_module()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[61]>", line 1, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[60]>", line 2, in <module>
+        bad_module()
+      File "...tests...examples.py", line 23, in bad_module
+        import badmodule
+      File "...tests...badmodule.py", line 3, in <module>
+        raise Exception("boom!")
+    Exception: boom!
+
+Or a traceback that's caused by exceeding the recursion limit (here we're
+forcing the type and value to have consistency across platforms)::
+
+    >>> def f(): f()
+    >>> try:
+    ...    f()
+    ... except RuntimeError:
+    ...    et, ev, tb = sys.exc_info()
+    ...    tb = Traceback(tb)
+    ...
+    >>> reraise(RuntimeError, RuntimeError("maximum recursion depth exceeded"), tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      File "<doctest README.rst[32]>", line 1, in f
+        def f(): f()
+      ...
+    RuntimeError: maximum recursion depth exceeded
+
+Reference
+~~~~~~~~~
+
+tblib.Traceback
+---------------
+
+It is used by the ``pickling_support``. You can use it too if you want more flexibility::
+
+    >>> from tblib import Traceback
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[21]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[21]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+tblib.Traceback.to_dict
+```````````````````````
+
+You can use the ``to_dict`` method and the ``from_dict`` classmethod to
+convert a Traceback into and from a dictionary serializable by the stdlib
+json.JSONDecoder::
+
+    >>> import json
+    >>> from pprint import pprint
+    >>> try:
+    ...     inner_2()
+    ... except:
+    ...     et, ev, tb = sys.exc_info()
+    ...     tb = Traceback(tb)
+    ...     tb_dict = tb.to_dict()
+    ...     pprint(tb_dict)
+    {'tb_frame': {'f_code': {'co_filename': '<doctest README.rst[...]>',
+                             'co_name': '<module>'},
+                  'f_globals': {'__name__': '__main__'},
+                  'f_lineno': 5},
+     'tb_lineno': 2,
+     'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                         'co_name': 'inner_2'},
+                              'f_globals': {'__name__': '__main__'},
+                              'f_lineno': 2},
+                 'tb_lineno': 2,
+                 'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                                     'co_name': 'inner_1'},
+                                          'f_globals': {'__name__': '__main__'},
+                                          'f_lineno': 2},
+                             'tb_lineno': 2,
+                             'tb_next': {'tb_frame': {'f_code': {'co_filename': ...,
+                                                                 'co_name': 'inner_0'},
+                                                      'f_globals': {'__name__': '__main__'},
+                                                      'f_lineno': 2},
+                                         'tb_lineno': 2,
+                                         'tb_next': None}}}}
+
+tblib.Traceback.from_dict
+`````````````````````````
+
+Building on the previous example::
+
+    >>> tb_json = json.dumps(tb_dict)
+    >>> tb = Traceback.from_dict(json.loads(tb_json))
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[21]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "<doctest README.rst[21]>", line 2, in <module>
+        inner_2()
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+tblib.Traceback.from_string
+```````````````````````````
+
+::
+
+    >>> tb = Traceback.from_string("""
+    ... File "skipped.py", line 123, in func_123
+    ... Traceback (most recent call last):
+    ...   File "tests/examples.py", line 2, in func_a
+    ...     func_b()
+    ...   File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...   File "tests/examples.py", line 10, in func_c
+    ...     func_d()
+    ...   File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """)
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[42]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: fail
+
+
+If you use the ``strict=False`` option then parsing is a bit more lax::
+
+    >>> tb = Traceback.from_string("""
+    ... File "bogus.py", line 123, in bogus
+    ... Traceback (most recent call last):
+    ...  File "tests/examples.py", line 2, in func_a
+    ...   func_b()
+    ...    File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...    File "tests/examples.py", line 10, in func_c
+    ...   func_d()
+    ...  File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """, strict=False)
+    >>> reraise(et, ev, tb.as_traceback())
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[42]>", line 6, in <module>
+        reraise(et, ev, tb.as_traceback())
+      File "bogus.py", line 123, in bogus
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: fail
+
+tblib.decorators.return_error
+-----------------------------
+
+::
+
+    >>> from tblib.decorators import return_error
+    >>> inner_2r = return_error(inner_2)
+    >>> e = inner_2r()
+    >>> e
+    <tblib.decorators.Error object at ...>
+    >>> e.reraise()
+    Traceback (most recent call last):
+      ...
+      File "<doctest README.rst[26]>", line 1, in <module>
+        e.reraise()
+      File "...tblib...decorators.py", line 19, in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line 25, in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "<doctest README.rst[5]>", line 2, in inner_2
+        inner_1()
+      File "<doctest README.rst[4]>", line 2, in inner_1
+        inner_0()
+      File "<doctest README.rst[3]>", line 2, in inner_0
+        raise Exception('fail')
+    Exception: fail
+
+How's this useful? Imagine you're using multiprocessing like this::
+
+    # Note that Python 3.4 and later will show the remote traceback (but as a string sadly) so we skip testing this.
+    >>> import traceback
+    >>> from multiprocessing import Pool
+    >>> from examples import func_a
+    >>> pool = Pool()  # doctest: +SKIP
+    >>> try:  # doctest: +SKIP
+    ...     for i in pool.map(func_a, range(5)):
+    ...         print(i)
+    ... except:
+    ...     print(traceback.format_exc())
+    ...
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 2, in <module>
+        for i in pool.map(func_a, range(5)):
+      File "...multiprocessing...pool.py", line ..., in map
+        ...
+      File "...multiprocessing...pool.py", line ..., in get
+        ...
+    Exception: Guessing time !
+    <BLANKLINE>
+    >>> pool.terminate()  # doctest: +SKIP
+
+Not very useful is it? Let's sort this out::
+
+    >>> from tblib.decorators import apply_with_return_error, Error
+    >>> from itertools import repeat
+    >>> pool = Pool()
+    >>> try:
+    ...     for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
+    ...         if isinstance(i, Error):
+    ...             i.reraise()
+    ...         else:
+    ...             print(i)
+    ... except:
+    ...     print(traceback.format_exc())
+    ...
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 4, in <module>
+        i.reraise()
+      File "...tblib...decorators.py", line ..., in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line ..., in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "...tblib...decorators.py", line ..., in apply_with_return_error
+        return args[0](*args[1:])
+      File "...examples.py", line 2, in func_a
+        func_b()
+      File "...examples.py", line 6, in func_b
+        func_c()
+      File "...examples.py", line 10, in func_c
+        func_d()
+      File "...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: Guessing time !
+    <BLANKLINE>
+    >>> pool.terminate()
+
+Much better !
+
+What if we have a local call stack ?
+````````````````````````````````````
+
+::
+
+    >>> def local_0():
+    ...     pool = Pool()
+    ...     try:
+    ...         for i in pool.map(apply_with_return_error, zip(repeat(func_a), range(5))):
+    ...             if isinstance(i, Error):
+    ...                 i.reraise()
+    ...             else:
+    ...                 print(i)
+    ...     finally:
+    ...         pool.close()
+    ...
+    >>> def local_1():
+    ...     local_0()
+    ...
+    >>> def local_2():
+    ...     local_1()
+    ...
+    >>> try:
+    ...     local_2()
+    ... except:
+    ...     print(traceback.format_exc())
+    Traceback (most recent call last):
+      File "<doctest README.rst[...]>", line 2, in <module>
+        local_2()
+      File "<doctest README.rst[...]>", line 2, in local_2
+        local_1()
+      File "<doctest README.rst[...]>", line 2, in local_1
+        local_0()
+      File "<doctest README.rst[...]>", line 6, in local_0
+        i.reraise()
+      File "...tblib...decorators.py", line 20, in reraise
+        reraise(self.exc_type, self.exc_value, self.traceback)
+      File "...tblib...decorators.py", line 27, in return_exceptions_wrapper
+        return func(*args, **kwargs)
+      File "...tblib...decorators.py", line 47, in apply_with_return_error
+        return args[0](*args[1:])
+      File "...tests...examples.py", line 2, in func_a
+        func_b()
+      File "...tests...examples.py", line 6, in func_b
+        func_c()
+      File "...tests...examples.py", line 10, in func_c
+        func_d()
+      File "...tests...examples.py", line 14, in func_d
+        raise Exception("Guessing time !")
+    Exception: Guessing time !
+    <BLANKLINE>
+
+Other weird stuff
+`````````````````
+
+Clearing traceback works (Python 3.4 and up)::
+
+    >>> tb = Traceback.from_string("""
+    ... File "skipped.py", line 123, in func_123
+    ... Traceback (most recent call last):
+    ...   File "tests/examples.py", line 2, in func_a
+    ...     func_b()
+    ...   File "tests/examples.py", line 6, in func_b
+    ...     func_c()
+    ...   File "tests/examples.py", line 10, in func_c
+    ...     func_d()
+    ...   File "tests/examples.py", line 14, in func_d
+    ... Doesn't: matter
+    ... """)
+    >>> import traceback, sys
+    >>> if sys.version_info > (3, 4):
+    ...     traceback.clear_frames(tb)
+
+Credits
+=======
+
+* `mitsuhiko/jinja2 <https://github.com/mitsuhiko/jinja2>`_ for figuring a way to create traceback objects.
+
+
+Changelog
+=========
+
+2.0.0 (2023-06-22)
+~~~~~~~~~~~~~~~~~~
+
+* Removed support for legacy Pythons (2.7 and 3.6) and added Python 3.11 in the test grid.
+* Some cleanups and refactors (mostly from ruff).
+
+1.7.0 (2020-07-24)
+~~~~~~~~~~~~~~~~~~
+
+* Add more attributes to ``Frame`` and ``Code`` objects for pytest compatibility. Contributed by Ivanq in
+  `#58 <https://github.com/ionelmc/python-tblib/pull/58>`_.
+
+1.6.0 (2019-12-07)
+~~~~~~~~~~~~~~~~~~
+
+* When pickling an Exception, also pickle its traceback and the Exception chain
+  (``raise ... from ...``). Contributed by Guido Imperiale in
+  `#53 <https://github.com/ionelmc/python-tblib/issues/53>`_.
+
+1.5.0 (2019-10-23)
+~~~~~~~~~~~~~~~~~~
+
+* Added support for Python 3.8. Contributed by Victor Stinner in
+  `#42 <https://github.com/ionelmc/python-tblib/issues/42>`_.
+* Removed support for end of life Python 3.4.
+* Few CI improvements and fixes.
+
+1.4.0 (2019-05-02)
+~~~~~~~~~~~~~~~~~~
+
+* Removed support for end of life Python 3.3.
+* Fixed tests for Python 3.7. Contributed by Elliott Sales de Andrade in
+  `#36 <https://github.com/ionelmc/python-tblib/issues/36>`_.
+* Fixed compatibility issue with Twised (``twisted.python.failure.Failure`` expected a ``co_code`` attribute).
+
+1.3.2 (2017-04-09)
+~~~~~~~~~~~~~~~~~~
+
+* Add support for PyPy3.5-5.7.1-beta. Previously ``AttributeError:
+  'Frame' object has no attribute 'clear'``  could be raised. See PyPy
+  issue `#2532 <https://foss.heptapod.net/pypy/pypy/-/issues/2532>`_.
+
+1.3.1 (2017-03-27)
+~~~~~~~~~~~~~~~~~~
+
+* Fixed handling for tracebacks due to exceeding the recursion limit.
+  Fixes `#15 <https://github.com/ionelmc/python-tblib/issues/15>`_.
+
+1.3.0 (2016-03-08)
+~~~~~~~~~~~~~~~~~~
+
+* Added ``Traceback.from_string``.
+
+1.2.0 (2015-12-18)
+~~~~~~~~~~~~~~~~~~
+
+* Fixed handling for tracebacks from generators and other internal improvements
+  and optimizations. Contributed by DRayX in `#10 <https://github.com/ionelmc/python-tblib/issues/10>`_
+  and `#11 <https://github.com/ionelmc/python-tblib/pull/11>`_.
+
+1.1.0 (2015-07-27)
+~~~~~~~~~~~~~~~~~~
+
+* Added support for Python 2.6. Contributed by Arcadiy Ivanov in
+  `#8 <https://github.com/ionelmc/python-tblib/pull/8>`_.
+
+1.0.0 (2015-03-30)
+~~~~~~~~~~~~~~~~~~
+
+* Added ``to_dict`` method and ``from_dict`` classmethod on Tracebacks.
+  Contributed by beckjake in `#5 <https://github.com/ionelmc/python-tblib/pull/5>`_.
```

### Comparing `tblib-1.7.0/src/tblib.egg-info/SOURCES.txt` & `tblib-2.0.0/src/tblib.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-.appveyor.yml
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
-.travis.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
+pytest.ini
 setup.py
 tox.ini
-ci/appveyor-download.py
-ci/appveyor-with-compiler.cmd
+.github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
-ci/templates/.appveyor.yml
-ci/templates/.travis.yml
+ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 src/tblib/__init__.py
-src/tblib/cpython.py
 src/tblib/decorators.py
 src/tblib/pickling_support.py
 src/tblib.egg-info/PKG-INFO
 src/tblib.egg-info/SOURCES.txt
 src/tblib.egg-info/dependency_links.txt
 src/tblib.egg-info/not-zip-safe
 src/tblib.egg-info/top_level.txt
```

### Comparing `tblib-1.7.0/tests/test_pickle_exception.py` & `tblib-2.0.0/tests/test_pickle_exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,60 +14,58 @@
 has_python3 = sys.version_info.major >= 3
 
 
 @pytest.fixture
 def clear_dispatch_table():
     bak = copyreg.dispatch_table.copy()
     copyreg.dispatch_table.clear()
-    yield
+    yield None
     copyreg.dispatch_table.clear()
     copyreg.dispatch_table.update(bak)
 
 
 class CustomError(Exception):
     pass
 
 
-@pytest.mark.parametrize(
-    "protocol", [None] + list(range(1, pickle.HIGHEST_PROTOCOL + 1))
-)
-@pytest.mark.parametrize("how", ["global", "instance", "class"])
+@pytest.mark.parametrize('protocol', [None, *list(range(1, pickle.HIGHEST_PROTOCOL + 1))])
+@pytest.mark.parametrize('how', ['global', 'instance', 'class'])
 def test_install(clear_dispatch_table, how, protocol):
-    if how == "global":
+    if how == 'global':
         tblib.pickling_support.install()
-    elif how == "class":
+    elif how == 'class':
         tblib.pickling_support.install(CustomError, ZeroDivisionError)
 
     try:
         try:
-            1 / 0
+            1 / 0  # noqa: B018
         except Exception as e:
             # Python 3 only syntax
             # raise CustomError("foo") from e
-            new_e = CustomError("foo")
+            new_e = CustomError('foo')
             if has_python3:
                 new_e.__cause__ = e
             raise new_e
     except Exception as e:
         exc = e
     else:
-        assert False
+        raise AssertionError
 
     # Populate Exception.__dict__, which is used in some cases
     exc.x = 1
     if has_python3:
         exc.__cause__.x = 2
 
-    if how == "instance":
+    if how == 'instance':
         tblib.pickling_support.install(exc)
     if protocol:
         exc = pickle.loads(pickle.dumps(exc, protocol=protocol))
 
     assert isinstance(exc, CustomError)
-    assert exc.args == ("foo",)
+    assert exc.args == ('foo',)
     assert exc.x == 1
     if has_python3:
         assert exc.__traceback__ is not None
         assert isinstance(exc.__cause__, ZeroDivisionError)
         assert exc.__cause__.__traceback__ is not None
         assert exc.__cause__.x == 2
         assert exc.__cause__.__cause__ is None
@@ -76,23 +74,23 @@
 @tblib.pickling_support.install
 class RegisteredError(Exception):
     pass
 
 
 def test_install_decorator():
     with pytest.raises(RegisteredError) as ewrap:
-        raise RegisteredError("foo")
+        raise RegisteredError('foo')
     exc = ewrap.value
     exc.x = 1
     exc = pickle.loads(pickle.dumps(exc))
 
     assert isinstance(exc, RegisteredError)
-    assert exc.args == ("foo",)
+    assert exc.args == ('foo',)
     assert exc.x == 1
     if has_python3:
         assert exc.__traceback__ is not None
 
 
-@pytest.mark.skipif(sys.version_info[0] < 3, reason="No checks done in Python 2")
+@pytest.mark.skipif(sys.version_info[0] < 3, reason='No checks done in Python 2')
 def test_install_typeerror():
     with pytest.raises(TypeError):
-        tblib.pickling_support.install("foo")
+        tblib.pickling_support.install('foo')
```

### Comparing `tblib-1.7.0/tests/test_tblib.py` & `tblib-2.0.0/tests/test_tblib.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import traceback
 
 from tblib import Traceback
 from tblib import pickling_support
 
 pickling_support.install()
 
-pytest_plugins = 'pytester',
+pytest_plugins = ('pytester',)
 
 
 def test_parse_traceback():
     tb1 = Traceback.from_string(
         """
 Traceback (most recent call last):
   File "file1", line 123, in <module>
@@ -27,118 +27,125 @@
         '  File "file1", line 123, in <module>\n',
         '  File "file2", line 234, in ???\n',
         '  File "file3", line 345, in function3\n',
     ]
     tb2 = Traceback(pytb)
 
     expected_dict = {
-        "tb_frame": {
-            "f_code": {"co_filename": "file1", "co_name": "<module>"},
-            "f_globals": {"__file__": "file1", "__name__": "?"},
-            "f_lineno": 123,
+        'tb_frame': {
+            'f_code': {'co_filename': 'file1', 'co_name': '<module>'},
+            'f_globals': {'__file__': 'file1', '__name__': '?'},
+            'f_lineno': 123,
         },
-        "tb_lineno": 123,
-        "tb_next": {
-            "tb_frame": {
-                "f_code": {"co_filename": "file2", "co_name": "???"},
-                "f_globals": {"__file__": "file2", "__name__": "?"},
-                "f_lineno": 234,
+        'tb_lineno': 123,
+        'tb_next': {
+            'tb_frame': {
+                'f_code': {'co_filename': 'file2', 'co_name': '???'},
+                'f_globals': {'__file__': 'file2', '__name__': '?'},
+                'f_lineno': 234,
             },
-            "tb_lineno": 234,
-            "tb_next": {
-                "tb_frame": {
-                    "f_code": {"co_filename": "file3", "co_name": "function3"},
-                    "f_globals": {"__file__": "file3", "__name__": "?"},
-                    "f_lineno": 345,
+            'tb_lineno': 234,
+            'tb_next': {
+                'tb_frame': {
+                    'f_code': {'co_filename': 'file3', 'co_name': 'function3'},
+                    'f_globals': {'__file__': 'file3', '__name__': '?'},
+                    'f_lineno': 345,
                 },
-                "tb_lineno": 345,
-                "tb_next": None,
+                'tb_lineno': 345,
+                'tb_next': None,
             },
         },
     }
     tb3 = Traceback.from_dict(expected_dict)
     tb4 = pickle.loads(pickle.dumps(tb3))
     assert tb4.as_dict() == tb3.as_dict() == tb2.as_dict() == tb1.as_dict() == expected_dict
 
 
 def test_pytest_integration(testdir):
-    test = testdir.makepyfile("""
-import six
-
+    test = testdir.makepyfile(
+        """
 from tblib import Traceback
 
 def test_raise():
     tb1 = Traceback.from_string('''
 Traceback (most recent call last):
   File "file1", line 123, in <module>
     code1
   File "file2", line 234, in ???
     code2
   File "file3", line 345, in function3
   File "file4", line 456, in ""
 ''')
     pytb = tb1.as_traceback()
-    six.reraise(RuntimeError, RuntimeError(), pytb)
-""")
+    raise RuntimeError().with_traceback(pytb)
+"""
+    )
 
     # mode(auto / long / short / line / native / no).
 
     result = testdir.runpytest_subprocess('--tb=long', '-vv', test)
-    result.stdout.fnmatch_lines([
-        "_ _ _ _ _ _ _ _ *",
-        "",
-        ">   [?][?][?]",
-        "",
-        "file1:123:*",
-        "_ _ _ _ _ _ _ _ *",
-        "",
-        ">   [?][?][?]",
-        "",
-        "file2:234:*",
-        "_ _ _ _ _ _ _ _ *",
-        "",
-        ">   [?][?][?]",
-        "",
-        "file3:345:*",
-        "_ _ _ _ _ _ _ _ *",
-        "",
-        ">   [?][?][?]",
-        "E   RuntimeError",
-        "",
-        "file4:456: RuntimeError",
-        "===*=== 1 failed in * ===*===",
-    ])
+    result.stdout.fnmatch_lines(
+        [
+            '_ _ _ _ _ _ _ _ *',
+            '',
+            '>   [?][?][?]',
+            '',
+            'file1:123:*',
+            '_ _ _ _ _ _ _ _ *',
+            '',
+            '>   [?][?][?]',
+            '',
+            'file2:234:*',
+            '_ _ _ _ _ _ _ _ *',
+            '',
+            '>   [?][?][?]',
+            '',
+            'file3:345:*',
+            '_ _ _ _ _ _ _ _ *',
+            '',
+            '>   [?][?][?]',
+            'E   RuntimeError',
+            '',
+            'file4:456: RuntimeError',
+            '===*=== 1 failed in * ===*===',
+        ]
+    )
 
     result = testdir.runpytest_subprocess('--tb=short', '-vv', test)
-    result.stdout.fnmatch_lines([
-        'test_pytest_integration.py:*: in test_raise',
-        '    six.reraise(RuntimeError, RuntimeError(), pytb)',
-        'file1:123: in <module>',
-        '    ???',
-        'file2:234: in ???',
-        '    ???',
-        'file3:345: in function3',
-        '    ???',
-        'file4:456: in ""',
-        '    ???',
-        'E   RuntimeError',
-    ])
+    result.stdout.fnmatch_lines(
+        [
+            'test_pytest_integration.py:*: in test_raise',
+            '    raise RuntimeError().with_traceback(pytb)',
+            'file1:123: in <module>',
+            '    ???',
+            'file2:234: in ???',
+            '    ???',
+            'file3:345: in function3',
+            '    ???',
+            'file4:456: in ""',
+            '    ???',
+            'E   RuntimeError',
+        ]
+    )
 
     result = testdir.runpytest_subprocess('--tb=line', '-vv', test)
-    result.stdout.fnmatch_lines([
-        "===*=== FAILURES ===*===",
-        "file4:456: RuntimeError",
-        "===*=== 1 failed in * ===*===",
-    ])
+    result.stdout.fnmatch_lines(
+        [
+            '===*=== FAILURES ===*===',
+            'file4:456: RuntimeError',
+            '===*=== 1 failed in * ===*===',
+        ]
+    )
 
     result = testdir.runpytest_subprocess('--tb=native', '-vv', test)
-    result.stdout.fnmatch_lines([
-        'Traceback (most recent call last):',
-        '  File "*test_pytest_integration.py", line *, in test_raise',
-        '    six.reraise(RuntimeError, RuntimeError(), pytb)',
-        '  File "file1", line 123, in <module>',
-        '  File "file2", line 234, in ???',
-        '  File "file3", line 345, in function3',
-        '  File "file4", line 456, in ""',
-        'RuntimeError',
-
-    ])
+    result.stdout.fnmatch_lines(
+        [
+            'Traceback (most recent call last):',
+            '  File "*test_pytest_integration.py", line *, in test_raise',
+            '    raise RuntimeError().with_traceback(pytb)',
+            '  File "file1", line 123, in <module>',
+            '  File "file2", line 234, in ???',
+            '  File "file3", line 345, in function3',
+            '  File "file4", line 456, in ""',
+            'RuntimeError',
+        ]
+    )
```

### Comparing `tblib-1.7.0/tox.ini` & `tblib-2.0.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,78 @@
 [testenv:bootstrap]
 deps =
     jinja2
-    matrix
     tox
 skip_install = true
 commands =
     python ci/bootstrap.py --no-env
 passenv =
     *
-; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
+; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py27,py35,py36,py37,py38,pypy,pypy3},
+    {py37,py38,py39,py310,py311,pypy37,pypy38,pypy39},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    pypy: {env:TOXPYTHON:pypy}
-    pypy3: {env:TOXPYTHON:pypy3}
-    py27: {env:TOXPYTHON:python2.7}
-    py35: {env:TOXPYTHON:python3.5}
-    py36: {env:TOXPYTHON:python3.6}
+    pypy37: {env:TOXPYTHON:pypy3.7}
+    pypy38: {env:TOXPYTHON:pypy3.8}
+    pypy39: {env:TOXPYTHON:pypy3.9}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
-    {bootstrap,clean,check,report,codecov,docs}: {env:TOXPYTHON:python3}
+    py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
+    py311: {env:TOXPYTHON:python3.11}
+    {bootstrap,clean,check,report,docs,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
 deps =
     pytest
-    pytest-travis-fold
     pytest-cov
-    pytest-clarity
-    six
-    py{27,35,36,37,38,py,py3}: twisted
 commands =
-    {posargs:py.test --cov=tblib --cov-report=term-missing -vv tests README.rst}
+    {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
-    flake8
+    pre-commit
     readme-renderer
     pygments
     isort
 skip_install = true
 commands =
     python setup.py check --strict --metadata --restructuredtext
-    check-manifest {toxinidir}
-    flake8 src tests setup.py
-    isort --verbose --check-only --diff --recursive src tests setup.py
+    check-manifest .
+    pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
 usedevelop = true
 deps =
     -r{toxinidir}/docs/requirements.txt
 commands =
     sphinx-build {posargs:-E} -b html docs dist/docs
     sphinx-build -b linkcheck docs dist/docs
 
-[testenv:codecov]
-deps =
-    codecov
-skip_install = true
-commands =
-    codecov []
-
 [testenv:report]
-deps = coverage
+deps =
+    coverage
 skip_install = true
 commands =
     coverage report
     coverage html
 
 [testenv:clean]
 commands = coverage erase
 skip_install = true
-deps = coverage
+deps =
+    coverage
```

