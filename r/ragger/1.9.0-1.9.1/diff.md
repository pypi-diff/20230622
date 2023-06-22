# Comparing `tmp/ragger-1.9.0.tar.gz` & `tmp/ragger-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragger-1.9.0.tar", last modified: Wed Jun 21 12:42:17 2023, max compression
+gzip compressed data, was "ragger-1.9.1.tar", last modified: Thu Jun 22 16:29:25 2023, max compression
```

## Comparing `ragger-1.9.0.tar` & `ragger-1.9.1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.058054 ragger-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 12:42:02.000000 ragger-1.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.038054 ragger-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-21 12:42:02.000000 ragger-1.9.0/.github/workflows/build_and_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-21 12:42:02.000000 ragger-1.9.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 12:42:02.000000 ragger-1.9.0/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 12:42:02.000000 ragger-1.9.0/.github/workflows/fast-checks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 12:42:02.000000 ragger-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-21 12:42:02.000000 ragger-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 12:42:02.000000 ragger-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 12:42:02.000000 ragger-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-21 12:42:17.058054 ragger-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-21 12:42:02.000000 ragger-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/_static/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/navigate.draw
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/navigate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/ragger.png
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/stax_infos.png
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/stax_welcome.png
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/usage.draw
--rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/images/usage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/rationale.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/source.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/tutorial_conftest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/tutorial_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-21 12:42:02.000000 ragger-1.9.0/doc/tutorial_screen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 12:42:02.000000 ragger-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-21 12:42:17.058054 ragger-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.038054 ragger-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.042054 ragger-1.9.0/src/ragger/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 12:42:16.000000 ragger-1.9.0/src/ragger/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/ledgercomm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/ledgerwallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/physical_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/speculos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/backend/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/bip/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/bip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/bip/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/bip/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/conftest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/conftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/conftest/base_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/conftest/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/firmware/stax/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/stax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/stax/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/stax/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/stax/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/stax/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/firmware/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/src/ragger/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanos_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanos_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanos_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanosp_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanosp_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanosp_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanox_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanox_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/nanox_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/stax_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/assets/touch_action.png
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/gui/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/src/ragger/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/navigator/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/navigator/nano_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/navigator/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/navigator/stax_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/src/ragger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-21 12:42:02.000000 ragger-1.9.0/src/ragger/utils/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.046054 ragger-1.9.0/src/ragger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-21 12:42:16.000000 ragger-1.9.0/src/ragger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-21 12:42:17.000000 ragger-1.9.0/src/ragger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:42:16.000000 ragger-1.9.0/src/ragger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-21 12:42:17.000000 ragger-1.9.0/src/ragger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 12:42:17.000000 ragger-1.9.0/src/ragger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/template/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 12:42:02.000000 ragger-1.9.0/template/.dispatch_to_your_test_folder
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 12:42:02.000000 ragger-1.9.0/template/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-21 12:42:02.000000 ragger-1.9.0/template/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/tests/functional/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/backend/test_speculos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/tests/functional/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/navigator/test_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/functional/test_boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.038054 ragger-1.9.0/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.038054 ragger-1.9.0/tests/snapshots/nanos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.050054 ragger-1.9.0/tests/snapshots/nanos/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/generic/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/generic/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/generic/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/generic/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/generic/00004.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00004.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00005.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00006.png
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare/00007.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare_no_golden/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare_no_golden/00000.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00001.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/snapshots/nanos/test_navigate_until_text_and_compare/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_until_text_and_compare/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_until_text_and_compare/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_until_text_and_compare/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/nanos/test_navigate_until_text_and_compare/00003.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.038054 ragger-1.9.0/tests/snapshots/stax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/snapshots/stax/waiting_screen/
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/stax/waiting_screen/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/stax/waiting_screen/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/stax/waiting_screen/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/stax/waiting_screen/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/snapshots/stax/waiting_screen/00004.png
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/unit/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_ledgercomm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_ledgerwallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_physical_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_speculos.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/backend/test_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.054054 ragger-1.9.0/tests/unit/bip/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/bip/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/bip/test_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.058054 ragger-1.9.0/tests/unit/firmware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.058054 ragger-1.9.0/tests/unit/firmware/stax/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/firmware/stax/test_layouts__Layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/firmware/stax/test_screen_FullScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/firmware/stax/test_screen_MetaScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/firmware/test_structs_Firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/firmware/test_versions_VersionManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.058054 ragger-1.9.0/tests/unit/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/navigator/test_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/test_error_ApplicationError.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:17.058054 ragger-1.9.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/utils/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 12:42:02.000000 ragger-1.9.0/tests/unit/utils/test_structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 16:29:13.000000 ragger-1.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.150336 ragger-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.158336 ragger-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/build_and_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/fast-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 16:29:13.000000 ragger-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-22 16:29:13.000000 ragger-1.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 16:29:13.000000 ragger-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 16:29:13.000000 ragger-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-22 16:29:25.178336 ragger-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-22 16:29:13.000000 ragger-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.158336 ragger-1.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/_static/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/navigate.draw
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/navigate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/ragger.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/stax_infos.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/stax_welcome.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/usage.draw
+-rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/usage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/rationale.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/source.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_conftest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_screen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 16:29:13.000000 ragger-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-22 16:29:25.178336 ragger-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.150336 ragger-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/src/ragger/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/ledgercomm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/ledgerwallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/physical_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/speculos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/bip/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/conftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/base_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/firmware/stax/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/stax_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/touch_action.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/nano_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/stax_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/src/ragger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 16:29:13.000000 ragger-1.9.1/template/.dispatch_to_your_test_folder
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-22 16:29:13.000000 ragger-1.9.1/template/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 16:29:13.000000 ragger-1.9.1/template/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/backend/test_speculos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/navigator/test_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/test_boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/nanos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00004.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00004.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00005.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00006.png
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00007.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_no_golden/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_no_golden/00000.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00001.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00003.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/stax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/stax/waiting_screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00004.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_ledgercomm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_ledgerwallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_physical_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_speculos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/bip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/bip/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/bip/test_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/firmware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/firmware/stax/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_layouts__Layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_screen_FullScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_screen_MetaScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/test_structs_Firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/test_versions_VersionManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/navigator/test_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/test_error_ApplicationError.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_structs.py
```

### Comparing `ragger-1.9.0/.github/workflows/build_and_tests.yml` & `ragger-1.9.1/.github/workflows/build_and_tests.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/.github/workflows/codeql-analysis.yml` & `ragger-1.9.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/.github/workflows/documentation.yml` & `ragger-1.9.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/.github/workflows/fast-checks.yml` & `ragger-1.9.1/.github/workflows/fast-checks.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/CHANGELOG.md` & `ragger-1.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.1] - 2023-06-22
+
+### Fixed
+- speculos: Only pause ticker during navigation steps
+
 ## [1.9.0] - 2023-06-21
 
 ### Changed
 - speculos: Default touch duration changed from 0.5sec to 0.1sec
 - speculos: Control the ticker allowing to avoid any race issue when comparing screen and accessing OCR result
 - speculos: Bump minimal speculos version to 0.2.5
