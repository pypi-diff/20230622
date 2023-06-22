# Comparing `tmp/pineko-0.4.0.tar.gz` & `tmp/pineko-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineko-0.4.0.tar", max compression
+gzip compressed data, was "pineko-0.4.1.tar", max compression
```

## Comparing `pineko-0.4.0.tar` & `pineko-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-05-23 14:39:56.669124 pineko-0.4.0/LICENSE
--rw-r--r--   0        0        0     2248 2023-05-23 14:39:56.669124 pineko-0.4.0/README.md
--rw-r--r--   0        0        0     3341 2023-05-23 14:44:37.762009 pineko-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/__init__.py
--rw-r--r--   0        0        0     5596 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/check.py
--rw-r--r--   0        0        0      134 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/__init__.py
--rw-r--r--   0        0        0      237 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/_base.py
--rw-r--r--   0        0        0     3289 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/check.py
--rw-r--r--   0        0        0     1529 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/compare.py
--rw-r--r--   0        0        0     2158 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/convolute.py
--rw-r--r--   0        0        0      850 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/gen_sv.py
--rw-r--r--   0        0        0     1083 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/kfactor.py
--rw-r--r--   0        0        0     1205 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/opcard.py
--rw-r--r--   0        0        0     1558 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/scaffold.py
--rw-r--r--   0        0        0     3822 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/theory_.py
--rw-r--r--   0        0        0     1639 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/comparator.py
--rw-r--r--   0        0        0     3700 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/configs.py
--rw-r--r--   0        0        0     1022 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/ekompatibility.py
--rw-r--r--   0        0        0     7957 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/evolve.py
--rw-r--r--   0        0        0    13751 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/kfactor.py
--rw-r--r--   0        0        0     2035 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/parser.py
--rw-r--r--   0        0        0     2534 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/scaffold.py
--rw-r--r--   0        0        0    10171 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/scale_variations.py
--rw-r--r--   0        0        0    14799 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/theory.py
--rw-r--r--   0        0        0     1734 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/theory_card.py
--rw-r--r--   0        0        0       49 2023-05-23 14:44:37.762009 pineko-0.4.0/src/pineko/version.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 pineko-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 15:18:16.799567 pineko-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2248 2023-06-22 15:18:16.799567 pineko-0.4.1/README.md
+-rw-r--r--   0        0        0     3049 2023-06-22 15:22:53.320868 pineko-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/__init__.py
+-rw-r--r--   0        0        0     5596 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/check.py
+-rw-r--r--   0        0        0      134 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/_base.py
+-rw-r--r--   0        0        0     3289 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/check.py
+-rw-r--r--   0        0        0     1529 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/compare.py
+-rw-r--r--   0        0        0     2158 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/convolute.py
+-rw-r--r--   0        0        0      850 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/gen_sv.py
+-rw-r--r--   0        0        0     1095 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/kfactor.py
+-rw-r--r--   0        0        0     1205 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/opcard.py
+-rw-r--r--   0        0        0     1558 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/scaffold.py
+-rw-r--r--   0        0        0     3822 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/cli/theory_.py
+-rw-r--r--   0        0        0     1639 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/comparator.py
+-rw-r--r--   0        0        0     3700 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/configs.py
+-rw-r--r--   0        0        0     1022 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/ekompatibility.py
+-rw-r--r--   0        0        0     7957 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/evolve.py
+-rw-r--r--   0        0        0    13736 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/kfactor.py
+-rw-r--r--   0        0        0     2035 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/parser.py
+-rw-r--r--   0        0        0     2534 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/scaffold.py
+-rw-r--r--   0        0        0    10171 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/scale_variations.py
+-rw-r--r--   0        0        0    14799 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/theory.py
+-rw-r--r--   0        0        0     1734 2023-06-22 15:18:16.803567 pineko-0.4.1/src/pineko/theory_card.py
+-rw-r--r--   0        0        0       49 2023-06-22 15:22:53.320868 pineko-0.4.1/src/pineko/version.py
+-rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 pineko-0.4.1/PKG-INFO
```

### Comparing `pineko-0.4.0/LICENSE` & `pineko-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/README.md` & `pineko-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/pyproject.toml` & `pineko-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pineko"
-version = "0.4.0"
+version = "0.4.1"
 description = "Combine PineAPPL grids and EKOs into FK tables"
 readme = "README.md"
 authors = [
   "Alessandro Candido <alessandro.candido@mi.infn.it>",
   "Andrea Barontini <andrea.barontini@mi.infn.it>",
   "Felix Hekhorn <felix.hekhorn@mi.infn.it>",
 ]
@@ -28,18 +28,14 @@
 pineappl = { version = "^0.6.0a17", allow-prereleases = true }
 PyYAML = "^6.0"
 numpy = "^1.21.0"
 pandas = "^1.4.1"
 rich = "^12.5.1"
 click = "^8.0.4"
 tomli = "^2.0.1"
