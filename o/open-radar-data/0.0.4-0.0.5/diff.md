# Comparing `tmp/open-radar-data-0.0.4.tar.gz` & `tmp/open-radar-data-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-radar-data-0.0.4.tar", last modified: Wed Feb  1 10:38:40 2023, max compression
+gzip compressed data, was "open-radar-data-0.0.5.tar", last modified: Thu Jun 22 16:06:34 2023, max compression
```

## Comparing `open-radar-data-0.0.4.tar` & `open-radar-data-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.585606 open-radar-data-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-01 10:38:21.000000 open-radar-data-0.0.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/make_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/open_radar_data/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/open_radar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/open_radar_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/open_radar_data/registry.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/open_radar_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/open_radar_data/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/open_radar_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-01 10:38:40.000000 open-radar-data-0.0.4/open_radar_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-01 10:38:40.589606 open-radar-data-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-01 10:38:22.000000 open-radar-data-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.905472 open-radar-data-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 16:06:06.000000 open-radar-data-0.0.5/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/make_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/open_radar_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/open_radar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/open_radar_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/open_radar_data/registry.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/open_radar_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/open_radar_data/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 16:06:33.000000 open-radar-data-0.0.5/open_radar_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:34.901471 open-radar-data-0.0.5/open_radar_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-22 16:06:33.000000 open-radar-data-0.0.5/open_radar_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 16:06:34.000000 open-radar-data-0.0.5/open_radar_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:06:33.000000 open-radar-data-0.0.5/open_radar_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 16:06:33.000000 open-radar-data-0.0.5/open_radar_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 16:06:33.000000 open-radar-data-0.0.5/open_radar_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 16:06:07.000000 open-radar-data-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:06:34.905472 open-radar-data-0.0.5/setup.cfg
```

### Comparing `open-radar-data-0.0.4/.github/workflows/ci.yaml` & `open-radar-data-0.0.5/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: CI
 env:
-  micromamba_version: 1.1
+  micromamba_version: 1.3
 
 on:
   push:
   pull_request:
   workflow_dispatch: # allows you to trigger manually
 
 jobs:
@@ -49,14 +49,14 @@
         run: |
           python -m pip install -e .
           conda list
       - name: Run Tests
         run: |
           python -m pytest --cov=./ --cov-report=xml --verbose
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `open-radar-data-0.0.4/.github/workflows/pypi-release.yml` & `open-radar-data-0.0.5/.github/workflows/pypi-release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         name: Install Python
         with:
-          python-version: 3.8
+          python-version: 3.11
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
         run: |
           git clean -xdf
           git restore -SW .
           python -m build --sdist --wheel .
       - name: Check built artifacts
         run: |
           python -m twine check dist/*
           pwd
-          if [ -f dist/pythia-datasets-0.0.0.tar.gz ]; then
+          if [ -f dist/open-radar-data-0.0.0.tar.gz ]; then
             echo "❌ INVALID VERSION NUMBER"
             exit 1
           else
             echo "✅ Looks good"
           fi
       - uses: actions/upload-artifact@v3
         with:
@@ -44,15 +44,15 @@
   test-built-dist:
     needs: build-artifacts
     runs-on: ubuntu-latest
     steps:
       - uses: actions/setup-python@v4
         name: Install Python
         with:
-          python-version: 3.8
+          python-version: 3.11
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: List contents of built dist
         run: |
           ls -ltrh
@@ -63,12 +63,12 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
           verbose: true
```

### Comparing `open-radar-data-0.0.4/.gitignore` & `open-radar-data-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.0.4/.pre-commit-config.yaml` & `open-radar-data-0.0.5/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
-
-  - repo: https://github.com/psf/black
-    rev: 22.8.0
-    hooks:
-      - id: black
-
-  - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.6
-    hooks:
-      - id: blackdoc
-
-  - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
     hooks:
-      - id: flake8
-
-  - repo: https://github.com/asottile/seed-isort-config
-    rev: v2.2.0
+      - id: pyupgrade
+        args:
+          - '--py39-plus'
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.252'
     hooks:
