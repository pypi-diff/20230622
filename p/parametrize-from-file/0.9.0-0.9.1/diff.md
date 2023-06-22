# Comparing `tmp/parametrize_from_file-0.9.0.tar.gz` & `tmp/parametrize_from_file-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parametrize_from_file-0.9.0.tar", last modified: Thu Dec 23 18:33:23 2021, max compression
+gzip compressed data, was "parametrize_from_file-0.9.1.tar", last modified: Thu Dec 23 20:26:25 2021, max compression
```

## Comparing `parametrize_from_file-0.9.0.tar` & `parametrize_from_file-0.9.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1459 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/.github/workflows/test_and_release.yml
--rw-r--r--   0        0        0      739 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/.gitignore
--rw-r--r--   0        0        0      392 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/.readthedocs.yml
--rw-r--r--   0        0        0     4683 2021-12-23 18:33:18.750489 parametrize_from_file-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1079 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     2602 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/README.rst
--rw-r--r--   0        0        0        4 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/.gitignore
--rw-r--r--   0        0        0     6828 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      237 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      435 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/api_reference.rst
--rw-r--r--   0        0        0     2389 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/conf.py
--rw-r--r--   0        0        0      522 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/examples.rst
--rw-r--r--   0        0        0     3109 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/exceptions.rst
--rw-r--r--   0        0        0      181 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/exceptions/test_vector.nt
--rw-r--r--   0        0        0      555 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/exceptions/test_vector.py
--rw-r--r--   0        0        0      327 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/exceptions/vector.py
--rw-r--r--   0        0        0     3071 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/getting_started.rst
--rw-r--r--   0        0        0      216 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/getting_started/test_vector.py
--rw-r--r--   0        0        0      203 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/getting_started/test_vector.yml
--rw-r--r--   0        0        0      132 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/getting_started/vector.py
--rw-r--r--   0        0        0      137 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/index.rst
--rw-r--r--   0        0        0     3074 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params.rst
--rw-r--r--   0        0        0     3568 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params.rst.bkup
--rw-r--r--   0        0        0      329 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params/test_vector_kwargs.nt
--rw-r--r--   0        0        0      649 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params/test_vector_kwargs.py
--rw-r--r--   0        0        0      291 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params/test_vector_schema.nt
--rw-r--r--   0        0        0      734 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params/test_vector_schema.py
--rw-r--r--   0        0        0      305 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/optional_params/vector.py
--rw-r--r--   0        0        0     7644 2021-12-23 18:33:17.934483 parametrize_from_file-0.9.0/docs/python_snippets.rst
--rw-r--r--   0        0        0      250 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/eval/test_vector.nt
--rw-r--r--   0        0        0      379 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/eval/test_vector.py
-lrwxr-xr-x   0        0        0        0 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/eval/vector.py -> ../../getting_started/vector.py
--rw-r--r--   0        0        0      285 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/exec/test_vector.nt
--rw-r--r--   0        0        0      344 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/exec/test_vector.py
--rw-r--r--   0        0        0      486 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/exec/vector.py
-lrwxr-xr-x   0        0        0        0 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/schema/test_vector.nt -> ../eval/test_vector.nt
--rw-r--r--   0        0        0      566 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/schema/test_vector.py
-lrwxr-xr-x   0        0        0        0 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/python_snippets/schema/vector.py -> ../eval/vector.py
--rw-r--r--   0        0        0      127 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/readme/test_misc.py
--rw-r--r--   0        0        0       70 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/readme/test_misc.yml
--rw-r--r--   0        0        0      289 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/requirements.txt
--rwxr-xr-x   0        0        0      470 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/test_docs.sh
--rw-r--r--   0        0        0      220 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/docs/tutorials.rst
--rw-r--r--   0        0        0     1650 2021-12-23 18:33:18.754489 parametrize_from_file-0.9.0/parametrize_from_file/__init__.py
--rw-r--r--   0        0        0      162 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/errors.py
--rw-r--r--   0        0        0     1547 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/loaders.py
--rw-r--r--   0        0        0    18550 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/namespace.py
--rw-r--r--   0        0        0    20784 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/parameters.py
--rw-r--r--   0        0        0     1033 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/utils.py
--rw-r--r--   0        0        0     7981 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/parametrize_from_file/voluptuous.py
--rw-r--r--   0        0        0     1644 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       76 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/.coveragerc
--rw-r--r--   0        0        0       37 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/mock_module.py
--rw-r--r--   0        0        0       53 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/mock_module_all.py
--rw-r--r--   0        0        0       30 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/mock_module_overwrite.py
--rw-r--r--   0        0        0    16922 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/test_namespace.py
--rw-r--r--   0        0        0    20911 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/test_parameters.py
--rw-r--r--   0        0        0     2955 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0     1770 2021-12-23 18:33:17.938483 parametrize_from_file-0.9.0/tests/test_voluptuous.py
--rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 parametrize_from_file-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1459 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/.github/workflows/test_and_release.yml
+-rw-r--r--   0        0        0      739 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/.gitignore
+-rw-r--r--   0        0        0      392 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     4855 2021-12-23 20:26:20.762877 parametrize_from_file-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1079 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/README.rst
+-rw-r--r--   0        0        0        4 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/.gitignore
+-rw-r--r--   0        0        0     6828 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      237 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      435 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/api_reference.rst
+-rw-r--r--   0        0        0     2389 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      522 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/examples.rst
+-rw-r--r--   0        0        0     3109 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/exceptions.rst
+-rw-r--r--   0        0        0      181 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/exceptions/test_vector.nt
+-rw-r--r--   0        0        0      555 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/exceptions/test_vector.py
+-rw-r--r--   0        0        0      327 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/exceptions/vector.py
+-rw-r--r--   0        0        0     3071 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/getting_started.rst
+-rw-r--r--   0        0        0      216 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/getting_started/test_vector.py
+-rw-r--r--   0        0        0      203 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/getting_started/test_vector.yml
+-rw-r--r--   0        0        0      132 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/getting_started/vector.py
+-rw-r--r--   0        0        0      137 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0     3074 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params.rst
+-rw-r--r--   0        0        0     3568 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params.rst.bkup
+-rw-r--r--   0        0        0      329 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params/test_vector_kwargs.nt
+-rw-r--r--   0        0        0      649 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params/test_vector_kwargs.py
+-rw-r--r--   0        0        0      291 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params/test_vector_schema.nt
+-rw-r--r--   0        0        0      734 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params/test_vector_schema.py
+-rw-r--r--   0        0        0      305 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/optional_params/vector.py
+-rw-r--r--   0        0        0     7644 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets.rst
+-rw-r--r--   0        0        0      250 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/eval/test_vector.nt
+-rw-r--r--   0        0        0      379 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/eval/test_vector.py
+lrwxr-xr-x   0        0        0        0 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/eval/vector.py -> ../../getting_started/vector.py
+-rw-r--r--   0        0        0      285 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/exec/test_vector.nt
+-rw-r--r--   0        0        0      344 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/exec/test_vector.py
+-rw-r--r--   0        0        0      486 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/exec/vector.py
+lrwxr-xr-x   0        0        0        0 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/schema/test_vector.nt -> ../eval/test_vector.nt
+-rw-r--r--   0        0        0      566 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/schema/test_vector.py
+lrwxr-xr-x   0        0        0        0 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/python_snippets/schema/vector.py -> ../eval/vector.py
+-rw-r--r--   0        0        0      127 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/readme/test_misc.py
+-rw-r--r--   0        0        0       70 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/readme/test_misc.yml
+-rw-r--r--   0        0        0      289 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/requirements.txt
+-rwxr-xr-x   0        0        0      470 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/test_docs.sh
+-rw-r--r--   0        0        0      220 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/docs/tutorials.rst
+-rw-r--r--   0        0        0     1650 2021-12-23 20:26:20.766877 parametrize_from_file-0.9.1/parametrize_from_file/__init__.py
+-rw-r--r--   0        0        0      162 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/errors.py
+-rw-r--r--   0        0        0     1547 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/loaders.py
+-rw-r--r--   0        0        0    18548 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/namespace.py
+-rw-r--r--   0        0        0    20784 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/parameters.py
+-rw-r--r--   0        0        0     1033 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/utils.py
+-rw-r--r--   0        0        0     7981 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/parametrize_from_file/voluptuous.py
+-rw-r--r--   0        0        0     1644 2021-12-23 20:26:20.090873 parametrize_from_file-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       76 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/.coveragerc
+-rw-r--r--   0        0        0       37 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/mock_module.py
+-rw-r--r--   0        0        0       53 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/mock_module_all.py
+-rw-r--r--   0        0        0       30 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/mock_module_overwrite.py
+-rw-r--r--   0        0        0    16922 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/test_namespace.py
+-rw-r--r--   0        0        0    20911 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/test_parameters.py
+-rw-r--r--   0        0        0     2955 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1770 2021-12-23 20:26:20.094873 parametrize_from_file-0.9.1/tests/test_voluptuous.py
+-rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 parametrize_from_file-0.9.1/PKG-INFO
```

### Comparing `parametrize_from_file-0.9.0/.github/workflows/test_and_release.yml` & `parametrize_from_file-0.9.1/.github/workflows/test_and_release.yml`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/.gitignore` & `parametrize_from_file-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/CHANGELOG.md` & `parametrize_from_file-0.9.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.9.1 (2021-12-23)
+### Fix
+* Improve debug message ([`08fa038`](https://github.com/kalekundert/parametrize_from_file/commit/08fa0382d20bbc73312f11232105fa5a1f325357))
+
 ## v0.9.0 (2021-12-23)
 ### Feature
 * Try to import the voluptuous submodule ([`4d5cca4`](https://github.com/kalekundert/parametrize_from_file/commit/4d5cca4581b82526acd1174d66256281b48d9185))
 
 ## v0.8.0 (2021-12-23)
 ### Feature
 * Allow exec() and eval() to be deferred ([`b8cf9d5`](https://github.com/kalekundert/parametrize_from_file/commit/b8cf9d5a10fa9389fb4f90980cce5cc48b30a5b0))
```

