# Comparing `tmp/explainy-0.2.1.tar.gz` & `tmp/explainy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainy-0.2.1.tar", last modified: Thu Jun 22 21:12:59 2023, max compression
+gzip compressed data, was "explainy-0.2.2.tar", last modified: Thu Jun 22 21:38:30 2023, max compression
```

## Comparing `explainy-0.2.1.tar` & `explainy-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.720724 explainy-0.2.1/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3535 2023-06-22 19:52:30.000000 explainy-0.2.1/CONTRIBUTING.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1073 2023-06-22 19:52:30.000000 explainy-0.2.1/LICENSE
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      324 2023-06-22 19:52:30.000000 explainy-0.2.1/MANIFEST.in
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 21:12:59.720867 explainy-0.2.1/PKG-INFO
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7435 2023-06-22 19:52:30.000000 explainy-0.2.1/README.md
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.713674 explainy-0.2.1/docs/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      609 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/Makefile
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.715116 explainy-0.2.1/docs/_static/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    24141 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/counterfactual.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    65810 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/logo.jpg
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    64388 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/logo.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7895 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/logo_original.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    17079 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/permutation.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    15037 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/shapley.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    23338 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/_static/surrogate.png
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/authors.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     5194 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/conf.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       33 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/contributing.rst
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.715571 explainy-0.2.1/docs/examples/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)   108808 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/examples/01-explainy-intro.ipynb
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    12925 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/examples/02-explainy-comparison.ipynb
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      312 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/examples.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      714 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/explainy.core.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1115 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/explainy.explanations.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      420 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/explainy.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      874 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/explainy.utils.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      330 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/index.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1142 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/installation.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      770 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/make.bat
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       61 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/modules.rst
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.1/docs/readme.rst
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.715878 explainy-0.2.1/explainy/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      156 2023-06-22 21:12:08.000000 explainy-0.2.1/explainy/__init__.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.717316 explainy-0.2.1/explainy/core/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/core/__init__.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      953 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/core/explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10951 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/core/explanation_base.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2000 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/core/explanation_mixin.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.718135 explainy-0.2.1/explainy/explanations/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      323 2023-06-22 21:08:57.000000 explainy-0.2.1/explainy/explanations/__init__.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    16525 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/explanations/counterfactual_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7467 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/explanations/permutation_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     9466 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/explanations/shap_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10067 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/explanations/surrogate_model_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1645 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/logger.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.718928 explainy-0.2.1/explainy/utils/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/__init__.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1766 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/category_mapper.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4061 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/surrogate_plot.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4263 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/surrogate_text.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      135 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/typing.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      880 2023-06-22 19:52:30.000000 explainy-0.2.1/explainy/utils/utils.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.716817 explainy-0.2.1/explainy.egg-info/
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/PKG-INFO
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)     1739 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/SOURCES.txt
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/dependency_links.txt
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)       48 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/entry_points.txt
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/not-zip-safe
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)      102 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/requires.txt
--rw-r--r--   0 mauroluzzatto   (501) staff       (20)        9 2023-06-22 21:12:59.000000 explainy-0.2.1/explainy.egg-info/top_level.txt
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      102 2023-06-22 21:11:25.000000 explainy-0.2.1/requirements.txt
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      425 2023-06-22 21:12:59.721163 explainy-0.2.1/setup.cfg
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1968 2023-06-22 21:12:08.000000 explainy-0.2.1/setup.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.720102 explainy-0.2.1/tests/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/__init__.py
-drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:12:59.720569 explainy-0.2.1/tests/core/
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/core/__init__.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      535 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/core/test_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1658 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/core/test_explanation_base.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2149 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/test_counterfactual_explanation_classifier.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2030 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/test_permutation_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2022 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/test_permutation_explanation_classifier.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2997 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/test_shap_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3460 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/test_surrogate_explanation.py
--rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      959 2023-06-22 19:52:30.000000 explainy-0.2.1/tests/utils.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.442930 explainy-0.2.2/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3535 2023-06-22 19:52:30.000000 explainy-0.2.2/CONTRIBUTING.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1073 2023-06-22 19:52:30.000000 explainy-0.2.2/LICENSE
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      324 2023-06-22 19:52:30.000000 explainy-0.2.2/MANIFEST.in
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 21:38:30.443073 explainy-0.2.2/PKG-INFO
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7435 2023-06-22 19:52:30.000000 explainy-0.2.2/README.md
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.433212 explainy-0.2.2/docs/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      609 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/Makefile
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.434915 explainy-0.2.2/docs/_static/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    24141 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/counterfactual.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    65810 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/logo.jpg
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    64388 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/logo.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7895 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/logo_original.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    17079 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/permutation.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    15037 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/shapley.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    23338 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/_static/surrogate.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/authors.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     5194 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/conf.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       33 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/contributing.rst
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.435531 explainy-0.2.2/docs/examples/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)   108808 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/examples/01-explainy-intro.ipynb
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    12925 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/examples/02-explainy-comparison.ipynb
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      312 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/examples.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      714 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/explainy.core.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1115 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/explainy.explanations.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      420 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/explainy.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      874 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/explainy.utils.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      330 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/index.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1142 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/installation.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      770 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/make.bat
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       61 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/modules.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.2/docs/readme.rst
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.435943 explainy-0.2.2/explainy/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      156 2023-06-22 21:38:22.000000 explainy-0.2.2/explainy/__init__.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.438161 explainy-0.2.2/explainy/core/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/core/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      953 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/core/explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10951 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/core/explanation_base.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2000 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/core/explanation_mixin.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.439325 explainy-0.2.2/explainy/explanations/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      323 2023-06-22 21:08:57.000000 explainy-0.2.2/explainy/explanations/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    16537 2023-06-22 21:36:47.000000 explainy-0.2.2/explainy/explanations/counterfactual_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7467 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/explanations/permutation_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     9466 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/explanations/shap_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10067 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/explanations/surrogate_model_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1645 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/logger.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.440536 explainy-0.2.2/explainy/utils/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1766 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/category_mapper.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4061 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/surrogate_plot.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4263 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/surrogate_text.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      135 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/typing.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      880 2023-06-22 19:52:30.000000 explainy-0.2.2/explainy/utils/utils.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.437368 explainy-0.2.2/explainy.egg-info/
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/PKG-INFO
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     1739 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/SOURCES.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/dependency_links.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)       48 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/entry_points.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/not-zip-safe
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)      117 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/requires.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        9 2023-06-22 21:38:30.000000 explainy-0.2.2/explainy.egg-info/top_level.txt
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      116 2023-06-22 21:32:38.000000 explainy-0.2.2/requirements.txt
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      425 2023-06-22 21:38:30.443393 explainy-0.2.2/setup.cfg
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1968 2023-06-22 21:38:22.000000 explainy-0.2.2/setup.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.442088 explainy-0.2.2/tests/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/__init__.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 21:38:30.442757 explainy-0.2.2/tests/core/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/core/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      535 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/core/test_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1658 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/core/test_explanation_base.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2149 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/test_counterfactual_explanation_classifier.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2030 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/test_permutation_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2022 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/test_permutation_explanation_classifier.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2997 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/test_shap_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3460 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/test_surrogate_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      959 2023-06-22 19:52:30.000000 explainy-0.2.2/tests/utils.py
```

### Comparing `explainy-0.2.1/CONTRIBUTING.rst` & `explainy-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/LICENSE` & `explainy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/PKG-INFO` & `explainy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainy
-Version: 0.2.1
+Version: 0.2.2
 Summary: explainy is a library for generating explanations for machine learning models in Python. It uses methods from Machine Learning Explainability and provides a standardized API to create feature importance explanations for samples. The explanations are generated in the form of plots and text.
 Home-page: https://github.com/MauroLuzzatto/explainy
 Author: Mauro Luzzatto
 Author-email: mauroluzzatto@hotmail.com
 License: MIT license
 Description: 
         <!-- <img src="https://github.com/MauroLuzzatto/explainy/raw/main/docs/_static/logo.png" width="180" height="180" align="right"/> -->
