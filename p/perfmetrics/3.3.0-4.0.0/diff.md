# Comparing `tmp/perfmetrics-3.3.0.tar.gz` & `tmp/perfmetrics-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfmetrics-3.3.0.tar", last modified: Sun Sep 25 11:35:18 2022, max compression
+gzip compressed data, was "perfmetrics-4.0.0.tar", last modified: Thu Jun 22 20:39:28 2023, max compression
```

## Comparing `perfmetrics-3.3.0.tar` & `perfmetrics-4.0.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.765002 perfmetrics-3.3.0/
--rw-r--r--   0 jmadden    (501) staff       (20)      929 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/.coveragerc
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.747025 perfmetrics-3.3.0/.github/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.752120 perfmetrics-3.3.0/.github/workflows/
--rw-r--r--   0 jmadden    (501) staff       (20)    12402 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/.github/workflows/tests.yml
--rw-r--r--   0 jmadden    (501) staff       (20)      205 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/.gitignore
--rw-r--r--   0 jmadden    (501) staff       (20)     4364 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/.pylintrc
--rw-r--r--   0 jmadden    (501) staff       (20)     3917 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     1791 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/LICENSE.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      622 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)    12023 2022-09-25 11:35:18.765215 perfmetrics-3.3.0/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     6594 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     5642 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/appveyor.yml
--rw-r--r--   0 jmadden    (501) staff       (20)        8 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.753458 perfmetrics-3.3.0/docs/
--rw-r--r--   0 jmadden    (501) staff       (20)     1288 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/docs/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       28 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/docs/changelog.rst
--rw-r--r--   0 jmadden    (501) staff       (20)    10582 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)      230 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     3273 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/docs/testing.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     1245 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/pyproject.toml
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.754101 perfmetrics-3.3.0/scripts/
--rw-r--r--   0 jmadden    (501) staff       (20)     7195 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/scripts/install.ps1
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.754363 perfmetrics-3.3.0/scripts/releases/
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1352 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/scripts/releases/make-manylinux
--rw-r--r--   0 jmadden    (501) staff       (20)     3366 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/scripts/run_with_env.cmd
--rw-r--r--   0 jmadden    (501) staff       (20)      135 2022-09-25 11:35:18.765801 perfmetrics-3.3.0/setup.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)     6203 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.747786 perfmetrics-3.3.0/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.758395 perfmetrics-3.3.0/src/perfmetrics/
--rw-r--r--   0 jmadden    (501) staff       (20)     1377 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)      965 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/_metric.pxd
--rw-r--r--   0 jmadden    (501) staff       (20)     1772 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/_util.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1986 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/clientstack.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4200 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/interfaces.py
--rw-r--r--   0 jmadden    (501) staff       (20)   656030 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics/metric.c
--rw-r--r--   0 jmadden    (501) staff       (20)     9463 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/metric.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1029 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/pyramid.py
--rw-r--r--   0 jmadden    (501) staff       (20)     6584 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/statsd.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.761333 perfmetrics-3.3.0/src/perfmetrics/testing/
--rw-r--r--   0 jmadden    (501) staff       (20)      661 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3213 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/client.py
--rw-r--r--   0 jmadden    (501) staff       (20)     5493 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/matchers.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3448 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/observation.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.762410 perfmetrics-3.3.0/src/perfmetrics/testing/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)      134 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4112 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_client.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3300 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_matchers.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3197 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_observation.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.764472 perfmetrics-3.3.0/src/perfmetrics/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)     5942 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2858 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/bench_metric.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.764752 perfmetrics-3.3.0/src/perfmetrics/tests/benchmarks/
--rw-r--r--   0 jmadden    (501) staff       (20)      482 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/benchmarks/spraytest.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1255 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_clientstack.py
--rw-r--r--   0 jmadden    (501) staff       (20)    14515 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_metric.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2907 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_perfmetrics.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2117 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_pyramid.py
--rw-r--r--   0 jmadden    (501) staff       (20)     8075 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_statsd.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1574 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/tests/test_wsgi.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1074 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/src/perfmetrics/wsgi.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2022-09-25 11:35:18.760171 perfmetrics-3.3.0/src/perfmetrics.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)    12023 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     1555 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)       64 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/entry_points.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      193 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)       12 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2022-09-25 11:35:18.000000 perfmetrics-3.3.0/src/perfmetrics.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)      575 2022-09-25 11:35:16.000000 perfmetrics-3.3.0/tox.ini
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.213890 perfmetrics-4.0.0/
+-rw-r--r--   0 jmadden    (501) staff       (20)      929 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/.coveragerc
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.206610 perfmetrics-4.0.0/.github/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.208640 perfmetrics-4.0.0/.github/workflows/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7267 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      205 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/.gitignore
+-rw-r--r--   0 jmadden    (501) staff       (20)     4364 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)     4066 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     1791 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/LICENSE.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      622 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)    12077 2023-06-22 20:39:28.213971 perfmetrics-4.0.0/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     6594 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     5781 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/appveyor.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)        8 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/doc-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.209187 perfmetrics-4.0.0/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1288 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       28 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/docs/changelog.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)    10582 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      230 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     3273 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/docs/testing.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     1245 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/pyproject.toml
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.209395 perfmetrics-4.0.0/scripts/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7195 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/scripts/install.ps1
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.209710 perfmetrics-4.0.0/scripts/releases/
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     1234 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/scripts/releases/geventrel.sh
+-rwxr-xr-x   0 jmadden    (501) staff       (20)      637 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/scripts/releases/geventreleases.sh
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     1392 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/scripts/releases/make-manylinux
+-rw-r--r--   0 jmadden    (501) staff       (20)     3366 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/scripts/run_with_env.cmd
+-rw-r--r--   0 jmadden    (501) staff       (20)      135 2023-06-22 20:39:28.214221 perfmetrics-4.0.0/setup.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)     6259 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.206954 perfmetrics-4.0.0/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.211248 perfmetrics-4.0.0/src/perfmetrics/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1377 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      965 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/_metric.pxd
+-rw-r--r--   0 jmadden    (501) staff       (20)     1741 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/_util.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1986 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/clientstack.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4200 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/interfaces.py
+-rw-r--r--   0 jmadden    (501) staff       (20)   649394 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/metric.c
+-rw-r--r--   0 jmadden    (501) staff       (20)     9463 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/metric.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1029 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/pyramid.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     6584 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/statsd.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.212442 perfmetrics-4.0.0/src/perfmetrics/testing/
+-rw-r--r--   0 jmadden    (501) staff       (20)      661 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3213 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/client.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     5493 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/matchers.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3448 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/observation.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.212854 perfmetrics-4.0.0/src/perfmetrics/testing/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)      134 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4112 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_client.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3300 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_matchers.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3197 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_observation.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.213679 perfmetrics-4.0.0/src/perfmetrics/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)     5924 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2858 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/bench_metric.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.213785 perfmetrics-4.0.0/src/perfmetrics/tests/benchmarks/
+-rw-r--r--   0 jmadden    (501) staff       (20)      414 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/benchmarks/spraytest.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1255 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_clientstack.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    14515 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_metric.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2907 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_perfmetrics.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2117 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_pyramid.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     8075 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_statsd.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1574 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/tests/test_wsgi.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1074 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/src/perfmetrics/wsgi.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-22 20:39:28.211989 perfmetrics-4.0.0/src/perfmetrics.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)    12077 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     1620 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)       64 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/entry_points.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      305 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)       12 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-06-22 20:39:28.000000 perfmetrics-4.0.0/src/perfmetrics.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)      554 2023-06-22 20:39:27.000000 perfmetrics-4.0.0/tox.ini
```

### Comparing `perfmetrics-3.3.0/.coveragerc` & `perfmetrics-4.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/.pylintrc` & `perfmetrics-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/CHANGES.rst` & `perfmetrics-4.0.0/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  CHANGES
 =========
 
+4.0.0 (2023-06-22)
+==================
+
+- Drop support for obsolete Python versions, including Python 2.7 and
+  3.6.
+- Add support for Python 3.12.
+
+
 3.3.0 (2022-09-25)
 ==================
 
 - Stop accidentally building manylinux wheels with unsafe math
   optimizations.
 - Add support for Python 3.11.
