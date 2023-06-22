# Comparing `tmp/ou_tm351_jl_extensions-0.1.2.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.1.2.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.0.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.1.2.tar` & `ou_tm351_jl_extensions-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-05-15 16:31:11.711058 ou_tm351_jl_extensions-0.1.2/LICENSE
--rw-r--r--   0        0        0      413 2023-05-15 16:31:11.711058 ou_tm351_jl_extensions-0.1.2/README.md
--rw-r--r--   0        0        0     2388 2023-05-15 16:31:11.711058 ou_tm351_jl_extensions-0.1.2/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      914 2023-05-15 16:31:11.711058 ou_tm351_jl_extensions-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/LICENSE
+-rw-r--r--   0        0        0      467 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/README.md
+-rw-r--r--   0        0        0     2388 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      938 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.0/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.1.2/LICENSE` & `ou_tm351_jl_extensions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.1.2/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.0/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.1.2/pyproject.toml` & `ou_tm351_jl_extensions-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-jupyterlab-ou-brand-extension = "^0.1.0"
+jupyterlab = "^4.0.1"
+jupyterlab-ou-brand-extension = "^0.2.0"
 jupyterlab-cell-status-extension = "^0.1.3"
 jupyterlab-myst = "^1.1.3"
-jupyterlab-empinken-extension = "^0.1.1"
+jupyterlab-empinken-extension = "^0.4.0"
 jupyterlab-geojson = "^3.3.1"
-jupyterlab-skip-traceback = "^4.0.4"
+jupyterlab-skip-traceback = "^5.0.0"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
-jupyterlab-spellchecker = "^0.7.3"
+#jupyterlab-spellchecker = "^0.7.3"
 jupyterlab-language-pack-fr-fr = "^3.6.post1"
 jupyterlab-language-pack-zh-cn = "^3.6.post1"
 jupyter-resource-usage = "^0.7.2"
 stickyland = "^0.2.1"
-jupyterlab-tour = "^3.1.4"
+#jupyterlab-tour = "^3.1.4"
 jupyter-compare-view = "^0.2.4"
 jupyterlab-filesystem-access = "^0.5.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ou_tm351_jl_extensions-0.1.2/PKG-INFO` & `ou_tm351_jl_extensions-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jupyter-archive (>=3.3.4,<4.0.0)
 Requires-Dist: jupyter-compare-view (>=0.2.4,<0.3.0)
 Requires-Dist: jupyter-resource-usage (>=0.7.2,<0.8.0)
+Requires-Dist: jupyterlab (>=4.0.1,<5.0.0)
 Requires-Dist: jupyterlab-cell-status-extension (>=0.1.3,<0.2.0)
-Requires-Dist: jupyterlab-empinken-extension (>=0.1.1,<0.2.0)
+Requires-Dist: jupyterlab-empinken-extension (>=0.4.0,<0.5.0)
 Requires-Dist: jupyterlab-filesystem-access (>=0.5.3,<0.6.0)
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
 Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
 Requires-Dist: jupyterlab-language-pack-fr-fr (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-language-pack-zh-cn (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-myst (>=1.1.3,<2.0.0)
-Requires-Dist: jupyterlab-ou-brand-extension (>=0.1.0,<0.2.0)
-Requires-Dist: jupyterlab-skip-traceback (>=4.0.4,<5.0.0)
-Requires-Dist: jupyterlab-spellchecker (>=0.7.3,<0.8.0)
-Requires-Dist: jupyterlab-tour (>=3.1.4,<4.0.0)
+Requires-Dist: jupyterlab-ou-brand-extension (>=0.2.0,<0.3.0)
+Requires-Dist: jupyterlab-skip-traceback (>=5.0.0,<6.0.0)
 Requires-Dist: jupytext (>=1.14.5,<2.0.0)
 Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
 
+Install:
+
+JupyterLab 3: v0.1.2
+JupyterLab 4: v 0.2.0
+
 Recommended JupyterLab extensions for use in the OU TM351 module.
 
 This package will install several JupyterLab extensions that brand and extend a JupyterLab environment to support its use as a teaching and learning environment.
 
 Check the installation by running:
```

