# Comparing `tmp/riscv_config-3.9.0.tar.gz` & `tmp/riscv_config-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_config-3.9.0.tar", last modified: Tue May 16 12:59:35 2023, max compression
+gzip compressed data, was "dist/riscv_config-3.9.1.tar", last modified: Thu Jun 22 04:01:23 2023, max compression
```

## Comparing `riscv_config-3.9.0.tar` & `riscv_config-3.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 12:59:06.000000 riscv_config-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 12:59:35.000000 riscv_config-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 12:59:06.000000 riscv_config-3.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96921 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/isa_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemaValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_custom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_isa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/warl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 12:59:35.000000 riscv_config-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-16 12:59:06.000000 riscv_config-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 04:01:00.000000 riscv_config-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 04:01:23.000000 riscv_config-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-22 04:01:00.000000 riscv_config-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97275 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/isa_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemaValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_isa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/warl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 04:01:23.000000 riscv_config-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-22 04:01:00.000000 riscv_config-3.9.1/setup.py
```

### Comparing `riscv_config-3.9.0/PKG-INFO` & `riscv_config-3.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv_config
-Version: 3.9.0
+Version: 3.9.1
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
```

### Comparing `riscv_config-3.9.0/riscv_config/checker.py` & `riscv_config-3.9.1/riscv_config/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1351,20 +1351,22 @@
     virtualization_possible = False
     if 'ro_constant' in satp_mode_type:
         if satp_mode_type['ro_constant'] == 0:
             virtualization_possible = False
         else:
             virtualization_possible = True
     elif 'warl' in satp_mode_type:
-        warl_inst = warl_class(satp_mode_type['warl'], 'satp::mode',63, 60)
-        for x in [1,2,3,4,5,6,7,11,12,13]:
-            err = warl_inst.islegal(x)
-            if not err:
-                errors.append(f'warl function for satp::mode accepts \
-"{x}" as a legal value - which is incorrect')
+        # these are the checks from _check_with_satp_modes64
+        if xlen == 64:
+            warl_inst = warl_class(satp_mode_type['warl'], 'satp::mode',63, 60)
+            for x in [1,2,3,4,5,6,7,11,12,13]:
+                err = warl_inst.islegal(x)
+                if not err:
+                    errors['satp_mode_checks'] = f'warl function for satp::mode accepts \
+    "{x}" as a legal value - which is incorrect'
         warl_inst = warl_class(satp_mode_type['warl'], 'satp::mode', msb, lsb, spec)
         for x in virt_modes:
             err = warl_inst.islegal(x)
             if not err:
                 virtualization_possible = True
                 break
 
@@ -2034,16 +2036,18 @@
 
     merged = {}
     hart_ids = []
     for entry in ispec_dict['hart_ids']:
         hart_ids.append(entry)
         merged[entry] = {}
         merged[entry].update(ispec_dict['hart'+str(entry)])
-        merged[entry].update(customspec_dict['hart'+str(entry)])
-        merged[entry].update(dspec_dict['hart'+str(entry)])
+        if custom_file is not None:
+            merged[entry].update(customspec_dict['hart'+str(entry)])
+        if debug_file is not None:
+            merged[entry].update(dspec_dict['hart'+str(entry)])
 
         try:
             uarch_signals = merged[entry]['uarch_signals']
         except KeyError as e:
             logger.info("No uarch signals found for hart"+str(entry))
             uarch_signals = {}
 
@@ -2087,15 +2091,19 @@
 
         errors = check_pmp(csr_db, logging)
         if errors:
             raise ValidationError("Error in csr definitions", errors)
 
         if logging:
             logger.info(f'Initiating validation checks for trigger csrs')
-        errors = check_triggers(csr_db, logging)
+        if dspec_dict == {}:
+            if logging:
+                logger.warning(f'No debug spec passed. Skipping trigger checks.')
+        else:
+            errors = check_triggers(csr_db, logging)
         if errors:
             raise ValidationError("Error in csr definitions", errors)
 
         if logging and not errors:
             logger.info(f'All checks completed for hart{entry}. No errors found.')
 
     return specs_list
```

### Comparing `riscv_config-3.9.0/riscv_config/constants.py` & `riscv_config-3.9.1/riscv_config/constants.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/errors.py` & `riscv_config-3.9.1/riscv_config/errors.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/isa_validator.py` & `riscv_config-3.9.1/riscv_config/isa_validator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/main.py` & `riscv_config-3.9.1/riscv_config/main.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/schemaValidator.py` & `riscv_config-3.9.1/riscv_config/schemaValidator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/schemas/schema_custom.yaml` & `riscv_config-3.9.1/riscv_config/schemas/schema_custom.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/schemas/schema_debug.yaml` & `riscv_config-3.9.1/riscv_config/schemas/schema_debug.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/schemas/schema_isa.yaml` & `riscv_config-3.9.1/riscv_config/schemas/schema_isa.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/schemas/schema_platform.yaml` & `riscv_config-3.9.1/riscv_config/schemas/schema_platform.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/utils.py` & `riscv_config-3.9.1/riscv_config/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config/warl.py` & `riscv_config-3.9.1/riscv_config/warl.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/riscv_config.egg-info/SOURCES.txt` & `riscv_config-3.9.1/riscv_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.0/setup.py` & `riscv_config-3.9.1/setup.py`

 * *Files identical despite different names*