```

### Comparing `perfmetrics-3.3.0/LICENSE.txt` & `perfmetrics-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/MANIFEST.in` & `perfmetrics-4.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/PKG-INFO` & `perfmetrics-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: perfmetrics
-Version: 3.3.0
+Version: 4.0.0
 Summary: Send performance metrics about Python code to Statsd
 Home-page: https://github.com/zodb/perfmetrics
 Author: Shane Hathaway
 Author-email: shane@hathawaymix.org
 Maintainer: Jason Madden
 Maintainer-email: jason@nextthought.com
 License: BSD-derived (http://www.repoze.org/LICENSE.txt)
 Project-URL: Bug Tracker, https://github.com/zodb/perfmetrics/issues
 Project-URL: Source Code, https://github.com/zodb/perfmetrics/
 Project-URL: Documentation, https://perfmetrics.readthedocs.io
 Keywords: statsd metrics performance monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: Repoze Public License
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =============
  perfmetrics
 =============
@@ -200,14 +199,22 @@
 You can turn on that option for each graph.
 
 
 =========
  CHANGES
 =========
 
+4.0.0 (2023-06-22)
+==================
+
+- Drop support for obsolete Python versions, including Python 2.7 and
+  3.6.
+- Add support for Python 3.12.
+
+
 3.3.0 (2022-09-25)
 ==================
 
 - Stop accidentally building manylinux wheels with unsafe math
   optimizations.
 - Add support for Python 3.11.
```

### Comparing `perfmetrics-3.3.0/README.rst` & `perfmetrics-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/appveyor.yml` & `perfmetrics-4.0.0/appveyor.yml`

 * *Files 6% similar despite different names*

```diff
@@ -32,52 +32,54 @@
     # Upload settings for twine.
     TWINE_USERNAME: __token__
     TWINE_PASSWORD:
       secure: uXZ6Juhz2hElaTsaJ2HnetZqz0mmNO3phE2IV3Am7hgfOAbaM4x3IeNSS7bMWL27TMGsOndOrKNgQTodirUt+vLZzZ+NYKjMImuM04P68BfIGDeZlA8ynYWG0vtjpqUTfrbhppyLuypHmzusV7+cnlSq4uaE3BtZ+bSwUZUYaeEQRAnCivzLki318kzOCLUUjDuyPSgyTdV+Z4GXOtUzGInvsbiU7k+9PbpE10915afTg82GUHHYn9BC5laBvxI1A07HX/JJZ6QjwS9+KjmEtw==
 
 
   matrix:
-    # Pre-installed Python versions, which Appveyor may upgrade to
-    # a later point release.
+    # http://www.appveyor.com/docs/installed-software#python
+
+    # Fully supported 64-bit versions, with testing. This should be
+    # all the current (non EOL) versions.
+    - PYTHON: "C:\\Python312-x64"
+      PYTHON_VERSION: "3.12.0b3"
+      PYTHON_ARCH: "64"
+      PYTHON_EXE: python
+      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+
+    - PYTHON: "C:\\Python311-x64"
+      PYTHON_VERSION: "3.11.0"
+      PYTHON_ARCH: "64"
+      PYTHON_EXE: python
+      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
 
-    # 64-bit
     - PYTHON: "C:\\Python310-x64"
       PYTHON_VERSION: "3.10.0"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
 
     - PYTHON: "C:\\Python39-x64"
       PYTHON_VERSION: "3.9.x"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
-    - PYTHON: "C:\\Python27-x64"
-      PYTHON_VERSION: "2.7.x" # currently 2.7.13
-      PYTHON_ARCH: "64"
-      PYTHON_EXE: python
-
     - PYTHON: "C:\\Python38-x64"
       PYTHON_VERSION: "3.8.x"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
     - PYTHON: "C:\\Python37-x64"
       PYTHON_VERSION: "3.7.x"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
-    - PYTHON: "C:\\Python36-x64"
-      PYTHON_VERSION: "3.6.x" # currently 3.6.8
-      PYTHON_ARCH: "64"
-      PYTHON_EXE: python
-
     # 32-bit, wheel only (no testing)
     - PYTHON: "C:\\Python39"
       PYTHON_VERSION: "3.9.x"
       PYTHON_ARCH: "32"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
```

### Comparing `perfmetrics-3.3.0/docs/api.rst` & `perfmetrics-4.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/docs/conf.py` & `perfmetrics-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/docs/testing.rst` & `perfmetrics-4.0.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/pyproject.toml` & `perfmetrics-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
      # and adds the 3str mode for transition to Python 3. 0.29.14+ is
      # required for Python 3.8. 3.0a2 introduced a change that prevented
      # us from compiling (https://github.com/gevent/gevent/issues/1599)
      # but once that was fixed, 3.0a4 led to all of our leak tests
      # failing in Python 2 (https://travis-ci.org/github/gevent/gevent/jobs/683782800);
      # This was fixed in 3.0a5 (https://github.com/cython/cython/issues/3578)
      # 3.0a6 fixes an issue cythonizing source on 32-bit platforms
-     "Cython >= 3.0a9; platform_python_implementation == 'CPython'",
+     "Cython >= 3.0b3; platform_python_implementation == 'CPython'",
 ]
```

### Comparing `perfmetrics-3.3.0/scripts/install.ps1` & `perfmetrics-4.0.0/scripts/install.ps1`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/scripts/releases/make-manylinux` & `perfmetrics-4.0.0/scripts/releases/make-manylinux`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 # Don't get warnings about Python 2 support being deprecated. We
 # know. The env var works for pip 20.
 export PIP_NO_PYTHON_VERSION_WARNING=1
 export PIP_NO_WARN_SCRIPT_LOCATION=1
 
 # Build configuration.
-export CFLAGS="-pipe -O3"
-export CXXFLAGS="-pipe -O3"
+export CFLAGS="-pipe -O3 -DNDEBUG"
+export CXXFLAGS="-pipe -O3 -DNDEBUG"
 
 if [ -d /io -a -d /opt/python ]; then
     # Running inside docker
     cd /io
     rm -rf wheelhouse
     mkdir wheelhouse
-    for variant in `ls -d /opt/python/cp*`; do
+    for variant in `ls -d /opt/python/cp{37,38,39,310,311,312}*`; do
         echo "Building $variant"
         mkdir /tmp/build
         cd /tmp/build
         git clone /io io
         cd io
         $variant/bin/pip install -U pip
-        $variant/bin/pip install -U 'cython>=3.0a9' setuptools
+        $variant/bin/pip install -U 'cython>=3.0b3' setuptools
         PATH=$variant/bin:$PATH $variant/bin/python setup.py bdist_wheel
         auditwheel show dist/*.whl
         auditwheel repair dist/*.whl
         cp wheelhouse/*.whl /io/wheelhouse
         cd /io
         rm -rf /tmp/build
     done
```

### Comparing `perfmetrics-3.3.0/scripts/run_with_env.cmd` & `perfmetrics-4.0.0/scripts/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/setup.py` & `perfmetrics-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 import sys
 
 from setuptools import setup
 from setuptools import find_packages
 from setuptools import Extension
 
 PYPY = hasattr(sys, 'pypy_version_info')
+PY312 = sys.version_info[:2] == (3, 12)
 
 def read(fname, here=os.path.dirname(__file__)):
-    with open(os.path.join(here, fname)) as f:
+    with open(os.path.join(here, fname), encoding='utf-8') as f:
         return f.read()
 
 README = read('README.rst')
 CHANGES = read('CHANGES.rst')
 
 tests_require = [
     'zope.testrunner',
-    # nti.testing > ZODB > zodbpickle.
-    # But zodbpickle 2.1.0 doesn't build on 3.10.
-    # Still waiting on 2.2 (https://github.com/zopefoundation/zodbpickle/pull/61)
-    'nti.testing; python_version < "3.10"',
+    # nti.testing > ZODB > persistent -> cffi
+    # But cffi won't build on apple silicon on 3.12.
+    # Can't get persistent to build on PyPy 3.9 either.
+    'nti.testing; (python_version != "3.12" and platform_machine != "arm64" and platform_system != "Darwin") and platform_python_implementation != "PyPy"',
     # transitive dep of nti.testing, which we don't always have, but need
     # for our emulation
     'zope.schema',
     'pyhamcrest >= 1.10',
     'pyperf',
 ]
 
@@ -75,15 +76,15 @@
     def _c(m):
         return _source(m, 'c')
     # Each module should list the python name of the
     # modules it cimports from as deps. We'll generate the rest.
     # (Not that this actually appears to do anything right now.)
 
     for mod_name, deps in (
-            ('metric', ()),
+        ('metric', ()),
     ):
         deps = ([_py_source(mod) for mod in deps]
                 + [_pxd(mod) for mod in deps]
                 + [_c(mod) for mod in deps])
 
         source = _py_source(mod_name)
         # 'foo.bar' -> 'foo._bar'
@@ -120,36 +121,35 @@
         # before doing any updates.
         import traceback
         traceback.print_exc()
         ext_modules = _dummy_cythonize(ext_modules)
 
 setup(
     name='perfmetrics',
-    version='3.3.0',
+    version='4.0.0',
     author='Shane Hathaway',
     author_email='shane@hathawaymix.org',
     maintainer='Jason Madden',
     maintainer_email='jason@nextthought.com',
     description='Send performance metrics about Python code to Statsd',
     keywords="statsd metrics performance monitoring",
     long_description=README + '\n\n' + CHANGES,
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
+    python_requires=">=3.7",
     # Get strings from https://pypi.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "License :: Repoze Public License",
         "Topic :: System :: Monitoring",
     ],
     url="https://github.com/zodb/perfmetrics",
     project_urls={
```

### Comparing `perfmetrics-3.3.0/src/perfmetrics/__init__.py` & `perfmetrics-4.0.0/src/perfmetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/_metric.pxd` & `perfmetrics-4.0.0/src/perfmetrics/_metric.pxd`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/_util.py` & `perfmetrics-4.0.0/src/perfmetrics/_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import os
 import sys
 
-PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] >= 3
 PYPY = hasattr(sys, 'pypy_version_info')
 WIN = sys.platform.startswith("win")
 LINUX = sys.platform.startswith('linux')
 OSX = sys.platform == 'darwin'
```

### Comparing `perfmetrics-3.3.0/src/perfmetrics/clientstack.py` & `perfmetrics-4.0.0/src/perfmetrics/clientstack.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/interfaces.py` & `perfmetrics-4.0.0/src/perfmetrics/interfaces.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/metric.c` & `perfmetrics-4.0.0/src/perfmetrics/metric.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0a11 */
+/* Generated by Cython 3.0.0b3 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "CYTHON_TRACE",
@@ -33,18 +33,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0a11"
+#define CYTHON_ABI "3_0_0b3"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000AB
+#define CYTHON_HEX_VERSION 0x030000B3
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -170,26 +170,30 @@
   #undef CYTHON_METH_FASTCALL
   #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
   #ifndef CYTHON_PEP487_INIT_SUBCLASS
     #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
   #endif
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 1
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
@@ -335,15 +339,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_GIL
-    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000)
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
   #endif
   #ifndef CYTHON_METH_FASTCALL
     #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
@@ -365,15 +369,15 @@
   #elif !defined(CYTHON_USE_TP_FINALIZE)
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #if PY_VERSION_HEX < 0x030600B1
     #undef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS 0
   #elif !defined(CYTHON_USE_DICT_VERSIONS)
-    #define CYTHON_USE_DICT_VERSIONS 1
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
@@ -413,14 +417,25 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
@@ -473,37 +488,57 @@
         #endif
     #endif
 #else
     #include <stdint.h>
     typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -511,17 +546,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -530,18 +562,18 @@
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
     static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
         if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
@@ -559,39 +591,31 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -637,14 +661,20 @@
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
@@ -838,15 +868,15 @@
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
 #elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #if PY_VERSION_HEX >= 0x030C0000
@@ -875,15 +905,15 @@
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
@@ -958,25 +988,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -1030,15 +1065,24 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
@@ -1134,14 +1178,15 @@
 static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
 {
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
 #endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -1159,14 +1204,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -1247,20 +1338,14 @@
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
 #if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
 #endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
@@ -1506,31 +1591,38 @@
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1689,15 +1781,15 @@
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
@@ -1879,17 +1971,14 @@
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_CyFunctionType = 0;
-#endif
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
 #define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
@@ -1932,15 +2021,15 @@
 
 /* ValidateBasesTuple.proto */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
 /* PyType_Ready.proto */
-static CYTHON_UNUSED int __Pyx_PyType_Ready(PyTypeObject *t);
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
@@ -1967,14 +2056,17 @@
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
@@ -1996,26 +2088,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -2086,15 +2178,15 @@
 #endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* FormatTypeName.proto */