```

### Comparing `explainy-0.2.1/README.md` & `explainy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/Makefile` & `explainy-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/counterfactual.png` & `explainy-0.2.2/docs/_static/counterfactual.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/logo.jpg` & `explainy-0.2.2/docs/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/logo.png` & `explainy-0.2.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/logo_original.png` & `explainy-0.2.2/docs/_static/logo_original.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/permutation.png` & `explainy-0.2.2/docs/_static/permutation.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/shapley.png` & `explainy-0.2.2/docs/_static/shapley.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/_static/surrogate.png` & `explainy-0.2.2/docs/_static/surrogate.png`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/conf.py` & `explainy-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/examples/01-explainy-intro.ipynb` & `explainy-0.2.2/docs/examples/01-explainy-intro.ipynb`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/examples/02-explainy-comparison.ipynb` & `explainy-0.2.2/docs/examples/02-explainy-comparison.ipynb`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/explainy.core.rst` & `explainy-0.2.2/docs/explainy.core.rst`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/explainy.explanations.rst` & `explainy-0.2.2/docs/explainy.explanations.rst`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/explainy.utils.rst` & `explainy-0.2.2/docs/explainy.utils.rst`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/installation.rst` & `explainy-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/docs/make.bat` & `explainy-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/core/explanation.py` & `explainy-0.2.2/explainy/core/explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/core/explanation_base.py` & `explainy-0.2.2/explainy/core/explanation_base.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/core/explanation_mixin.py` & `explainy-0.2.2/explainy/core/explanation_mixin.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/explanations/counterfactual_explanation.py` & `explainy-0.2.2/explainy/explanations/counterfactual_explanation.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,30 +363,30 @@
         )
         table.auto_set_font_size(False)
         table.set_fontsize(12)
         table.scale(1.25, 2)
 
         # if show_rating:
         # make the last row bold
