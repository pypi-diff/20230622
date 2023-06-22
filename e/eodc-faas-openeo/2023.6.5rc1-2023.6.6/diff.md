# Comparing `tmp/eodc_faas_openeo-2023.6.5rc1.tar.gz` & `tmp/eodc_faas_openeo-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_openeo-2023.6.5rc1.tar", max compression
+gzip compressed data, was "eodc_faas_openeo-2023.6.6.tar", max compression
```

## Comparing `eodc_faas_openeo-2023.6.5rc1.tar` & `eodc_faas_openeo-2023.6.6.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       11 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/README.md
--rw-r--r--   0        0        0      107 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/__init__.py
--rw-r--r--   0        0        0      272 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/model.py
--rw-r--r--   0        0        0     4827 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/workflow.py
--rw-r--r--   0        0        0      699 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.5rc1/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/README.md
+-rw-r--r--   0        0        0      102 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/openeo_executor_bindings/__init__.py
+-rw-r--r--   0        0        0      901 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/openeo_executor_bindings/model.py
+-rw-r--r--   0        0        0      612 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/pyproject.toml
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.6/PKG-INFO
```

### Comparing `eodc_faas_openeo-2023.6.5rc1/PKG-INFO` & `eodc_faas_openeo-2023.6.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: eodc-faas-openeo
-Version: 2023.6.5rc1
+Version: 2023.6.6
 Summary: Bindings for the OpenEO processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyproj (>=3.5.0,<4.0.0)
-Requires-Dist: pystac (>=1.7.3,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Bindings
```