```

### Comparing `ragger-1.9.0/LICENSE` & `ragger-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/PKG-INFO` & `ragger-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragger
-Version: 1.9.0
+Version: 1.9.1
 Summary: Testing framework using Speculos and LedgerComm as backends
 Home-page: https://github.com/LedgerHQ/ragger
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/ragger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -97,14 +97,17 @@
 * `exchange_async`: send a formatted APDU and give back the control to the caller (asynchronous).
 * `exchange_async_raw`: send a raw APDU and give back the control to the caller.
 * `right_click`: perform a right click on a device.
 * `left_click`: perform a left click on a device.
 * `both_click`: perform a click on both buttons (left + right) of a device.
 * `finger_touch`: performs a finger touch on the device screen.
 * `compare_screen_with_snapshot`: compare the current device screen with the provided snapshot.
+* `pause_ticker`: pause the backend time.
+* `resume_ticker`: resume the backend time.
+* `send_tick`: request the backend to increase time by a single step.
 
 The `src/ragger/navigator/navigator.py` file describes the methods that can be implemented by the
 different device navigators and that allow to interact with an emulated device:
 * `navigate`: navigate on the device according to a set of navigation instructions provided.
 * `navigate_and_compare`: navigate on the device according to a set of navigation instructions
   provided then compare each step screenshot with "golden images".
 * `navigate_until_snap`: navigate on the device until a snapshot is found and then validate.
