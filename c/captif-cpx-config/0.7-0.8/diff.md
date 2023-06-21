# Comparing `tmp/captif_cpx_config-0.7.tar.gz` & `tmp/captif_cpx_config-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.7.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.8.tar", max compression
```

## Comparing `captif_cpx_config-0.7.tar` & `captif_cpx_config-0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/LICENSE
--rw-r--r--   0        0        0       19 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/README.md
--rw-r--r--   0        0        0       44 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4153 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      522 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/README.md
+-rw-r--r--   0        0        0       44 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4185 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      522 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.8/PKG-INFO
```

### Comparing `captif_cpx_config-0.7/LICENSE` & `captif_cpx_config-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.7/captif_cpx_config/metadata.py` & `captif_cpx_config-0.8/captif_cpx_config/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,16 @@
     )
     wav_scale: condecimal(decimal_places=1) = Field(
         description=(
             "scale factor to apply to the raw wav file data (-1 to + 1 range) "
             "to convert the data back into volts."
         ),
     )
-    notes: str = Field(
+    notes: Optional[str] = Field(
+        default=None,
         description="any additional notes",
     )
 
     wheel_bay_details: list["WheelBayDetails"] = []
 
     def write(self, path: str):
         with open(path, "w") as f:
```

### Comparing `captif_cpx_config-0.7/pyproject.toml` & `captif_cpx_config-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.7"
+version = "0.8"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `captif_cpx_config-0.7/PKG-INFO` & `captif_cpx_config-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.7
+Version: 0.8
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

