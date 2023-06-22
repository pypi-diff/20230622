# Comparing `tmp/cmem_plugin_base-3.1.0rc1.tar.gz` & `tmp/cmem_plugin_base-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_base-3.1.0rc1.tar", max compression
+gzip compressed data, was "cmem_plugin_base-4.0.0rc1.tar", max compression
```

## Comparing `cmem_plugin_base-3.1.0rc1.tar` & `cmem_plugin_base-4.0.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11334 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/LICENSE
--rw-r--r--   0        0        0      246 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/README-public.md
--rw-r--r--   0        0        0       76 2023-03-10 08:38:40.281874 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/__init__.py
--rw-r--r--   0        0        0     3992 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/context.py
--rw-r--r--   0        0        0     8897 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/description.py
--rw-r--r--   0        0        0     2742 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/discovery.py
--rw-r--r--   0        0        0     1370 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/entity.py
--rw-r--r--   0        0        0       37 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/__init__.py
--rw-r--r--   0        0        0     1557 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py
--rw-r--r--   0        0        0     2243 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py
--rw-r--r--   0        0        0     3629 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py
--rw-r--r--   0        0        0      334 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/multiline.py
--rw-r--r--   0        0        0     1739 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/password.py
--rw-r--r--   0        0        0     2625 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/plugins.py
--rw-r--r--   0        0        0     8501 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/types.py
--rw-r--r--   0        0        0     3429 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/utils.py
--rw-r--r--   0        0        0     2088 2023-03-10 08:38:40.281874 cmem_plugin_base-3.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 cmem_plugin_base-3.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2022-02-21 20:33:41.000000 cmem_plugin_base-4.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      246 2022-04-01 14:58:42.645640 cmem_plugin_base-4.0.0rc1/README-public.md
+-rw-r--r--   0        0        0       76 2023-06-22 12:52:05.577458 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-22 01:06:38.000000 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/__init__.py
+-rw-r--r--   0        0        0     3992 2023-03-15 08:18:43.081458 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/context.py
+-rw-r--r--   0        0        0     8897 2023-03-15 08:18:43.081597 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/description.py
+-rw-r--r--   0        0        0     2765 2023-04-27 12:51:39.614863 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/discovery.py
+-rw-r--r--   0        0        0     1370 2022-02-22 12:38:14.000000 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/entity.py
+-rw-r--r--   0        0        0       37 2022-05-04 12:15:39.899212 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/__init__.py
+-rw-r--r--   0        0        0     1557 2023-03-15 08:18:43.081854 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py
+-rw-r--r--   0        0        0     2243 2023-03-15 08:18:43.081961 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py
+-rw-r--r--   0        0        0     3629 2023-03-15 08:18:43.082069 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py
+-rw-r--r--   0        0        0      334 2022-06-15 11:32:12.636378 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/multiline.py
+-rw-r--r--   0        0        0     1739 2023-03-15 08:18:43.082177 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/password.py
+-rw-r--r--   0        0        0     2625 2023-03-15 08:18:43.082282 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/plugins.py
+-rw-r--r--   0        0        0     8501 2023-03-15 08:18:43.082793 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/types.py
+-rw-r--r--   0        0        0     3429 2023-03-15 08:18:43.082970 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/utils.py
+-rw-r--r--   0        0        0     2059 2023-06-22 12:52:05.576580 cmem_plugin_base-4.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 cmem_plugin_base-4.0.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_base-3.1.0rc1/LICENSE` & `cmem_plugin_base-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/context.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/context.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/description.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/description.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/discovery.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 def get_packages():
     """Get installed python packages.
 
     Returns a list of dict with the following keys:
      - name - package name
      - version - package version
     """
-    return json.loads(check_output(["pip", "list", "--format", "json"], shell=False))
+    return json.loads(
+        check_output(["pip", "list", "--format", "json"], shell=False)  # nosec
+    )
 
 
 def discover_plugins_in_module(
     package_name: str = "cmem",
 ) -> list[PluginDescription]:
     """Finds all plugins within a base package.
```

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/entity.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/entity.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/password.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/password.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/plugins.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/plugins.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/types.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/types.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/utils.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0rc1/pyproject.toml` & `cmem_plugin_base-4.0.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-base"
-version = "3.1.0rc1"
+version = "4.0.0rc1"
 license = "Apache-2.0"
 description = "Base classes for developing eccenca Coporate Memory plugins."
 authors = ["eccenca <cmempy-developer@eccenca.com>"]
 maintainers = [
     "Sebastian Tramp <sebastian.tramp@eccenca.com>",
     "Robert Isele <robert.isele@eccenca.com>"
 ]
@@ -15,38 +15,36 @@
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugins", "DataIntegration"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-cmempy = ">=22.1"
+python = "^3.11"
+cmem-cmempy = "==23.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^4.0.0"
-pytest-memray = "^1.3.0"
-black = "^23.1.0"
-bandit = "^1.7.2"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.7"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.4.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pytest-memray = "^1.4.1"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^1.0.0"
-coverage = "^7.1.0"
-defusedxml = "^0.7.1"
-wheel = "^0.38.3"
+typed-ast = "^1.5.4"
+types-requests = "^2.28.11.15"
+wheel = "^0.38.4"
 # added in order to have something to discover (>=0.0.0 <1.0.0)
 # cmem-plugin-examples = "*"
 
-[tool.poetry.group.dev.dependencies]
-types-requests = "^2.28.11.15"
-
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `cmem_plugin_base-3.1.0rc1/PKG-INFO` & `cmem_plugin_base-4.0.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-base
-Version: 3.1.0rc1
+Version: 4.0.0rc1
 Summary: Base classes for developing eccenca Coporate Memory plugins.
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugins,DataIntegration
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-cmempy (>=22.1)
+Requires-Dist: cmem-cmempy (==23.1)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-base
 
 Python base classes for developing eccenca Coporate Memory plugins.
 
 In order to kick-start developing eccenca Corporate Memory Plugins, please check out this project template: https://github.com/eccenca/cmem-plugin-template
```