@@ -2126,48 +2218,34 @@
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
-#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_Occurred(), err1, err2)
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrExport.proto */
 static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig);
 
 /* InitStrings.proto */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str);
-#else
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
-#endif
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_f_11perfmetrics_7_metric_19_AbstractMetricImpl__compute_stat(CYTHON_UNUSED struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto*/
 static PyObject *__pyx_f_11perfmetrics_7_metric_20_GivenStatMetricImpl__compute_stat(struct __pyx_obj_11perfmetrics_7_metric__GivenStatMetricImpl *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto*/
 static PyObject *__pyx_f_11perfmetrics_7_metric_17_MethodMetricImpl__compute_stat(struct __pyx_obj_11perfmetrics_7_metric__MethodMetricImpl *__pyx_v_self, PyObject *__pyx_v_args); /* proto*/
 
 /* Module declarations from "cython" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "perfmetrics._metric" */
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin = 0;
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl = 0;
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl = 0;
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl = 0;
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric_Metric = 0;
-static PyTypeObject *__pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__ = 0;
-#endif
 static PyObject *__pyx_v_11perfmetrics_7_metric_time = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_MethodType = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_WeakKeyDictionary = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_functools = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_stdrandom = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_statsd_client = 0;
 static PyObject *__pyx_v_11perfmetrics_7_metric_statsd_client_stack = 0;
@@ -2293,125 +2371,14 @@
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_perfmetrics__metric[] = "perfmetrics._metric";
 static const char __pyx_k_statsd_client_stack[] = "statsd_client_stack";
 static const char __pyx_k_Implementation_of_metrics[] = "\nImplementation of metrics.\n\n";
 static const char __pyx_k_src_perfmetrics_metric_py[] = "src/perfmetrics/metric.py";
 static const char __pyx_k_Decorator_context_manager_that_m[] = "Decorator/context manager that modifies the name of metrics in context.\n\n    format is a format string such as 'XYZ.%s'.\n    ";
 static const char __pyx_k_MetricMod___call___locals_call_w[] = "MetricMod.__call__.<locals>.call_with_mod";
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_n_s_AbstractMetricImpl;
-static PyObject *__pyx_kp_s_Decorator_context_manager_that_m;
-static PyObject *__pyx_n_s_GivenStatMetricImpl;
-static PyObject *__pyx_n_s_KeyError;
-static PyObject *__pyx_n_s_MethodLikeMixin;
-static PyObject *__pyx_n_s_MethodMetricImpl;
-static PyObject *__pyx_n_s_MethodType;
-static PyObject *__pyx_n_s_Metric;
-static PyObject *__pyx_n_s_MetricMod;
-static PyObject *__pyx_n_s_MetricMod___call;
-static PyObject *__pyx_n_s_MetricMod___call___locals_call_w;
-static PyObject *__pyx_n_s_MetricMod___enter;
-static PyObject *__pyx_n_s_MetricMod___exit;
-static PyObject *__pyx_n_s_MetricMod___init;
-static PyObject *__pyx_n_s_Metric___enter;
-static PyObject *__pyx_n_s_Metric___exit;
-static PyObject *__pyx_n_s_NotImplementedError;
-static PyObject *__pyx_n_s_StatsdClientMod;
-static PyObject *__pyx_n_s_WeakKeyDictionary;
-static PyObject *__pyx_n_s__24;
-static PyObject *__pyx_kp_u__4;
-static PyObject *__pyx_n_s__5;
-static PyObject *__pyx_n_s_args;
-static PyObject *__pyx_n_s_asyncio_coroutines;
-static PyObject *__pyx_n_s_buf;
-static PyObject *__pyx_n_s_call;
-static PyObject *__pyx_n_s_call_with_mod;
-static PyObject *__pyx_n_s_class;
-static PyObject *__pyx_n_s_class_getitem;
-static PyObject *__pyx_n_s_client;
-static PyObject *__pyx_n_s_client_stack;
-static PyObject *__pyx_n_s_clientstack;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_count;
-static PyObject *__pyx_n_s_dict;
-static PyObject *__pyx_kp_u_disable;
-static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_elapsed;
-static PyObject *__pyx_kp_u_enable;
-static PyObject *__pyx_n_s_enter;
-static PyObject *__pyx_n_s_exit;
-static PyObject *__pyx_n_s_f;
-static PyObject *__pyx_n_s_format;
-static PyObject *__pyx_n_s_functools;
-static PyObject *__pyx_kp_u_gc;
-static PyObject *__pyx_n_s_get;
-static PyObject *__pyx_n_s_getLogger;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_import_c_accel;
-static PyObject *__pyx_n_s_incr;
-static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_s_init_subclass;
-static PyObject *__pyx_n_s_initializing;
-static PyObject *__pyx_n_s_is_coroutine;
-static PyObject *__pyx_kp_u_isenabled;
-static PyObject *__pyx_n_s_klass_dict;
-static PyObject *__pyx_n_s_kw;
-static PyObject *__pyx_n_s_logger;
-static PyObject *__pyx_n_s_logging;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_metaclass;
-static PyObject *__pyx_n_s_method;
-static PyObject *__pyx_n_s_metric_count;
-static PyObject *__pyx_n_s_metric_rate;
-static PyObject *__pyx_n_s_metric_timing;
-static PyObject *__pyx_n_s_module;
-static PyObject *__pyx_n_s_mro_entries;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_null_client;
-static PyObject *__pyx_n_s_object;
-static PyObject *__pyx_n_s_perfmetrics__metric;
-static PyObject *__pyx_n_s_perfmetrics__util;
-static PyObject *__pyx_n_s_pop;
-static PyObject *__pyx_n_s_prepare;
-static PyObject *__pyx_n_s_push;
-static PyObject *__pyx_n_s_pyx_capi;
-static PyObject *__pyx_n_s_pyx_vtable;
-static PyObject *__pyx_n_s_qualname;
-static PyObject *__pyx_n_s_random;
-static PyObject *__pyx_n_s_rate;
-static PyObject *__pyx_n_s_rate_applied;
-static PyObject *__pyx_kp_s_s_s;
-static PyObject *__pyx_kp_s_s_s_s;
-static PyObject *__pyx_kp_s_s_t;
-static PyObject *__pyx_n_s_self;
-static PyObject *__pyx_n_s_sendbuf;
-static PyObject *__pyx_n_s_set_name;
-static PyObject *__pyx_n_s_slots;
-static PyObject *__pyx_n_s_spec;
-static PyObject *__pyx_kp_s_src_perfmetrics_metric_py;
-static PyObject *__pyx_n_s_stat;
-static PyObject *__pyx_n_s_stat_name;
-static PyObject *__pyx_n_s_statsd;
-static PyObject *__pyx_n_s_statsd_client;
-static PyObject *__pyx_n_s_statsd_client_stack;
-static PyObject *__pyx_n_s_stdrandom;
-static PyObject *__pyx_n_s_super;
-static PyObject *__pyx_n_s_tb;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_time;
-static PyObject *__pyx_n_s_timing;
-static PyObject *__pyx_n_s_timing_format;
-static PyObject *__pyx_n_s_typ;
-static PyObject *__pyx_n_s_types;
-static PyObject *__pyx_n_s_update_wrapper;
-static PyObject *__pyx_n_s_value;
-static PyObject *__pyx_n_s_weakref;
-static PyObject *__pyx_n_s_wrapped;
-static PyObject *__pyx_n_s_wraps;
-#endif
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_11perfmetrics_7_metric_16_MethodLikeMixin___get__(struct __pyx_obj_11perfmetrics_7_metric__MethodLikeMixin *__pyx_v_self, PyObject *__pyx_v_inst, PyObject *__pyx_v_klass); /* proto */
 static int __pyx_pf_11perfmetrics_7_metric_19_AbstractMetricImpl___init__(struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self, PyObject *__pyx_v_f, PyObject *__pyx_v_timing, PyObject *__pyx_v_count, PyObject *__pyx_v_rate, PyObject *__pyx_v_timing_format, PyObject *__pyx_v_random); /* proto */
 static PyObject *__pyx_pf_11perfmetrics_7_metric_19_AbstractMetricImpl_2__call__(struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_11perfmetrics_7_metric_19_AbstractMetricImpl_13metric_timing___get__(struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self); /* proto */
 static int __pyx_pf_11perfmetrics_7_metric_19_AbstractMetricImpl_13metric_timing_2__set__(struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_11perfmetrics_7_metric_19_AbstractMetricImpl_12metric_count___get__(struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *__pyx_v_self); /* proto */
@@ -2450,69 +2417,57 @@
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__MethodLikeMixin(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__AbstractMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__GivenStatMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__MethodMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric_Metric(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric___pyx_scope_struct____call__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, 0, 0, 0, 0};
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_float_1000_0;
-static PyObject *__pyx_int_1;
-#endif
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_k_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-#endif
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
-#if CYTHON_USE_MODULE_STATE
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
   PyObject *__pyx_empty_bytes;
   PyObject *__pyx_empty_unicode;
   #ifdef __Pyx_CyFunction_USED
   PyTypeObject *__pyx_CyFunctionType;
   #endif
   #ifdef __Pyx_FusedFunction_USED
   PyTypeObject *__pyx_FusedFunctionType;
   #endif
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin;
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_11perfmetrics_7_metric__MethodLikeMixin;
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl;
   PyObject *__pyx_type_11perfmetrics_7_metric__AbstractMetricImpl;
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl;
   PyObject *__pyx_type_11perfmetrics_7_metric__GivenStatMetricImpl;
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl;
   PyObject *__pyx_type_11perfmetrics_7_metric__MethodMetricImpl;
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric_Metric;
   PyObject *__pyx_type_11perfmetrics_7_metric_Metric;
-  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__;
   PyObject *__pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call__;
+  #endif
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin;
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl;
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl;
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl;
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric_Metric;
+  PyTypeObject *__pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__;
   PyObject *__pyx_n_s_AbstractMetricImpl;
   PyObject *__pyx_kp_s_Decorator_context_manager_that_m;
   PyObject *__pyx_n_s_GivenStatMetricImpl;
   PyObject *__pyx_n_s_KeyError;
   PyObject *__pyx_n_s_MethodLikeMixin;
   PyObject *__pyx_n_s_MethodMetricImpl;
   PyObject *__pyx_n_s_MethodType;
@@ -2639,27 +2594,36 @@
   PyObject *__pyx_codeobj__13;
   PyObject *__pyx_codeobj__17;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__23;
 } __pyx_mstate;
 
+#if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
 #else
 static struct PyModuleDef __pyx_moduledef;
 #endif
 
 #define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
 
 #define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
 
 #define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
 #endif
 /* #### Code section: module_state_clear ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_clear(PyObject *m) {
   __pyx_mstate *clear_module_state = __pyx_mstate(m);
   if (!clear_module_state) return 0;
   Py_CLEAR(clear_module_state->__pyx_d);
@@ -2982,39 +2946,54 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
-#if CYTHON_USE_MODULE_STATE
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
 #define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
 #define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
 #define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
 #ifdef __Pyx_CyFunction_USED
 #define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
 #endif
 #ifdef __Pyx_FusedFunction_USED
 #define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
 #endif
-#define __pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
 #define __pyx_type_11perfmetrics_7_metric__MethodLikeMixin __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric__MethodLikeMixin
-#define __pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl
 #define __pyx_type_11perfmetrics_7_metric__AbstractMetricImpl __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric__AbstractMetricImpl
-#define __pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl
 #define __pyx_type_11perfmetrics_7_metric__GivenStatMetricImpl __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric__GivenStatMetricImpl
-#define __pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl
 #define __pyx_type_11perfmetrics_7_metric__MethodMetricImpl __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric__MethodMetricImpl
-#define __pyx_ptype_11perfmetrics_7_metric_Metric __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric_Metric
 #define __pyx_type_11perfmetrics_7_metric_Metric __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric_Metric
-#define __pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__ __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__
 #define __pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call__ __pyx_mstate_global->__pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call__
+#endif
+#define __pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin
+#define __pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__AbstractMetricImpl
+#define __pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__GivenStatMetricImpl
+#define __pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric__MethodMetricImpl
+#define __pyx_ptype_11perfmetrics_7_metric_Metric __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric_Metric
+#define __pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__ __pyx_mstate_global->__pyx_ptype_11perfmetrics_7_metric___pyx_scope_struct____call__
 #define __pyx_n_s_AbstractMetricImpl __pyx_mstate_global->__pyx_n_s_AbstractMetricImpl
 #define __pyx_kp_s_Decorator_context_manager_that_m __pyx_mstate_global->__pyx_kp_s_Decorator_context_manager_that_m
 #define __pyx_n_s_GivenStatMetricImpl __pyx_mstate_global->__pyx_n_s_GivenStatMetricImpl
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
 #define __pyx_n_s_MethodLikeMixin __pyx_mstate_global->__pyx_n_s_MethodLikeMixin
 #define __pyx_n_s_MethodMetricImpl __pyx_mstate_global->__pyx_n_s_MethodMetricImpl
 #define __pyx_n_s_MethodType __pyx_mstate_global->__pyx_n_s_MethodType
@@ -3139,15 +3118,14 @@
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
-#endif
 /* #### Code section: module_code ### */
 
 /* "src/perfmetrics/metric.py":33
  *     # a __get__ impl; the last one defined wins, so we must take the conditional
  *     # inside the method.
  *     def __get__(self, inst, klass):             # <<<<<<<<<<<<<<
  *         if inst is None:
@@ -3319,19 +3297,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,&__pyx_n_s_timing,&__pyx_n_s_count,&__pyx_n_s_rate,&__pyx_n_s_timing_format,&__pyx_n_s_random,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,&__pyx_n_s_timing,&__pyx_n_s_count,&__pyx_n_s_rate,&__pyx_n_s_timing_format,&__pyx_n_s_random,0};
-    #endif
     PyObject* values[6] = {0,0,0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  6: values[5] = __Pyx_Arg_VARARGS(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_VARARGS(__pyx_args, 4);
@@ -4826,19 +4800,15 @@
   __pyx_v_args = __Pyx_ArgsSlice_VARARGS(__pyx_args, 1, __pyx_nargs);
   if (unlikely(!__pyx_v_args)) {
     __Pyx_RefNannyFinishContext();
     return -1;
   }
   __Pyx_GOTREF(__pyx_v_args);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_stat_name,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_stat_name,0};
-    #endif
     PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         default:
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -5300,23 +5270,23 @@
       if (unlikely((PyObject_SetItem(__pyx_v_self->klass_dict, __pyx_v_klass, __pyx_v_stat_name) < 0))) __PYX_ERR(0, 130, __pyx_L5_except_error)
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L4_exception_handled;
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
     /* "src/perfmetrics/metric.py":126
  *     def _compute_stat(self, args):
  *         klass = args[0].__class__
  *         try:             # <<<<<<<<<<<<<<
  *             stat_name = self.klass_dict[klass]
  *         except KeyError:
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     goto __pyx_L1_error;
     __pyx_L4_exception_handled:;
     __Pyx_XGIVEREF(__pyx_t_3);
@@ -5389,19 +5359,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_stat,&__pyx_n_s_rate,&__pyx_n_s_method,&__pyx_n_s_count,&__pyx_n_s_timing,&__pyx_n_s_timing_format,&__pyx_n_s_random,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_stat,&__pyx_n_s_rate,&__pyx_n_s_method,&__pyx_n_s_count,&__pyx_n_s_timing,&__pyx_n_s_timing_format,&__pyx_n_s_random,0};
-    #endif
     PyObject* values[7] = {0,0,0,0,0,0,0};
     values[0] = ((PyObject *)Py_None);
     values[1] = ((PyObject *)__pyx_int_1);
     values[2] = ((PyObject *)Py_False);
 
     /* "src/perfmetrics/metric.py":186
  * 
@@ -5686,19 +5652,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,0};
-    #endif
     PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -6157,19 +6119,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__exit__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_typ,&__pyx_n_s_value,&__pyx_n_s_tb,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_typ,&__pyx_n_s_value,&__pyx_n_s_tb,0};
-    #endif
     PyObject* values[3] = {0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
@@ -7248,19 +7206,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_format,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_format,0};
-    #endif
     PyObject* values[2] = {0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -7381,19 +7335,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_f,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_f,0};
-    #endif
     PyObject* values[2] = {0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -8145,19 +8095,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__exit__ (wrapper)", 0);
   {
-    #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_typ,&__pyx_n_s_value,&__pyx_n_s_tb,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_typ,&__pyx_n_s_value,&__pyx_n_s_tb,0};
-    #endif
     PyObject* values[4] = {0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -8391,18 +8337,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 static struct __pyx_vtabstruct_11perfmetrics_7_metric__AbstractMetricImpl __pyx_vtable_11perfmetrics_7_metric__AbstractMetricImpl;
 
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__AbstractMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k) {
@@ -8431,18 +8380,14 @@
   #endif
   PyObject_GC_UnTrack(o);
   if (p->__dict__) PyDict_Clear(p->__dict__);
   Py_CLEAR(p->f);
   Py_CLEAR(p->timing_format);
   Py_CLEAR(p->__wrapped__);
   Py_CLEAR(p->__dict__);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
   __pyx_tp_dealloc_11perfmetrics_7_metric__MethodLikeMixin(o);
 }
 
 static int __pyx_tp_traverse_11perfmetrics_7_metric__AbstractMetricImpl(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *p = (struct __pyx_obj_11perfmetrics_7_metric__AbstractMetricImpl *)o;
   e = ((likely(__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin)) ? ((__pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin->tp_traverse) ? __pyx_ptype_11perfmetrics_7_metric__MethodLikeMixin->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_11perfmetrics_7_metric__AbstractMetricImpl)); if (e) return e;
@@ -8646,18 +8591,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 static struct __pyx_vtabstruct_11perfmetrics_7_metric__GivenStatMetricImpl __pyx_vtable_11perfmetrics_7_metric__GivenStatMetricImpl;
 
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__GivenStatMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k) {
@@ -8806,18 +8754,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 static struct __pyx_vtabstruct_11perfmetrics_7_metric__MethodMetricImpl __pyx_vtable_11perfmetrics_7_metric__MethodMetricImpl;
 
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric__MethodMetricImpl(PyTypeObject *t, PyObject *a, PyObject *k) {
@@ -8981,18 +8932,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric_Metric(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_11perfmetrics_7_metric_Metric *p;
@@ -9263,51 +9217,61 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 static struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__ *__pyx_freelist_11perfmetrics_7_metric___pyx_scope_struct____call__[8];
 static int __pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__ = 0;
 
 static PyObject *__pyx_tp_new_11perfmetrics_7_metric___pyx_scope_struct____call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__ > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__)))) {
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((int)(__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__)))) {
     o = (PyObject*)__pyx_freelist_11perfmetrics_7_metric___pyx_scope_struct____call__[--__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__];
     memset(o, 0, sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_11perfmetrics_7_metric___pyx_scope_struct____call__(PyObject *o) {
   struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__ *p = (struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__ *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_11perfmetrics_7_metric___pyx_scope_struct____call__) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_f);
   Py_CLEAR(p->__pyx_v_self);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__ < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__)))) {
+  if (CYTHON_COMPILING_IN_CPYTHON && ((int)(__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__)))) {
     __pyx_freelist_11perfmetrics_7_metric___pyx_scope_struct____call__[__pyx_freecount_11perfmetrics_7_metric___pyx_scope_struct____call__++] = ((struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__ *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_11perfmetrics_7_metric___pyx_scope_struct____call__(PyObject *o, visitproc v, void *a) {
@@ -9341,15 +9305,15 @@
   {Py_tp_new, (void *)__pyx_tp_new_11perfmetrics_7_metric___pyx_scope_struct____call__},
   {0, 0},
 };
 static PyType_Spec __pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call___spec = {
   "perfmetrics._metric.__pyx_scope_struct____call__",
   sizeof(struct __pyx_obj_11perfmetrics_7_metric___pyx_scope_struct____call__),
   0,
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
   __pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call___slots,
 };
 #else
 
 static PyTypeObject __pyx_type_11perfmetrics_7_metric___pyx_scope_struct____call__ = {
   PyVarObject_HEAD_INIT(0, 0)
   "perfmetrics._metric.""__pyx_scope_struct____call__", /*tp_name*/
@@ -9376,15 +9340,15 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_11perfmetrics_7_metric___pyx_scope_struct____call__, /*tp_traverse*/
   __pyx_tp_clear_11perfmetrics_7_metric___pyx_scope_struct____call__, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
@@ -9416,18 +9380,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
@@ -9439,238 +9406,129 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  #if CYTHON_USE_MODULE_STATE
-  {0, __pyx_k_AbstractMetricImpl, sizeof(__pyx_k_AbstractMetricImpl), 0, 0, 1, 1},
-  {0, __pyx_k_Decorator_context_manager_that_m, sizeof(__pyx_k_Decorator_context_manager_that_m), 0, 0, 1, 0},
-  {0, __pyx_k_GivenStatMetricImpl, sizeof(__pyx_k_GivenStatMetricImpl), 0, 0, 1, 1},
-  {0, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
-  {0, __pyx_k_MethodLikeMixin, sizeof(__pyx_k_MethodLikeMixin), 0, 0, 1, 1},
-  {0, __pyx_k_MethodMetricImpl, sizeof(__pyx_k_MethodMetricImpl), 0, 0, 1, 1},
-  {0, __pyx_k_MethodType, sizeof(__pyx_k_MethodType), 0, 0, 1, 1},
-  {0, __pyx_k_Metric, sizeof(__pyx_k_Metric), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod, sizeof(__pyx_k_MetricMod), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod___call, sizeof(__pyx_k_MetricMod___call), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod___call___locals_call_w, sizeof(__pyx_k_MetricMod___call___locals_call_w), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod___enter, sizeof(__pyx_k_MetricMod___enter), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod___exit, sizeof(__pyx_k_MetricMod___exit), 0, 0, 1, 1},
-  {0, __pyx_k_MetricMod___init, sizeof(__pyx_k_MetricMod___init), 0, 0, 1, 1},
-  {0, __pyx_k_Metric___enter, sizeof(__pyx_k_Metric___enter), 0, 0, 1, 1},
-  {0, __pyx_k_Metric___exit, sizeof(__pyx_k_Metric___exit), 0, 0, 1, 1},
-  {0, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
-  {0, __pyx_k_StatsdClientMod, sizeof(__pyx_k_StatsdClientMod), 0, 0, 1, 1},
-  {0, __pyx_k_WeakKeyDictionary, sizeof(__pyx_k_WeakKeyDictionary), 0, 0, 1, 1},
-  {0, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
-  {0, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-  {0, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 1},
-  {0, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {0, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-  {0, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
-  {0, __pyx_k_call, sizeof(__pyx_k_call), 0, 0, 1, 1},
-  {0, __pyx_k_call_with_mod, sizeof(__pyx_k_call_with_mod), 0, 0, 1, 1},
-  {0, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
-  {0, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
-  {0, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
-  {0, __pyx_k_client_stack, sizeof(__pyx_k_client_stack), 0, 0, 1, 1},
-  {0, __pyx_k_clientstack, sizeof(__pyx_k_clientstack), 0, 0, 1, 1},
-  {0, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {0, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
-  {0, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {0, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
-  {0, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {0, __pyx_k_elapsed, sizeof(__pyx_k_elapsed), 0, 0, 1, 1},
-  {0, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
-  {0, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
-  {0, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {0, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
-  {0, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
-  {0, __pyx_k_functools, sizeof(__pyx_k_functools), 0, 0, 1, 1},
-  {0, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
-  {0, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
-  {0, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
-  {0, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {0, __pyx_k_import_c_accel, sizeof(__pyx_k_import_c_accel), 0, 0, 1, 1},
-  {0, __pyx_k_incr, sizeof(__pyx_k_incr), 0, 0, 1, 1},
-  {0, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {0, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
-  {0, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-  {0, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-  {0, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
-  {0, __pyx_k_klass_dict, sizeof(__pyx_k_klass_dict), 0, 0, 1, 1},
-  {0, __pyx_k_kw, sizeof(__pyx_k_kw), 0, 0, 1, 1},
-  {0, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
-  {0, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
-  {0, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {0, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {0, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
-  {0, __pyx_k_metric_count, sizeof(__pyx_k_metric_count), 0, 0, 1, 1},
-  {0, __pyx_k_metric_rate, sizeof(__pyx_k_metric_rate), 0, 0, 1, 1},
-  {0, __pyx_k_metric_timing, sizeof(__pyx_k_metric_timing), 0, 0, 1, 1},
-  {0, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-  {0, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
-  {0, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {0, __pyx_k_null_client, sizeof(__pyx_k_null_client), 0, 0, 1, 1},
-  {0, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
-  {0, __pyx_k_perfmetrics__metric, sizeof(__pyx_k_perfmetrics__metric), 0, 0, 1, 1},
-  {0, __pyx_k_perfmetrics__util, sizeof(__pyx_k_perfmetrics__util), 0, 0, 1, 1},
-  {0, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
-  {0, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {0, __pyx_k_push, sizeof(__pyx_k_push), 0, 0, 1, 1},
-  {0, __pyx_k_pyx_capi, sizeof(__pyx_k_pyx_capi), 0, 0, 1, 1},
-  {0, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-  {0, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {0, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
-  {0, __pyx_k_rate, sizeof(__pyx_k_rate), 0, 0, 1, 1},
-  {0, __pyx_k_rate_applied, sizeof(__pyx_k_rate_applied), 0, 0, 1, 1},
-  {0, __pyx_k_s_s, sizeof(__pyx_k_s_s), 0, 0, 1, 0},
-  {0, __pyx_k_s_s_s, sizeof(__pyx_k_s_s_s), 0, 0, 1, 0},
-  {0, __pyx_k_s_t, sizeof(__pyx_k_s_t), 0, 0, 1, 0},
-  {0, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-  {0, __pyx_k_sendbuf, sizeof(__pyx_k_sendbuf), 0, 0, 1, 1},
-  {0, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
-  {0, __pyx_k_slots, sizeof(__pyx_k_slots), 0, 0, 1, 1},
-  {0, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
-  {0, __pyx_k_src_perfmetrics_metric_py, sizeof(__pyx_k_src_perfmetrics_metric_py), 0, 0, 1, 0},
-  {0, __pyx_k_stat, sizeof(__pyx_k_stat), 0, 0, 1, 1},
-  {0, __pyx_k_stat_name, sizeof(__pyx_k_stat_name), 0, 0, 1, 1},
-  {0, __pyx_k_statsd, sizeof(__pyx_k_statsd), 0, 0, 1, 1},
-  {0, __pyx_k_statsd_client, sizeof(__pyx_k_statsd_client), 0, 0, 1, 1},
-  {0, __pyx_k_statsd_client_stack, sizeof(__pyx_k_statsd_client_stack), 0, 0, 1, 1},
-  {0, __pyx_k_stdrandom, sizeof(__pyx_k_stdrandom), 0, 0, 1, 1},
-  {0, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
-  {0, __pyx_k_tb, sizeof(__pyx_k_tb), 0, 0, 1, 1},
-  {0, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {0, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-  {0, __pyx_k_timing, sizeof(__pyx_k_timing), 0, 0, 1, 1},
-  {0, __pyx_k_timing_format, sizeof(__pyx_k_timing_format), 0, 0, 1, 1},
-  {0, __pyx_k_typ, sizeof(__pyx_k_typ), 0, 0, 1, 1},
-  {0, __pyx_k_types, sizeof(__pyx_k_types), 0, 0, 1, 1},
-  {0, __pyx_k_update_wrapper, sizeof(__pyx_k_update_wrapper), 0, 0, 1, 1},
-  {0, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {0, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
-  {0, __pyx_k_wrapped, sizeof(__pyx_k_wrapped), 0, 0, 1, 1},
-  {0, __pyx_k_wraps, sizeof(__pyx_k_wraps), 0, 0, 1, 1},
-  #else
-  {&__pyx_n_s_AbstractMetricImpl, __pyx_k_AbstractMetricImpl, sizeof(__pyx_k_AbstractMetricImpl), 0, 0, 1, 1},
-  {&__pyx_kp_s_Decorator_context_manager_that_m, __pyx_k_Decorator_context_manager_that_m, sizeof(__pyx_k_Decorator_context_manager_that_m), 0, 0, 1, 0},
-  {&__pyx_n_s_GivenStatMetricImpl, __pyx_k_GivenStatMetricImpl, sizeof(__pyx_k_GivenStatMetricImpl), 0, 0, 1, 1},
-  {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
-  {&__pyx_n_s_MethodLikeMixin, __pyx_k_MethodLikeMixin, sizeof(__pyx_k_MethodLikeMixin), 0, 0, 1, 1},
-  {&__pyx_n_s_MethodMetricImpl, __pyx_k_MethodMetricImpl, sizeof(__pyx_k_MethodMetricImpl), 0, 0, 1, 1},
-  {&__pyx_n_s_MethodType, __pyx_k_MethodType, sizeof(__pyx_k_MethodType), 0, 0, 1, 1},
-  {&__pyx_n_s_Metric, __pyx_k_Metric, sizeof(__pyx_k_Metric), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod, __pyx_k_MetricMod, sizeof(__pyx_k_MetricMod), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod___call, __pyx_k_MetricMod___call, sizeof(__pyx_k_MetricMod___call), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod___call___locals_call_w, __pyx_k_MetricMod___call___locals_call_w, sizeof(__pyx_k_MetricMod___call___locals_call_w), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod___enter, __pyx_k_MetricMod___enter, sizeof(__pyx_k_MetricMod___enter), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod___exit, __pyx_k_MetricMod___exit, sizeof(__pyx_k_MetricMod___exit), 0, 0, 1, 1},
-  {&__pyx_n_s_MetricMod___init, __pyx_k_MetricMod___init, sizeof(__pyx_k_MetricMod___init), 0, 0, 1, 1},
-  {&__pyx_n_s_Metric___enter, __pyx_k_Metric___enter, sizeof(__pyx_k_Metric___enter), 0, 0, 1, 1},
-  {&__pyx_n_s_Metric___exit, __pyx_k_Metric___exit, sizeof(__pyx_k_Metric___exit), 0, 0, 1, 1},
-  {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
-  {&__pyx_n_s_StatsdClientMod, __pyx_k_StatsdClientMod, sizeof(__pyx_k_StatsdClientMod), 0, 0, 1, 1},
-  {&__pyx_n_s_WeakKeyDictionary, __pyx_k_WeakKeyDictionary, sizeof(__pyx_k_WeakKeyDictionary), 0, 0, 1, 1},
-  {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
-  {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-  {&__pyx_n_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 1},
-  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-  {&__pyx_n_s_buf, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
-  {&__pyx_n_s_call, __pyx_k_call, sizeof(__pyx_k_call), 0, 0, 1, 1},
-  {&__pyx_n_s_call_with_mod, __pyx_k_call_with_mod, sizeof(__pyx_k_call_with_mod), 0, 0, 1, 1},
-  {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
-  {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
-  {&__pyx_n_s_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
-  {&__pyx_n_s_client_stack, __pyx_k_client_stack, sizeof(__pyx_k_client_stack), 0, 0, 1, 1},
-  {&__pyx_n_s_clientstack, __pyx_k_clientstack, sizeof(__pyx_k_clientstack), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
-  {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
-  {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_elapsed, __pyx_k_elapsed, sizeof(__pyx_k_elapsed), 0, 0, 1, 1},
-  {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
-  {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
-  {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
-  {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
-  {&__pyx_n_s_functools, __pyx_k_functools, sizeof(__pyx_k_functools), 0, 0, 1, 1},
-  {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
-  {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
-  {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_import_c_accel, __pyx_k_import_c_accel, sizeof(__pyx_k_import_c_accel), 0, 0, 1, 1},
-  {&__pyx_n_s_incr, __pyx_k_incr, sizeof(__pyx_k_incr), 0, 0, 1, 1},
-  {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
-  {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-  {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-  {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
-  {&__pyx_n_s_klass_dict, __pyx_k_klass_dict, sizeof(__pyx_k_klass_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_kw, __pyx_k_kw, sizeof(__pyx_k_kw), 0, 0, 1, 1},
-  {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
-  {&__pyx_n_s_logging, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {&__pyx_n_s_method, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
-  {&__pyx_n_s_metric_count, __pyx_k_metric_count, sizeof(__pyx_k_metric_count), 0, 0, 1, 1},
-  {&__pyx_n_s_metric_rate, __pyx_k_metric_rate, sizeof(__pyx_k_metric_rate), 0, 0, 1, 1},
-  {&__pyx_n_s_metric_timing, __pyx_k_metric_timing, sizeof(__pyx_k_metric_timing), 0, 0, 1, 1},
-  {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-  {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_null_client, __pyx_k_null_client, sizeof(__pyx_k_null_client), 0, 0, 1, 1},
-  {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
-  {&__pyx_n_s_perfmetrics__metric, __pyx_k_perfmetrics__metric, sizeof(__pyx_k_perfmetrics__metric), 0, 0, 1, 1},
-  {&__pyx_n_s_perfmetrics__util, __pyx_k_perfmetrics__util, sizeof(__pyx_k_perfmetrics__util), 0, 0, 1, 1},
-  {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
-  {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {&__pyx_n_s_push, __pyx_k_push, sizeof(__pyx_k_push), 0, 0, 1, 1},
-  {&__pyx_n_s_pyx_capi, __pyx_k_pyx_capi, sizeof(__pyx_k_pyx_capi), 0, 0, 1, 1},
-  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-  {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
-  {&__pyx_n_s_rate, __pyx_k_rate, sizeof(__pyx_k_rate), 0, 0, 1, 1},
-  {&__pyx_n_s_rate_applied, __pyx_k_rate_applied, sizeof(__pyx_k_rate_applied), 0, 0, 1, 1},
-  {&__pyx_kp_s_s_s, __pyx_k_s_s, sizeof(__pyx_k_s_s), 0, 0, 1, 0},
-  {&__pyx_kp_s_s_s_s, __pyx_k_s_s_s, sizeof(__pyx_k_s_s_s), 0, 0, 1, 0},
-  {&__pyx_kp_s_s_t, __pyx_k_s_t, sizeof(__pyx_k_s_t), 0, 0, 1, 0},
-  {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-  {&__pyx_n_s_sendbuf, __pyx_k_sendbuf, sizeof(__pyx_k_sendbuf), 0, 0, 1, 1},
-  {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
-  {&__pyx_n_s_slots, __pyx_k_slots, sizeof(__pyx_k_slots), 0, 0, 1, 1},
-  {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
-  {&__pyx_kp_s_src_perfmetrics_metric_py, __pyx_k_src_perfmetrics_metric_py, sizeof(__pyx_k_src_perfmetrics_metric_py), 0, 0, 1, 0},
-  {&__pyx_n_s_stat, __pyx_k_stat, sizeof(__pyx_k_stat), 0, 0, 1, 1},
-  {&__pyx_n_s_stat_name, __pyx_k_stat_name, sizeof(__pyx_k_stat_name), 0, 0, 1, 1},
-  {&__pyx_n_s_statsd, __pyx_k_statsd, sizeof(__pyx_k_statsd), 0, 0, 1, 1},
-  {&__pyx_n_s_statsd_client, __pyx_k_statsd_client, sizeof(__pyx_k_statsd_client), 0, 0, 1, 1},
-  {&__pyx_n_s_statsd_client_stack, __pyx_k_statsd_client_stack, sizeof(__pyx_k_statsd_client_stack), 0, 0, 1, 1},
-  {&__pyx_n_s_stdrandom, __pyx_k_stdrandom, sizeof(__pyx_k_stdrandom), 0, 0, 1, 1},
-  {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
-  {&__pyx_n_s_tb, __pyx_k_tb, sizeof(__pyx_k_tb), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-  {&__pyx_n_s_timing, __pyx_k_timing, sizeof(__pyx_k_timing), 0, 0, 1, 1},
-  {&__pyx_n_s_timing_format, __pyx_k_timing_format, sizeof(__pyx_k_timing_format), 0, 0, 1, 1},
-  {&__pyx_n_s_typ, __pyx_k_typ, sizeof(__pyx_k_typ), 0, 0, 1, 1},
-  {&__pyx_n_s_types, __pyx_k_types, sizeof(__pyx_k_types), 0, 0, 1, 1},
-  {&__pyx_n_s_update_wrapper, __pyx_k_update_wrapper, sizeof(__pyx_k_update_wrapper), 0, 0, 1, 1},
-  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
-  {&__pyx_n_s_wrapped, __pyx_k_wrapped, sizeof(__pyx_k_wrapped), 0, 0, 1, 1},
-  {&__pyx_n_s_wraps, __pyx_k_wraps, sizeof(__pyx_k_wraps), 0, 0, 1, 1},
-  #endif
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_AbstractMetricImpl, __pyx_k_AbstractMetricImpl, sizeof(__pyx_k_AbstractMetricImpl), 0, 0, 1, 1},
+    {&__pyx_kp_s_Decorator_context_manager_that_m, __pyx_k_Decorator_context_manager_that_m, sizeof(__pyx_k_Decorator_context_manager_that_m), 0, 0, 1, 0},
+    {&__pyx_n_s_GivenStatMetricImpl, __pyx_k_GivenStatMetricImpl, sizeof(__pyx_k_GivenStatMetricImpl), 0, 0, 1, 1},
+    {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
+    {&__pyx_n_s_MethodLikeMixin, __pyx_k_MethodLikeMixin, sizeof(__pyx_k_MethodLikeMixin), 0, 0, 1, 1},
+    {&__pyx_n_s_MethodMetricImpl, __pyx_k_MethodMetricImpl, sizeof(__pyx_k_MethodMetricImpl), 0, 0, 1, 1},
+    {&__pyx_n_s_MethodType, __pyx_k_MethodType, sizeof(__pyx_k_MethodType), 0, 0, 1, 1},
+    {&__pyx_n_s_Metric, __pyx_k_Metric, sizeof(__pyx_k_Metric), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod, __pyx_k_MetricMod, sizeof(__pyx_k_MetricMod), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod___call, __pyx_k_MetricMod___call, sizeof(__pyx_k_MetricMod___call), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod___call___locals_call_w, __pyx_k_MetricMod___call___locals_call_w, sizeof(__pyx_k_MetricMod___call___locals_call_w), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod___enter, __pyx_k_MetricMod___enter, sizeof(__pyx_k_MetricMod___enter), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod___exit, __pyx_k_MetricMod___exit, sizeof(__pyx_k_MetricMod___exit), 0, 0, 1, 1},
+    {&__pyx_n_s_MetricMod___init, __pyx_k_MetricMod___init, sizeof(__pyx_k_MetricMod___init), 0, 0, 1, 1},
+    {&__pyx_n_s_Metric___enter, __pyx_k_Metric___enter, sizeof(__pyx_k_Metric___enter), 0, 0, 1, 1},
+    {&__pyx_n_s_Metric___exit, __pyx_k_Metric___exit, sizeof(__pyx_k_Metric___exit), 0, 0, 1, 1},
+    {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
+    {&__pyx_n_s_StatsdClientMod, __pyx_k_StatsdClientMod, sizeof(__pyx_k_StatsdClientMod), 0, 0, 1, 1},
+    {&__pyx_n_s_WeakKeyDictionary, __pyx_k_WeakKeyDictionary, sizeof(__pyx_k_WeakKeyDictionary), 0, 0, 1, 1},
+    {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
+    {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+    {&__pyx_n_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 1},
+    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_buf, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
+    {&__pyx_n_s_call, __pyx_k_call, sizeof(__pyx_k_call), 0, 0, 1, 1},
+    {&__pyx_n_s_call_with_mod, __pyx_k_call_with_mod, sizeof(__pyx_k_call_with_mod), 0, 0, 1, 1},
+    {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
+    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
+    {&__pyx_n_s_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
+    {&__pyx_n_s_client_stack, __pyx_k_client_stack, sizeof(__pyx_k_client_stack), 0, 0, 1, 1},
+    {&__pyx_n_s_clientstack, __pyx_k_clientstack, sizeof(__pyx_k_clientstack), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
+    {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+    {&__pyx_n_s_elapsed, __pyx_k_elapsed, sizeof(__pyx_k_elapsed), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
+    {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+    {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
+    {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
+    {&__pyx_n_s_functools, __pyx_k_functools, sizeof(__pyx_k_functools), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
+    {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_import_c_accel, __pyx_k_import_c_accel, sizeof(__pyx_k_import_c_accel), 0, 0, 1, 1},
+    {&__pyx_n_s_incr, __pyx_k_incr, sizeof(__pyx_k_incr), 0, 0, 1, 1},
+    {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
+    {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_klass_dict, __pyx_k_klass_dict, sizeof(__pyx_k_klass_dict), 0, 0, 1, 1},
+    {&__pyx_n_s_kw, __pyx_k_kw, sizeof(__pyx_k_kw), 0, 0, 1, 1},
+    {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
+    {&__pyx_n_s_logging, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
+    {&__pyx_n_s_method, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
+    {&__pyx_n_s_metric_count, __pyx_k_metric_count, sizeof(__pyx_k_metric_count), 0, 0, 1, 1},
+    {&__pyx_n_s_metric_rate, __pyx_k_metric_rate, sizeof(__pyx_k_metric_rate), 0, 0, 1, 1},
+    {&__pyx_n_s_metric_timing, __pyx_k_metric_timing, sizeof(__pyx_k_metric_timing), 0, 0, 1, 1},
+    {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
+    {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_null_client, __pyx_k_null_client, sizeof(__pyx_k_null_client), 0, 0, 1, 1},
+    {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
+    {&__pyx_n_s_perfmetrics__metric, __pyx_k_perfmetrics__metric, sizeof(__pyx_k_perfmetrics__metric), 0, 0, 1, 1},
+    {&__pyx_n_s_perfmetrics__util, __pyx_k_perfmetrics__util, sizeof(__pyx_k_perfmetrics__util), 0, 0, 1, 1},
+    {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
+    {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+    {&__pyx_n_s_push, __pyx_k_push, sizeof(__pyx_k_push), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_capi, __pyx_k_pyx_capi, sizeof(__pyx_k_pyx_capi), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+    {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+    {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
+    {&__pyx_n_s_rate, __pyx_k_rate, sizeof(__pyx_k_rate), 0, 0, 1, 1},
+    {&__pyx_n_s_rate_applied, __pyx_k_rate_applied, sizeof(__pyx_k_rate_applied), 0, 0, 1, 1},
+    {&__pyx_kp_s_s_s, __pyx_k_s_s, sizeof(__pyx_k_s_s), 0, 0, 1, 0},
+    {&__pyx_kp_s_s_s_s, __pyx_k_s_s_s, sizeof(__pyx_k_s_s_s), 0, 0, 1, 0},
+    {&__pyx_kp_s_s_t, __pyx_k_s_t, sizeof(__pyx_k_s_t), 0, 0, 1, 0},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_sendbuf, __pyx_k_sendbuf, sizeof(__pyx_k_sendbuf), 0, 0, 1, 1},
+    {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
+    {&__pyx_n_s_slots, __pyx_k_slots, sizeof(__pyx_k_slots), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_kp_s_src_perfmetrics_metric_py, __pyx_k_src_perfmetrics_metric_py, sizeof(__pyx_k_src_perfmetrics_metric_py), 0, 0, 1, 0},
+    {&__pyx_n_s_stat, __pyx_k_stat, sizeof(__pyx_k_stat), 0, 0, 1, 1},
+    {&__pyx_n_s_stat_name, __pyx_k_stat_name, sizeof(__pyx_k_stat_name), 0, 0, 1, 1},
+    {&__pyx_n_s_statsd, __pyx_k_statsd, sizeof(__pyx_k_statsd), 0, 0, 1, 1},
+    {&__pyx_n_s_statsd_client, __pyx_k_statsd_client, sizeof(__pyx_k_statsd_client), 0, 0, 1, 1},
+    {&__pyx_n_s_statsd_client_stack, __pyx_k_statsd_client_stack, sizeof(__pyx_k_statsd_client_stack), 0, 0, 1, 1},
+    {&__pyx_n_s_stdrandom, __pyx_k_stdrandom, sizeof(__pyx_k_stdrandom), 0, 0, 1, 1},
+    {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
+    {&__pyx_n_s_tb, __pyx_k_tb, sizeof(__pyx_k_tb), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
+    {&__pyx_n_s_timing, __pyx_k_timing, sizeof(__pyx_k_timing), 0, 0, 1, 1},
+    {&__pyx_n_s_timing_format, __pyx_k_timing_format, sizeof(__pyx_k_timing_format), 0, 0, 1, 1},
+    {&__pyx_n_s_typ, __pyx_k_typ, sizeof(__pyx_k_typ), 0, 0, 1, 1},
+    {&__pyx_n_s_types, __pyx_k_types, sizeof(__pyx_k_types), 0, 0, 1, 1},
+    {&__pyx_n_s_update_wrapper, __pyx_k_update_wrapper, sizeof(__pyx_k_update_wrapper), 0, 0, 1, 1},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
+    {&__pyx_n_s_wrapped, __pyx_k_wrapped, sizeof(__pyx_k_wrapped), 0, 0, 1, 1},
+    {&__pyx_n_s_wraps, __pyx_k_wraps, sizeof(__pyx_k_wraps), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(0, 22, __pyx_L1_error)
   __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 244, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 102, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 128, __pyx_L1_error)
@@ -9832,128 +9690,15 @@
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   __pyx_umethod_PyList_Type_pop.type = (PyObject*)&PyList_Type;
   __pyx_umethod_PyList_Type_pop.method_name = &__pyx_n_s_pop;
-  #if CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_s_AbstractMetricImpl) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_kp_s_Decorator_context_manager_that_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_GivenStatMetricImpl) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_KeyError) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_MethodLikeMixin) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_MethodMetricImpl) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_MethodType) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s_Metric) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s_MetricMod) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_MetricMod___call) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_MetricMod___call___locals_call_w) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_MetricMod___enter) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_MetricMod___exit) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_MetricMod___init) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_Metric___enter) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_Metric___exit) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_NotImplementedError) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_StatsdClientMod) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_WeakKeyDictionary) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s__24) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_kp_u__4) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s__5) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_args) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_asyncio_coroutines) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_buf) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_call) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_call_with_mod) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_class) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_class_getitem) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_client) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_client_stack) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_clientstack) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_cline_in_traceback) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_count) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_n_s_dict) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_kp_u_disable) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_doc) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_elapsed) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_kp_u_enable) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_enter) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_exit) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_f) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_format) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_functools) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_kp_u_gc) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_get) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_s_getLogger) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_n_s_import) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_n_s_import_c_accel) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[49], &__pyx_n_s_incr) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[50], &__pyx_n_s_init) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[51], &__pyx_n_s_init_subclass) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[52], &__pyx_n_s_initializing) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[53], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[54], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[55], &__pyx_n_s_klass_dict) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[56], &__pyx_n_s_kw) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[57], &__pyx_n_s_logger) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[58], &__pyx_n_s_logging) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[59], &__pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[60], &__pyx_n_s_metaclass) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[61], &__pyx_n_s_method) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[62], &__pyx_n_s_metric_count) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[63], &__pyx_n_s_metric_rate) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[64], &__pyx_n_s_metric_timing) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[65], &__pyx_n_s_module) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[66], &__pyx_n_s_mro_entries) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[67], &__pyx_n_s_name) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[68], &__pyx_n_s_null_client) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[69], &__pyx_n_s_object) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[70], &__pyx_n_s_perfmetrics__metric) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[71], &__pyx_n_s_perfmetrics__util) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[72], &__pyx_n_s_pop) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[73], &__pyx_n_s_prepare) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[74], &__pyx_n_s_push) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[75], &__pyx_n_s_pyx_capi) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[76], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[77], &__pyx_n_s_qualname) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[78], &__pyx_n_s_random) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[79], &__pyx_n_s_rate) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[80], &__pyx_n_s_rate_applied) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[81], &__pyx_kp_s_s_s) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[82], &__pyx_kp_s_s_s_s) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[83], &__pyx_kp_s_s_t) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[84], &__pyx_n_s_self) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[85], &__pyx_n_s_sendbuf) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[86], &__pyx_n_s_set_name) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[87], &__pyx_n_s_slots) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[88], &__pyx_n_s_spec) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[89], &__pyx_kp_s_src_perfmetrics_metric_py) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[90], &__pyx_n_s_stat) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[91], &__pyx_n_s_stat_name) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[92], &__pyx_n_s_statsd) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[93], &__pyx_n_s_statsd_client) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[94], &__pyx_n_s_statsd_client_stack) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[95], &__pyx_n_s_stdrandom) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[96], &__pyx_n_s_super) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[97], &__pyx_n_s_tb) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[98], &__pyx_n_s_test) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[99], &__pyx_n_s_time) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[100], &__pyx_n_s_timing) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[101], &__pyx_n_s_timing_format) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[102], &__pyx_n_s_typ) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[103], &__pyx_n_s_types) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[104], &__pyx_n_s_update_wrapper) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[105], &__pyx_n_s_value) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[106], &__pyx_n_s_weakref) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[107], &__pyx_n_s_wrapped) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[108], &__pyx_n_s_wraps) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  #endif
-  #if !CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  #endif
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float_1000_0 = PyFloat_FromDouble(1000.0); if (unlikely(!__pyx_float_1000_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
@@ -10357,14 +10102,17 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__metric(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -10383,34 +10131,35 @@
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_metric", __pyx_methods, __pyx_k_Implementation_of_metrics, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #elif CYTHON_COMPILING_IN_LIMITED_API
+  #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    Py_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _metric pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -10931,14 +10680,22 @@
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init perfmetrics._metric", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
     #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init perfmetrics._metric");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
@@ -10949,15 +10706,15 @@
   return;
   #endif
 }
 /* #### Code section: cleanup_globals ### */
 /* #### Code section: cleanup_module ### */
 /* #### Code section: main_method ### */
 /* #### Code section: utility_code_pragmas ### */
-#if _MSC_VER
+#ifdef _MSC_VER
 #pragma warning( push )
 /* Warning 4127: conditional expression is constant
  * Cython uses constant conditional expressions to allow in inline functions to be optimized at
  * compile-time, so this warning is not useful
  */
 #pragma warning( disable : 4127 )
 #endif
@@ -10996,44 +10753,95 @@
 #endif
     for (i=0; i<n; i++) {
         if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
     }
     return 0;
 }
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
     if (exc_type == err) return 1;
     if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
 }
 #endif
 
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
     tstate->curexc_traceback = tb;
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+#endif
 }
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
     *type = tstate->curexc_type;
     *value = tstate->curexc_value;
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+#endif
 }
 #endif
 
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
@@ -11462,15 +11270,15 @@
     Py_DECREF(argstuple);
     return result;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
         if (__Pyx_IsCyOrPyCFunction(func))
 #else
         if (PyCFunction_Check(func))
 #endif
         {
             if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
                 return __Pyx_PyObject_CallMethO(func, NULL);
@@ -11765,28 +11573,40 @@
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
-    PyObject *local_type, *local_value, *local_tb;
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
 #if CYTHON_FAST_THREAD_STATE
     PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
     local_type = tstate->curexc_type;
     local_value = tstate->curexc_value;
     local_tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+  #endif
 #else
     PyErr_Fetch(&local_type, &local_value, &local_tb);
 #endif
     PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
     if (unlikely(tstate->curexc_type))
 #else
     if (unlikely(PyErr_Occurred()))
 #endif
         goto bad;
     #if PY_MAJOR_VERSION >= 3
     if (local_tb) {
@@ -11857,15 +11677,20 @@
         Py_XDECREF(tmp_value);
         tmp_value = NULL;
         tmp_type = NULL;
         tmp_tb = NULL;
     } else {
         tmp_type = (PyObject*) Py_TYPE(tmp_value);
         Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
         tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
     }
   #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
@@ -11891,15 +11716,15 @@
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
 /* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
@@ -12109,28 +11934,30 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY ||  CYTHON_COMPILING_IN_LIMITED_API
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -12235,15 +12062,15 @@
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
         return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
     }
     if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
         __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
@@ -12409,30 +12236,73 @@
     result = __Pyx_PyObject_CallNoArg(method);
     Py_DECREF(method);
 bad:
     return result;
 }
 
 /* UnpackUnboundCMethod */
+static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
+    if (unlikely(!selfless_args)) return NULL;
+    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    Py_DECREF(selfless_args);
+    return result;
+}
+static PyMethodDef __Pyx_UnboundCMethod_Def = {
+     "CythonUnboundCMethod",
+     __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
+     METH_VARARGS | METH_KEYWORDS,
+     NULL
+};
 static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
     PyObject *method;
     method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
     if (unlikely(!method))
         return -1;
     target->method = method;
 #if CYTHON_COMPILING_IN_CPYTHON
     #if PY_MAJOR_VERSION >= 3
     if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
+    #else
+    if (likely(!PyCFunction_Check(method)))
     #endif
     {
         PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
         target->func = descr->d_method->ml_meth;
         target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
-    }
+    } else
+#endif
+#if defined(CYTHON_COMPILING_IN_PYPY)
+#elif PY_VERSION_HEX >= 0x03090000
+    if (PyCFunction_CheckExact(method))
+#else
+    if (PyCFunction_Check(method))
+#endif
+    {
+        PyObject *self;
+        int self_found;
+#if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
+        self = PyObject_GetAttrString(method, "__self__");
+        if (!self) {
+            PyErr_Clear();
+        }
+#else
+        self = PyCFunction_GET_SELF(method);
 #endif
+        self_found = (self && self != Py_None);
+#if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
+        Py_XDECREF(self);
+#endif
+        if (self_found) {
+            PyObject *unbound_method = PyCFunction_New(&__Pyx_UnboundCMethod_Def, method);
+            if (unlikely(!unbound_method)) return -1;
+            Py_DECREF(method);
+            target->method = unbound_method;
+        }
+    }
     return 0;
 }
 
 /* CallUnboundCMethod0 */
 static PyObject* __Pyx__CallUnboundCMethod0(__Pyx_CachedCFunction* cfunc, PyObject* self) {
     PyObject *args, *result = NULL;
     if (unlikely(!cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
@@ -12468,16 +12338,16 @@
 }
 #endif
 
 /* FixUpExtensionType */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
 #if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    (void) spec;
-    (void) type;
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
 #else
     const PyType_Slot *slot = spec->slots;
     while (slot && slot->slot && slot->slot != Py_tp_members)
         slot++;
     if (slot && slot->slot == Py_tp_members) {
         int changed = 0;
 #if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
@@ -12630,15 +12500,15 @@
               spec->basicsize) < 0) {
             goto bad;
         }
         goto done;
     }
     if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
     PyErr_Clear();
-    (void) module;
+    CYTHON_UNUSED_VAR(module);
     cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
     if (unlikely(!cached_type)) goto bad;
     if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
     if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
 done:
     Py_DECREF(abi_module);
     assert(cached_type == NULL || PyType_Check(cached_type));
@@ -13277,17 +13147,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -13519,27 +13394,30 @@
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #endif
 static int __pyx_CyFunction_init(PyObject *module) {
 #if CYTHON_USE_TYPE_SPECS
     __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
 #else
-    (void) module;
+    CYTHON_UNUSED_VAR(module);
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
 #endif
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
 }
@@ -13692,14 +13570,17 @@
             Py_DECREF(ret);
         } else if (unlikely(gc_was_enabled == -1)) {
             Py_DECREF(gc);
             return -1;
         }
     #endif
         t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
 #else
         (void)__Pyx_PyObject_CallMethod0;
 #endif
     r = PyType_Ready(t);
 #if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
         t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
     #if PY_VERSION_HEX >= 0x030A00b1
@@ -14030,56 +13911,62 @@
     Py_XINCREF(imported_module);
 #else
     imported_module = PyImport_GetModule(name);
 #endif
     return imported_module;
 }
 #endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
     PyObject *module, *from_list, *star = __pyx_n_s__5;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
     Py_DECREF(from_list);
     return module;
 #else
-    Py_ssize_t i, nparts;
     PyObject *imported_module;
     PyObject *module = __Pyx_Import(name, NULL, 0);
     if (!parts_tuple || unlikely(!module))
         return module;
     imported_module = __Pyx__ImportDottedModule_Lookup(name);
     if (likely(imported_module)) {
         Py_DECREF(module);
         return imported_module;
     }
     PyErr_Clear();
-    nparts = PyTuple_GET_SIZE(parts_tuple);
-    for (i=1; i < nparts && module; i++) {
-        PyObject *part, *submodule;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        part = PyTuple_GET_ITEM(parts_tuple, i);
-#else
-        part = PySequence_ITEM(parts_tuple, i);
-#endif
-        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
-#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-        Py_DECREF(part);
-#endif
-        Py_DECREF(module);
-        module = submodule;
-    }
-    if (likely(module))
-        return module;
-    return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
 #endif
 }
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
     PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
     if (likely(module)) {
         PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
@@ -14533,20 +14420,21 @@
 /* Globals */
 static PyObject* __Pyx_Globals(void) {
     return __Pyx_NewRef(__pyx_d);
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
@@ -14876,48 +14764,53 @@
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14931,108 +14824,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -15072,48 +15037,53 @@
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15127,108 +15097,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -15443,15 +15485,14 @@
     if (!*str)
         return -1;
     if (PyObject_Hash(*str) == -1)
         return -1;
     return 0;
 }
 #endif
-#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION >= 3
         __Pyx_InitString(*t, t->p);
         #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
@@ -15465,15 +15506,14 @@
         if (PyObject_Hash(*t->p) == -1)
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
-#endif
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
@@ -15637,21 +15677,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -15712,15 +15750,15 @@
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
 /* #### Code section: utility_code_pragmas_end ### */
-#if _MSV_VER
+#ifdef _MSC_VER
 #pragma warning( pop )
 #endif
 
 
 
 /* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `perfmetrics-3.3.0/src/perfmetrics/metric.py` & `perfmetrics-4.0.0/src/perfmetrics/metric.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/pyramid.py` & `perfmetrics-4.0.0/src/perfmetrics/pyramid.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/statsd.py` & `perfmetrics-4.0.0/src/perfmetrics/statsd.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/__init__.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/client.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/client.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/matchers.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/matchers.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/observation.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/observation.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_client.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_matchers.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/testing/tests/test_observation.py` & `perfmetrics-4.0.0/src/perfmetrics/testing/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/__init__.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,18 +72,17 @@
         def __init__(self, iface):
             super(VerifyProvides, self).__init__()
             self.iface = iface
 
         def _matches(self, item):
             try:
                 verifyObject(self.iface, item)
+                return True
             except Invalid:
                 return False
-            else:
-                return True
 
         def describe_to(self, description):
             description.append_text('object verifiably providing ').append_description_of(
                 self.iface)
 
         def describe_mismatch(self, item, mismatch_description):
             md = mismatch_description
```

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/bench_metric.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/bench_metric.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_clientstack.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_clientstack.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_metric.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_perfmetrics.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_perfmetrics.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_pyramid.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_statsd.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/tests/test_wsgi.py` & `perfmetrics-4.0.0/src/perfmetrics/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics/wsgi.py` & `perfmetrics-4.0.0/src/perfmetrics/wsgi.py`

 * *Files identical despite different names*

### Comparing `perfmetrics-3.3.0/src/perfmetrics.egg-info/PKG-INFO` & `perfmetrics-4.0.0/src/perfmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: perfmetrics
-Version: 3.3.0
+Version: 4.0.0
 Summary: Send performance metrics about Python code to Statsd
 Home-page: https://github.com/zodb/perfmetrics
 Author: Shane Hathaway
 Author-email: shane@hathawaymix.org
 Maintainer: Jason Madden
 Maintainer-email: jason@nextthought.com
 License: BSD-derived (http://www.repoze.org/LICENSE.txt)
 Project-URL: Bug Tracker, https://github.com/zodb/perfmetrics/issues
 Project-URL: Source Code, https://github.com/zodb/perfmetrics/
 Project-URL: Documentation, https://perfmetrics.readthedocs.io
 Keywords: statsd metrics performance monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: Repoze Public License
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =============
  perfmetrics
 =============
@@ -200,14 +199,22 @@
 You can turn on that option for each graph.
 
 
 =========
  CHANGES
 =========
 
+4.0.0 (2023-06-22)
+==================
+
+- Drop support for obsolete Python versions, including Python 2.7 and
+  3.6.
+- Add support for Python 3.12.
+
+
 3.3.0 (2022-09-25)
 ==================
 
 - Stop accidentally building manylinux wheels with unsafe math
   optimizations.
 - Add support for Python 3.11.
```

### Comparing `perfmetrics-3.3.0/src/perfmetrics.egg-info/SOURCES.txt` & `perfmetrics-4.0.0/src/perfmetrics.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/testing.rst
 scripts/install.ps1
 scripts/run_with_env.cmd
+scripts/releases/geventrel.sh
+scripts/releases/geventreleases.sh
 scripts/releases/make-manylinux
 src/perfmetrics/__init__.py
 src/perfmetrics/_metric.pxd
 src/perfmetrics/_util.py
 src/perfmetrics/clientstack.py
 src/perfmetrics/interfaces.py
 src/perfmetrics/metric.c
```

### Comparing `perfmetrics-3.3.0/tox.ini` & `perfmetrics-4.0.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = pypy,py27,py36,py37,py38,py39,py310,pypy3,py37,coverage
+envlist = py37,py38,py39,py310,py311,py312,pypy3,py37,coverage
 
 [testenv]
 extras =
      test
 commands =
          zope-testrunner --test-path=src  --auto-color --auto-progress [] # substitute with tox positional args
 
@@ -14,14 +14,14 @@
 basepython =
     python3
 commands =
     coverage run -m zope.testrunner --test-path=src []
     coverage report --fail-under=100
 deps =
     coverage
-    pyhamcrest < 2
+
 
 [testenv:docs]
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
 extras =
     docs
```

