# Comparing `tmp/ssm-ps-template-2.4.1.tar.gz` & `tmp/ssm-ps-template-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.4.1.tar", last modified: Wed Jun 21 18:19:42 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.5.0.tar", last modified: Thu Jun 22 17:15:29 2023, max compression
```

## Comparing `ssm-ps-template-2.4.1.tar` & `ssm-ps-template-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    12757 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10121 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2814 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12757 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3021 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:15:29.532581 ssm-ps-template-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12896 2023-06-22 17:15:29.532581 ssm-ps-template-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10260 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:15:29.532581 ssm-ps-template-2.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:15:29.528581 ssm-ps-template-2.5.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:15:29.528581 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12896 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 17:15:29.000000 ssm-ps-template-2.5.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:15:29.532581 ssm-ps-template-2.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-22 17:15:18.000000 ssm-ps-template-2.5.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.4.1/LICENSE.txt` & `ssm-ps-template-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/PKG-INFO` & `ssm-ps-template-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.4.1
+Version: 2.5.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -175,14 +175,15 @@
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `coerce_types`          | Recursively cast bools, ints, and NULL from strings in data structures                                       |
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
 | `fromjson`              | Convert a JSON blob to a data structure                                                                      |
 | `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
```

### Comparing `ssm-ps-template-2.4.1/README.md` & `ssm-ps-template-2.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `coerce_types`          | Recursively cast bools, ints, and NULL from strings in data structures                                       |
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
 | `fromjson`              | Convert a JSON blob to a data structure                                                                      |
 | `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
```

### Comparing `ssm-ps-template-2.4.1/pyproject.toml` & `ssm-ps-template-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.4.1"
+version = "2.5.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template/__main__.py` & `ssm-ps-template-2.5.0/ssm_ps_template/__main__.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template/config.py` & `ssm-ps-template-2.5.0/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template/discovery.py` & `ssm-ps-template-2.5.0/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template/render.py` & `ssm-ps-template-2.5.0/ssm_ps_template/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,46 @@
 from jinja2 import sandbox
 
 from ssm_ps_template import ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
+def coerce_type(value_in: str) -> typing.Union[bool, int, None, str]:
+    if value_in.lower() in ['true', 'false']:
+        return True if value_in.lower() == 'true' else False
+    elif value_in.lower() in ['~', 'null']:
+        return None
+    elif value_in.isnumeric() and '.' not in value_in:
+        return int(value_in)
+    return value_in
+
+
+def coerce(value_in: typing.Union[dict, list]) -> typing.Union[dict, list]:
+    if isinstance(value_in, dict):
+        output = {}
+        for key, value in value_in.items():
+            new_key = key.replace('-', '_')
+            if isinstance(value, (dict, list)):
+                output[new_key] = coerce(value)
+            else:
+                output[new_key] = coerce_type(value)
+        return output
+    elif isinstance(value_in, list):
+        output = []
+        for value in value_in:
+            if isinstance(value, (dict, list)):
+                output.append(coerce(value))
+            else:
+                output.append(coerce_type(value))
+        return output
+    else:
+        raise TypeError('Method invoked with incorrect data type')
+
+
 def path_to_dict(value: dict) -> dict:
     flat = flatdict.FlatDict(value, delimiter='/')
     return flat.as_dict()
 
 
 def replace_dashes_with_underscores(value_in: typing.Union[dict, list]) \
         -> typing.Union[dict, list]:
@@ -49,14 +81,15 @@
             self._source = handle.read()
         self._values: typing.Optional[ssm.Values] = None
 
     def render(self, values: ssm.Values) -> str:
         """Render the template to the internal buffer"""
         self._values = values
         environment = sandbox.ImmutableSandboxedEnvironment()
+        environment.filters['coerce_types'] = coerce
         environment.filters['dashes_to_underscores'] = \
             replace_dashes_with_underscores
         environment.filters['fromjson'] = lambda v: json.loads(v)
         environment.filters['fromyaml'] = lambda v: yaml.safe_load(v)
         environment.filters['path_to_dict'] = path_to_dict
         environment.filters['toyaml'] = lambda v: yaml.safe_dump(v)
         environment.globals['get_parameter'] = self._get_parameter
```

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template/ssm.py` & `ssm-ps-template-2.5.0/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.5.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.4.1
+Version: 2.5.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -175,14 +175,15 @@
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `coerce_types`          | Recursively cast bools, ints, and NULL from strings in data structures                                       |
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
 | `fromjson`              | Convert a JSON blob to a data structure                                                                      |
 | `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
```

### Comparing `ssm-ps-template-2.4.1/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.5.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/tests/test_config.py` & `ssm-ps-template-2.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/tests/test_discovery.py` & `ssm-ps-template-2.5.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/tests/test_main.py` & `ssm-ps-template-2.5.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.1/tests/test_render.py` & `ssm-ps-template-2.5.0/tests/test_render.py`

 * *Files 20% similar despite different names*

```diff
@@ -74,7 +74,37 @@
                 'bar': {
                     'baz': 'qux',
                     'qux': 'quux'
                 }
             }
         }
         self.assertDictEqual(render.path_to_dict(value), expectation)
+
+
+class CoerceTestCase(unittest.TestCase):
+
+    def test_dict_coercion(self):
+        value = {
+            'foo': {
+                'bool_true': 'true',
+                'bool_false': 'false',
+                'float': '10.0',
+                'int': '1',
+                'null_tilde': '~',
+                'null_word': 'NULL',
+                'str': 'value'
+            },
+            'bar': ['true', 'false', '10.0', '2', '~', 'null', 'value']
+        }
+        expectation = {
+            'foo': {
+                'bool_true': True,
+                'bool_false': False,
+                'float': '10.0',
+                'int': 1,
+                'null_tilde': None,
+                'null_word': None,
+                'str': 'value'
+            },
+            'bar': [True, False, '10.0', 2, None, None, 'value']
+        }
+        self.assertDictEqual(render.coerce(value), expectation)
```

### Comparing `ssm-ps-template-2.4.1/tests/test_ssm.py` & `ssm-ps-template-2.5.0/tests/test_ssm.py`

 * *Files identical despite different names*