-# docs dependencies (for readthedocs, https://github.com/readthedocs/readthedocs.org/issues/4912#issuecomment-664002569)
-Sphinx = { version = "^4.3.2", optional = true }
-sphinx-rtd-theme = { version = "^1.0.0", optional = true }
-sphinxcontrib-bibtex = { version = "^2.4.1", optional = true }
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `pineko-0.4.0/src/pineko/check.py` & `pineko-0.4.1/src/pineko/check.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/check.py` & `pineko-0.4.1/src/pineko/cli/check.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/compare.py` & `pineko-0.4.1/src/pineko/cli/compare.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/convolute.py` & `pineko-0.4.1/src/pineko/cli/convolute.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/gen_sv.py` & `pineko-0.4.1/src/pineko/cli/gen_sv.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/kfactor.py` & `pineko-0.4.1/src/pineko/cli/kfactor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """CLI entry point to generation of the inclusion of kfactor in a grid."""
 
 import pathlib
 
 import click
+import rich
 
 from .. import kfactor
 from ._base import command
 
 
 @command.command("kfactor")
 @click.argument("grids_folder", type=click.Path(exists=True))
```

### Comparing `pineko-0.4.0/src/pineko/cli/opcard.py` & `pineko-0.4.1/src/pineko/cli/opcard.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/scaffold.py` & `pineko-0.4.1/src/pineko/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/cli/theory_.py` & `pineko-0.4.1/src/pineko/cli/theory_.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/comparator.py` & `pineko-0.4.1/src/pineko/comparator.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/configs.py` & `pineko-0.4.1/src/pineko/configs.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/ekompatibility.py` & `pineko-0.4.1/src/pineko/ekompatibility.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/evolve.py` & `pineko-0.4.1/src/pineko/evolve.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/kfactor.py` & `pineko-0.4.1/src/pineko/kfactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Module to include QCD K-factors in grids."""
 import io
-import pathlib
 
 import numpy as np
 import pineappl
 import rich
 import yaml
 from pineappl import import_only_subgrid
```

### Comparing `pineko-0.4.0/src/pineko/parser.py` & `pineko-0.4.1/src/pineko/parser.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/scaffold.py` & `pineko-0.4.1/src/pineko/scaffold.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/scale_variations.py` & `pineko-0.4.1/src/pineko/scale_variations.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/theory.py` & `pineko-0.4.1/src/pineko/theory.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/src/pineko/theory_card.py` & `pineko-0.4.1/src/pineko/theory_card.py`

 * *Files identical despite different names*

### Comparing `pineko-0.4.0/PKG-INFO` & `pineko-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineko
-Version: 0.4.0
+Version: 0.4.1
 Summary: Combine PineAPPL grids and EKOs into FK tables
 Home-page: https://github.com/N3PDF/pineko
 Author: Alessandro Candido
 Author-email: alessandro.candido@mi.infn.it
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -13,23 +13,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra == "docs"
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: eko (>=0.13.2,<0.14.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: pineappl (>=0.6.0a17,<0.7.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0) ; extra == "docs"
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/N3PDF/pineko
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://pineko.readthedocs.io/"><img alt="PINEKO" src="https://raw.githubusercontent.com/N3PDF/pineko/main/docs/source/img/Logo.png" width=200></a>
 </p>
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1 Name: pineko Version: 0.4.0 Summary: Combine PineAPPL
+Metadata-Version: 2.1 Name: pineko Version: 0.4.1 Summary: Combine PineAPPL
 grids and EKOs into FK tables Home-page: https://github.com/N3PDF/pineko
 Author: Alessandro Candido Author-email: alessandro.candido@mi.infn.it
 Requires-Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics Provides-Extra: docs
-Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ;
-extra == "docs" Requires-Dist: click (>=8.0.4,<9.0.0) Requires-Dist: eko
-(>=0.13.2,<0.14.0) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-Dist: pandas
-(>=1.4.1,<2.0.0) Requires-Dist: pineappl (>=0.6.0a17,<0.7.0) Requires-Dist:
-rich (>=12.5.1,<13.0.0) Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ;
-extra == "docs" Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0) ; extra ==
-"docs" Requires-Dist: tomli (>=2.0.1,<3.0.0) Project-URL: Repository, https://
-github.com/N3PDF/pineko Description-Content-Type: text/markdown
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: click (>=8.0.4,<9.0.0)
+Requires-Dist: eko (>=0.13.2,<0.14.0) Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: pandas (>=1.4.1,<2.0.0) Requires-Dist: pineappl
+(>=0.6.0a17,<0.7.0) Requires-Dist: rich (>=12.5.1,<13.0.0) Requires-Dist: tomli
+(>=2.0.1,<3.0.0) Project-URL: Repository, https://github.com/N3PDF/pineko
+Description-Content-Type: text/markdown
                                    [PINEKO]
 [Tests] [Docs] [https://codecov.io/gh/NNPDF/pineko/branch/main/graph/badge.svg]
                                  [CodeFactor]
 PINEKO is a Python module to produce fktables from interpolation grids and
 EKOs. ## Installation PINEKO is available via - PyPI: [PyPI] ```bash pip
 install pineko ``` ### Development If you want to install from source you can
 run ```bash git clone git@github.com:N3PDF/pineko.git cd pineko poetry install
```

