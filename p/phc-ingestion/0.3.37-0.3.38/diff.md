# Comparing `tmp/phc-ingestion-0.3.37.tar.gz` & `tmp/phc-ingestion-0.3.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.37.tar", last modified: Tue Jun 13 17:21:35 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.38.tar", last modified: Thu Jun 22 13:28:11 2023, max compression
```

## Comparing `phc-ingestion-0.3.37.tar` & `phc-ingestion-0.3.38.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5907 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     4949 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.37/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5907 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5216 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-22 13:27:43.831796 phc-ingestion-0.3.38/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-22 13:27:43.835795 phc-ingestion-0.3.38/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-22 13:27:43.835795 phc-ingestion-0.3.38/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-22 13:27:43.835795 phc-ingestion-0.3.38/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-22 13:27:43.835795 phc-ingestion-0.3.38/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-22 13:27:43.835795 phc-ingestion-0.3.38/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.38/PKG-INFO
```

### Comparing `phc-ingestion-0.3.37/ingestion/caris/process.py` & `phc-ingestion-0.3.38/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.38/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.38/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.38/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.38/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/json.py` & `phc-ingestion-0.3.38/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.38/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.38/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.38/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.38/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/foundation/process.py` & `phc-ingestion-0.3.38/ingestion/foundation/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         results_payload_dict = xml_dict["rr:ResultsReport"]["rr:ResultsPayload"]
 
         sample_name = get_specimen_name(results_payload_dict)
 
         base_xml_name = Path(xml_file).stem
 
         vcf_name = f"{local_output_dir}/{base_xml_name}/{base_xml_name}.tcf"
-        vcf_line_count = vcf_etl(vcf_file, vcf_name, base_xml_name, xml_file)
+        vcf_line_count = vcf_etl(vcf_file, vcf_name, base_xml_name, xml_file, log)
         write_cnv = extract_copy_numbers(results_payload_dict, base_xml_name, local_output_dir, log)
         write_fnv = extract_fusion_variant(
             results_payload_dict, base_xml_name, local_output_dir, log
         )
 
         yaml_file = get_test_yml(
             customer_info_dict,
```

### Comparing `phc-ingestion-0.3.37/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.38/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.38/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.38/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.38/ingestion/foundation/util/vcf_etl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import gzip
 import xmltodict
 from natsort import natsorted
+from logging import Logger
 import re
 import os
 import errno
 
 
-def vcf_etl(in_vcf: str, out_vcf: str, base_xml_name: str, xml_file: str) -> int:
+def vcf_etl(in_vcf: str, out_vcf: str, base_xml_name: str, xml_file: str, log: Logger) -> int:
     headers = []
     vars = []
 
     # Get xml short variant entries for scraping vendsig
-    xml_short_vars = get_xml_short_vars(xml_file)
+    xml_short_vars = get_xml_short_vars(xml_file, log)
 
     if not os.path.exists(os.path.dirname(out_vcf)):
         try:
             os.makedirs(os.path.dirname(out_vcf))
         except OSError as exc:
             if exc.errno != errno.EEXIST:
                 raise
@@ -73,20 +74,24 @@
                     sample = ":".join([gt, str(depth), ad])
                     var = untouched_var + f"\t{new_vcf_info}\t{vcf_format}\t{sample}\n"
                     w.write(var)
 
             return line_count
 
 
-def get_xml_short_vars(xml_file: str) -> dict:
+def get_xml_short_vars(xml_file: str, log) -> dict:
     with open(xml_file) as fd:
         xml_dict = xmltodict.parse(fd.read())
-    xml_short_vars = xml_dict["rr:ResultsReport"]["rr:ResultsPayload"]["variant-report"][
-        "short-variants"
-    ]["short-variant"]
+    try:
+        xml_short_vars = xml_dict["rr:ResultsReport"]["rr:ResultsPayload"]["variant-report"][
+            "short-variants"
+        ]["short-variant"]
+    except TypeError:
+        log.error("No short variants found in xml")
+        return {}
     return xml_short_vars
 
 
 def map_vendsig(vendsig: str) -> str:
     if vendsig in ["known"]:
         return "VENDSIG=Pathogenic"
     elif vendsig in ["likely"]:
@@ -98,23 +103,27 @@
 
 
 def add_vendsig_to_info(var: str, xml_short_vars: dict) -> str:
     info = var.split("\t")[7]
     # using transcript name, find it in xml_short_vars
     transcript_name = info.split(";")[-1].split("=")[1].strip()
     # dictionary comprehension to get the short_var in xml_short_vars that matches the transcript_name
-    matched_xml_var = [
-        short_var
-        for short_var in xml_short_vars
-        if short_var.get("@transcript", "") == transcript_name
-    ]
-    if not matched_xml_var:
+    if xml_short_vars == {}:
         vendsig = "Unknown"
     else:
-        vendsig = matched_xml_var[0]["@status"]
+
+        matched_xml_var = [
+            short_var
+            for short_var in xml_short_vars
+            if short_var.get("@transcript", "") == transcript_name
+        ]
+        if not matched_xml_var:
+            vendsig = "Unknown"
+        else:
+            vendsig = matched_xml_var[0]["@status"]
 
     mapped_vendsig = map_vendsig(vendsig)
     new_vcf_info = f"{info.strip()};{mapped_vendsig}"
     return new_vcf_info
 
 
 def transform_scientific_notation_in_af(var: str) -> str:
```

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/process.py` & `phc-ingestion-0.3.38/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.38/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.38/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.38/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.38/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.38/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.38/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.38/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.38/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.38/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.37/pyproject.toml` & `phc-ingestion-0.3.38/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.37"
+version = "0.3.38"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

