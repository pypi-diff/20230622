# Comparing `tmp/sospice-0.0.2.tar.gz` & `tmp/sospice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sospice-0.0.2.tar", last modified: Thu Jun 22 10:04:07 2023, max compression
+gzip compressed data, was "sospice-0.0.3.tar", last modified: Thu Jun 22 21:36:06 2023, max compression
```

## Comparing `sospice-0.0.2.tar` & `sospice-0.0.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/
--rw-rw-r--   0 eric      (1001) eric      (1001)      112 2023-06-22 10:02:44.000000 sospice-0.0.2/.flake8
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.703499 sospice-0.0.2/.github/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.719499 sospice-0.0.2/.github/workflows/
--rw-rw-r--   0 eric      (1001) eric      (1001)     1313 2023-06-20 07:30:27.000000 sospice-0.0.2/.github/workflows/python-package.yml
--rw-rw-r--   0 eric      (1001) eric      (1001)     3130 2023-06-22 10:02:44.000000 sospice-0.0.2/.gitignore
--rw-rw-r--   0 eric      (1001) eric      (1001)      931 2023-06-03 17:29:19.000000 sospice-0.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 eric      (1001) eric      (1001)     1483 2023-04-28 17:14:31.000000 sospice-0.0.2/LICENSE
--rw-rw-r--   0 eric      (1001) eric      (1001)      190 2023-06-22 10:02:44.000000 sospice-0.0.2/Makefile
--rw-rw-r--   0 eric      (1001) eric      (1001)      854 2023-06-22 10:04:07.735499 sospice-0.0.2/PKG-INFO
--rw-rw-r--   0 eric      (1001) eric      (1001)     2461 2023-06-22 10:02:44.000000 sospice-0.0.2/README.rst
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.719499 sospice-0.0.2/docs/
--rw-rw-r--   0 eric      (1001) eric      (1001)      638 2023-04-26 09:59:38.000000 sospice-0.0.2/docs/Makefile
--rw-rw-r--   0 eric      (1001) eric      (1001)      804 2023-04-26 09:59:38.000000 sospice-0.0.2/docs/make.bat
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.723499 sospice-0.0.2/docs/source/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.707499 sospice-0.0.2/docs/source/_templates/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.723499 sospice-0.0.2/docs/source/_templates/autosummary/
--rw-rw-r--   0 eric      (1001) eric      (1001)       77 2023-06-22 10:02:44.000000 sospice-0.0.2/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      259 2023-06-22 10:02:44.000000 sospice-0.0.2/docs/source/api.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      201 2023-06-05 21:42:41.000000 sospice-0.0.2/docs/source/changelog.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)       40 2023-06-05 21:42:41.000000 sospice-0.0.2/docs/source/citation.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)     3465 2023-06-22 10:02:44.000000 sospice-0.0.2/docs/source/conf.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5558 2023-06-05 21:42:41.000000 sospice-0.0.2/docs/source/develop.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      394 2023-06-05 21:42:41.000000 sospice-0.0.2/docs/source/getting_started.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)     1076 2023-06-22 09:32:46.000000 sospice-0.0.2/docs/source/index.rst
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.723499 sospice-0.0.2/examples/
--rw-rw-r--   0 eric      (1001) eric      (1001)      104 2023-04-26 09:59:38.000000 sospice-0.0.2/examples/README.md
--rw-rw-r--   0 eric      (1001) eric      (1001)     1381 2023-06-22 10:02:44.000000 sospice-0.0.2/pyproject.toml
--rw-rw-r--   0 eric      (1001) eric      (1001)      243 2023-06-22 10:02:44.000000 sospice-0.0.2/requirements.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)       38 2023-06-22 10:04:07.735499 sospice-0.0.2/setup.cfg
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.723499 sospice-0.0.2/sospice/
--rw-rw-r--   0 eric      (1001) eric      (1001)      283 2023-06-13 15:46:15.000000 sospice-0.0.2/sospice/CITATION.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      123 2023-06-22 09:58:11.000000 sospice-0.0.2/sospice/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.727499 sospice-0.0.2/sospice/calibrate/
--rw-rw-r--   0 eric      (1001) eric      (1001)       39 2023-05-29 22:03:18.000000 sospice-0.0.2/sospice/calibrate/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.727499 sospice-0.0.2/sospice/calibrate/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/calibrate/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     2228 2023-06-03 14:31:07.000000 sospice-0.0.2/sospice/calibrate/tests/test_uncertainties.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1525 2023-06-03 17:30:17.000000 sospice-0.0.2/sospice/calibrate/uncertainties.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.727499 sospice-0.0.2/sospice/catalog/
--rw-rw-r--   0 eric      (1001) eric      (1001)       58 2023-06-22 10:02:44.000000 sospice-0.0.2/sospice/catalog/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5485 2023-06-22 10:02:44.000000 sospice-0.0.2/sospice/catalog/catalog.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1890 2023-06-22 10:02:44.000000 sospice-0.0.2/sospice/catalog/release.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/catalog/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/catalog/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     3638 2023-06-22 10:02:44.000000 sospice-0.0.2/sospice/catalog/tests/test_catalog.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      975 2023-06-22 10:02:44.000000 sospice-0.0.2/sospice/catalog/tests/test_release.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/data/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/data/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/data/calibration/
--rw-rw-r--   0 eric      (1001) eric      (1001)     2708 2023-05-12 20:53:10.000000 sospice-0.0.2/sospice/data/calibration/effective_area.sav
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/data/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/data/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/instrument_modelling/
--rw-rw-r--   0 eric      (1001) eric      (1001)       87 2023-06-14 09:12:07.000000 sospice-0.0.2/sospice/instrument_modelling/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5983 2023-05-31 21:34:22.000000 sospice-0.0.2/sospice/instrument_modelling/observation.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     4801 2023-06-01 21:25:28.000000 sospice-0.0.2/sospice/instrument_modelling/spice.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1666 2023-05-30 07:01:03.000000 sospice-0.0.2/sospice/instrument_modelling/study.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.731499 sospice-0.0.2/sospice/instrument_modelling/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-05-12 21:08:37.000000 sospice-0.0.2/sospice/instrument_modelling/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     2720 2023-05-31 22:03:33.000000 sospice-0.0.2/sospice/instrument_modelling/tests/test_observation.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     3183 2023-05-30 07:01:03.000000 sospice-0.0.2/sospice/instrument_modelling/tests/test_spice.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1473 2023-05-30 07:01:03.000000 sospice-0.0.2/sospice/instrument_modelling/tests/test_study.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/sospice/psf/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/psf/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/sospice/psf/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/psf/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/sospice/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 14:38:35.000000 sospice-0.0.2/sospice/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/sospice/util/
--rw-rw-r--   0 eric      (1001) eric      (1001)       21 2023-05-13 07:03:48.000000 sospice-0.0.2/sospice/util/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      405 2023-05-30 06:42:04.000000 sospice-0.0.2/sospice/util/rss.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.735499 sospice-0.0.2/sospice/util/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.2/sospice/util/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      316 2023-06-01 22:04:59.000000 sospice-0.0.2/sospice/util/tests/test_rss.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 10:04:07.727499 sospice-0.0.2/sospice.egg-info/
--rw-rw-r--   0 eric      (1001) eric      (1001)      854 2023-06-22 10:04:07.000000 sospice-0.0.2/sospice.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1001) eric      (1001)     1583 2023-06-22 10:04:07.000000 sospice-0.0.2/sospice.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)        1 2023-06-22 10:04:07.000000 sospice-0.0.2/sospice.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)      243 2023-06-22 10:04:07.000000 sospice-0.0.2/sospice.egg-info/requires.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)        8 2023-06-22 10:04:07.000000 sospice-0.0.2/sospice.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      112 2023-06-22 21:35:39.000000 sospice-0.0.3/.flake8
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/.github/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/.github/workflows/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1313 2023-06-20 07:30:27.000000 sospice-0.0.3/.github/workflows/python-package.yml
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3130 2023-06-22 21:35:39.000000 sospice-0.0.3/.gitignore
+-rw-rw-r--   0 eric      (1001) eric      (1001)      931 2023-06-03 17:29:19.000000 sospice-0.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1483 2023-04-28 17:14:31.000000 sospice-0.0.3/LICENSE
+-rw-rw-r--   0 eric      (1001) eric      (1001)      467 2023-06-22 21:35:39.000000 sospice-0.0.3/Makefile
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3313 2023-06-22 21:36:06.199324 sospice-0.0.3/PKG-INFO
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2461 2023-06-22 21:35:39.000000 sospice-0.0.3/README.rst
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/docs/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      638 2023-04-26 09:59:38.000000 sospice-0.0.3/docs/Makefile
+-rw-rw-r--   0 eric      (1001) eric      (1001)      804 2023-04-26 09:59:38.000000 sospice-0.0.3/docs/make.bat
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/docs/source/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/docs/source/_templates/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/docs/source/_templates/autosummary/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       77 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      259 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/api.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      201 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/changelog.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)       40 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/citation.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3465 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/conf.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5558 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/develop.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      394 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/getting_started.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1076 2023-06-22 09:32:46.000000 sospice-0.0.3/docs/source/index.rst
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/examples/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      104 2023-04-26 09:59:38.000000 sospice-0.0.3/examples/README.md
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1381 2023-06-22 21:35:39.000000 sospice-0.0.3/pyproject.toml
+-rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-22 21:35:39.000000 sospice-0.0.3/requirements.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)       38 2023-06-22 21:36:06.199324 sospice-0.0.3/setup.cfg
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      283 2023-06-13 15:46:15.000000 sospice-0.0.3/sospice/CITATION.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      100 2023-06-22 21:34:09.000000 sospice-0.0.3/sospice/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/calibrate/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       39 2023-05-29 22:03:18.000000 sospice-0.0.3/sospice/calibrate/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/calibrate/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/calibrate/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2228 2023-06-03 14:31:07.000000 sospice-0.0.3/sospice/calibrate/tests/test_uncertainties.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1525 2023-06-03 17:30:17.000000 sospice-0.0.3/sospice/calibrate/uncertainties.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/catalog/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       58 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5485 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/catalog.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1890 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/release.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/catalog/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/catalog/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3638 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/tests/test_catalog.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      975 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/tests/test_release.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/data/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/calibration/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2708 2023-05-12 20:53:10.000000 sospice-0.0.3/sospice/data/calibration/effective_area.sav
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/data/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/instrument_modelling/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       87 2023-06-14 09:12:07.000000 sospice-0.0.3/sospice/instrument_modelling/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5983 2023-05-31 21:34:22.000000 sospice-0.0.3/sospice/instrument_modelling/observation.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     4801 2023-06-01 21:25:28.000000 sospice-0.0.3/sospice/instrument_modelling/spice.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1666 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/study.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/instrument_modelling/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-05-12 21:08:37.000000 sospice-0.0.3/sospice/instrument_modelling/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2720 2023-05-31 22:03:33.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_observation.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3183 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_spice.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1473 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_study.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/psf/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/psf/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/psf/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/psf/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 14:38:35.000000 sospice-0.0.3/sospice/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/util/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       21 2023-05-13 07:03:48.000000 sospice-0.0.3/sospice/util/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      405 2023-05-30 06:42:04.000000 sospice-0.0.3/sospice/util/rss.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/util/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/util/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      316 2023-06-01 22:04:59.000000 sospice-0.0.3/sospice/util/tests/test_rss.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice.egg-info/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3313 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1583 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)        1 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)        8 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/top_level.txt
```

### Comparing `sospice-0.0.2/.github/workflows/python-package.yml` & `sospice-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/.gitignore` & `sospice-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/.pre-commit-config.yaml` & `sospice-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/LICENSE` & `sospice-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/README.rst` & `sospice-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/docs/Makefile` & `sospice-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/docs/make.bat` & `sospice-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/docs/source/conf.py` & `sospice-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/docs/source/develop.rst` & `sospice-0.0.3/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/docs/source/index.rst` & `sospice-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/pyproject.toml` & `sospice-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 [project]
 name = "sospice"
 authors = [
   { name="SPICE consortium", email="spice-github.ias@universite-paris-saclay.fr" },
 ]
 description = "Python data analysis tools for Solar Orbiter/SPICE"
