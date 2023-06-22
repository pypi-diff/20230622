# Comparing `tmp/explainy-0.1.8.tar.gz` & `tmp/explainy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\explainy-0.1.8.tar", last modified: Sun Sep 19 16:53:02 2021, max compression
+gzip compressed data, was "explainy-0.2.0.tar", last modified: Thu Jun 22 20:20:17 2023, max compression
```

## Comparing `explainy-0.1.8.tar` & `explainy-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,76 @@
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:02.258748 explainy-0.1.8/
--rw-rw-rw-   0        0        0      178 2021-07-27 08:44:48.000000 explainy-0.1.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3663 2021-07-27 08:44:48.000000 explainy-0.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1095 2021-07-27 08:44:48.000000 explainy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      338 2021-09-16 20:41:22.000000 explainy-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7824 2021-09-19 16:53:02.260074 explainy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5596 2021-09-19 16:41:20.000000 explainy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.117807 explainy-0.1.8/docs/
--rw-rw-rw-   0        0        0      629 2021-07-27 08:44:49.000000 explainy-0.1.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:00.902404 explainy-0.1.8/docs/_build/
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:00.902826 explainy-0.1.8/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.399696 explainy-0.1.8/docs/_build/html/_static/
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.407210 explainy-0.1.8/docs/_build/html/_static/_archive/
--rw-rw-rw-   0        0        0    15352 2021-06-26 20:28:13.000000 explainy-0.1.8/docs/_build/html/_static/_archive/logo.png
--rw-rw-rw-   0        0        0    24141 2021-09-09 20:44:42.000000 explainy-0.1.8/docs/_build/html/_static/counterfactual.png
--rw-rw-rw-   0        0        0      286 2021-08-28 07:14:54.000000 explainy-0.1.8/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0    65810 2021-06-27 19:42:36.000000 explainy-0.1.8/docs/_build/html/_static/logo.jpg
--rw-rw-rw-   0        0        0     7895 2021-06-27 19:36:32.000000 explainy-0.1.8/docs/_build/html/_static/logo.png
--rw-rw-rw-   0        0        0       90 2021-08-28 07:14:54.000000 explainy-0.1.8/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0    17079 2021-06-20 19:16:13.000000 explainy-0.1.8/docs/_build/html/_static/permutation.png
--rw-rw-rw-   0        0        0       90 2021-08-28 07:14:54.000000 explainy-0.1.8/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0    15037 2021-06-20 19:15:22.000000 explainy-0.1.8/docs/_build/html/_static/shapley.png
--rw-rw-rw-   0        0        0    23338 2021-06-20 18:55:42.000000 explainy-0.1.8/docs/_build/html/_static/surrogate.png
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.573693 explainy-0.1.8/docs/_static/
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.586816 explainy-0.1.8/docs/_static/_archive/
--rw-rw-rw-   0        0        0    15352 2021-06-26 20:28:13.000000 explainy-0.1.8/docs/_static/_archive/logo.png
--rw-rw-rw-   0        0        0    24141 2021-09-09 20:44:42.000000 explainy-0.1.8/docs/_static/counterfactual.png
--rw-rw-rw-   0        0        0    65810 2021-06-27 19:42:36.000000 explainy-0.1.8/docs/_static/logo.jpg
--rw-rw-rw-   0        0        0     7895 2021-06-27 19:36:32.000000 explainy-0.1.8/docs/_static/logo.png
--rw-rw-rw-   0        0        0    17079 2021-06-20 19:16:13.000000 explainy-0.1.8/docs/_static/permutation.png
--rw-rw-rw-   0        0        0    15037 2021-06-20 19:15:22.000000 explainy-0.1.8/docs/_static/shapley.png
--rw-rw-rw-   0        0        0    23338 2021-06-20 18:55:42.000000 explainy-0.1.8/docs/_static/surrogate.png
--rw-rw-rw-   0        0        0       29 2021-07-27 08:44:48.000000 explainy-0.1.8/docs/authors.rst
--rw-rw-rw-   0        0        0     5304 2021-09-16 20:48:58.000000 explainy-0.1.8/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-07-27 08:44:48.000000 explainy-0.1.8/docs/contributing.rst
--rw-rw-rw-   0        0        0      289 2021-09-16 20:56:52.000000 explainy-0.1.8/docs/examples.rst
--rw-rw-rw-   0        0        0     1973 2021-09-08 20:09:26.000000 explainy-0.1.8/docs/explainy.explanation.rst
--rw-rw-rw-   0        0        0      552 2021-09-19 16:28:27.000000 explainy-0.1.8/docs/explainy.rst
--rw-rw-rw-   0        0        0      351 2021-09-16 20:34:28.000000 explainy-0.1.8/docs/index.rst
--rw-rw-rw-   0        0        0     1193 2021-07-27 08:44:49.000000 explainy-0.1.8/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2021-07-27 08:44:49.000000 explainy-0.1.8/docs/make.bat
--rw-rw-rw-   0        0        0       68 2021-09-19 16:28:27.000000 explainy-0.1.8/docs/modules.rst
--rw-rw-rw-   0        0        0       29 2021-09-09 20:50:31.000000 explainy-0.1.8/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.634365 explainy-0.1.8/explainy/
--rw-rw-rw-   0        0        0      225 2021-09-16 21:18:47.000000 explainy-0.1.8/explainy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:02.141324 explainy-0.1.8/explainy/explanation/
--rw-rw-rw-   0        0        0       81 2021-08-27 20:36:35.000000 explainy-0.1.8/explainy/explanation/__init__.py
--rw-rw-rw-   0        0        0     1929 2021-06-19 09:52:56.000000 explainy-0.1.8/explainy/explanation/category_mapper.py
--rw-rw-rw-   0        0        0    16176 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/counterfactual_explanation.py
--rw-rw-rw-   0        0        0     8130 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/explanation_base.py
--rw-rw-rw-   0        0        0     2198 2021-09-16 21:08:55.000000 explainy-0.1.8/explainy/explanation/explanation_mixin.py
--rw-rw-rw-   0        0        0     7293 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/permutation_explanation.py
--rw-rw-rw-   0        0        0     7882 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/surrogate_model_explanation.py
--rw-rw-rw-   0        0        0     4308 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/surrogate_plot.py
--rw-rw-rw-   0        0        0     4274 2021-09-16 21:10:50.000000 explainy-0.1.8/explainy/explanation/surrogate_text.py
--rw-rw-rw-   0        0        0     1700 2021-01-17 18:05:29.000000 explainy-0.1.8/explainy/logger.py
--rw-rw-rw-   0        0        0      276 2021-01-17 19:01:24.000000 explainy-0.1.8/explainy/utils.py
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:01.711271 explainy-0.1.8/explainy.egg-info/
--rw-rw-rw-   0        0        0     7824 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-08-29 14:25:31.000000 explainy-0.1.8/explainy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-09-19 16:53:00.000000 explainy-0.1.8/explainy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       67 2021-09-09 20:17:28.000000 explainy-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0      500 2021-09-19 16:53:02.268151 explainy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1929 2021-09-19 16:51:36.000000 explainy-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-19 16:53:02.218018 explainy-0.1.8/tests/
--rw-rw-rw-   0        0        0        2 2021-03-30 19:59:28.000000 explainy-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2897 2021-09-16 21:10:52.000000 explainy-0.1.8/tests/test_permutation_explanation.py
--rw-rw-rw-   0        0        0     2809 2021-09-16 21:10:52.000000 explainy-0.1.8/tests/test_permutation_explanation_classifier.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.541352 explainy-0.2.0/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3535 2023-06-22 19:52:30.000000 explainy-0.2.0/CONTRIBUTING.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1073 2023-06-22 19:52:30.000000 explainy-0.2.0/LICENSE
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      324 2023-06-22 19:52:30.000000 explainy-0.2.0/MANIFEST.in
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 20:20:17.541493 explainy-0.2.0/PKG-INFO
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7435 2023-06-22 19:52:30.000000 explainy-0.2.0/README.md
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.533319 explainy-0.2.0/docs/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      609 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/Makefile
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.534650 explainy-0.2.0/docs/_static/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    24141 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/counterfactual.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    65810 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/logo.jpg
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    64388 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/logo.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7895 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/logo_original.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    17079 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/permutation.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    15037 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/shapley.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    23338 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/_static/surrogate.png
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     5194 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/conf.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       33 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/contributing.rst
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.535120 explainy-0.2.0/docs/examples/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)   108808 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/examples/01-explainy-intro.ipynb
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    12925 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/examples/02-explainy-comparison.ipynb
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      312 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/examples.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      714 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/explainy.core.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1115 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/explainy.explanations.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      420 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/explainy.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      874 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/explainy.utils.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      330 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/index.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1142 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/installation.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      770 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/make.bat
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       61 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/modules.rst
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)       28 2023-06-22 19:52:30.000000 explainy-0.2.0/docs/readme.rst
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.535535 explainy-0.2.0/explainy/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      156 2023-06-22 20:18:32.000000 explainy-0.2.0/explainy/__init__.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.537310 explainy-0.2.0/explainy/core/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/core/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      953 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/core/explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10951 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/core/explanation_base.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2000 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/core/explanation_mixin.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.538120 explainy-0.2.0/explainy/explanations/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/explanations/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    16525 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/explanations/counterfactual_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     7467 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/explanations/permutation_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     9466 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/explanations/shap_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)    10067 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/explanations/surrogate_model_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1645 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/logger.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.538969 explainy-0.2.0/explainy/utils/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1766 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/category_mapper.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4061 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/surrogate_plot.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     4263 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/surrogate_text.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      135 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/typing.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      880 2023-06-22 19:52:30.000000 explainy-0.2.0/explainy/utils/utils.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.536647 explainy-0.2.0/explainy.egg-info/
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     9779 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/PKG-INFO
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)     1739 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/SOURCES.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/dependency_links.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)       48 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/entry_points.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/not-zip-safe
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)      118 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/requires.txt
+-rw-r--r--   0 mauroluzzatto   (501) staff       (20)        9 2023-06-22 20:20:17.000000 explainy-0.2.0/explainy.egg-info/top_level.txt
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      117 2023-06-22 20:10:47.000000 explainy-0.2.0/requirements.txt
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      425 2023-06-22 20:20:17.541885 explainy-0.2.0/setup.cfg
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1968 2023-06-22 20:18:34.000000 explainy-0.2.0/setup.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.540633 explainy-0.2.0/tests/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/__init__.py
+drwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        0 2023-06-22 20:20:17.541189 explainy-0.2.0/tests/core/
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)        1 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/core/__init__.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      535 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/core/test_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     1658 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/core/test_explanation_base.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2149 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/test_counterfactual_explanation_classifier.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2030 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/test_permutation_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2022 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/test_permutation_explanation_classifier.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     2997 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/test_shap_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)     3460 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/test_surrogate_explanation.py
+-rwxr-xr-x   0 mauroluzzatto   (501) staff       (20)      959 2023-06-22 19:52:30.000000 explainy-0.2.0/tests/utils.py
```

### Comparing `explainy-0.1.8/LICENSE` & `explainy-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2021, Mauro Luzzatto
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2021, Mauro Luzzatto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `explainy-0.1.8/PKG-INFO` & `explainy-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,489 +1,465 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7870  : 2.1..Name: exp
-00000020: 6c61 696e 790d 0a56 6572 7369 6f6e 3a20  lainy..Version: 
-00000030: 302e 312e 380d 0a53 756d 6d61 7279 3a20  0.1.8..Summary: 
-00000040: 1665 7870 6c61 696e 7920 6973 2061 206c  .explainy is a l
-00000050: 6962 7261 7279 2066 6f72 2067 656e 6572  ibrary for gener
-00000060: 6174 696e 6720 6578 706c 616e 6174 696f  ating explanatio
-00000070: 6e73 2066 6f72 206d 6163 6869 6e65 206c  ns for machine l
-00000080: 6561 726e 696e 6720 6d6f 6465 6c73 2069  earning models i
-00000090: 6e20 5079 7468 6f6e 2e20 4974 2075 7365  n Python. It use
-000000a0: 7320 6d65 7468 6f64 7320 6672 6f6d 204d  s methods from M
-000000b0: 6163 6869 6e65 204c 6561 726e 696e 6720  achine Learning 
-000000c0: 4578 706c 6169 6e61 6269 6c69 7479 2061  Explainability a
-000000d0: 6e64 2070 726f 7669 6465 7320 6120 7374  nd provides a st
-000000e0: 616e 6461 7264 697a 6564 2041 5049 2074  andardized API t
-000000f0: 6f20 6372 6561 7465 2066 6561 7475 7265  o create feature
-00000100: 2069 6d70 6f72 7461 6e63 6520 6578 706c   importance expl
-00000110: 616e 6174 696f 6e73 2066 6f72 2073 616d  anations for sam
-00000120: 706c 6573 2e20 5468 6520 6578 706c 616e  ples. The explan
-00000130: 6174 696f 6e73 2061 7265 2067 656e 6572  ations are gener
-00000140: 6174 6564 2069 6e20 7468 6520 666f 726d  ated in the form
-00000150: 206f 6620 706c 6f74 7320 616e 6420 7465   of plots and te
-00000160: 7874 2e0d 0a48 6f6d 652d 7061 6765 3a20  xt...Home-page: 
-00000170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000180: 6f6d 2f4d 6175 726f 4c75 7a7a 6174 746f  om/MauroLuzzatto
-00000190: 2f65 7870 6c61 696e 790d 0a41 7574 686f  /explainy..Autho
-000001a0: 723a 204d 6175 726f 204c 757a 7a61 7474  r: Mauro Luzzatt
-000001b0: 6f0d 0a41 7574 686f 722d 656d 6169 6c3a  o..Author-email:
-000001c0: 206d 6175 726f 6c75 7a7a 6174 746f 4068   mauroluzzatto@h
-000001d0: 6f74 6d61 696c 2e63 6f6d 0d0a 4c69 6365  otmail.com..Lice
-000001e0: 6e73 653a 204d 4954 206c 6963 656e 7365  nse: MIT license
-000001f0: 0d0a 4465 7363 7269 7074 696f 6e3a 2022  ..Description: "
-00000200: 2222 0d0a 2020 2020 2020 2020 0d0a 2020  ""..        ..  
-00000210: 2020 2020 2020 3c21 2d2d 203c 6120 6872        <!-- <a hr
-00000220: 6566 3d22 6874 7470 733a 2f2f 6578 706c  ef="https://expl
-00000230: 6f73 696f 6e2e 6169 223e 3c69 6d67 2073  osion.ai"><img s
-00000240: 7263 3d22 6874 7470 733a 2f2f 6578 706c  rc="https://expl
-00000250: 6f73 696f 6e2e 6169 2f61 7373 6574 732f  osion.ai/assets/
-00000260: 696d 672f 6c6f 676f 2e73 7667 2220 7769  img/logo.svg" wi
-00000270: 6474 683d 2231 3235 2220 6865 6967 6874  dth="125" height
-00000280: 3d22 3132 3522 2061 6c69 676e 3d22 7269  ="125" align="ri
-00000290: 6768 7422 202f 3e3c 2f61 3e20 2d2d 3e0d  ght" /></a> -->.
-000002a0: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
-000002b0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-000002c0: 622e 636f 6d2f 4d61 7572 6f4c 757a 7a61  b.com/MauroLuzza
-000002d0: 7474 6f2f 6578 706c 6169 6e79 2f62 6c6f  tto/explainy/blo
-000002e0: 622f 6d61 696e 2f64 6f63 732f 5f73 7461  b/main/docs/_sta
-000002f0: 7469 632f 6c6f 676f 2e70 6e67 2220 7769  tic/logo.png" wi
-00000300: 6474 683d 2232 3530 2220 6865 6967 6874  dth="250" height
-00000310: 3d22 3235 3022 2061 6c69 676e 3d22 7269  ="250" align="ri
-00000320: 6768 7422 202f 3e3c 2f61 3e0d 0a20 2020  ght" /></a>..   
-00000330: 2020 2020 2023 2065 7870 6c61 696e 7920       # explainy 
-00000340: 2d20 626c 6163 6b2d 626f 7820 6d6f 6465  - black-box mode
-00000350: 6c20 6578 706c 616e 6174 696f 6e73 2066  l explanations f
-00000360: 6f72 2068 756d 616e 730d 0a20 2020 2020  or humans..     
-00000370: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-00000380: 2020 2020 2020 205b 215b 7079 7069 2076         [![pypi v
-00000390: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000003a0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000003b0: 7970 692f 762f 6578 706c 6169 6e79 2e73  ypi/v/explainy.s
-000003c0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-000003d0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-000003e0: 692f 6578 706c 6169 6e79 290d 0a20 2020  i/explainy)..   
-000003f0: 2020 2020 205b 215b 7472 6176 6973 5d28       [![travis](
-00000400: 6874 7470 733a 2f2f 6170 702e 7472 6176  https://app.trav
-00000410: 6973 2d63 692e 636f 6d2f 4d61 7572 6f4c  is-ci.com/MauroL
-00000420: 757a 7a61 7474 6f2f 6578 706c 6169 6e79  uzzatto/explainy
-00000430: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-00000440: 295d 2868 7474 7073 3a2f 2f61 7070 2e74  )](https://app.t
-00000450: 7261 7669 732d 6369 2e63 6f6d 2f67 6974  ravis-ci.com/git
-00000460: 6875 622f 4d61 7572 6f4c 757a 7a61 7474  hub/MauroLuzzatt
-00000470: 6f2f 6578 706c 6169 6e79 3f62 7261 6e63  o/explainy?branc
-00000480: 683d 6d61 7374 6572 290d 0a20 2020 2020  h=master)..     
-00000490: 2020 205b 215b 646f 6373 5d28 6874 7470     [![docs](http
-000004a0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-000004b0: 6f72 672f 7072 6f6a 6563 7473 2f65 7870  org/projects/exp
-000004c0: 6c61 696e 792f 6261 6467 652f 3f76 6572  lainy/badge/?ver
-000004d0: 7369 6f6e 3d6c 6174 6573 7429 5d28 6874  sion=latest)](ht
-000004e0: 7470 733a 2f2f 6578 706c 6169 6e79 2e72  tps://explainy.r
-000004f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000500: 2f6c 6174 6573 742f 3f76 6572 7369 6f6e  /latest/?version
-00000510: 3d6c 6174 6573 7429 0d0a 2020 2020 2020  =latest)..      
-00000520: 2020 5b21 5b53 7570 706f 7274 6564 2076    [![Supported v
-00000530: 6572 7369 6f6e 735d 2868 7474 7073 3a2f  ersions](https:/
-00000540: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000550: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000560: 6578 706c 6169 6e79 2e73 7667 295d 2868  explainy.svg)](h
-00000570: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000580: 7072 6f6a 6563 742f 6578 706c 6169 6e79  project/explainy
-00000590: 290d 0a20 2020 2020 2020 205b 215b 436f  )..        [![Co
-000005a0: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
-000005b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000005c0: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-000005d0: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-000005e0: 2d30 3030 3030 302e 7376 673f 7374 796c  -000000.svg?styl
-000005f0: 653d 666c 6174 2d73 7175 6172 6529 5d28  e=flat-square)](
-00000600: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000610: 6f6d 2f61 6d62 762f 626c 6163 6b29 0d0a  om/ambv/black)..
-00000620: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000630: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-00000640: 2020 2020 2020 6578 706c 6169 6e79 2069        explainy i
-00000650: 7320 6120 6c69 6272 6172 7920 666f 7220  s a library for 
-00000660: 6765 6e65 7261 7469 6e67 2065 7870 6c61  generating expla
-00000670: 6e61 7469 6f6e 7320 666f 7220 6d61 6368  nations for mach
-00000680: 696e 6520 6c65 6172 6e69 6e67 206d 6f64  ine learning mod
-00000690: 656c 7320 696e 2050 7974 686f 6e2e 2049  els in Python. I
-000006a0: 7420 7573 6573 206d 6574 686f 6473 2066  t uses methods f
-000006b0: 726f 6d20 2a2a 4d61 6368 696e 6520 4c65  rom **Machine Le
-000006c0: 6172 6e69 6e67 2045 7870 6c61 696e 6162  arning Explainab
-000006d0: 696c 6974 792a 2a20 616e 6420 7072 6f76  ility** and prov
-000006e0: 6964 6573 2061 2073 7461 6e64 6172 6469  ides a standardi
-000006f0: 7a65 6420 4150 4920 746f 2063 7265 6174  zed API to creat
-00000700: 6520 6665 6174 7572 6520 696d 706f 7274  e feature import
-00000710: 616e 6365 2065 7870 6c61 6e61 7469 6f6e  ance explanation
-00000720: 7320 666f 7220 7361 6d70 6c65 732e 2054  s for samples. T
-00000730: 6865 2065 7870 6c61 6e61 7469 6f6e 7320  he explanations 
-00000740: 6172 6520 6765 6e65 7261 7465 6420 696e  are generated in
-00000750: 2074 6865 2066 6f72 6d20 6f66 2070 6c6f   the form of plo
-00000760: 7473 2061 6e64 2074 6578 742e 0d0a 2020  ts and text...  
-00000770: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000780: 6578 706c 6169 6e79 2063 6f6d 6573 2077  explainy comes w
-00000790: 6974 6820 666f 7572 2064 6966 6665 7265  ith four differe
-000007a0: 6e74 2061 6c67 6f72 6974 686d 7320 746f  nt algorithms to
-000007b0: 2063 7265 6174 6520 6569 7468 6572 2067   create either g
-000007c0: 6c6f 6261 6c20 6f72 206c 6f63 616c 2061  lobal or local a
-000007d0: 6e64 2063 6f6e 7472 6173 7469 7665 206f  nd contrastive o
-000007e0: 7220 6e6f 6e2d 636f 6e74 7261 7374 6976  r non-contrastiv
-000007f0: 6520 6d61 6368 696e 6520 6c65 6172 6e69  e machine learni
-00000800: 6e67 206d 6f64 656c 2065 7870 6c61 6e61  ng model explana
-00000810: 7469 6f6e 732e 0d0a 2020 2020 2020 2020  tions...        
-00000820: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00000830: 2020 2020 2323 2044 6f63 756d 656e 7461      ## Documenta
-00000840: 7469 6f6e 0d0a 2020 2020 2020 2020 6874  tion..        ht
-00000850: 7470 733a 2f2f 6578 706c 6169 6e79 2e72  tps://explainy.r
-00000860: 6561 6474 6865 646f 6373 2e69 6f0d 0a20  eadthedocs.io.. 
-00000870: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000880: 200d 0a20 2020 2020 2020 2023 2320 496e   ..        ## In
-00000890: 7374 616c 6c20 6578 706c 6169 6e79 0d0a  stall explainy..
-000008a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000008b0: 2020 6060 600d 0a20 2020 2020 2020 2070    ```..        p
-000008c0: 6970 2069 6e73 7461 6c6c 2065 7870 6c61  ip install expla
-000008d0: 696e 790d 0a20 2020 2020 2020 2060 6060  iny..        ```
-000008e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000008f0: 2020 2020 2323 2055 7361 6765 0d0a 2020      ## Usage..  
-00000900: 2020 2020 2020 6060 6070 7974 686f 6e0d        ```python.
-00000910: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00000920: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00000930: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000940: 6672 6f6d 2073 6b6c 6561 726e 2e64 6174  from sklearn.dat
-00000950: 6173 6574 7320 696d 706f 7274 206c 6f61  asets import loa
-00000960: 645f 6469 6162 6574 6573 0d0a 2020 2020  d_diabetes..    
-00000970: 2020 2020 6672 6f6d 2073 6b6c 6561 726e      from sklearn
-00000980: 2e65 6e73 656d 626c 6520 696d 706f 7274  .ensemble import
-00000990: 2052 616e 646f 6d46 6f72 6573 7452 6567   RandomForestReg
-000009a0: 7265 7373 6f72 0d0a 2020 2020 2020 2020  ressor..        
-000009b0: 6672 6f6d 2073 6b6c 6561 726e 2e6d 6f64  from sklearn.mod
-000009c0: 656c 5f73 656c 6563 7469 6f6e 2069 6d70  el_selection imp
-000009d0: 6f72 7420 7472 6169 6e5f 7465 7374 5f73  ort train_test_s
-000009e0: 706c 6974 0d0a 2020 2020 2020 2020 0d0a  plit..        ..
-000009f0: 2020 2020 2020 2020 6469 6162 6574 6573          diabetes
-00000a00: 203d 206c 6f61 645f 6469 6162 6574 6573   = load_diabetes
-00000a10: 2829 0d0a 2020 2020 2020 2020 585f 7472  ()..        X_tr
-00000a20: 6169 6e2c 2058 5f74 6573 742c 2079 5f74  ain, X_test, y_t
-00000a30: 7261 696e 2c20 795f 7465 7374 203d 2074  rain, y_test = t
-00000a40: 7261 696e 5f74 6573 745f 7370 6c69 7428  rain_test_split(
-00000a50: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-00000a60: 6162 6574 6573 2e64 6174 612c 2064 6961  abetes.data, dia
-00000a70: 6265 7465 732e 7461 7267 6574 2c20 7261  betes.target, ra
-00000a80: 6e64 6f6d 5f73 7461 7465 3d30 0d0a 2020  ndom_state=0..  
-00000a90: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00000aa0: 2058 5f74 6573 7420 3d20 7064 2e44 6174   X_test = pd.Dat
-00000ab0: 6146 7261 6d65 2858 5f74 6573 742c 2063  aFrame(X_test, c
-00000ac0: 6f6c 756d 6e73 3d64 6961 6265 7465 732e  olumns=diabetes.
-00000ad0: 6665 6174 7572 655f 6e61 6d65 7329 0d0a  feature_names)..
-00000ae0: 2020 2020 2020 2020 795f 7465 7374 203d          y_test =
-00000af0: 2070 642e 4461 7461 4672 616d 6528 795f   pd.DataFrame(y_
-00000b00: 7465 7374 290d 0a20 2020 2020 2020 200d  test)..        .
-00000b10: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
-00000b20: 2052 616e 646f 6d46 6f72 6573 7452 6567   RandomForestReg
-00000b30: 7265 7373 6f72 2872 616e 646f 6d5f 7374  ressor(random_st
-00000b40: 6174 653d 3029 2e66 6974 2858 5f74 7261  ate=0).fit(X_tra
-00000b50: 696e 2c20 795f 7472 6169 6e29 0d0a 2020  in, y_train)..  
-00000b60: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
-00000b70: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-00000b80: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00000b90: 0d0a 2020 2020 2020 2020 6672 6f6d 2065  ..        from e
-00000ba0: 7870 6c61 696e 792e 6578 706c 616e 6174  xplainy.explanat
-00000bb0: 696f 6e2e 7065 726d 7574 6174 696f 6e5f  ion.permutation_
-00000bc0: 6578 706c 616e 6174 696f 6e20 696d 706f  explanation impo
-00000bd0: 7274 2050 6572 6d75 7461 7469 6f6e 4578  rt PermutationEx
-00000be0: 706c 616e 6174 696f 6e0d 0a20 2020 2020  planation..     
-00000bf0: 2020 200d 0a20 2020 2020 2020 206e 756d     ..        num
-00000c00: 6265 725f 6f66 5f66 6561 7475 7265 7320  ber_of_features 
-00000c10: 3d20 340d 0a20 2020 2020 2020 2073 616d  = 4..        sam
-00000c20: 706c 655f 696e 6465 7820 3d20 310d 0a20  ple_index = 1.. 
-00000c30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000c40: 2065 7870 6c61 696e 6572 203d 2050 6572   explainer = Per
-00000c50: 6d75 7461 7469 6f6e 4578 706c 616e 6174  mutationExplanat
-00000c60: 696f 6e28 0d0a 2020 2020 2020 2020 2020  ion(..          
-00000c70: 2020 585f 7465 7374 2c20 795f 7465 7374    X_test, y_test
-00000c80: 2c20 6d6f 6465 6c2c 206e 756d 6265 725f  , model, number_
-00000c90: 6f66 5f66 6561 7475 7265 730d 0a20 2020  of_features..   
-00000ca0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00000cb0: 0d0a 2020 2020 2020 2020 6578 706c 616e  ..        explan
-00000cc0: 6174 696f 6e20 3d20 6578 706c 6169 6e65  ation = explaine
-00000cd0: 722e 6578 706c 6169 6e28 0d0a 2020 2020  r.explain(..    
-00000ce0: 2020 2020 2020 2020 7361 6d70 6c65 5f69          sample_i
-00000cf0: 6e64 6578 2c20 7365 7061 7261 746f 723d  ndex, separator=
-00000d00: 275c 6e27 0d0a 2020 2020 2020 2020 290d  '\n'..        ).
-00000d10: 0a20 2020 2020 2020 2070 7269 6e74 2865  .        print(e
-00000d20: 7870 6c61 6e61 7469 6f6e 290d 0a20 2020  xplanation)..   
-00000d30: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
-00000d40: 2020 3e20 5468 6520 5261 6e64 6f6d 466f    > The RandomFo
-00000d50: 7265 7374 5265 6772 6573 736f 7220 7573  restRegressor us
-00000d60: 6564 2031 3020 6665 6174 7572 6573 2074  ed 10 features t
-00000d70: 6f20 7072 6f64 7563 6520 7468 6520 7072  o produce the pr
-00000d80: 6564 6963 7469 6f6e 732e 2054 6865 2070  edictions. The p
-00000d90: 7265 6469 6374 696f 6e20 6f66 2074 6869  rediction of thi
-00000da0: 7320 7361 6d70 6c65 2077 6173 2032 3531  s sample was 251
-00000db0: 2e38 2e0d 0a20 2020 2020 2020 200d 0a20  .8...        .. 
-00000dc0: 2020 2020 2020 203e 2054 6865 2066 6561         > The fea
-00000dd0: 7475 7265 2069 6d70 6f72 7461 6e63 6520  ture importance 
-00000de0: 7761 7320 6361 6c63 756c 6174 6564 2075  was calculated u
-00000df0: 7369 6e67 2074 6865 2050 6572 6d75 7461  sing the Permuta
-00000e00: 7469 6f6e 2046 6561 7475 7265 2049 6d70  tion Feature Imp
-00000e10: 6f72 7461 6e63 6520 6d65 7468 6f64 2e0d  ortance method..
-00000e20: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000e30: 2020 203e 2054 6865 2066 6f75 7220 6665     > The four fe
-00000e40: 6174 7572 6573 2077 6869 6368 2077 6572  atures which wer
-00000e50: 6520 6d6f 7374 2069 6d70 6f72 7461 6e74  e most important
-00000e60: 2066 6f72 2074 6865 2070 7265 6469 6374   for the predict
-00000e70: 696f 6e73 2077 6572 6520 2866 726f 6d20  ions were (from 
-00000e80: 6869 6768 6573 7420 746f 206c 6f77 6573  highest to lowes
-00000e90: 7429 3a20 2762 6d69 2720 2830 2e31 3529  t): 'bmi' (0.15)
-00000ea0: 2c20 2773 3527 2028 302e 3132 292c 2027  , 's5' (0.12), '
-00000eb0: 6270 2720 2830 2e30 3329 2c20 616e 6420  bp' (0.03), and 
-00000ec0: 2761 6765 2720 2830 2e30 3229 2e0d 0a20  'age' (0.02)... 
-00000ed0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000ee0: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
-00000ef0: 2020 2020 6578 706c 6169 6e65 722e 706c      explainer.pl
-00000f00: 6f74 2829 0d0a 2020 2020 2020 2020 6060  ot()..        ``
-00000f10: 600d 0a20 2020 2020 2020 2021 5b50 6572  `..        ![Per
-00000f20: 6d75 7461 7469 6f6e 2046 6561 7475 7265  mutation Feature
-00000f30: 2049 6d70 6f72 7461 6e63 655d 2873 7461   Importance](sta
-00000f40: 7469 632f 7065 726d 7574 6174 696f 6e5f  tic/permutation_
-00000f50: 696d 706f 7274 616e 6365 2e70 6e67 290d  importance.png).
-00000f60: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-00000f70: 6f6e 0d0a 2020 2020 2020 2020 6578 706c  on..        expl
-00000f80: 6169 6e65 722e 7361 7665 2873 616d 706c  ainer.save(sampl
-00000f90: 655f 696e 6465 7829 0d0a 2020 2020 2020  e_index)..      
-00000fa0: 2020 6060 600d 0a20 2020 2020 2020 200d    ```..        .
-00000fb0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000fc0: 2020 2023 2320 4d6f 6465 6c20 4578 706c     ## Model Expl
-00000fd0: 616e 6174 696f 6e73 0d0a 2020 2020 2020  anations..      
-00000fe0: 2020 0d0a 2020 2020 2020 2020 7c20 4d65    ..        | Me
-00000ff0: 7468 6f64 0909 0909 7c54 7970 6520 7c20  thod....|Type | 
-00001000: 4578 706c 616e 6174 696f 6e73 207c 2043  Explanations | C
-00001010: 6c61 7373 6966 6963 6174 696f 6e20 7c20  lassification | 
-00001020: 5265 6772 6573 7369 6f6e 207c 200d 0a20  Regression | .. 
-00001030: 2020 2020 2020 207c 202d 2d2d 2009 0909         | --- ...
-00001040: 097c 202d 2d2d 207c 202d 2d2d 207c 203a  .| --- | --- | :
-00001050: 2d2d 2d3a 207c 203a 2d2d 2d3a 207c 200d  ---: | :---: | .
-00001060: 0a20 2020 2020 2020 207c 5b50 6572 6d75  .        |[Permu
-00001070: 7461 7469 6f6e 2046 6561 7475 7265 2049  tation Feature I
-00001080: 6d70 6f72 7461 6e63 655d 2868 7474 7073  mportance](https
-00001090: 3a2f 2f65 7870 6c61 696e 792e 7265 6164  ://explainy.read
-000010a0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000010b0: 7465 7374 2f65 7870 6c61 696e 792e 6578  test/explainy.ex
-000010c0: 706c 616e 6174 696f 6e2e 6874 6d6c 236d  planation.html#m
-000010d0: 6f64 756c 652d 6578 706c 6169 6e79 2e65  odule-explainy.e
-000010e0: 7870 6c61 6e61 7469 6f6e 2e70 6572 6d75  xplanation.permu
-000010f0: 7461 7469 6f6e 5f65 7870 6c61 6e61 7469  tation_explanati
-00001100: 6f6e 2909 7c20 4e6f 6e2d 636f 6e74 7261  on).| Non-contra
-00001110: 7374 6976 6520 7c20 676c 6f62 616c 207c  stive | global |
-00001120: 2020 3a73 7461 723a 207c 203a 7374 6172    :star: | :star
-00001130: 3a7c 0d0a 2020 2020 2020 2020 7c20 5368  :|..        | Sh
-00001140: 6170 6c65 7920 5661 6c75 6573 0909 7c20  apley Values..| 
-00001150: 4e6f 6e2d 636f 6e74 7261 7374 6976 6520  Non-contrastive 
-00001160: 7c20 6c6f 6361 6c20 7c20 2020 3a73 7461  | local |   :sta
-00001170: 723a 207c 203a 7374 6172 3a7c 0d0a 2020  r: | :star:|..  
-00001180: 2020 2020 2020 7c47 6c6f 6261 6c20 5375        |Global Su
-00001190: 7272 6f67 6174 6520 4d6f 6465 6c7c 436f  rrogate Model|Co
-000011a0: 6e74 7261 7374 6976 6520 7c20 676c 6f62  ntrastive | glob
-000011b0: 616c 207c 203a 7374 6172 3a20 7c20 3a73  al | :star: | :s
-000011c0: 7461 723a 7c0d 0a20 2020 2020 2020 207c  tar:|..        |
-000011d0: 436f 756e 7465 7266 6163 7475 616c 2045  Counterfactual E
-000011e0: 7861 6d70 6c65 7c20 436f 6e74 7261 7374  xample| Contrast
-000011f0: 6976 6520 7c20 6c6f 6361 6c20 7c3a 7374  ive | local |:st
-00001200: 6172 3a20 7c20 3a73 7461 723a 7c0d 0a20  ar: | :star:|.. 
-00001210: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001220: 200d 0a20 2020 2020 2020 2044 6573 6372   ..        Descr
-00001230: 6970 7469 6f6e 0d0a 2020 2020 2020 2020  iption..        
-00001240: 2d20 676c 6f62 616c 3a20 0d0a 2020 2020  - global: ..    
-00001250: 2020 2020 2d20 6c6f 6361 6c3a 0d0a 2020      - local:..  
-00001260: 2020 2020 2020 2d20 636f 6e74 7261 7374        - contrast
-00001270: 6976 653a 090d 0a20 2020 2020 2020 202d  ive:...        -
-00001280: 206e 6f6e 2d63 6f6e 7472 6173 7469 7665   non-contrastive
-00001290: 3a09 0d0a 2020 2020 2020 2020 0d0a 2020  :...        ..  
-000012a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000012b0: 0d0a 2020 2020 2020 2020 2323 2046 6561  ..        ## Fea
-000012c0: 7475 7265 730d 0a20 2020 2020 2020 200d  tures..        .
-000012d0: 0a20 2020 2020 2020 2054 4f44 4f0d 0a20  .        TODO.. 
-000012e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000012f0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00001300: 2020 2020 2023 2320 4578 706c 616e 6174       ## Explanat
-00001310: 696f 6e73 0d0a 2020 2020 2020 2020 0d0a  ions..        ..
-00001320: 2020 2020 2020 2020 2323 2320 5065 726d          ### Perm
-00001330: 7574 6174 696f 6e20 4665 6174 7572 6520  utation Feature 
-00001340: 496d 706f 7274 616e 6365 0d0a 2020 2020  Importance..    
-00001350: 2020 2020 0d0a 2020 2020 2020 2020 5065      ..        Pe
-00001360: 726d 7574 6174 696f 6e20 6665 6174 7572  rmutation featur
-00001370: 6520 696d 706f 7274 616e 6365 206d 6561  e importance mea
-00001380: 7375 7265 7320 7468 6520 696e 6372 6561  sures the increa
-00001390: 7365 2069 6e20 7468 6520 7072 6564 6963  se in the predic
-000013a0: 7469 6f6e 2065 7272 6f72 206f 6620 7468  tion error of th
-000013b0: 6520 6d6f 6465 6c20 6166 7465 7220 7765  e model after we
-000013c0: 2070 6572 6d75 7465 6420 7468 6520 6665   permuted the fe
-000013d0: 6174 7572 6527 7320 7661 6c75 6573 2c20  ature's values, 
-000013e0: 7768 6963 6820 6272 6561 6b73 2074 6865  which breaks the
-000013f0: 2072 656c 6174 696f 6e73 6869 7020 6265   relationship be
-00001400: 7477 6565 6e20 7468 6520 6665 6174 7572  tween the featur
-00001410: 6520 616e 6420 7468 6520 7472 7565 206f  e and the true o
-00001420: 7574 636f 6d65 205b 315d 2e0d 0a20 2020  utcome [1]...   
-00001430: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00001440: 2323 2320 4368 6172 6163 7465 7269 7374  ### Characterist
-00001450: 6963 730d 0a20 2020 2020 2020 202d 2067  ics..        - g
-00001460: 6c6f 6261 6c0d 0a20 2020 2020 2020 202d  lobal..        -
-00001470: 206e 6f6e 2d63 6f6e 7472 6173 7469 7665   non-contrastive
-00001480: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001490: 2020 2020 215b 5065 726d 7574 6174 696f      ![Permutatio
-000014a0: 6e20 4665 6174 7572 6520 496d 706f 7274  n Feature Import
-000014b0: 616e 6365 5d28 646f 6373 2f5f 7374 6174  ance](docs/_stat
-000014c0: 6963 2f70 6572 6d75 7461 7469 6f6e 2e70  ic/permutation.p
-000014d0: 6e67 290d 0a20 2020 2020 2020 200d 0a20  ng)..        .. 
-000014e0: 2020 2020 2020 2023 2323 2053 6861 706c         ### Shapl
-000014f0: 6579 2056 616c 7565 730d 0a20 2020 2020  ey Values..     
-00001500: 2020 2041 2070 7265 6469 6374 696f 6e20     A prediction 
-00001510: 6361 6e20 6265 2065 7870 6c61 696e 6564  can be explained
-00001520: 2062 7920 6173 7375 6d69 6e67 2074 6861   by assuming tha
-00001530: 7420 6561 6368 2066 6561 7475 7265 2076  t each feature v
-00001540: 616c 7565 206f 6620 2074 6865 2069 6e73  alue of  the ins
-00001550: 7461 6e63 6520 6973 2061 2022 706c 6179  tance is a "play
-00001560: 6572 2220 696e 2061 2067 616d 6520 7768  er" in a game wh
-00001570: 6572 6520 7468 6520 7072 6564 6963 7469  ere the predicti
-00001580: 6f6e 2069 7320 7468 6520 7061 796f 7574  on is the payout
-00001590: 2e20 2053 6861 706c 6579 2076 616c 7565  .  Shapley value
-000015a0: 7320 2861 206d 6574 686f 6420 6672 6f6d  s (a method from
-000015b0: 2063 6f61 6c69 7469 6f6e 616c 2067 616d   coalitional gam
-000015c0: 6520 7468 656f 7279 2920 7465 6c6c 7320  e theory) tells 
-000015d0: 7573 2068 6f77 2020 746f 2066 6169 726c  us how  to fairl
-000015e0: 7920 6469 7374 7269 6275 7465 2074 6865  y distribute the
-000015f0: 2022 7061 796f 7574 2220 616d 6f6e 6720   "payout" among 
-00001600: 7468 6520 6665 6174 7572 6573 2e20 5468  the features. Th
-00001610: 6520 5368 6170 6c65 7920 7661 6c75 6520  e Shapley value 
-00001620: 6973 2074 6865 2061 7665 7261 6765 206d  is the average m
-00001630: 6172 6769 6e61 6c20 636f 6e74 7269 6275  arginal contribu
-00001640: 7469 6f6e 206f 6620 6120 6665 6174 7572  tion of a featur
-00001650: 6520 7661 6c75 6520 6163 726f 7373 2061  e value across a
-00001660: 6c6c 2070 6f73 7369 626c 6520 636f 616c  ll possible coal
-00001670: 6974 696f 6e73 205b 315d 2e0d 0a20 2020  itions [1]...   
-00001680: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00001690: 2323 2320 4368 6172 6163 7465 7269 7374  ### Characterist
-000016a0: 6963 730d 0a20 2020 2020 2020 202d 206c  ics..        - l
-000016b0: 6f63 616c 0d0a 2020 2020 2020 2020 2d20  ocal..        - 
-000016c0: 6e6f 6e2d 636f 6e74 7261 7374 6976 650d  non-contrastive.
-000016d0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000016e0: 2020 2021 5b53 6861 706c 6579 2056 616c     ![Shapley Val
-000016f0: 7565 735d 2864 6f63 732f 5f73 7461 7469  ues](docs/_stati
-00001700: 632f 7368 6170 6c65 792e 706e 6729 0d0a  c/shapley.png)..
-00001710: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001720: 2020 0d0a 2020 2020 2020 2020 2323 2320    ..        ### 
-00001730: 436f 756e 7465 7266 6163 7475 616c 2065  Counterfactual e
-00001740: 7870 6c61 6e61 7469 6f6e 730d 0a20 2020  xplanations..   
-00001750: 2020 2020 2043 6f75 6e74 6572 6661 6374       Counterfact
-00001760: 7561 6c20 6578 706c 616e 6174 696f 6e73  ual explanations
-00001770: 2074 656c 6c20 7573 2068 6f77 2074 6865   tell us how the
-00001780: 2076 616c 7565 7320 6f66 2061 6e20 696e   values of an in
-00001790: 7374 616e 6365 2068 6176 6520 746f 2063  stance have to c
-000017a0: 6861 6e67 6520 746f 2073 6967 6e69 6669  hange to signifi
-000017b0: 6361 6e74 6c79 2063 6861 6e67 6520 6974  cantly change it
-000017c0: 7320 7072 6564 6963 7469 6f6e 2e20 4120  s prediction. A 
-000017d0: 636f 756e 7465 7266 6163 7475 616c 2065  counterfactual e
-000017e0: 7870 6c61 6e61 7469 6f6e 206f 6620 6120  xplanation of a 
-000017f0: 7072 6564 6963 7469 6f6e 2064 6573 6372  prediction descr
-00001800: 6962 6573 2074 6865 2073 6d61 6c6c 6573  ibes the smalles
-00001810: 7420 6368 616e 6765 2074 6f20 7468 6520  t change to the 
-00001820: 6665 6174 7572 6520 7661 6c75 6573 2074  feature values t
-00001830: 6861 7420 6368 616e 6765 7320 7468 6520  hat changes the 
-00001840: 7072 6564 6963 7469 6f6e 2074 6f20 6120  prediction to a 
-00001850: 7072 6564 6566 696e 6564 206f 7574 7075  predefined outpu
-00001860: 742e 2042 7920 6372 6561 7469 6e67 2063  t. By creating c
-00001870: 6f75 6e74 6572 6661 6374 7561 6c20 696e  ounterfactual in
-00001880: 7374 616e 6365 732c 2077 6520 6c65 6172  stances, we lear
-00001890: 6e20 6162 6f75 7420 686f 7720 7468 6520  n about how the 
-000018a0: 6d6f 6465 6c20 6d61 6b65 7320 6974 7320  model makes its 
-000018b0: 7072 6564 6963 7469 6f6e 7320 616e 6420  predictions and 
-000018c0: 6361 6e20 6578 706c 6169 6e20 696e 6469  can explain indi
-000018d0: 7669 6475 616c 2070 7265 6469 6374 696f  vidual predictio
-000018e0: 6e73 205b 315d 2e0d 0a20 2020 2020 2020  ns [1]...       
-000018f0: 200d 0a20 2020 2020 2020 2023 2323 2320   ..        #### 
-00001900: 4368 6172 6163 7465 7269 7374 6963 730d  Characteristics.
-00001910: 0a20 2020 2020 2020 202d 206c 6f63 616c  .        - local
-00001920: 0d0a 2020 2020 2020 2020 2d20 636f 6e74  ..        - cont
-00001930: 7261 7374 6976 650d 0a20 2020 2020 2020  rastive..       
-00001940: 200d 0a20 2020 2020 2020 2021 5b43 6f75   ..        ![Cou
-00001950: 6e74 6572 6661 6374 7561 6c20 4578 616d  nterfactual Exam
-00001960: 706c 655d 2864 6f63 732f 5f73 7461 7469  ple](docs/_stati
-00001970: 632f 636f 756e 7465 7266 6163 7475 616c  c/counterfactual
-00001980: 2e70 6e67 290d 0a20 2020 2020 2020 200d  .png)..        .
-00001990: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000019a0: 2020 2023 2323 2047 6c6f 6261 6c20 5375     ### Global Su
-000019b0: 7272 6f67 6174 6520 4d6f 6465 6c20 2844  rrogate Model (D
-000019c0: 6563 6973 696f 6e20 5472 6565 290d 0a20  ecision Tree).. 
-000019d0: 2020 2020 2020 2041 2067 6c6f 6261 6c20         A global 
-000019e0: 7375 7272 6f67 6174 6520 6d6f 6465 6c20  surrogate model 
-000019f0: 6973 2061 6e20 696e 7465 7270 7265 7461  is an interpreta
-00001a00: 626c 6520 6d6f 6465 6c20 7468 6174 2069  ble model that i
-00001a10: 7320 7472 6169 6e65 6420 746f 2061 7070  s trained to app
-00001a20: 726f 7869 6d61 7465 2074 6865 2070 7265  roximate the pre
-00001a30: 6469 6374 696f 6e73 206f 6620 6120 626c  dictions of a bl
-00001a40: 6163 6b20 626f 7820 6d6f 6465 6c2e 2057  ack box model. W
-00001a50: 6520 6361 6e20 6472 6177 2063 6f6e 636c  e can draw concl
-00001a60: 7573 696f 6e73 2061 626f 7574 2074 6865  usions about the
-00001a70: 2062 6c61 636b 2062 6f78 206d 6f64 656c   black box model
-00001a80: 2062 7920 696e 7465 7270 7265 7469 6e67   by interpreting
-00001a90: 2074 6865 2073 7572 726f 6761 7465 206d   the surrogate m
-00001aa0: 6f64 656c 205b 315d 2e0d 0a20 2020 2020  odel [1]...     
-00001ab0: 2020 200d 0a20 2020 2020 2020 2023 2323     ..        ###
-00001ac0: 2320 4368 6172 6163 7465 7269 7374 6963  # Characteristic
-00001ad0: 730d 0a20 2020 2020 2020 202d 2067 6c6f  s..        - glo
-00001ae0: 6261 6c0d 0a20 2020 2020 2020 202d 2063  bal..        - c
-00001af0: 6f6e 7472 6173 7469 7665 0d0a 2020 2020  ontrastive..    
-00001b00: 2020 2020 0d0a 2020 2020 2020 2020 215b      ..        ![
-00001b10: 476c 6f62 616c 2053 7572 726f 6761 7465  Global Surrogate
-00001b20: 204d 6f64 656c 5d28 646f 6373 2f5f 7374   Model](docs/_st
-00001b30: 6174 6963 2f73 7572 726f 6761 7465 2e70  atic/surrogate.p
-00001b40: 6e67 290d 0a20 2020 2020 2020 200d 0a20  ng)..        .. 
-00001b50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001b60: 2023 2320 536f 7572 6365 0d0a 2020 2020   ## Source..    
-00001b70: 2020 2020 0d0a 2020 2020 2020 2020 5b31      ..        [1
-00001b80: 5d20 4d6f 6c6e 6172 2c20 4368 7269 7374  ] Molnar, Christ
-00001b90: 6f70 682e 2022 496e 7465 7270 7265 7461  oph. "Interpreta
-00001ba0: 626c 6520 6d61 6368 696e 6520 6c65 6172  ble machine lear
-00001bb0: 6e69 6e67 2e20 4120 4775 6964 6520 666f  ning. A Guide fo
-00001bc0: 7220 4d61 6b69 6e67 2042 6c61 636b 2042  r Making Black B
-00001bd0: 6f78 204d 6f64 656c 7320 4578 706c 6169  ox Models Explai
-00001be0: 6e61 626c 6522 2c20 3230 3139 2e20 6874  nable", 2019. ht
-00001bf0: 7470 733a 2f2f 6368 7269 7374 6f70 686d  tps://christophm
-00001c00: 2e67 6974 6875 622e 696f 2f69 6e74 6572  .github.io/inter
-00001c10: 7072 6574 6162 6c65 2d6d 6c2d 626f 6f6b  pretable-ml-book
-00001c20: 2f0d 0a20 2020 2020 2020 200d 0a20 2020  /..        ..   
-00001c30: 2020 2020 2023 2320 4175 7468 6f72 730d       ## Authors.
-00001c40: 0a20 2020 2020 2020 202a 202a 2a4d 6175  .        * **Mau
-00001c50: 726f 204c 757a 7a61 7474 6f2a 2a20 2d20  ro Luzzatto** - 
-00001c60: 5b4d 6175 726f 6c5d 2868 7474 7073 3a2f  [Maurol](https:/
-00001c70: 2f67 6974 6875 622e 636f 6d2f 4d61 7572  /github.com/Maur
-00001c80: 6f4c 757a 7a61 7474 6f29 0d0a 2020 2020  oLuzzatto)..    
-00001c90: 2020 2020 0d0a 2020 2020 2020 2020 2222      ..        ""
-00001ca0: 220d 0a4b 6579 776f 7264 733a 2065 7870  "..Keywords: exp
-00001cb0: 6c61 696e 790d 0a50 6c61 7466 6f72 6d3a  lainy..Platform:
-00001cc0: 2055 4e4b 4e4f 574e 0d0a 436c 6173 7369   UNKNOWN..Classi
-00001cd0: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
-00001ce0: 7420 5374 6174 7573 203a 3a20 3220 2d20  t Status :: 2 - 
-00001cf0: 5072 652d 416c 7068 610d 0a43 6c61 7373  Pre-Alpha..Class
-00001d00: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-00001d10: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00001d20: 6c6f 7065 7273 0d0a 436c 6173 7369 6669  lopers..Classifi
-00001d30: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00001d40: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00001d50: 4954 204c 6963 656e 7365 0d0a 436c 6173  IT License..Clas
-00001d60: 7369 6669 6572 3a20 4e61 7475 7261 6c20  sifier: Natural 
-00001d70: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
-00001d80: 6973 680d 0a43 6c61 7373 6966 6965 723a  ish..Classifier:
-00001d90: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00001da0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00001db0: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
-00001dc0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00001dd0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00001de0: 203a 3a20 332e 360d 0a43 6c61 7373 6966   :: 3.6..Classif
-00001df0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00001e00: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00001e10: 686f 6e20 3a3a 2033 2e37 0d0a 436c 6173  hon :: 3.7..Clas
-00001e20: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00001e30: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00001e40: 5079 7468 6f6e 203a 3a20 332e 380d 0a52  Python :: 3.8..R
-00001e50: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00001e60: 3e3d 332e 360d 0a44 6573 6372 6970 7469  >=3.6..Descripti
-00001e70: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-00001e80: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000000: 0a3c 212d 2d20 3c69 6d67 2073 7263 3d22  .<!-- <img src="
+00000010: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000020: 6f6d 2f4d 6175 726f 4c75 7a7a 6174 746f  om/MauroLuzzatto
+00000030: 2f65 7870 6c61 696e 792f 7261 772f 6d61  /explainy/raw/ma
+00000040: 696e 2f64 6f63 732f 5f73 7461 7469 632f  in/docs/_static/
+00000050: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
+00000060: 2231 3830 2220 6865 6967 6874 3d22 3138  "180" height="18
+00000070: 3022 2061 6c69 676e 3d22 7269 6768 7422  0" align="right"
+00000080: 2f3e 202d 2d3e 0a3c 7020 616c 6967 6e3d  /> -->.<p align=
+00000090: 2263 656e 7465 7222 3e0a 3c69 6d67 2073  "center">.<img s
+000000a0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+000000b0: 7562 2e63 6f6d 2f4d 6175 726f 4c75 7a7a  ub.com/MauroLuzz
+000000c0: 6174 746f 2f65 7870 6c61 696e 792f 7261  atto/explainy/ra
+000000d0: 772f 6d61 696e 2f64 6f63 732f 5f73 7461  w/main/docs/_sta
+000000e0: 7469 632f 6c6f 676f 2e70 6e67 2220 7769  tic/logo.png" wi
+000000f0: 6474 683d 2232 3030 2220 6865 6967 6874  dth="200" height
+00000100: 3d22 3230 3022 2f3e 0a3c 2f70 3e0a 3c21  ="200"/>.</p>.<!
+00000110: 2d2d 2023 2065 7870 6c61 696e 7920 2d20  -- # explainy - 
+00000120: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000130: 206d 6f64 656c 2065 7870 6c61 6e61 7469   model explanati
+00000140: 6f6e 7320 666f 7220 6875 6d61 6e73 202d  ons for humans -
+00000150: 2d3e 0a3c 212d 2d20 2320 6578 706c 6169  ->.<!-- # explai
+00000160: 6e79 202d 2062 6c61 636b 2d62 6f78 206d  ny - black-box m
+00000170: 6f64 656c 2065 7870 6c61 6e61 7469 6f6e  odel explanation
+00000180: 7320 666f 7220 6875 6d61 6e73 202d 2d3e  s for humans -->
+00000190: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
+000001a0: 7465 7222 3e65 7870 6c61 696e 7920 2d20  ter">explainy - 
+000001b0: 626c 6163 6b2d 626f 7820 6d6f 6465 6c20  black-box model 
+000001c0: 6578 706c 616e 6174 696f 6e73 2066 6f72  explanations for
+000001d0: 2068 756d 616e 733c 2f68 313e 0a0a 5b21   humans</h1>..[!
+000001e0: 5b70 7970 6920 7665 7273 696f 6e5d 2868  [pypi version](h
+000001f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000200: 6473 2e69 6f2f 7079 7069 2f76 2f65 7870  ds.io/pypi/v/exp
+00000210: 6c61 696e 792e 7376 6729 5d28 6874 7470  lainy.svg)](http
+00000220: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000230: 6f72 672f 7079 7069 2f65 7870 6c61 696e  org/pypi/explain
+00000240: 7929 0a5b 215b 636f 6465 636f 765d 2868  y).[![codecov](h
+00000250: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
+00000260: 6f2f 6768 2f4d 6175 726f 4c75 7a7a 6174  o/gh/MauroLuzzat
+00000270: 746f 2f65 7870 6c61 696e 792f 6272 616e  to/explainy/bran
+00000280: 6368 2f6d 6169 6e2f 6772 6170 682f 6261  ch/main/graph/ba
+00000290: 6467 652e 7376 673f 746f 6b65 6e3d 4e36  dge.svg?token=N6
+000002a0: 454b 484d 4541 5152 295d 2868 7474 7073  EKHMEAQR)](https
+000002b0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+000002c0: 2f4d 6175 726f 4c75 7a7a 6174 746f 2f65  /MauroLuzzatto/e
+000002d0: 7870 6c61 696e 7929 0a5b 215b 646f 6373  xplainy).[![docs
+000002e0: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
+000002f0: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000300: 7473 2f65 7870 6c61 696e 792f 6261 6467  ts/explainy/badg
+00000310: 652f 3f76 6572 7369 6f6e 3d6c 6174 6573  e/?version=lates
+00000320: 7429 5d28 6874 7470 733a 2f2f 6578 706c  t)](https://expl
+00000330: 6169 6e79 2e72 6561 6474 6865 646f 6373  ainy.readthedocs
+00000340: 2e69 6f2f 656e 2f6c 6174 6573 742f 3f76  .io/en/latest/?v
+00000350: 6572 7369 6f6e 3d6c 6174 6573 7429 0a5b  ersion=latest).[
+00000360: 215b 5375 7070 6f72 7465 6420 7665 7273  ![Supported vers
+00000370: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
+00000380: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000390: 692f 7079 7665 7273 696f 6e73 2f65 7870  i/pyversions/exp
+000003a0: 6c61 696e 792e 7376 6729 5d28 6874 7470  lainy.svg)](http
+000003b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000003c0: 6a65 6374 2f65 7870 6c61 696e 7929 0a5b  ject/explainy).[
+000003d0: 215b 436f 6465 2073 7479 6c65 3a20 626c  ![Code style: bl
+000003e0: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
+000003f0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000400: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+00000410: 6c61 636b 2d30 3030 3030 302e 7376 673f  lack-000000.svg?
+00000420: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+00000430: 6529 5d28 6874 7470 733a 2f2f 6769 7468  e)](https://gith
+00000440: 7562 2e63 6f6d 2f61 6d62 762f 626c 6163  ub.com/ambv/blac
+00000450: 6b29 0a5b 215b 496d 706f 7274 733a 2069  k).[![Imports: i
+00000460: 736f 7274 5d28 6874 7470 733a 2f2f 696d  sort](https://im
+00000470: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000480: 6765 2f25 3230 696d 706f 7274 732d 6973  ge/%20imports-is
+00000490: 6f72 742d 2532 3331 3637 3462 313f 7374  ort-%231674b1?st
+000004a0: 796c 653d 666c 6174 266c 6162 656c 436f  yle=flat&labelCo
+000004b0: 6c6f 723d 6566 3833 3336 295d 2868 7474  lor=ef8336)](htt
+000004c0: 7073 3a2f 2f70 7963 7161 2e67 6974 6875  ps://pycqa.githu
+000004d0: 622e 696f 2f69 736f 7274 2f29 0a5b 215b  b.io/isort/).[![
+000004e0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
+000004f0: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+00000500: 6765 2f65 7870 6c61 696e 7929 5d28 6874  ge/explainy)](ht
+00000510: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00000520: 7072 6f6a 6563 742f 6578 706c 6169 6e79  project/explainy
+00000530: 290a 0a3c 212d 2d20 5b21 5b74 7261 7669  )..<!-- [![travi
+00000540: 735d 2868 7474 7073 3a2f 2f61 7070 2e74  s](https://app.t
+00000550: 7261 7669 732d 6369 2e63 6f6d 2f4d 6175  ravis-ci.com/Mau
+00000560: 726f 4c75 7a7a 6174 746f 2f65 7870 6c61  roLuzzatto/expla
+00000570: 696e 792e 7376 673f 6272 616e 6368 3d6d  iny.svg?branch=m
+00000580: 6169 6e29 5d28 6874 7470 733a 2f2f 6170  ain)](https://ap
+00000590: 702e 7472 6176 6973 2d63 692e 636f 6d2f  p.travis-ci.com/
+000005a0: 6769 7468 7562 2f4d 6175 726f 4c75 7a7a  github/MauroLuzz
+000005b0: 6174 746f 2f65 7870 6c61 696e 793f 6272  atto/explainy?br
+000005c0: 616e 6368 3d6d 6173 7465 7229 202d 2d3e  anch=master) -->
+000005d0: 0a0a 0a2a 2a65 7870 6c61 696e 792a 2a20  ...**explainy** 
+000005e0: 6973 2061 206c 6962 7261 7279 2066 6f72  is a library for
+000005f0: 2067 656e 6572 6174 696e 6720 6d61 6368   generating mach
+00000600: 696e 6520 6c65 6172 6e69 6e67 206d 6f64  ine learning mod
+00000610: 656c 7320 6578 706c 616e 6174 696f 6e73  els explanations
+00000620: 2069 6e20 5079 7468 6f6e 2e20 4974 2075   in Python. It u
+00000630: 7365 7320 6d65 7468 6f64 7320 6672 6f6d  ses methods from
+00000640: 202a 2a4d 6163 6869 6e65 204c 6561 726e   **Machine Learn
+00000650: 696e 6720 4578 706c 6169 6e61 6269 6c69  ing Explainabili
+00000660: 7479 2a2a 2061 6e64 2070 726f 7669 6465  ty** and provide
+00000670: 7320 6120 7374 616e 6461 7264 697a 6564  s a standardized
+00000680: 2041 5049 2074 6f20 6372 6561 7465 2066   API to create f
+00000690: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
+000006a0: 6520 6578 706c 616e 6174 696f 6e73 2066  e explanations f
+000006b0: 6f72 2073 616d 706c 6573 2e20 0a0a 5468  or samples. ..Th
+000006c0: 6520 4150 4920 6973 2069 6e73 7069 7265  e API is inspire
+000006d0: 6420 6279 2060 7363 696b 6974 2d6c 6561  d by `scikit-lea
+000006e0: 726e 6020 616e 6420 6861 7320 7468 7265  rn` and has thre
+000006f0: 6520 636f 7265 206d 6574 686f 6473 2060  e core methods `
+00000700: 6578 706c 6169 6e28 2960 2c20 6070 6c6f  explain()`, `plo
+00000710: 7428 2960 2061 6e64 2c20 6069 6d70 6f72  t()` and, `impor
+00000720: 7461 6e63 6528 2960 2e20 5468 6520 6578  tance()`. The ex
+00000730: 706c 616e 6174 696f 6e73 2061 7265 2067  planations are g
+00000740: 656e 6572 6174 6564 2069 6e20 7468 6520  enerated in the 
+00000750: 666f 726d 206f 6620 7465 7874 7320 616e  form of texts an
+00000760: 6420 706c 6f74 732e 0a0a 2a2a 6578 706c  d plots...**expl
+00000770: 6169 6e79 2a2a 2063 6f6d 6573 2077 6974  ainy** comes wit
+00000780: 6820 666f 7572 2064 6966 6665 7265 6e74  h four different
+00000790: 2061 6c67 6f72 6974 686d 7320 746f 2063   algorithms to c
+000007a0: 7265 6174 6520 6569 7468 6572 202a 676c  reate either *gl
+000007b0: 6f62 616c 2a20 6f72 202a 6c6f 6361 6c2a  obal* or *local*
+000007c0: 2061 6e64 202a 636f 6e74 7261 7374 6976   and *contrastiv
+000007d0: 652a 206f 7220 2a6e 6f6e 2d63 6f6e 7472  e* or *non-contr
+000007e0: 6173 7469 7665 2a20 6d6f 6465 6c20 6578  astive* model ex
+000007f0: 706c 616e 6174 696f 6e73 2e0a 0a0a 7c20  planations....| 
+00000800: 4d65 7468 6f64 0909 0909 7c54 7970 6520  Method....|Type 
+00000810: 7c20 4578 706c 616e 6174 696f 6e73 207c  | Explanations |
+00000820: 2043 6c61 7373 6966 6963 6174 696f 6e20   Classification 
+00000830: 7c20 5265 6772 6573 7369 6f6e 207c 200a  | Regression | .
+00000840: 7c20 2d2d 2d20 0909 0909 7c20 2d2d 2d20  | --- ....| --- 
+00000850: 7c20 3a2d 2d2d 3a20 7c20 3a2d 2d2d 3a20  | :---: | :---: 
+00000860: 7c20 3a2d 2d2d 3a20 7c20 0a7c 5b50 6572  | :---: | .|[Per
+00000870: 6d75 7461 7469 6f6e 2046 6561 7475 7265  mutation Feature
+00000880: 2049 6d70 6f72 7461 6e63 655d 2868 7474   Importance](htt
+00000890: 7073 3a2f 2f65 7870 6c61 696e 792e 7265  ps://explainy.re
+000008a0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000008b0: 6c61 7465 7374 2f65 7870 6c61 696e 792e  latest/explainy.
+000008c0: 6578 706c 616e 6174 696f 6e73 2e68 746d  explanations.htm
+000008d0: 6c23 6d6f 6475 6c65 2d65 7870 6c61 696e  l#module-explain
+000008e0: 792e 6578 706c 616e 6174 696f 6e2e 7065  y.explanation.pe
+000008f0: 726d 7574 6174 696f 6e5f 6578 706c 616e  rmutation_explan
+00000900: 6174 696f 6e29 097c 206e 6f6e 2d63 6f6e  ation).| non-con
+00000910: 7472 6173 7469 7665 207c 2067 6c6f 6261  trastive | globa
+00000920: 6c20 7c20 203a 7374 6172 3a20 7c20 3a73  l |  :star: | :s
+00000930: 7461 723a 7c0a 7c5b 5368 6170 2056 616c  tar:|.|[Shap Val
+00000940: 7565 735d 2868 7474 7073 3a2f 2f65 7870  ues](https://exp
+00000950: 6c61 696e 792e 7265 6164 7468 6564 6f63  lainy.readthedoc
+00000960: 732e 696f 2f65 6e2f 6c61 7465 7374 2f65  s.io/en/latest/e
+00000970: 7870 6c61 696e 792e 6578 706c 616e 6174  xplainy.explanat
+00000980: 696f 6e73 2e68 746d 6c3f 6869 6768 6c69  ions.html?highli
+00000990: 6768 743d 7368 6170 236d 6f64 756c 652d  ght=shap#module-
+000009a0: 6578 706c 6169 6e79 2e65 7870 6c61 6e61  explainy.explana
+000009b0: 7469 6f6e 732e 7368 6170 5f65 7870 6c61  tions.shap_expla
+000009c0: 6e61 7469 6f6e 2909 097c 206e 6f6e 2d63  nation)..| non-c
+000009d0: 6f6e 7472 6173 7469 7665 207c 206c 6f63  ontrastive | loc
+000009e0: 616c 207c 2020 2009 3a73 7461 723a 207c  al |   .:star: |
+000009f0: 203a 7374 6172 3a7c 0a7c 5b53 7572 726f   :star:|.|[Surro
+00000a00: 6761 7465 204d 6f64 656c 5d28 6874 7470  gate Model](http
+00000a10: 733a 2f2f 6578 706c 6169 6e79 2e72 6561  s://explainy.rea
+00000a20: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000a30: 6174 6573 742f 6578 706c 6169 6e79 2e65  atest/explainy.e
+00000a40: 7870 6c61 6e61 7469 6f6e 732e 6874 6d6c  xplanations.html
+00000a50: 236d 6f64 756c 652d 6578 706c 6169 6e79  #module-explainy
+00000a60: 2e65 7870 6c61 6e61 7469 6f6e 2e73 7572  .explanation.sur
+00000a70: 726f 6761 7465 5f6d 6f64 656c 5f65 7870  rogate_model_exp
+00000a80: 6c61 6e61 7469 6f6e 297c 636f 6e74 7261  lanation)|contra
+00000a90: 7374 6976 6520 7c20 676c 6f62 616c 207c  stive | global |
+00000aa0: 203a 7374 6172 3a20 7c20 3a73 7461 723a   :star: | :star:
+00000ab0: 207c 200a 7c5b 436f 756e 7465 7266 6163   | .|[Counterfac
+00000ac0: 7475 616c 2045 7861 6d70 6c65 5d28 6874  tual Example](ht
+00000ad0: 7470 733a 2f2f 6578 706c 6169 6e79 2e72  tps://explainy.r
+00000ae0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000af0: 2f6c 6174 6573 742f 6578 706c 6169 6e79  /latest/explainy
+00000b00: 2e65 7870 6c61 6e61 7469 6f6e 732e 6874  .explanations.ht
+00000b10: 6d6c 236d 6f64 756c 652d 6578 706c 6169  ml#module-explai
+00000b20: 6e79 2e65 7870 6c61 6e61 7469 6f6e 2e63  ny.explanation.c
+00000b30: 6f75 6e74 6572 6661 6374 7561 6c5f 6578  ounterfactual_ex
+00000b40: 706c 616e 6174 696f 6e29 7c20 636f 6e74  planation)| cont
+00000b50: 7261 7374 6976 6520 7c20 6c6f 6361 6c20  rastive | local 
+00000b60: 7c3a 7374 6172 3a7c 203a 7374 6172 3a7c  |:star:| :star:|
+00000b70: 0a0a 0a44 6573 6372 6970 7469 6f6e 3a0a  ...Description:.
+00000b80: 2d20 2a2a 676c 6f62 616c 2a2a 3a20 6578  - **global**: ex
+00000b90: 706c 616e 6174 696f 6e20 6f66 2073 7973  planation of sys
+00000ba0: 7465 6d20 6675 6e63 7469 6f6e 616c 6974  tem functionalit
+00000bb0: 7920 2861 6c6c 2073 616d 706c 6573 2068  y (all samples h
+00000bc0: 6176 6520 7468 6520 7361 6d65 2065 7870  ave the same exp
+00000bd0: 6c61 6e61 7469 6f6e 290a 2d20 2a2a 6c6f  lanation).- **lo
+00000be0: 6361 6c2a 2a3a 2065 7870 6c61 6e61 7469  cal**: explanati
+00000bf0: 6f6e 206f 6620 6465 6369 7369 6f6e 2072  on of decision r
+00000c00: 6174 696f 6e61 6c65 2028 6561 6368 2073  ationale (each s
+00000c10: 616d 706c 6520 6861 7320 6974 7320 6f77  ample has its ow
+00000c20: 6e20 6578 706c 616e 6174 696f 6e29 0a2d  n explanation).-
+00000c30: 202a 2a63 6f6e 7472 6173 7469 7665 2a2a   **contrastive**
+00000c40: 3a20 7472 6163 696e 6720 6f66 2064 6563  : tracing of dec
+00000c50: 6973 696f 6e20 7061 7468 2028 6469 6666  ision path (diff
+00000c60: 6572 656e 6365 7320 746f 206f 7468 6572  erences to other
+00000c70: 206f 7574 636f 6d65 7320 6172 6520 6465   outcomes are de
+00000c80: 7363 7269 6265 6429 0a2d 202a 2a6e 6f6e  scribed).- **non
+00000c90: 2d63 6f6e 7472 6173 7469 7665 2a2a 3a20  -contrastive**: 
+00000ca0: 7061 7261 6d65 7465 7220 7765 6967 6874  parameter weight
+00000cb0: 696e 6720 2874 6865 2066 6561 7475 7265  ing (the feature
+00000cc0: 2069 6d70 6f72 7461 6e63 6520 6973 2072   importance is r
+00000cd0: 6570 6f72 7465 6429 0a0a 0a23 2320 446f  eported)...## Do
+00000ce0: 6375 6d65 6e74 6174 696f 6e0a 6874 7470  cumentation.http
+00000cf0: 733a 2f2f 6578 706c 6169 6e79 2e72 6561  s://explainy.rea
+00000d00: 6474 6865 646f 6373 2e69 6f0a 0a0a 2323  dthedocs.io...##
+00000d10: 2049 6e73 7461 6c6c 2065 7870 6c61 696e   Install explain
+00000d20: 790a 0a60 6060 0a70 6970 2069 6e73 7461  y..```.pip insta
+00000d30: 6c6c 2065 7870 6c61 696e 790a 6060 600a  ll explainy.```.
+00000d40: 0a23 2320 5573 6167 650a 0af0 9f93 9a20  .## Usage...... 
+00000d50: 4120 636f 6d70 7265 6865 6e73 6976 6520  A comprehensive 
+00000d60: 6578 616d 706c 6520 6f66 2074 6865 2060  example of the `
+00000d70: 6578 706c 6169 6e79 6020 4150 4920 6361  explainy` API ca
+00000d80: 6e20 6265 2066 6f75 6e64 2069 6e20 7468  n be found in th
+00000d90: 6973 2021 5b4a 7570 7974 6572 204e 6f74  is ![Jupyter Not
+00000da0: 6562 6f6f 6b5d 2868 7474 7073 3a2f 2f67  ebook](https://g
+00000db0: 6974 6875 622e 636f 6d2f 4d61 7572 6f4c  ithub.com/MauroL
+00000dc0: 757a 7a61 7474 6f2f 6578 706c 6169 6e79  uzzatto/explainy
+00000dd0: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
+00000de0: 6c65 732f 3031 2d65 7870 6c61 696e 792d  les/01-explainy-
+00000df0: 696e 7472 6f2e 6970 796e 6229 200a 200a  intro.ipynb) . .
+00000e00: f09f 9396 204f 7220 696e 2074 6865 205b  .... Or in the [
+00000e10: 6578 616d 706c 6520 7365 6374 696f 6e5d  example section]
+00000e20: 2868 7474 7073 3a2f 2f65 7870 6c61 696e  (https://explain
+00000e30: 792e 7265 6164 7468 6564 6f63 732e 696f  y.readthedocs.io
+00000e40: 2f65 6e2f 6c61 7465 7374 2f65 7861 6d70  /en/latest/examp
+00000e50: 6c65 732f 3031 2d65 7870 6c61 696e 792d  les/01-explainy-
+00000e60: 696e 7472 6f2e 6874 6d6c 2920 6f66 2074  intro.html) of t
+00000e70: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00000e80: 0a0a 0a49 6e69 7469 616c 697a 6520 616e  ...Initialize an
+00000e90: 6420 7472 6169 6e20 6120 6073 6369 6b69  d train a `sciki
+00000ea0: 742d 6c65 6172 6e60 206d 6f64 656c 3a0a  t-learn` model:.
+00000eb0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000ec0: 2070 616e 6461 7320 6173 2070 640a 6672   pandas as pd.fr
+00000ed0: 6f6d 2073 6b6c 6561 726e 2e64 6174 6173  om sklearn.datas
+00000ee0: 6574 7320 696d 706f 7274 206c 6f61 645f  ets import load_
+00000ef0: 6469 6162 6574 6573 0a66 726f 6d20 736b  diabetes.from sk
+00000f00: 6c65 6172 6e2e 656e 7365 6d62 6c65 2069  learn.ensemble i
+00000f10: 6d70 6f72 7420 5261 6e64 6f6d 466f 7265  mport RandomFore
+00000f20: 7374 5265 6772 6573 736f 720a 6672 6f6d  stRegressor.from
+00000f30: 2073 6b6c 6561 726e 2e6d 6f64 656c 5f73   sklearn.model_s
+00000f40: 656c 6563 7469 6f6e 2069 6d70 6f72 7420  election import 
+00000f50: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
+00000f60: 0a0a 6469 6162 6574 6573 203d 206c 6f61  ..diabetes = loa
+00000f70: 645f 6469 6162 6574 6573 2829 0a58 5f74  d_diabetes().X_t
+00000f80: 7261 696e 2c20 585f 7465 7374 2c20 795f  rain, X_test, y_
+00000f90: 7472 6169 6e2c 2079 5f74 6573 7420 3d20  train, y_test = 
+00000fa0: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
+00000fb0: 280a 2020 2020 6469 6162 6574 6573 2e64  (.    diabetes.d
+00000fc0: 6174 612c 2064 6961 6265 7465 732e 7461  ata, diabetes.ta
+00000fd0: 7267 6574 2c20 7261 6e64 6f6d 5f73 7461  rget, random_sta
+00000fe0: 7465 3d30 0a29 0a58 5f74 6573 7420 3d20  te=0.).X_test = 
+00000ff0: 7064 2e44 6174 6146 7261 6d65 2858 5f74  pd.DataFrame(X_t
+00001000: 6573 742c 2063 6f6c 756d 6e73 3d64 6961  est, columns=dia
+00001010: 6265 7465 732e 6665 6174 7572 655f 6e61  betes.feature_na
+00001020: 6d65 7329 0a79 5f74 6573 7420 3d20 7064  mes).y_test = pd
+00001030: 2e44 6174 6146 7261 6d65 2879 5f74 6573  .DataFrame(y_tes
+00001040: 7429 0a0a 6d6f 6465 6c20 3d20 5261 6e64  t)..model = Rand
+00001050: 6f6d 466f 7265 7374 5265 6772 6573 736f  omForestRegresso
+00001060: 7228 7261 6e64 6f6d 5f73 7461 7465 3d30  r(random_state=0
+00001070: 290a 6d6f 6465 6c2e 6669 7428 585f 7472  ).model.fit(X_tr
+00001080: 6169 6e2c 2079 5f74 7261 696e 290a 6060  ain, y_train).``
+00001090: 600a 0a49 6e69 7469 616c 697a 6520 7468  `..Initialize th
+000010a0: 6520 6050 6572 6d75 7461 7469 6f6e 4578  e `PermutationEx
+000010b0: 706c 616e 6174 696f 6e60 2028 6f72 2061  planation` (or a
+000010c0: 6e79 206f 7468 6572 2065 7870 6c61 6e61  ny other explana
+000010d0: 7469 6f6e 2920 6f62 6a65 6374 2061 6e64  tion) object and
+000010e0: 2070 6173 7320 696e 2074 6865 2074 7261   pass in the tra
+000010f0: 696e 6564 206d 6f64 656c 2061 6e64 2074  ined model and t
+00001100: 6865 2074 6f20 6265 2065 7870 6c61 696e  he to be explain
+00001110: 6564 2064 6174 6173 6574 2e20 0a0a 4164  ed dataset. ..Ad
+00001120: 6474 696f 6e61 6c6c 792c 2064 6566 696e  dtionally, defin
+00001130: 6520 7468 6520 6e75 6d62 6572 206f 6620  e the number of 
+00001140: 6665 6174 7572 6573 2075 7365 6420 696e  features used in
+00001150: 2074 6865 2065 7870 6c61 6e61 7469 6f6e   the explanation
+00001160: 2e20 5468 6973 2061 6c6c 6f77 7320 796f  . This allows yo
+00001170: 7520 746f 2063 6f6e 6669 6775 7265 2074  u to configure t
+00001180: 6865 2076 6572 626f 7369 7479 206f 6620  he verbosity of 
+00001190: 796f 7572 2065 7861 706c 616e 6174 696f  your exaplanatio
+000011a0: 6e2e 0a0a 2053 6574 2074 6865 2069 6e64  n... Set the ind
+000011b0: 6578 206f 6620 7468 6520 7361 6d70 6c65  ex of the sample
+000011c0: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+000011d0: 6578 706c 6169 6e65 642e 0a0a 6060 6070  explained...```p
+000011e0: 7974 686f 6e0a 6672 6f6d 2065 7870 6c61  ython.from expla
+000011f0: 696e 792e 6578 706c 616e 6174 696f 6e73  iny.explanations
+00001200: 2069 6d70 6f72 7420 5065 726d 7574 6174   import Permutat
+00001210: 696f 6e45 7870 6c61 6e61 7469 6f6e 0a0a  ionExplanation..
+00001220: 6e75 6d62 6572 5f6f 665f 6665 6174 7572  number_of_featur
+00001230: 6573 203d 2034 0a0a 6578 706c 6169 6e65  es = 4..explaine
+00001240: 7220 3d20 5065 726d 7574 6174 696f 6e45  r = PermutationE
+00001250: 7870 6c61 6e61 7469 6f6e 280a 2020 2020  xplanation(.    
+00001260: 585f 7465 7374 2c20 795f 7465 7374 2c20  X_test, y_test, 
+00001270: 6d6f 6465 6c2c 206e 756d 6265 725f 6f66  model, number_of
+00001280: 5f66 6561 7475 7265 730a 290a 6060 600a  _features.).```.
+00001290: 4361 6c6c 2074 6865 2060 6578 706c 6169  Call the `explai
+000012a0: 6e28 2960 206d 6574 686f 6420 616e 6420  n()` method and 
+000012b0: 7072 696e 7420 7468 6520 6578 706c 616e  print the explan
+000012c0: 6174 696f 6e20 666f 7220 7468 6520 7361  ation for the sa
+000012d0: 6d70 6c65 2028 696e 2063 6173 6520 6f66  mple (in case of
+000012e0: 2061 206c 6f63 616c 2065 7870 6c61 6e61   a local explana
+000012f0: 7469 6f6e 2065 7665 7279 2073 616d 706c  tion every sampl
+00001300: 6520 6861 7320 6120 6469 6666 6572 656e  e has a differen
+00001310: 7420 6578 706c 616e 6174 696f 6e29 2e0a  t explanation)..
+00001320: 0a60 6060 7079 7468 6f6e 0a65 7870 6c61  .```python.expla
+00001330: 6e61 7469 6f6e 203d 2065 7870 6c61 696e  nation = explain
+00001340: 6572 2e65 7870 6c61 696e 2873 616d 706c  er.explain(sampl
+00001350: 655f 696e 6465 783d 3129 0a70 7269 6e74  e_index=1).print
+00001360: 2865 7870 6c61 6e61 7469 6f6e 290a 6060  (explanation).``
+00001370: 600a 3e20 5468 6520 5261 6e64 6f6d 466f  `.> The RandomFo
+00001380: 7265 7374 5265 6772 6573 736f 7220 7573  restRegressor us
+00001390: 6564 2031 3020 6665 6174 7572 6573 2074  ed 10 features t
+000013a0: 6f20 7072 6f64 7563 6520 7468 6520 7072  o produce the pr
+000013b0: 6564 6963 7469 6f6e 732e 2054 6865 2070  edictions. The p
+000013c0: 7265 6469 6374 696f 6e20 6f66 2074 6869  rediction of thi
+000013d0: 7320 7361 6d70 6c65 2077 6173 2032 3531  s sample was 251
+000013e0: 2e38 2e0a 0a3e 2054 6865 2066 6561 7475  .8...> The featu
+000013f0: 7265 2069 6d70 6f72 7461 6e63 6520 7761  re importance wa
+00001400: 7320 6361 6c63 756c 6174 6564 2075 7369  s calculated usi
+00001410: 6e67 2074 6865 2050 6572 6d75 7461 7469  ng the Permutati
+00001420: 6f6e 2046 6561 7475 7265 2049 6d70 6f72  on Feature Impor
+00001430: 7461 6e63 6520 6d65 7468 6f64 2e0a 0a3e  tance method...>
+00001440: 2054 6865 2066 6f75 7220 6665 6174 7572   The four featur
+00001450: 6573 2077 6869 6368 2077 6572 6520 6d6f  es which were mo
+00001460: 7374 2069 6d70 6f72 7461 6e74 2066 6f72  st important for
+00001470: 2074 6865 2070 7265 6469 6374 696f 6e73   the predictions
+00001480: 2077 6572 6520 2866 726f 6d20 6869 6768   were (from high
+00001490: 6573 7420 746f 206c 6f77 6573 7429 3a20  est to lowest): 
+000014a0: 2762 6d69 2720 2830 2e31 3529 2c20 2773  'bmi' (0.15), 's
+000014b0: 3527 2028 302e 3132 292c 2027 6270 2720  5' (0.12), 'bp' 
+000014c0: 2830 2e30 3329 2c20 616e 6420 2761 6765  (0.03), and 'age
+000014d0: 2720 2830 2e30 3229 2e0a 0a55 7365 2074  ' (0.02)...Use t
+000014e0: 6865 2060 706c 6f74 2829 6020 6d65 7468  he `plot()` meth
+000014f0: 6f64 2074 6f20 6372 6561 7465 2061 2066  od to create a f
+00001500: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
+00001510: 6520 706c 6f74 206f 6620 7468 6174 2073  e plot of that s
+00001520: 616d 706c 652e 0a0a 6060 6070 7974 686f  ample...```pytho
+00001530: 6e0a 6578 706c 6169 6e65 722e 706c 6f74  n.explainer.plot
+00001540: 2829 0a60 6060 0a21 5b50 6572 6d75 7461  ().```.![Permuta
+00001550: 7469 6f6e 2046 6561 7475 7265 2049 6d70  tion Feature Imp
+00001560: 6f72 7461 6e63 655d 2868 7474 7073 3a2f  ortance](https:/
+00001570: 2f67 6974 6875 622e 636f 6d2f 4d61 7572  /github.com/Maur
+00001580: 6f4c 757a 7a61 7474 6f2f 6578 706c 6169  oLuzzatto/explai
+00001590: 6e79 2f72 6177 2f6d 6169 6e2f 7374 6174  ny/raw/main/stat
+000015a0: 6963 2f70 6572 6d75 7461 7469 6f6e 5f69  ic/permutation_i
+000015b0: 6d70 6f72 7461 6e63 652e 706e 6729 0a0a  mportance.png)..
+000015c0: 4966 2079 6f75 7220 7072 6566 6572 2c20  If your prefer, 
+000015d0: 796f 7520 6361 6e20 616c 736f 2063 7265  you can also cre
+000015e0: 6174 6520 616e 6f74 6865 7220 7479 7065  ate another type
+000015f0: 206f 6620 706c 6f74 2c20 6173 2066 6f72   of plot, as for
+00001600: 2065 7861 6d70 6c65 2061 2062 6f78 706c   example a boxpl
+00001610: 6f74 2e0a 6060 6070 7974 686f 6e0a 6578  ot..```python.ex
+00001620: 706c 6169 6e65 722e 706c 6f74 286b 696e  plainer.plot(kin
+00001630: 643d 2762 6f78 2729 0a60 6060 0a21 5b50  d='box').```.![P
+00001640: 6572 6d75 7461 7469 6f6e 2046 6561 7475  ermutation Featu
+00001650: 7265 2049 6d70 6f72 7461 6e63 6520 426f  re Importance Bo
+00001660: 7850 6c6f 745d 2868 7474 7073 3a2f 2f67  xPlot](https://g
+00001670: 6974 6875 622e 636f 6d2f 4d61 7572 6f4c  ithub.com/MauroL
+00001680: 757a 7a61 7474 6f2f 6578 706c 6169 6e79  uzzatto/explainy
+00001690: 2f72 6177 2f6d 6169 6e2f 7374 6174 6963  /raw/main/static
+000016a0: 2f70 6572 6d75 7461 7469 6f6e 5f69 6d70  /permutation_imp
+000016b0: 6f72 7461 6e63 655f 626f 782e 706e 6729  ortance_box.png)
+000016c0: 0a0a 0a46 696e 616c 6c79 2c20 796f 7520  ...Finally, you 
+000016d0: 6361 6e20 616c 736f 206c 6f6f 6b20 6174  can also look at
+000016e0: 2074 6865 2069 6d70 6f72 7461 6e63 6520   the importance 
+000016f0: 7661 6c75 6573 206f 6620 7468 6520 6665  values of the fe
+00001700: 6174 7572 6573 2028 696e 2066 6f72 6d20  atures (in form 
+00001710: 6f66 2061 2060 7064 2e44 6174 6146 7261  of a `pd.DataFra
+00001720: 6d65 6029 2e0a 0a60 6060 7079 7468 6f6e  me`)...```python
+00001730: 0a66 6561 7475 7265 5f69 6d70 6f72 7461  .feature_importa
+00001740: 6e63 6520 3d20 6578 706c 6169 6e65 722e  nce = explainer.
+00001750: 696d 706f 7274 616e 6365 2829 0a70 7269  importance().pri
+00001760: 6e74 2866 6561 7475 7265 5f69 6d70 6f72  nt(feature_impor
+00001770: 7461 6e63 6529 0a60 6060 0a0a 6060 6070  tance).```..```p
+00001780: 7974 686f 6e0a 2020 4665 6174 7572 6520  ython.  Feature 
+00001790: 2049 6d70 6f72 7461 6e63 650a 3020 2020   Importance.0   
+000017a0: 2020 626d 6920 2020 2020 2020 2030 2e31    bmi        0.1
+000017b0: 350a 3120 2020 2020 2073 3520 2020 2020  5.1      s5     
+000017c0: 2020 2030 2e31 320a 3220 2020 2020 2062     0.12.2      b
+000017d0: 7020 2020 2020 2020 2030 2e30 330a 3320  p        0.03.3 
+000017e0: 2020 2020 6167 6520 2020 2020 2020 2030      age        0
+000017f0: 2e30 320a 3420 2020 2020 2073 3220 2020  .02.4      s2   
+00001800: 2020 2020 2d30 2e30 300a 3520 2020 2020      -0.00.5     
+00001810: 7365 7820 2020 2020 2020 2d30 2e30 300a  sex       -0.00.
+00001820: 3620 2020 2020 2073 3320 2020 2020 2020  6      s3       
+00001830: 2d30 2e30 300a 3720 2020 2020 2073 3120  -0.00.7      s1 
+00001840: 2020 2020 2020 2d30 2e30 310a 3820 2020        -0.01.8   
+00001850: 2020 2073 3620 2020 2020 2020 2d30 2e30     s6       -0.0
+00001860: 310a 3920 2020 2020 2073 3420 2020 2020  1.9      s4     
+00001870: 2020 2d30 2e30 310a 6060 600a 0a3c 212d    -0.01.```..<!-
+00001880: 2d20 4669 6e61 6c6c 7920 7468 6520 7265  - Finally the re
+00001890: 7375 6c74 2063 616e 2062 6520 7361 7665  sult can be save
+000018a0: 640a 0a60 6060 7079 7468 6f6e 0a65 7870  d..```python.exp
+000018b0: 6c61 696e 6572 2e73 6176 6528 7361 6d70  lainer.save(samp
+000018c0: 6c65 5f69 6e64 6578 290a 6060 6020 2d2d  le_index).``` --
+000018d0: 3e0a 0a3c 212d 2d20 0a23 2320 4d6f 6465  >..<!-- .## Mode
+000018e0: 6c20 4578 706c 616e 6174 696f 6e73 0a2d  l Explanations.-
+000018f0: 2d3e 0a0a 0a23 2320 4665 6174 7572 6573  ->...## Features
+00001900: 0a2d 2041 6c67 6f72 6974 686d 7320 666f  .- Algorithms fo
+00001910: 7220 696e 7370 6563 7469 6e67 2062 6c61  r inspecting bla
+00001920: 636b 2d62 6f78 206d 6163 6869 6e65 206c  ck-box machine l
+00001930: 6561 726e 696e 6720 6d6f 6465 6c73 200a  earning models .
+00001940: 2d20 5375 7070 6f72 7420 666f 7220 7468  - Support for th
+00001950: 6520 6d61 6368 696e 6520 6c65 6172 6e69  e machine learni
+00001960: 6e67 2066 7261 6d65 776f 726b 7320 6073  ng frameworks `s
+00001970: 6369 6b69 742d 6c65 6172 6e60 2061 6e64  cikit-learn` and
+00001980: 2060 7867 626f 6f73 7460 0a2d 202a 2a65   `xgboost`.- **e
+00001990: 7870 6c61 696e 792a 2a20 6f66 6665 7273  xplainy** offers
+000019a0: 2061 2073 7461 6e64 6172 6469 7a65 6420   a standardized 
+000019b0: 4150 4920 7769 7468 2074 6872 6565 2063  API with three c
+000019c0: 6f72 6520 6d65 7468 6f64 7320 6065 7870  ore methods `exp
+000019d0: 6c61 696e 2829 602c 2060 706c 6f74 2829  lain()`, `plot()
+000019e0: 602c 2060 696d 706f 7274 616e 6365 2829  `, `importance()
+000019f0: 600a 0a23 2320 4f74 6865 7220 4d61 6368  `..## Other Mach
+00001a00: 696e 6520 4c65 6172 6e69 6e67 2045 7870  ine Learning Exp
+00001a10: 6c61 696e 6162 696c 6974 7920 6c69 6272  lainability libr
+00001a20: 6172 6965 7320 746f 2077 6174 6368 0a2d  aries to watch.-
+00001a30: 205b 7368 6170 5d28 6874 7470 733a 2f2f   [shap](https://
+00001a40: 6769 7468 7562 2e63 6f6d 2f73 6c75 6e64  github.com/slund
+00001a50: 6265 7267 2f73 6861 7029 3a20 4120 6761  berg/shap): A ga
+00001a60: 6d65 2074 6865 6f72 6574 6963 2061 7070  me theoretic app
+00001a70: 726f 6163 6820 746f 2065 7870 6c61 696e  roach to explain
+00001a80: 2074 6865 206f 7574 7075 7420 6f66 2061   the output of a
+00001a90: 6e79 206d 6163 6869 6e65 206c 6561 726e  ny machine learn
+00001aa0: 696e 6720 6d6f 6465 6c0a 2d20 5b65 6c69  ing model.- [eli
+00001ab0: 355d 2868 7474 7073 3a2f 2f67 6974 6875  5](https://githu
+00001ac0: 622e 636f 6d2f 5465 616d 4847 2d4d 656d  b.com/TeamHG-Mem
+00001ad0: 6578 2f65 6c69 3529 3a20 4120 6c69 6272  ex/eli5): A libr
+00001ae0: 6172 7920 666f 7220 6465 6275 6767 696e  ary for debuggin
+00001af0: 672f 696e 7370 6563 7469 6e67 206d 6163  g/inspecting mac
+00001b00: 6869 6e65 206c 6561 726e 696e 6720 636c  hine learning cl
+00001b10: 6173 7369 6669 6572 7320 616e 6420 6578  assifiers and ex
+00001b20: 706c 6169 6e69 6e67 2074 6865 6972 2070  plaining their p
+00001b30: 7265 6469 6374 696f 6e73 200a 2d20 5b61  redictions .- [a
+00001b40: 6c69 6269 5d28 6874 7470 733a 2f2f 6769  libi](https://gi
+00001b50: 7468 7562 2e63 6f6d 2f53 656c 646f 6e49  thub.com/SeldonI
+00001b60: 4f2f 616c 6962 6929 3a20 416c 676f 7269  O/alibi): Algori
+00001b70: 7468 6d73 2066 6f72 2065 7870 6c61 696e  thms for explain
+00001b80: 696e 6720 6d61 6368 696e 6520 6c65 6172  ing machine lear
+00001b90: 6e69 6e67 206d 6f64 656c 7320 0a2d 205b  ning models .- [
+00001ba0: 696e 7465 7270 7265 745d 2868 7474 7073  interpret](https
+00001bb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 696e  ://github.com/in
+00001bc0: 7465 7270 7265 746d 6c2f 696e 7465 7270  terpretml/interp
+00001bd0: 7265 7429 3a20 4669 7420 696e 7465 7270  ret): Fit interp
+00001be0: 7265 7461 626c 6520 6d6f 6465 6c73 2e20  retable models. 
+00001bf0: 4578 706c 6169 6e20 626c 6163 6b62 6f78  Explain blackbox
+00001c00: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00001c10: 670a 0a0a 2323 2053 6f75 7263 650a 0a4d  g...## Source..M
+00001c20: 6f6c 6e61 722c 2043 6872 6973 746f 7068  olnar, Christoph
+00001c30: 2e20 2249 6e74 6572 7072 6574 6162 6c65  . "Interpretable
+00001c40: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00001c50: 672e 2041 2047 7569 6465 2066 6f72 204d  g. A Guide for M
+00001c60: 616b 696e 6720 426c 6163 6b20 426f 7820  aking Black Box 
+00001c70: 4d6f 6465 6c73 2045 7870 6c61 696e 6162  Models Explainab
+00001c80: 6c65 222c 2032 3031 392e 2068 7474 7073  le", 2019. https
+00001c90: 3a2f 2f63 6872 6973 746f 7068 6d2e 6769  ://christophm.gi
+00001ca0: 7468 7562 2e69 6f2f 696e 7465 7270 7265  thub.io/interpre
+00001cb0: 7461 626c 652d 6d6c 2d62 6f6f 6b2f 0a0a  table-ml-book/..
+00001cc0: 2323 2041 7574 686f 720a 2a2a 4d61 7572  ## Author.**Maur
+00001cd0: 6f20 4c75 7a7a 6174 746f 2a2a 202d 205b  o Luzzatto** - [
+00001ce0: 4d61 7572 6f6c 5d28 6874 7470 733a 2f2f  Maurol](https://
+00001cf0: 6769 7468 7562 2e63 6f6d 2f4d 6175 726f  github.com/Mauro
+00001d00: 4c75 7a7a 6174 746f 290a 0a              Luzzatto)..
```

### Comparing `explainy-0.1.8/docs/Makefile` & `explainy-0.2.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = explainy
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python -msphinx
+SPHINXPROJ    = explainy
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `explainy-0.1.8/docs/_build/html/_static/counterfactual.png` & `explainy-0.2.0/docs/_static/counterfactual.png`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/_build/html/_static/logo.jpg` & `explainy-0.2.0/docs/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/_build/html/_static/logo.png` & `explainy-0.2.0/docs/_static/logo_original.png`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/_build/html/_static/permutation.png` & `explainy-0.2.0/docs/_static/permutation.png`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/_build/html/_static/shapley.png` & `explainy-0.2.0/docs/_static/shapley.png`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/_build/html/_static/surrogate.png` & `explainy-0.2.0/docs/_static/surrogate.png`

 * *Files identical despite different names*

### Comparing `explainy-0.1.8/docs/conf.py` & `explainy-0.2.0/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-#!/usr/bin/env python
-#
-# explainy documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import explainy
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'sphinx.ext.napoleon', 'm2r2', 'sphinx_markdown_tables',
-'sphinxemoji.sphinxemoji', 'nbsphinx']
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-
-
-source_parsers = {
-    '.md': 'recommonmark.parser.CommonMarkParser',
-}
-
-source_suffix = ['.rst', '.md']
-# source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'explainy'
-copyright = "2021, Mauro Luzzatto"
-author = "Mauro Luzzatto"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = explainy.__version__
-# The full version, including alpha/beta/rc tags.
-release = explainy.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-# html_theme = 'alabaster'
-html_theme = 'pydata_sphinx_theme'
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_logo = "_static/logo.png"
-html_theme_options = {
-  "github_url": "https://github.com/MauroLuzzatto/explainy",
-  "search_bar_position": "navbar",
-}
-
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'explainydoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'explainy.tex',
-     'explainy Documentation',
-     'Mauro Luzzatto', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'explainy',
-     'explainy Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'explainy',
-     'explainy Documentation',
-     author,
-     'explainy',
-     'One line description of project.',
-     'Miscellaneous'),
-]
-
-
-
+#!/usr/bin/env python
+#
+# explainy documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath(".."))
+
+import explainy
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "m2r2",
+    "sphinx_markdown_tables",
+    "sphinxemoji.sphinxemoji",
+    "nbsphinx",
+    "nbsphinx_link",
+]
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+
+
+source_parsers = {
+    ".md": "recommonmark.parser.CommonMarkParser",
+}
+
+source_suffix = [".rst", ".md"]
+# source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "explainy"
+copyright = "2021, Mauro Luzzatto"
+author = "Mauro Luzzatto"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = explainy.__version__
+# The full version, including alpha/beta/rc tags.
+release = explainy.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+# html_theme = 'alabaster'
+html_theme = "pydata_sphinx_theme"
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_logo = "_static/logo.png"
+html_theme_options = {
+    "github_url": "https://github.com/MauroLuzzatto/explainy",
+    "search_bar_position": "navbar",
+}
+
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "explainydoc"
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, "explainy.tex", "explainy Documentation", "Mauro Luzzatto", "manual"),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [(master_doc, "explainy", "explainy Documentation", [author], 1)]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (
+        master_doc,
+        "explainy",
+        "explainy Documentation",
+        author,
+        "explainy",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
+]
```

### Comparing `explainy-0.1.8/docs/installation.rst` & `explainy-0.2.0/docs/installation.rst`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install explainy, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install explainy
-
-This is the preferred method to install explainy, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for explainy can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/MauroLuzzatto/explainy
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/MauroLuzzatto/explainy/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/MauroLuzzatto/explainy
-.. _tarball: https://github.com/MauroLuzzatto/explainy/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install explainy, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install explainy
+
+This is the preferred method to install explainy, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for explainy can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/MauroLuzzatto/explainy
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/MauroLuzzatto/explainy/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/MauroLuzzatto/explainy
+.. _tarball: https://github.com/MauroLuzzatto/explainy/tarball/master
```