-      - id: seed-isort-config
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.7.1
+      - id: ruff
+        args: ['--fix']
+  - repo: https://github.com/psf/black
+    rev: 23.1.0
     hooks:
-      - id: prettier
+      - id: black
```

### Comparing `open-radar-data-0.0.4/LICENSE` & `open-radar-data-0.0.5/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 openradar
+Copyright (c) 2022-2023 openradar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `open-radar-data-0.0.4/PKG-INFO` & `open-radar-data-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 Metadata-Version: 2.1
 Name: open-radar-data
-Version: 0.0.4
-Summary: Provides utility functions for accessing data repository for Project Pythia examples/notebooks
-Home-page: https://github.com/openradar/open-radar-data
-Maintainer: Open Radar Team
-Maintainer-email: 
-License: MIT
-Project-URL: Documentation, https://github.com/openradar/open-radar-data
-Project-URL: Source, https://github.com/openradar/open-radar-data
-Project-URL: Tracker, https://github.com/openradar/open-radar-data/issues
-Keywords: Radar,Pooch
+Version: 0.0.5
+Summary: Provides utility functions for accessing data repository for openradar examples/notebooks
+Author: Open Radar Team
+License: MIT License
+        
+        Copyright (c) 2022-2023 openradar
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/openradar/open-radar-data
+Project-URL: documentation, https://github.com/openradar/open-radar-data
+Project-URL: repository, https://github.com/openradar/open-radar-data
+Project-URL: tracker, https://github.com/openradar/open-radar-data/issues
+Keywords: open-radar-data,xradar
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,20 +41,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Open-Radar-Data
+[![CI](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml/badge.svg)](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/open-radar-data.svg)](https://pypi.python.org/pypi/open-radar-data)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/open-radar-data.svg)](https://anaconda.org/conda-forge/open-radar-data)
 
 A place to share radar data with the community, shared between the open radar packages
 
 ## Sample data sets
 
-These files are used as sample data in Pythia Project examples/notebooks and are downloaded by `open-radar-data` package:
+These files are used as sample data in openradar examples/notebooks and are downloaded by `open-radar-data` package:
 
 - `0080_20210730_160000_01_02.scn.gz`
 - `2006_20220324_000000_000.scnx.gz`
 - `2013051000000600dBZ.vol`
 - `71_20181220_060628.pvol.h5`
 - `DWD-Vol-2_99999_20180601054047_00.h5`
 - `SUR210819000227.RAWKPJV`
@@ -42,14 +65,18 @@
 - `MLA2119412050U.nc`
 - `MLL2217907250U.003.nc`
 - `T_PAGZ35_C_ENMI_20170421090837.hdf`
 - `cfrad.20080604_002217_000_SPOL_v36_SUR.nc`
 - `cor-main131125105503.RAW2049`
 - `sample_sgp_data.nc`
 - `sample_rainbow_5_59.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.021559.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.024239.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.025840.nc`
+- `corcsapr2cmacppiM1.c1.20181111.030003.nc`
 
 ## Adding new datasets
 
 To add a new dataset file, please follow these steps:
 
 1. Add the dataset file to the `data/` directory
 2. From the command line, run `python make_registry.py` script to update the registry file residing in `open_radar_data/registry.txt`
@@ -61,14 +88,18 @@
 
   ```bash
   python -m pip install open-radar-data
 
   # or
 
   python -m pip install git+https://github.com/openradar/open-radar-data
+
+  # or
+
+  conda install -c conda-forge open-radar-data
   ```
 
 - Import `DATASETS` and inspect the registry to find out which datasets are available
 
   ```python
   In [1]: from open_radar_data import DATASETS