```

### Comparing `ragger-1.9.0/README.md` & `ragger-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 * `exchange_async`: send a formatted APDU and give back the control to the caller (asynchronous).
 * `exchange_async_raw`: send a raw APDU and give back the control to the caller.
 * `right_click`: perform a right click on a device.
 * `left_click`: perform a left click on a device.
 * `both_click`: perform a click on both buttons (left + right) of a device.
 * `finger_touch`: performs a finger touch on the device screen.
 * `compare_screen_with_snapshot`: compare the current device screen with the provided snapshot.
+* `pause_ticker`: pause the backend time.
+* `resume_ticker`: resume the backend time.
+* `send_tick`: request the backend to increase time by a single step.
 
 The `src/ragger/navigator/navigator.py` file describes the methods that can be implemented by the
 different device navigators and that allow to interact with an emulated device:
 * `navigate`: navigate on the device according to a set of navigation instructions provided.
 * `navigate_and_compare`: navigate on the device according to a set of navigation instructions
   provided then compare each step screenshot with "golden images".
 * `navigate_until_snap`: navigate on the device until a snapshot is found and then validate.
```

### Comparing `ragger-1.9.0/doc/Makefile` & `ragger-1.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/conf.py` & `ragger-1.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/faq.rst` & `ragger-1.9.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/glossary.rst` & `ragger-1.9.1/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/navigate.draw` & `ragger-1.9.1/doc/images/navigate.draw`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/navigate.svg` & `ragger-1.9.1/doc/images/navigate.svg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/stax_infos.png` & `ragger-1.9.1/doc/images/stax_infos.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/stax_welcome.png` & `ragger-1.9.1/doc/images/stax_welcome.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/usage.draw` & `ragger-1.9.1/doc/images/usage.draw`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/images/usage.svg` & `ragger-1.9.1/doc/images/usage.svg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/index.rst` & `ragger-1.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/installation.rst` & `ragger-1.9.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/rationale.rst` & `ragger-1.9.1/doc/rationale.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/source.rst` & `ragger-1.9.1/doc/source.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/tutorial_conftest.rst` & `ragger-1.9.1/doc/tutorial_conftest.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/tutorial_installation.rst` & `ragger-1.9.1/doc/tutorial_installation.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/doc/tutorial_screen.rst` & `ragger-1.9.1/doc/tutorial_screen.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/setup.cfg` & `ragger-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/__init__.py` & `ragger-1.9.1/src/ragger/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/backend/__init__.py` & `ragger-1.9.1/src/ragger/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/backend/interface.py` & `ragger-1.9.1/src/ragger/backend/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -490,7 +490,52 @@
         action is performed on the device.
 
         :return: Current screen content as an opaque type depending on backend
                  implem.
         :rtype: Any
         """
         raise NotImplementedError
+
+    @abstractmethod
+    def pause_ticker(self) -> None:
+        """
+        Pause the backend time.
+
+        This method may be left void on backends connecting to physical devices,
+        where a physical interaction must be performed instead.
+        This will prevent the instrumentation to fail (the void method won't
+        raise `NotImplementedError`).
+
+        :return: None
+        :rtype: NoneType
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def resume_ticker(self) -> None:
+        """
+        Resume the backend time.
+
+        This method may be left void on backends connecting to physical devices,
+        where a physical interaction must be performed instead.
+        This will prevent the instrumentation to fail (the void method won't
+        raise `NotImplementedError`).
+
+        :return: None
+        :rtype: NoneType
+        """
+        pass
+
+    @abstractmethod
+    def send_tick(self) -> None:
+        """
+        Request the backend to increase time by a single step.
+
+        This method may be left void on backends connecting to physical devices,
+        where a physical interaction must be performed instead.
+        This will prevent the instrumentation to fail (the void method won't
+        raise `NotImplementedError`).
+
+        :return: None
+        :rtype: NoneType
+        """
+        pass
```

### Comparing `ragger-1.9.0/src/ragger/backend/ledgercomm.py` & `ragger-1.9.1/src/ragger/backend/ledgercomm.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/backend/ledgerwallet.py` & `ragger-1.9.1/src/ragger/backend/ledgerwallet.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/backend/physical_backend.py` & `ragger-1.9.1/src/ragger/backend/physical_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,7 +113,16 @@
             return self._ui.check_text(text)
 
     def wait_for_screen_change(self, timeout: float = 10.0) -> None:
         return
 
     def get_current_screen_content(self) -> List:
         return list()