### Comparing `parametrize_from_file-0.9.0/LICENSE.txt` & `parametrize_from_file-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/README.rst` & `parametrize_from_file-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/Makefile` & `parametrize_from_file-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/conf.py` & `parametrize_from_file-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/examples.rst` & `parametrize_from_file-0.9.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/exceptions.rst` & `parametrize_from_file-0.9.1/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/exceptions/test_vector.py` & `parametrize_from_file-0.9.1/docs/exceptions/test_vector.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/getting_started.rst` & `parametrize_from_file-0.9.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/optional_params.rst` & `parametrize_from_file-0.9.1/docs/optional_params.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/optional_params.rst.bkup` & `parametrize_from_file-0.9.1/docs/optional_params.rst.bkup`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/optional_params/test_vector_kwargs.py` & `parametrize_from_file-0.9.1/docs/optional_params/test_vector_kwargs.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/optional_params/test_vector_schema.py` & `parametrize_from_file-0.9.1/docs/optional_params/test_vector_schema.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/python_snippets.rst` & `parametrize_from_file-0.9.1/docs/python_snippets.rst`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/docs/python_snippets/schema/test_vector.py` & `parametrize_from_file-0.9.1/docs/python_snippets/schema/test_vector.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/__init__.py` & `parametrize_from_file-0.9.1/parametrize_from_file/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from .errors import ConfigError
 
 try:
     from . import voluptuous
 except ImportError:
     pass
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 for obj in [parametrize, fixture, Namespace, star, ConfigError, add_loader, drop_loader, load_parameters]:
     obj.__module__ = 'parametrize_from_file'
 
 del obj
 
 # Hack to make the module directly usable as a decorator.  Only works for