-        for (row, col), cell in table.get_celld().items():
+        for (row, _), cell in table.get_celld().items():
             if row == array_subset.shape[0]:
                 cell.set_text_props(fontproperties=FontProperties(weight="bold"))
 
         plt.axis("off")
         plt.grid("off")
         # draw canvas once
         plt.gcf().canvas.draw()
-        # get bounding box of table
-        points = table.get_window_extent(plt.gcf()._cachedRenderer).get_points()
-        # add 10 pixel spacing
-        points[0, :] -= 10
-        points[1, :] += 10
+        # # get bounding box of table
+        # points = table.get_window_extent(plt.gcf()._cachedRenderer).get_points()
+        # # add 10 pixel spacing
+        # points[0, :] -= 10
+        # points[1, :] += 10
 
-        # get new bounding box in inches
-        self.nbbox = matplotlib.transforms.Bbox.from_extents(points / plt.gcf().dpi)
+        # # get new bounding box in inches
+        # self.nbbox = matplotlib.transforms.Bbox.from_extents(points / plt.gcf().dpi)
         plt.show()
         return fig
 
     def get_method_text(self) -> str:
         """
         Define the method introduction text of the explanation type.
```

### Comparing `explainy-0.2.1/explainy/explanations/permutation_explanation.py` & `explainy-0.2.2/explainy/explanations/permutation_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/explanations/shap_explanation.py` & `explainy-0.2.2/explainy/explanations/shap_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/explanations/surrogate_model_explanation.py` & `explainy-0.2.2/explainy/explanations/surrogate_model_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/logger.py` & `explainy-0.2.2/explainy/logger.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/utils/category_mapper.py` & `explainy-0.2.2/explainy/utils/category_mapper.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/utils/surrogate_plot.py` & `explainy-0.2.2/explainy/utils/surrogate_plot.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/utils/surrogate_text.py` & `explainy-0.2.2/explainy/utils/surrogate_text.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy/utils/utils.py` & `explainy-0.2.2/explainy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/explainy.egg-info/PKG-INFO` & `explainy-0.2.2/explainy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainy
-Version: 0.2.1
+Version: 0.2.2
 Summary: explainy is a library for generating explanations for machine learning models in Python. It uses methods from Machine Learning Explainability and provides a standardized API to create feature importance explanations for samples. The explanations are generated in the form of plots and text.
 Home-page: https://github.com/MauroLuzzatto/explainy
 Author: Mauro Luzzatto
 Author-email: mauroluzzatto@hotmail.com
 License: MIT license
 Description: 
         <!-- <img src="https://github.com/MauroLuzzatto/explainy/raw/main/docs/_static/logo.png" width="180" height="180" align="right"/> -->
```

### Comparing `explainy-0.2.1/explainy.egg-info/SOURCES.txt` & `explainy-0.2.2/explainy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/setup.py` & `explainy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,11 +55,11 @@
     include_package_data=True,
     keywords="explainy",
     name="explainy",
     packages=find_packages(include=["explainy", "explainy.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/MauroLuzzatto/explainy",
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
 # fmt: on
```

### Comparing `explainy-0.2.1/tests/core/test_explanation.py` & `explainy-0.2.2/tests/core/test_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/core/test_explanation_base.py` & `explainy-0.2.2/tests/core/test_explanation_base.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/test_counterfactual_explanation_classifier.py` & `explainy-0.2.2/tests/test_counterfactual_explanation_classifier.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/test_permutation_explanation.py` & `explainy-0.2.2/tests/test_permutation_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/test_permutation_explanation_classifier.py` & `explainy-0.2.2/tests/test_permutation_explanation_classifier.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/test_shap_explanation.py` & `explainy-0.2.2/tests/test_shap_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/test_surrogate_explanation.py` & `explainy-0.2.2/tests/test_surrogate_explanation.py`

 * *Files identical despite different names*

### Comparing `explainy-0.2.1/tests/utils.py` & `explainy-0.2.2/tests/utils.py`

 * *Files identical despite different names*

