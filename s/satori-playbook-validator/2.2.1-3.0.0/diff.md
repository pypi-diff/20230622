# Comparing `tmp/satori_playbook_validator-2.2.1.tar.gz` & `tmp/satori_playbook_validator-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.2.1.tar", last modified: Wed Jun 21 23:46:39 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.0.0.tar", last modified: Thu Jun 22 03:46:32 2023, max compression
```

## Comparing `satori_playbook_validator-2.2.1.tar` & `satori_playbook_validator-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       30 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/README.md
--rw-r--r--   0        0        0      474 2023-06-21 23:46:39.830358 satori_playbook_validator-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5171 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      284 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2439 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0     1262 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-22 03:46:18.452247 satori_playbook_validator-3.0.0/README.md
+-rw-r--r--   0        0        0      474 2023-06-22 03:46:32.880395 satori_playbook_validator-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-06-22 03:46:18.452247 satori_playbook_validator-3.0.0/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5706 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      298 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     1613 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-3.0.0/PKG-INFO
```

### Comparing `satori_playbook_validator-2.2.1/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.0.0/src/satorici/validator/_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import json
 import re
+import warnings
 from copy import deepcopy
 from pathlib import Path
 from urllib.parse import urlsplit
 
 from fastjsonschema import JsonSchemaValueException, compile
 
 from .exceptions import (
     NoExecutionsError,
     PlaybookValidationError,
     PlaybookVariableError,
 )
+from .warnings import NoLogMonitorWarning
 
 INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
 
 SCHEMAS = Path(__file__).parent / "schemas"
 
 with (
     open(SCHEMAS / "command.json") as commands,
@@ -36,52 +38,80 @@
     settings_schema = compile(json.loads(settings.read()))
     test_schema = compile(
         definition=json.loads(test.read()),
         handlers={"file": file_ref_loc},
     )
 
 
-def _validate(schema, value, raise_exception=False):
+def _validate(schema, value):
     try:
         schema(value)
-        return True
     except JsonSchemaValueException as e:
-        if raise_exception:
-            raise e
+        raise PlaybookValidationError(e.message)
+
 
+def _is(validator, value):
+    try:
+        validator(value)
+        return True
+    except PlaybookValidationError:
         return False
 
 
-def validate_inputs(inputs: list, raise_exception=False):
-    return _validate(inputs_schema, inputs, raise_exception)
+def validate_input_group(inputs: list):
+    _validate(inputs_schema, inputs)
+
+
+def is_input_group(inputs: list):
+    return _is(validate_input_group, inputs)
+
+
+def validate_command_group(commands: list):
+    _validate(commands_schema, commands)
+
+
+def is_command_group(commands: list):
+    return _is(validate_command_group, commands)
 
 
-def validate_commands(commands: list, raise_exception=False):
-    return _validate(commands_schema, commands, raise_exception)
+def validate_import_group(imports: list):
+    _validate(imports_schema, imports)
 
 
-def validate_imports(inports: list, raise_exception=False):
-    return _validate(imports_schema, inports, raise_exception)
+def is_import_group(imports: list):
+    return _is(validate_import_group, imports)
 
 
-def validate_test(test: dict, raise_exception=False):
-    return _validate(test_schema, test, raise_exception)
+def validate_test(test: dict):
+    _validate(test_schema, test)
 
 
-def validate_settings(settings: dict, raise_exception=False):
-    return _validate(settings_schema, settings, raise_exception)
+def is_test(test: dict):
+    return _is(validate_test, test)
+
+
+def validate_settings(settings: dict):
+    _validate(settings_schema, settings)
+
+    if "cron" in settings or "rate" in settings:
+        if not any(k.startswith("log") for k in settings):
+            warnings.warn(NoLogMonitorWarning("Monitor without notifications."))
+
+
+def is_settings(settings: dict):
+    return _is(validate_settings, settings)
 
 
 def has_input(d: dict[str]):
     stack = [v for k, v in d.items() if "^" not in k]
 
     while stack:
         current = stack.pop()
 
-        if validate_inputs(current):
+        if is_input_group(current):
             return True
         elif isinstance(current, dict):
             stack.extend(v for k, v in current.items() if "^" not in k)
 
     return False
 
 
@@ -113,15 +143,15 @@
         for key, value in (i for i in current.items() if "^" not in i[0]):
             if key == limit_key:
                 limit_key = current.get("^key")
                 current = current.get("^dict")
                 break
 
             if key in variables:
-                if validate_inputs(value) or (
+                if is_input_group(value) or (
                     isinstance(value, dict) and has_input(value)
                 ):
                     valid.add(key)
                 else:
                     failed = True
                     break
 
@@ -139,15 +169,15 @@
 
     while stack:
         path, current = stack.pop()
 
         for k, v in (i for i in current.items() if "^" not in i[0]):
             if isinstance(v, dict):
                 stack.append((path + (k,), v))
-            elif validate_commands(v):
+            elif is_command_group(v):
                 execution_found = True
                 if get_reference_names(v):
                     validate_references(current, k)
 
     if not execution_found:
         raise NoExecutionsError("No executions found.")
 
@@ -175,16 +205,18 @@
     """
 
     if not isinstance(config, dict):
         raise TypeError("config must be a dict")
 
     config_copy = deepcopy(config)
 
-    try:
-        test_schema(config_copy)
-    except JsonSchemaValueException as e:
-        raise PlaybookValidationError(e.message)
+    if "settings" in config_copy:
+        validate_settings(config_copy.pop("settings"))
+
+    validate_test(config_copy)
 
     add_parent_info(config_copy)
     iterate_dict(config_copy)
 
-    return config
+
+def is_playbook(config: dict):
+    _is(validate_playbook, config)
```

### Comparing `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.0.0/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-3.0.0/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.0.0/src/satorici/validator/schemas/test.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {"'properties'": "{delete: ['settings']}"}*

```diff
@@ -63,17 +63,14 @@
             "type": "boolean"
         },
         "assertKilled": {
             "type": "boolean"
         },
         "assertReturnCode": {
             "type": "integer"
-        },
-        "settings": {
-            "$ref": "file://./settings.json"
         }
     },
     "propertyNames": {
         "if": {
             "pattern": "^assert"
         },
         "pattern": "^[\\w-]+$",
```

### Comparing `satori_playbook_validator-2.2.1/tests/test_playbook_validator.py` & `satori_playbook_validator-3.0.0/tests/test_playbook_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from satorici.validator import validate_playbook
 from satorici.validator.exceptions import PlaybookValidationError
+from satorici.validator.warnings import NoLogMonitorWarning
 
 
 def test_empty_settings():
     playbook = {
         "settings": {},
         "tests": {
             "cmd": [["echo"]],
@@ -63,7 +64,22 @@
         "assertReturnCode": 1,
         "cmd": [
             ["echo"],
         ],
     }
 
     validate_playbook(playbook)
+
+
+def test_monitor_without_notification():
+    playbook = {
+        "settings": {
+            "name": "aaaa",
+            "cron": "0 0 0 0 0",
+        },
+        "cmd": [
+            ["echo"],
+        ],
+    }
+
+    with pytest.warns(NoLogMonitorWarning):
+        validate_playbook(playbook)
```

### Comparing `satori_playbook_validator-2.2.1/tests/test_reference_finder.py` & `satori_playbook_validator-3.0.0/tests/test_reference_finder.py`

 * *Files identical despite different names*