```

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/loaders.py` & `parametrize_from_file-0.9.1/parametrize_from_file/loaders.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/namespace.py` & `parametrize_from_file-0.9.1/parametrize_from_file/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,22 +463,20 @@
         if isinstance(type, list):
             type = tuple(type)
 
         self.raises_cm = pytest.raises(type)
         self.exc_info = self.raises_cm.__enter__()
 
     def __exit__(self, *args):
-        __tracebackhide__ = True
-
         if self.raises_cm.__exit__(*args):
             ns = self.namespace
             exc = self.exc_info.value
 
             for msg in self.messages:
-                assert msg in str(exc)
+                assert msg in str(exc), f'{msg!r} not in {str(exc)!r}'
 
             for pat in self.patterns:
                 self.exc_info.match(pat)
 
             for attr, value_str in self.attr_strs.items():
                 assert hasattr(exc, attr)
                 assert getattr(exc, attr) == ns.eval(value_str)
```

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/parameters.py` & `parametrize_from_file-0.9.1/parametrize_from_file/parameters.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/utils.py` & `parametrize_from_file-0.9.1/parametrize_from_file/utils.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/parametrize_from_file/voluptuous.py` & `parametrize_from_file-0.9.1/parametrize_from_file/voluptuous.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/pyproject.toml` & `parametrize_from_file-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/tests/test_namespace.py` & `parametrize_from_file-0.9.1/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/tests/test_parameters.py` & `parametrize_from_file-0.9.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/tests/test_utils.py` & `parametrize_from_file-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/tests/test_voluptuous.py` & `parametrize_from_file-0.9.1/tests/test_voluptuous.py`

 * *Files identical despite different names*

### Comparing `parametrize_from_file-0.9.0/PKG-INFO` & `parametrize_from_file-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parametrize_from_file
-Version: 0.9.0
+Version: 0.9.1
 Summary: Parametrize test functions with values read from config files.
 Home-page: https://github.com/kalekundert/parametrize_from_file
 Author: Kale Kundert
 Author-email: kale@thekunderts.net
 Requires-Python: ~=3.6
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
```