+
+    def pause_ticker(self) -> None:
+        pass
+
+    def resume_ticker(self) -> None:
+        pass
+
+    def send_tick(self) -> None:
+        pass
```

### Comparing `ragger-1.9.0/src/ragger/backend/speculos.py` & `ragger-1.9.1/src/ragger/backend/speculos.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    limitations under the License.
 """
 from contextlib import contextmanager
 from io import BytesIO
 from pathlib import Path
 from PIL import Image
 from typing import Optional, Generator
-from time import time
+from time import time, sleep
 from json import dumps
 
 from speculos.client import SpeculosClient, screenshot_equal, ApduResponse, ApduException
 from speculos.mcu.seproxyhal import TICKER_DELAY
 
 from ragger.error import ExceptionRAPDU
 from ragger.firmware import Firmware
@@ -73,14 +73,15 @@
             kwargs[self._ARGS_KEY] = args
         self._client: SpeculosClient = SpeculosClient(app=str(application),
                                                       api_url=self.url,
                                                       **kwargs)
         self._pending: Optional[ApduResponse] = None
         self._last_screenshot: Optional[BytesIO] = None
         self._home_screenshot: Optional[BytesIO] = None
+        self._ticker_paused_count = 0
 
     @property
     def url(self) -> str:
         return f"http://{self._host}:{self._port}"
 
     def _retrieve_client_screen_content(self) -> dict:
         raw_content = self._client.get_current_screen_content()
@@ -92,30 +93,37 @@
         # what we want here.
         events = []
         for event in raw_content.get("events", []):
             if event.get("text", "").strip():
                 events.append(event)
         return {"events": events}
 
+    def pause_ticker(self) -> None:
+        if self._ticker_paused_count == 0:
+            self._client.ticker_ctl("pause")
+        self._ticker_paused_count += 1
+
+    def resume_ticker(self) -> None:
+        self._ticker_paused_count -= 1
+        if self._ticker_paused_count == 0:
+            self._client.ticker_ctl("resume")
+        assert self._ticker_paused_count >= 0
+
+    def send_tick(self) -> None:
+        self._client.ticker_ctl("single-step")
+
     def __enter__(self) -> "SpeculosBackend":
         self.logger.info(f"Starting {self.__class__.__name__} stream")
         self._client.__enter__()
 
-        # Disable Speculos autonomous ticker thread.
-        # This avoid timing issue with OCR or screenshot comparison.
-        self._client.ticker_ctl("pause")
-
-        # Send a ticker event and let the app process it
-        self._client.ticker_ctl("single-step")
-
         # Wait until some text is displayed on the screen.
         start = time()
         while not self._retrieve_client_screen_content()["events"]:
             # Send a ticker event and let the app process it
-            self._client.ticker_ctl("single-step")
+            sleep(0.1)
             if (time() - start > 20.0):
                 raise TimeoutError(
                     "Timeout waiting for screen content upon Ragger Speculos Instance start")
 
         self._last_screenshot = BytesIO(self._client.get_screenshot())
 
         # Save current screenshot as _home_screenshot.
@@ -211,15 +219,15 @@
     def wait_for_screen_change(self, timeout: float = 10.0) -> None:
         screenshot = BytesIO(self._client.get_screenshot())
         for _ in range(int(timeout / TICKER_DELAY)):
             if not screenshot_equal(screenshot, self._last_screenshot):
                 break
 
             # Send a ticker event and let the app process it
-            self._client.ticker_ctl("single-step")
+            self.send_tick()
             screenshot = BytesIO(self._client.get_screenshot())
         else:
             raise TimeoutError("Timeout waiting for screen change")
 
         # Update self._last_screenshot to use it as reference for next calls
         self._last_screenshot = screenshot
```

### Comparing `ragger-1.9.0/src/ragger/backend/stub.py` & `ragger-1.9.1/src/ragger/backend/stub.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,7 +77,16 @@
         pass
 
     def compare_screen_with_text(self, text: str) -> bool:
         return True
 
     def get_current_screen_content(self) -> Any:
         pass
+
+    def pause_ticker(self) -> None:
+        pass
+
+    def resume_ticker(self) -> None:
+        pass
+
+    def send_tick(self) -> None:
+        pass
```

### Comparing `ragger-1.9.0/src/ragger/bip/__init__.py` & `ragger-1.9.1/src/ragger/bip/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/bip/path.py` & `ragger-1.9.1/src/ragger/bip/path.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/bip/seed.py` & `ragger-1.9.1/src/ragger/bip/seed.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/conftest/base_conftest.py` & `ragger-1.9.1/src/ragger/conftest/base_conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/conftest/configuration.py` & `ragger-1.9.1/src/ragger/conftest/configuration.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/error.py` & `ragger-1.9.1/src/ragger/error.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/__init__.py` & `ragger-1.9.1/src/ragger/firmware/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/stax/__init__.py` & `ragger-1.9.1/src/ragger/firmware/stax/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/stax/layouts.py` & `ragger-1.9.1/src/ragger/firmware/stax/layouts.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/stax/positions.py` & `ragger-1.9.1/src/ragger/firmware/stax/positions.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/stax/screen.py` & `ragger-1.9.1/src/ragger/firmware/stax/screen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/stax/use_cases.py` & `ragger-1.9.1/src/ragger/firmware/stax/use_cases.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/structs.py` & `ragger-1.9.1/src/ragger/firmware/structs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/firmware/versions.py` & `ragger-1.9.1/src/ragger/firmware/versions.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/__init__.py` & `ragger-1.9.1/src/ragger/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanos_body.png` & `ragger-1.9.1/src/ragger/gui/assets/nanos_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanos_leftbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanos_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanos_rightbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanos_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanosp_body.png` & `ragger-1.9.1/src/ragger/gui/assets/nanosp_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanosp_leftbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanosp_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanosp_rightbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanosp_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanox_body.png` & `ragger-1.9.1/src/ragger/gui/assets/nanox_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanox_leftbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanox_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/nanox_rightbutton.png` & `ragger-1.9.1/src/ragger/gui/assets/nanox_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/stax_body.png` & `ragger-1.9.1/src/ragger/gui/assets/stax_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/assets/touch_action.png` & `ragger-1.9.1/src/ragger/gui/assets/touch_action.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/interface.py` & `ragger-1.9.1/src/ragger/gui/interface.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/gui/process.py` & `ragger-1.9.1/src/ragger/gui/process.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/logger.py` & `ragger-1.9.1/src/ragger/logger.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/navigator/__init__.py` & `ragger-1.9.1/src/ragger/navigator/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/navigator/instruction.py` & `ragger-1.9.1/src/ragger/navigator/instruction.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/navigator/nano_navigator.py` & `ragger-1.9.1/src/ragger/navigator/nano_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/navigator/navigator.py` & `ragger-1.9.1/src/ragger/navigator/navigator.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,16 @@
 
         :raises ValueError: If one of the snapshots does not match.
 
         :return: None
         :rtype: NoneType
         """
 