### Comparing `explainy-0.1.8/explainy/explanation/explanation_mixin.py` & `explainy-0.2.0/explainy/core/explanation_mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,82 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu May 13 21:49:43 2021
-
-@author: maurol
-"""
-import os
-
-from explainy.explanation.category_mapper import CategoryMapper
-
-
-class ExplanationMixin:
-    def map_category(self, feature_name, feature_value):
-        """
-
-
-        Args:
-            feature_name (TYPE): DESCRIPTION.
-            feature_value (TYPE): DESCRIPTION.
-
-        Returns:
-            feature_value (TYPE): DESCRIPTION.
-
-        """
-        # TODO: fix path
-        path_json = r"C:\Users\maurol\OneDrive\Dokumente\Python_Scripts\model_explanation_study\dataset\training\mapping"
-        if f"{feature_name}.json" in os.listdir(path_json):
-            mapper = CategoryMapper(path_json, feature_name)
-            # print(mapper[int(feature_value)])
-            feature_value = mapper[int(feature_value)]
-        return feature_value
-
-    @staticmethod
-    def join_text_with_comma_and_and(values: list) -> str:
-        """
-        Merge values for text output with commas and only the last value
-        with an "and""
-
-        Args:
-            values (list): list of values to be merged.
-
-        Returns:
-            str: new text.
-
-        """
-
-        if len(values) > 2:
-            last_value = values[-1]
-            values = ", ".join(values[:-1])
-            text = values + ", and " + last_value
-
-        else:
-            text = ", and ".join(values)
-        return text
-
-    def get_number_to_string_dict(self) -> None:
-        """
-        map number of features to string values
-        """
-
-        number_text = (
-            "one",
-            "two",
-            "three",
-            "four",
-            "five",
-            "six",
-            "seven",
-            "eight",
-            "nine",
-            "ten",
-            "eleven",
-            "twelve",
-            "thirteen",
-            "fourteen",
-            "fifteen",
-            "sixteen",
-            "seventeen",
-            "eighteen",
-            "nineteen",
-            "twenty",
-        )
-        self.num_to_str = {}
-        for text, number in zip(number_text, range(1, 21)):
-            self.num_to_str[number] = text
+import os
+
+from explainy.utils.category_mapper import CategoryMapper
+
+
+class ExplanationMixin:
+    def map_category(self, feature_name, feature_value):
+        """
+
+
+        Args:
+            feature_name (TYPE): DESCRIPTION.
+            feature_value (TYPE): DESCRIPTION.
+
+        Returns:
+            feature_value (TYPE): DESCRIPTION.
+        """
+        # TODO: fix path
+        path_json = r""
+
+        if not os.path.exists(path_json):
+            return feature_value
+
+        if f"{feature_name}.json" in os.listdir(path_json):
+            mapper = CategoryMapper(path_json, feature_name)
+            # print(mapper[int(feature_value)])
+            feature_value = mapper[int(feature_value)]
+        return feature_value
+
+    @staticmethod
+    def join_text_with_comma_and_and(values: list) -> str:
+        """
+        Merge values for text output with commas and only the last value
+        with an "and""
+
+        Args:
+            values (list): list of values to be merged.
+
+        Returns:
+            str: new text.
+
+        """
+
+        if len(values) > 2:
+            last_value = values[-1]
+            values = ", ".join(values[:-1])
+            text = values + ", and " + last_value
+
+        else:
+            text = ", and ".join(values)
+        return text
+
+    def get_number_to_string_dict(self) -> None:
+        """
+        map number of features to string values
+        """
+
+        number_text = (
+            "one",
+            "two",
+            "three",
+            "four",
+            "five",
+            "six",
+            "seven",
+            "eight",
+            "nine",
+            "ten",
+            "eleven",
+            "twelve",
+            "thirteen",
+            "fourteen",
+            "fifteen",
+            "sixteen",
+            "seventeen",
+            "eighteen",
+            "nineteen",
+            "twenty",
+        )
+        self.num_to_str = {}
+        for text, number in zip(number_text, range(1, 21)):
+            self.num_to_str[number] = text
```

### Comparing `explainy-0.1.8/explainy/logger.py` & `explainy-0.2.0/explainy/logger.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Jul 19 20:13:34 2020
-
-@author: mauro
-"""
-import logging
-import os
-
-
-class Logger(object):
-    def __init__(self, name, path_log):
-        self.name = name
-        self.path_log = path_log
-
-    def get_logger(self):
-        """
-        Create a log file to record the experiment's logs
-
-        Args:
-
-        Retunr:
-            logger (obj): logger that record logs
-        """
-        # check if the file exist
-        log_file = os.path.join(self.path_log, "{}.log".format(self.name))
-
-        file_logging_format = "%(asctime)s: %(levelname)s: %(message)s"
-        # configure logger
-        logging.basicConfig(level=logging.INFO)
-        logger = logging.getLogger()
-
-        # Reset the logger.handlers if it already exists.
-        if logger.handlers:
-            logger.handlers = []
-
-        # create a file handler for output file
-        handler = logging.FileHandler(filename=log_file, mode="w")
-        formatter = logging.Formatter(file_logging_format)
-        handler.setFormatter(formatter)
-        logger.setLevel(logging.DEBUG)
-        logger.addHandler(handler)
-
-        # set logging format
-        console_logging_format = "%(asctime)s: %(levelname)s: %(message)s"
-        # console log
-        consoleHandler = logging.StreamHandler()
-        # set the logging level for log file
-        consoleHandler.setLevel(level=logging.INFO)
-        # set the logging format
-        formatter = logging.Formatter(console_logging_format)
-        consoleHandler.setFormatter(formatter)
-        # add the handlers to the logger
-        logger.addHandler(consoleHandler)
-        return logger
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Jul 19 20:13:34 2020
+
+@author: mauro
+"""
+import logging
+import os
+
+
+class Logger(object):
+    def __init__(self, name, path_log):
+        self.name = name
+        self.path_log = path_log
+
+    def get_logger(self):
+        """
+        Create a log file to record the experiment's logs
+
+        Args:
+
+        Retunr:
+            logger (obj): logger that record logs
+        """
+        # check if the file exist
+        log_file = os.path.join(self.path_log, "{}.log".format(self.name))
+
+        file_logging_format = "%(asctime)s: %(levelname)s: %(message)s"
+        # configure logger
+        logging.basicConfig(level=logging.INFO)
+        logger = logging.getLogger()
+
+        # Reset the logger.handlers if it already exists.
+        if logger.handlers:
+            logger.handlers = []
+
+        # create a file handler for output file
+        handler = logging.FileHandler(filename=log_file, mode="w")
+        formatter = logging.Formatter(file_logging_format)
+        handler.setFormatter(formatter)
+        logger.setLevel(logging.DEBUG)
+        logger.addHandler(handler)
+
+        # set logging format
+        console_logging_format = "%(asctime)s: %(levelname)s: %(message)s"
+        # console log
+        consoleHandler = logging.StreamHandler()
+        # set the logging level for log file
+        consoleHandler.setLevel(level=logging.INFO)
+        # set the logging format
+        formatter = logging.Formatter(console_logging_format)
+        consoleHandler.setFormatter(formatter)
+        # add the handlers to the logger
+        logger.addHandler(consoleHandler)
+        return logger
```