-readme = "README.md"
-requires-python = ">=3.7"
+readme = "README.rst"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
-
 dynamic = ["version", "dependencies"]
 
 [tool.setuptools.dynamic]
 version = {attr = "sospice.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 #[project.optional-dependencies]
```

### Comparing `sospice-0.0.2/sospice/calibrate/tests/test_uncertainties.py` & `sospice-0.0.3/sospice/calibrate/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/calibrate/uncertainties.py` & `sospice-0.0.3/sospice/calibrate/uncertainties.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/catalog/catalog.py` & `sospice-0.0.3/sospice/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/catalog/release.py` & `sospice-0.0.3/sospice/catalog/release.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/catalog/tests/test_catalog.py` & `sospice-0.0.3/sospice/catalog/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/catalog/tests/test_release.py` & `sospice-0.0.3/sospice/catalog/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/data/calibration/effective_area.sav` & `sospice-0.0.3/sospice/data/calibration/effective_area.sav`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/observation.py` & `sospice-0.0.3/sospice/instrument_modelling/observation.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/spice.py` & `sospice-0.0.3/sospice/instrument_modelling/spice.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/study.py` & `sospice-0.0.3/sospice/instrument_modelling/study.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/tests/test_observation.py` & `sospice-0.0.3/sospice/instrument_modelling/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/tests/test_spice.py` & `sospice-0.0.3/sospice/instrument_modelling/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice/instrument_modelling/tests/test_study.py` & `sospice-0.0.3/sospice/instrument_modelling/tests/test_study.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.2/sospice.egg-info/SOURCES.txt` & `sospice-0.0.3/sospice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