+        self._backend.pause_ticker()
+
         # Navigation initialization: no-op instruction to:
         # - wait for screen change depending on screen_change_before_first_instruction.
         #   this is necessary:
         #   - when an APDU was just sent and we want to make sure the screen already
         #     displays the first review page.
         #   - when called to finish the execution of a navigate_until_text() call.
         # - compare the initial screen content with the golden reference if path and
@@ -239,14 +241,16 @@
                 # => no wait_for_screen_change()
                 # => no screenshot comparison
                 self._run_instruction(instruction,
                                       timeout,
                                       wait_for_screen_change=False,
                                       snap_idx=snap_start_idx + idx + 1)
 
+        self._backend.resume_ticker()
+
     def navigate(self,
                  instructions: List[Union[NavIns, NavInsID]],
                  timeout: float = 10.0,
                  screen_change_before_first_instruction: bool = True,
                  screen_change_after_last_instruction: bool = True) -> None:
         """
         Navigate on the device according to a set of navigation instructions provided.
@@ -440,14 +444,16 @@
         start = time()
         if not isinstance(self._backend, SpeculosBackend):
             # Update timeout default value for other backends. User needs time to
             # to perform actions.
             if timeout == 30:
                 timeout = 200
 
+        self._backend.pause_ticker()
+
         # Navigation initialization: no-op instruction to:
         # - wait for screen change depending on screen_change_before_first_instruction.
         #   this is necessary when an APDU was just sent and we want to make sure the
         #   screen already displays the first review page.
         # - compare the initial screen content with the golden reference if path and
         #   test_case_name are valid.
         self._run_instruction(NavIns(NavInsID.WAIT, (0, )),
@@ -485,14 +491,16 @@
                 test_case_name,
                 validation_instructions,
                 timeout=remaining,
                 screen_change_before_first_instruction=False,
                 screen_change_after_last_instruction=screen_change_after_last_instruction,
                 snap_start_idx=idx)
 
+        self._backend.resume_ticker()
+
     def navigate_until_text(self,
                             navigate_instruction: Union[NavIns, NavInsID],
                             validation_instructions: List[Union[NavIns, NavInsID]],
                             text: str,
                             timeout: int = 300,
                             screen_change_before_first_instruction: bool = True,
                             screen_change_after_last_instruction: bool = True) -> None:
```

### Comparing `ragger-1.9.0/src/ragger/navigator/stax_navigator.py` & `ragger-1.9.1/src/ragger/navigator/stax_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/utils/__init__.py` & `ragger-1.9.1/src/ragger/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/utils/misc.py` & `ragger-1.9.1/src/ragger/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/utils/packing.py` & `ragger-1.9.1/src/ragger/utils/packing.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger/utils/structs.py` & `ragger-1.9.1/src/ragger/utils/structs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/src/ragger.egg-info/PKG-INFO` & `ragger-1.9.1/src/ragger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragger
-Version: 1.9.0
+Version: 1.9.1
 Summary: Testing framework using Speculos and LedgerComm as backends
 Home-page: https://github.com/LedgerHQ/ragger
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/ragger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -97,14 +97,17 @@
 * `exchange_async`: send a formatted APDU and give back the control to the caller (asynchronous).
 * `exchange_async_raw`: send a raw APDU and give back the control to the caller.
 * `right_click`: perform a right click on a device.
 * `left_click`: perform a left click on a device.
 * `both_click`: perform a click on both buttons (left + right) of a device.
 * `finger_touch`: performs a finger touch on the device screen.
 * `compare_screen_with_snapshot`: compare the current device screen with the provided snapshot.
+* `pause_ticker`: pause the backend time.
+* `resume_ticker`: resume the backend time.
+* `send_tick`: request the backend to increase time by a single step.
 
 The `src/ragger/navigator/navigator.py` file describes the methods that can be implemented by the
 different device navigators and that allow to interact with an emulated device:
 * `navigate`: navigate on the device according to a set of navigation instructions provided.
 * `navigate_and_compare`: navigate on the device according to a set of navigation instructions
   provided then compare each step screenshot with "golden images".
 * `navigate_until_snap`: navigate on the device until a snapshot is found and then validate.
```

### Comparing `ragger-1.9.0/src/ragger.egg-info/SOURCES.txt` & `ragger-1.9.1/src/ragger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/template/conftest.py` & `ragger-1.9.1/template/conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/template/usage.md` & `ragger-1.9.1/template/usage.md`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/conftest.py` & `ragger-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/functional/backend/test_speculos.py` & `ragger-1.9.1/tests/functional/backend/test_speculos.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/functional/navigator/test_navigator.py` & `ragger-1.9.1/tests/functional/navigator/test_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/functional/test_boilerplate.py` & `ragger-1.9.1/tests/functional/test_boilerplate.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/snapshots/stax/waiting_screen/00000.png` & `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00000.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/snapshots/stax/waiting_screen/00001.png` & `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00001.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/snapshots/stax/waiting_screen/00002.png` & `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00002.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/snapshots/stax/waiting_screen/00003.png` & `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00003.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/snapshots/stax/waiting_screen/00004.png` & `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00004.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/stubs.py` & `ragger-1.9.1/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/backend/test_interface.py` & `ragger-1.9.1/tests/unit/backend/test_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 
     def compare_screen_with_text(self, text: str):
         return self.mock.compare_screen_with_text()
 
     def get_current_screen_content(self):
         return self.mock.get_current_screen_content()
 
+    def pause_ticker(self) -> None:
+        pass
+
+    def resume_ticker(self) -> None:
+        pass
+
+    def send_tick(self) -> None:
+        pass
+
 
 class TestBackendInterface(TestCase):
 
     def setUp(self):
         self.firmware = _Firmware("nanos", "2.0.1", "other")
         self.errors = (ExceptionRAPDU(0x8888, "ERROR1"), ExceptionRAPDU(0x7777, "ERROR2"))
         self.valid_statuses = (0x9000, 0x9001, 0x9002)
```

### Comparing `ragger-1.9.0/tests/unit/backend/test_ledgercomm.py` & `ragger-1.9.1/tests/unit/backend/test_ledgercomm.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/backend/test_ledgerwallet.py` & `ragger-1.9.1/tests/unit/backend/test_ledgerwallet.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/backend/test_physical_backend.py` & `ragger-1.9.1/tests/unit/backend/test_physical_backend.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/backend/test_speculos.py` & `ragger-1.9.1/tests/unit/backend/test_speculos.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/bip/test_path.py` & `ragger-1.9.1/tests/unit/bip/test_path.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/bip/test_seed.py` & `ragger-1.9.1/tests/unit/bip/test_seed.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/firmware/stax/test_layouts__Layout.py` & `ragger-1.9.1/tests/unit/firmware/stax/test_layouts__Layout.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/firmware/stax/test_screen_FullScreen.py` & `ragger-1.9.1/tests/unit/firmware/stax/test_screen_FullScreen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/firmware/stax/test_screen_MetaScreen.py` & `ragger-1.9.1/tests/unit/firmware/stax/test_screen_MetaScreen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/firmware/test_structs_Firmware.py` & `ragger-1.9.1/tests/unit/firmware/test_structs_Firmware.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/firmware/test_versions_VersionManager.py` & `ragger-1.9.1/tests/unit/firmware/test_versions_VersionManager.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/navigator/test_navigator.py` & `ragger-1.9.1/tests/unit/navigator/test_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/utils/test_misc.py` & `ragger-1.9.1/tests/unit/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.0/tests/unit/utils/test_packing.py` & `ragger-1.9.1/tests/unit/utils/test_packing.py`

 * *Files identical despite different names*

