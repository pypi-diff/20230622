# Comparing `tmp/satori_playbook_validator-2.2.0.tar.gz` & `tmp/satori_playbook_validator-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.2.0.tar", last modified: Mon Jun 19 22:18:14 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.2.1.tar", last modified: Wed Jun 21 23:46:39 2023, max compression
```

## Comparing `satori_playbook_validator-2.2.0.tar` & `satori_playbook_validator-2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/README.md
--rw-r--r--   0        0        0      474 2023-06-19 22:18:14.296859 satori_playbook_validator-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5171 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      284 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1888 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      874 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/README.md
+-rw-r--r--   0        0        0      474 2023-06-21 23:46:39.830358 satori_playbook_validator-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5171 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      284 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2439 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0     1262 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-21 23:46:25.666255 satori_playbook_validator-2.2.1/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.2.1/PKG-INFO
```

### Comparing `satori_playbook_validator-2.2.0/src/satorici/validator/_validator.py` & `satori_playbook_validator-2.2.1/src/satorici/validator/_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.2.1/src/satorici/validator/schemas/test.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {"'propertyNames'": "{'if': OrderedDict([('pattern', '^assert')]), 'then': OrderedDict([('oneOf', "*

 * *                    "[OrderedDict([('pattern', '^assert(ReturnCode|Different|Killed)$')]), "*

 * *                    "OrderedDict([('pattern', '^assertStd(out|err)(SHA256)?$')]), "*

 * *                    "OrderedDict([('pattern', "*

 * *                    "'^assertStd(out|err)(Not)?(Contains|Equal|Regex)$')]), "*

 * *                    "OrderedDict([('pattern', '^assert(File|Command)Exists$')])])])}"}*

```diff
@@ -69,11 +69,30 @@
             "type": "integer"
         },
         "settings": {
             "$ref": "file://./settings.json"
         }
     },
     "propertyNames": {
-        "pattern": "^[\\w-]+$"
+        "if": {
+            "pattern": "^assert"
+        },
+        "pattern": "^[\\w-]+$",
+        "then": {
+            "oneOf": [
+                {
+                    "pattern": "^assert(ReturnCode|Different|Killed)$"
+                },
+                {
+                    "pattern": "^assertStd(out|err)(SHA256)?$"
+                },
+                {
+                    "pattern": "^assertStd(out|err)(Not)?(Contains|Equal|Regex)$"
+                },
+                {
+                    "pattern": "^assert(File|Command)Exists$"
+                }
+            ]
+        }
     },
     "type": "object"
 }
```

### Comparing `satori_playbook_validator-2.2.0/tests/test_reference_finder.py` & `satori_playbook_validator-2.2.1/tests/test_reference_finder.py`

 * *Files identical despite different names*

