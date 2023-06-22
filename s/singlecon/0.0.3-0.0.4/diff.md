# Comparing `tmp/singlecon-0.0.3.tar.gz` & `tmp/singlecon-0.0.4.tar.gz`

## Comparing `singlecon-0.0.3.tar` & `singlecon-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 singlecon-0.0.3/src/singlecon/__init__.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 singlecon-0.0.3/src/singlecon/template_config.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 singlecon-0.0.3/tests/test_config.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 singlecon-0.0.3/.gitignore
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 singlecon-0.0.3/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 singlecon-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 singlecon-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 singlecon-0.0.4/src/singlecon/__init__.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 singlecon-0.0.4/src/singlecon/template_config.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 singlecon-0.0.4/tests/test_config.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 singlecon-0.0.4/tests/test_pydantic.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 singlecon-0.0.4/.gitignore
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 singlecon-0.0.4/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 singlecon-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 singlecon-0.0.4/PKG-INFO
```

### Comparing `singlecon-0.0.3/src/singlecon/template_config.py` & `singlecon-0.0.4/src/singlecon/template_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 def toml_settings(settings: TemplateConfig) -> Dict[str, Any]:
     if not settings.__config__.config_file:
         return {}
     path = Path(settings.__config__.config_file)
     if path.exists():
         with open(path, 'r') as f:
-            conf_dict = tomlkit.load(f)
+            conf_dict = tomlkit.load(f).value
         return conf_dict
     else:
         return {}
 
 class FileConfig(TemplateConfig):
     _extra_file = True
```

### Comparing `singlecon-0.0.3/.gitignore` & `singlecon-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `singlecon-0.0.3/pyproject.toml` & `singlecon-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singlecon"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Victor Serban", email="serban.victor@gmail.com" },
 ]
 description = "One config to rule them all"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `singlecon-0.0.3/PKG-INFO` & `singlecon-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: singlecon
-Version: 0.0.3
+Version: 0.0.4
 Summary: One config to rule them all
 Author-email: Victor Serban <serban.victor@gmail.com>
+License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
```