```

### Comparing `open-radar-data-0.0.4/README.md` & `open-radar-data-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Open-Radar-Data
+[![CI](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml/badge.svg)](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/open-radar-data.svg)](https://pypi.python.org/pypi/open-radar-data)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/open-radar-data.svg)](https://anaconda.org/conda-forge/open-radar-data)
 
 A place to share radar data with the community, shared between the open radar packages
 
 ## Sample data sets
 
-These files are used as sample data in Pythia Project examples/notebooks and are downloaded by `open-radar-data` package:
+These files are used as sample data in openradar examples/notebooks and are downloaded by `open-radar-data` package:
 
 - `0080_20210730_160000_01_02.scn.gz`
 - `2006_20220324_000000_000.scnx.gz`
 - `2013051000000600dBZ.vol`
 - `71_20181220_060628.pvol.h5`
 - `DWD-Vol-2_99999_20180601054047_00.h5`
 - `SUR210819000227.RAWKPJV`
@@ -16,14 +19,18 @@
 - `MLA2119412050U.nc`
 - `MLL2217907250U.003.nc`
 - `T_PAGZ35_C_ENMI_20170421090837.hdf`
 - `cfrad.20080604_002217_000_SPOL_v36_SUR.nc`
 - `cor-main131125105503.RAW2049`
 - `sample_sgp_data.nc`
 - `sample_rainbow_5_59.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.021559.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.024239.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.025840.nc`
+- `corcsapr2cmacppiM1.c1.20181111.030003.nc`
 
 ## Adding new datasets
 
 To add a new dataset file, please follow these steps:
 
 1. Add the dataset file to the `data/` directory
 2. From the command line, run `python make_registry.py` script to update the registry file residing in `open_radar_data/registry.txt`
@@ -35,14 +42,18 @@
 
   ```bash
   python -m pip install open-radar-data
 
   # or
 
   python -m pip install git+https://github.com/openradar/open-radar-data
+
+  # or
+
+  conda install -c conda-forge open-radar-data
   ```
 
 - Import `DATASETS` and inspect the registry to find out which datasets are available
 
   ```python
   In [1]: from open_radar_data import DATASETS
```

### Comparing `open-radar-data-0.0.4/open_radar_data/dataset.py` & `open-radar-data-0.0.5/open_radar_data/dataset.py`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.0.4/open_radar_data/registry.txt` & `open-radar-data-0.0.5/open_radar_data/registry.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,9 +6,13 @@
 DWD-Vol-2_99999_20180601054047_00.h5 9879ff9e79eaebb7e1a8972fb4126c09537cdc21f6941510322658b263b9bcfc
 MLA2119412050U.nc 5fa7c8fd36c1a5ec2401be6adaa4b3b4263a685efe0c7ecda7815067cb093cdc
 MLL2217907250U.003.nc 6954f4c71e625f39ee738be229a7a2b8262e0d0af96827615473228614e1a3a1
 SUR210819000227.RAWKPJV c1859c46571d9d0db9aaa86f23d4724a8f8a4e8ad9201209d83656b1010d9106
 T_PAGZ35_C_ENMI_20170421090837.hdf 207d8b90867324030b919db66f2fc30f8c5d25b9c468bdee2829185d8e995cf2
 cfrad.20080604_002217_000_SPOL_v36_SUR.nc 67821b6c2bb0f27b5de49dee636f36e6e5bbad95f1ee168cb2d1af48e98992fe
 cor-main131125105503.RAW2049 db2c58c21a5ea828b24e4397aac42127fbbf8df6577b99eea0b888ab20dde4a9
+corcsapr2cmacppiM1.c1.20181111.030003.nc 0d0d14e17cec4651d4f1ae7c09bca46fb44228bc9cba0edd3c141dd9bba3efe9
+gucxprecipradarcmacppiS2.c1.20220314.021559.nc 9c81103b2f0287431c6a098767b34d3b313116af09430ae054d2ac04c1e4c15d
+gucxprecipradarcmacppiS2.c1.20220314.024239.nc c179bb73b7a10191b6f0485051aa0b2094e9143449948179c63f335872d0cd18
+gucxprecipradarcmacppiS2.c1.20220314.025840.nc 458c80f8c68ed1215ce320839d6b8768881ca2bf9ceabccf071a9cf318020821
 sample_rainbow_5_59.vol 426199994f5bfdda4da73a96737e31f24fb90f2f9755a617e2790cfd06153010
 sample_sgp_data.nc 9c0cdad3a0e138a8d11802057ba03cee1cfcb54bf8d4e469dea9eeacc3c442c4
```

### Comparing `open-radar-data-0.0.4/open_radar_data.egg-info/PKG-INFO` & `open-radar-data-0.0.5/open_radar_data.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 Metadata-Version: 2.1
 Name: open-radar-data
-Version: 0.0.4
-Summary: Provides utility functions for accessing data repository for Project Pythia examples/notebooks
-Home-page: https://github.com/openradar/open-radar-data
-Maintainer: Open Radar Team
-Maintainer-email: 
-License: MIT
-Project-URL: Documentation, https://github.com/openradar/open-radar-data
-Project-URL: Source, https://github.com/openradar/open-radar-data
-Project-URL: Tracker, https://github.com/openradar/open-radar-data/issues
-Keywords: Radar,Pooch
+Version: 0.0.5
+Summary: Provides utility functions for accessing data repository for openradar examples/notebooks
+Author: Open Radar Team
+License: MIT License
+        
+        Copyright (c) 2022-2023 openradar
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/openradar/open-radar-data
+Project-URL: documentation, https://github.com/openradar/open-radar-data
+Project-URL: repository, https://github.com/openradar/open-radar-data
+Project-URL: tracker, https://github.com/openradar/open-radar-data/issues
+Keywords: open-radar-data,xradar
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,20 +41,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Open-Radar-Data
+[![CI](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml/badge.svg)](https://github.com/openradar/open-radar-data/actions/workflows/ci.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/open-radar-data.svg)](https://pypi.python.org/pypi/open-radar-data)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/open-radar-data.svg)](https://anaconda.org/conda-forge/open-radar-data)
 
 A place to share radar data with the community, shared between the open radar packages
 
 ## Sample data sets
 
-These files are used as sample data in Pythia Project examples/notebooks and are downloaded by `open-radar-data` package:
+These files are used as sample data in openradar examples/notebooks and are downloaded by `open-radar-data` package:
 
 - `0080_20210730_160000_01_02.scn.gz`
 - `2006_20220324_000000_000.scnx.gz`
 - `2013051000000600dBZ.vol`
 - `71_20181220_060628.pvol.h5`
 - `DWD-Vol-2_99999_20180601054047_00.h5`
 - `SUR210819000227.RAWKPJV`
@@ -42,14 +65,18 @@
 - `MLA2119412050U.nc`
 - `MLL2217907250U.003.nc`
 - `T_PAGZ35_C_ENMI_20170421090837.hdf`
 - `cfrad.20080604_002217_000_SPOL_v36_SUR.nc`
 - `cor-main131125105503.RAW2049`
 - `sample_sgp_data.nc`
 - `sample_rainbow_5_59.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.021559.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.024239.nc`
+- `gucxprecipradarcmacppiS2.c1.20220314.025840.nc`
+- `corcsapr2cmacppiM1.c1.20181111.030003.nc`
 
 ## Adding new datasets
 
 To add a new dataset file, please follow these steps:
 
 1. Add the dataset file to the `data/` directory
 2. From the command line, run `python make_registry.py` script to update the registry file residing in `open_radar_data/registry.txt`
@@ -61,14 +88,18 @@
 
   ```bash
   python -m pip install open-radar-data
 
   # or
 
   python -m pip install git+https://github.com/openradar/open-radar-data
+
+  # or
+
+  conda install -c conda-forge open-radar-data
   ```
 
 - Import `DATASETS` and inspect the registry to find out which datasets are available
 
   ```python
   In [1]: from open_radar_data import DATASETS
```

### Comparing `open-radar-data-0.0.4/open_radar_data.egg-info/SOURCES.txt` & `open-radar-data-0.0.5/open_radar_data.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 .gitignore
 .pre-commit-config.yaml
-.prettierrc.toml
 LICENSE
 MANIFEST.in
 README.md
 codecov.yml
 make_registry.py
 pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/pypi-release.yml
 open_radar_data/__init__.py
 open_radar_data/dataset.py
 open_radar_data/registry.txt
+open_radar_data/version.py
 open_radar_data.egg-info/PKG-INFO
 open_radar_data.egg-info/SOURCES.txt
 open_radar_data.egg-info/dependency_links.txt
-open_radar_data.egg-info/not-zip-safe
 open_radar_data.egg-info/requires.txt
 open_radar_data.egg-info/top_level.txt
 open_radar_data/tests/test_dataset.py
```

### Comparing `open-radar-data-0.0.4/setup.py` & `open-radar-data-0.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,89 @@
-#!/usr/bin/env python3
+[project]
+name = "open-radar-data"
+description = """Provides utility functions for accessing data repository for openradar examples/notebooks"""
+requires-python = ">=3.9"
+license = {file = "LICENSE"}
+keywords = ["open-radar-data", "xradar"]
+authors = [
+    {name = "Open Radar Team"},
+]
+classifiers=[
+    'Development Status :: 2 - Pre-Alpha',
+    'License :: OSI Approved :: MIT License',
+    'Natural Language :: English',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: Scientific/Engineering',
+    'Operating System :: OS Independent',
+    'Intended Audience :: Science/Research',
+]
+dynamic = ["version", "dependencies", "readme"]
 
-"""The setup script."""
+[build-system]
+requires = [
+    "setuptools>=45",
+    "wheel",
+    "setuptools_scm[toml]>=7.0",
+]
+build-backend = "setuptools.build_meta"
 
-from setuptools import find_packages, setup
+[project.urls]
+homepage = "https://github.com/openradar/open-radar-data"
+documentation = "https://github.com/openradar/open-radar-data"
+repository = "https://github.com/openradar/open-radar-data"
+tracker = "https://github.com/openradar/open-radar-data/issues"
 
-with open('requirements.txt') as f:
-    requirements = f.read().strip().split('\n')
+[tool.setuptools]
+packages = ["open_radar_data"]
 
-with open('README.md') as f:
-    long_description = f.read()
-setup(
-    maintainer='Open Radar Team',
-    maintainer_email='',
-    python_requires='>=3.9',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Scientific/Engineering',
-        'Operating System :: OS Independent',
-        'Intended Audience :: Science/Research',
-    ],
-    description='Provides utility functions for accessing data repository for Project Pythia examples/notebooks',
-    install_requires=requirements,
-    license='MIT',
-    long_description_content_type='text/markdown',
-    long_description=long_description,
-    include_package_data=True,
-    package_data={'open_radar_data': ['registry.txt']},
-    keywords='Radar, Pooch',
-    name='open-radar-data',
-    packages=find_packages(include=['open_radar_data', 'open_radar_data.*']),
-    entry_points={},
-    url='https://github.com/openradar/open-radar-data',
-    project_urls={
-        'Documentation': 'https://github.com/openradar/open-radar-data',
-        'Source': 'https://github.com/openradar/open-radar-data',
-        'Tracker': 'https://github.com/openradar/open-radar-data/issues',
-    },
-    use_scm_version={
-        'version_scheme': 'post-release',
-        'local_scheme': 'dirty-tag',
-    },
-    setup_requires=['setuptools_scm', 'setuptools>=30.3.0'],
-    zip_safe=False,
-)
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+readme = {file = ["README.md"], content-type = "text/markdown"}
+
+[tool.setuptools_scm]
+write_to = "open_radar_data/version.py"
+version_scheme = "post-release"
+local_scheme= "dirty-tag"
+fallback_version = "999"
+
+
+[tool.black]
+line-length = 100
+target-version = ['py39']
+skip-string-normalization = true
+
+[tool.ruff]
+target-version = "py39"
+builtins = ["ellipsis"]
+exclude = [
+    ".eggs",
+    "doc",
+]
+
+# E402: module level import not at top of file
+# E501: line too long - let black worry about that
+# E731: do not assign a lambda expression, use a def
+ignore = [
+    "E402",
+    "E501",
+    "E731",
+]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # Pyupgrade
+    "UP",
+]
+
+[tool.ruff.isort]
+known-first-party = ["open-radar-data"]
+
+[tool.check-manifest]
+ignore = ["docs/*", "tests/*", "ci/*"]
```

