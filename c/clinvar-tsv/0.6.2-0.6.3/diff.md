# Comparing `tmp/clinvar-tsv-0.6.2.tar.gz` & `tmp/clinvar-tsv-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinvar-tsv-0.6.2.tar", last modified: Wed Jun 21 15:02:30 2023, max compression
+gzip compressed data, was "clinvar-tsv-0.6.3.tar", last modified: Thu Jun 22 09:36:59 2023, max compression
```

## Comparing `clinvar-tsv-0.6.2.tar` & `clinvar-tsv-0.6.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/clinvar_tsv/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/clinvar_tsv/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/parse_clinvar_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-92148661.xml
--rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-in-context-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-spta1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-in-context-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-spta1.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_parse_xml_small.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_parse_xml_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/clinvar_tsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/clinvar_tsv/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/clinvar_tsv/parse_clinvar_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.224187 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 09:36:59.000000 clinvar-tsv-0.6.3/clinvar_tsv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.224187 clinvar-tsv-0.6.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.224187 clinvar-tsv-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:36:59.228187 clinvar-tsv-0.6.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/clinvar-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/clinvar-92148661.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/clinvar-in-context-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/clinvar-spta1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/parsed-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/parsed-in-context-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/data/parsed-spta1.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/test_merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/test_parse_xml_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/tests/test_parse_xml_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-22 09:36:56.000000 clinvar-tsv-0.6.3/versioneer.py
```

### Comparing `clinvar-tsv-0.6.2/LICENSE` & `clinvar-tsv-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/PKG-INFO` & `clinvar-tsv-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,22 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+### [0.6.3](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.2...v0.6.3) (2023-06-22)
+
+
+### Bug Fixes
+
+* improved debugging for normalize ([#29](https://www.github.com/bihealth/clinvar-tsv/issues/29)) ([4124a34](https://www.github.com/bihealth/clinvar-tsv/commit/4124a3434294ee6736e5487b1586f9a9f0921b02))
+* memory usage in normalize command ([#31](https://www.github.com/bihealth/clinvar-tsv/issues/31)) ([33f8ac7](https://www.github.com/bihealth/clinvar-tsv/commit/33f8ac79891f1a36f788bc619e2ad728ebdabbae))
+
 ### [0.6.2](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.1...v0.6.2) (2023-06-21)
 
 
 ### Bug Fixes
 
 * failure to determine location only goes to debug level ([#22](https://www.github.com/bihealth/clinvar-tsv/issues/22)) ([76bc510](https://www.github.com/bihealth/clinvar-tsv/commit/76bc5105e6f0b26146dcaca43465c1dd59d1aee2))
 * higher verbosity in Snakemake rules ([#26](https://www.github.com/bihealth/clinvar-tsv/issues/26)) ([a3fc327](https://www.github.com/bihealth/clinvar-tsv/commit/a3fc3271a8984b39d52c8852f6fe77b05b1193c0))
```

### Comparing `clinvar-tsv-0.6.2/README.md` & `clinvar-tsv-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/Snakefile` & `clinvar-tsv-0.6.3/clinvar_tsv/Snakefile`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/__main__.py` & `clinvar-tsv-0.6.3/clinvar_tsv/__main__.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/common.py` & `clinvar-tsv-0.6.3/clinvar_tsv/common.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/merge_tsvs.py` & `clinvar-tsv-0.6.3/clinvar_tsv/merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/normalize.py` & `clinvar-tsv-0.6.3/clinvar_tsv/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 (we have encountered this when parsing the ClinVar XML dump) may be not only
 non-minimal but also right-aligned rather than left-aligned, and may contain
 hyphens. For those situations, use this script (or just run vt normalize).
 
 Usage: normalize.py -R $b37ref < bad_file.txt > good_file.txt
 """
 
+import os
+import subprocess
 import sys
 
 import pysam
+import tqdm
 
 
 class RefEqualsAltError(Exception):
     """
     An Error class for rare cases where REF == ALT (seen in ClinVar XML)
     """
 
@@ -150,61 +153,67 @@
     columns = header.strip("\n").split("\t")  # parse col names
     outfile.write("\t".join(columns) + "\n")  # write header line plus the CpG col to be generated
     counter = 0
     ref_equals_alt = 0
     wrong_ref = 0
     invalid_nucleotide = 0
     unknown_contig = 0
-    for line in infile.readlines():
-        data = dict(zip(columns, line.strip("\n").split("\t")))
-        # fill the data with blanks for any missing data
-        for column in columns:
-            if column not in data.keys():
-                data[column] = ""
-        pos = int(data.get("position", data["start"]))
-        # Normalize "chr" prefix towards reference and fix M/MT
-        if ref_chr_prefix == has_chr(data["chromosome"]):
-            chrom = data["chromosome"]
-        elif ref_chr_prefix:
-            chrom = "chr%s" % data["chromosome"]
-        else:
-            chrom = data["chrom"][3:]
-        if ref_chr_prefix and chrom.endswith("MT"):
-            chrom = "chrM"
-        # Perform normalization
-        try:
-            _, pos, data["reference"], data["alternative"] = normalize(
-                pysam_fasta, chrom, pos, data["reference"], data["alternative"]
-            )
-            if data["chromosome"].startswith("chr"):
-                data["chromosome"] = data["chromosome"][3:]
-        except KeyError as e:
-            sys.stderr.write("\n" + str(e) + "\n")
-            unknown_contig += 1
-            continue
-        except RefEqualsAltError as e:
-            sys.stderr.write("\n" + str(e) + "\n")
-            ref_equals_alt += 1
-            continue
-        except WrongRefError as e:
-            sys.stderr.write("\n" + str(e) + "\n")
-            wrong_ref += 1
-            continue
-        except InvalidNucleotideSequenceError as e:
-            sys.stderr.write("\n" + str(e) + "\n")
-            invalid_nucleotide += 1
-            continue
-        if "position" in columns:
-            data["position"] = str(pos)
-        else:
-            data["start"] = str(pos)
-            data["end"] = str(pos + len(data["reference"]) - 1)
-        outfile.write("\t".join([data[column] for column in columns]) + "\n")
-        counter += 1
-        if verbose and counter % 1000 == 0:
-            sys.stderr.write("\r%s records processed\n" % (counter))
+    # Reduce the progress bar refresh rate if we're not in a TTY
+    mininterval = 0.1 if sys.stdout.isatty() else 60
+    with tqdm.tqdm(unit="lines", mininterval=mininterval) as progress:
+        for line in infile:
+            data = dict(zip(columns, line.strip("\n").split("\t")))
+            # fill the data with blanks for any missing data
+            for column in columns:
+                if column not in data.keys():
+                    data[column] = ""
+            pos = int(data.get("position", data["start"]))
+            # Normalize "chr" prefix towards reference and fix M/MT
+            if ref_chr_prefix == has_chr(data["chromosome"]):
+                chrom = data["chromosome"]
+            elif ref_chr_prefix:
+                chrom = "chr%s" % data["chromosome"]
+            else:
+                chrom = data["chrom"][3:]
+            if ref_chr_prefix and chrom.endswith("MT"):
+                chrom = "chrM"
+            # Perform normalization
+            try:
+                _, pos, data["reference"], data["alternative"] = normalize(
+                    pysam_fasta, chrom, pos, data["reference"], data["alternative"]
+                )
+                if data["chromosome"].startswith("chr"):
+                    data["chromosome"] = data["chromosome"][3:]
+            except KeyError as e:
+                sys.stderr.write("\n" + str(e) + "\n")
+                unknown_contig += 1
+                continue
+            except RefEqualsAltError as e:
+                sys.stderr.write("\n" + str(e) + "\n")
+                ref_equals_alt += 1
+                continue
+            except WrongRefError as e:
+                sys.stderr.write("\n" + str(e) + "\n")
+                wrong_ref += 1
+                continue
+            except InvalidNucleotideSequenceError as e:
+                sys.stderr.write("\n" + str(e) + "\n")
+                invalid_nucleotide += 1
+                continue
+            if "position" in columns:
+                data["position"] = str(pos)
+            else:
+                data["start"] = str(pos)
+                data["end"] = str(pos + len(data["reference"]) - 1)
+            outfile.write("\t".join([data[column] for column in columns]) + "\n")
+            counter += 1
+            if verbose and counter % 1000 == 0:
+                sys.stderr.write("\r%s records processed\n" % (counter))
+            if os.environ.get("DEBUG_MEM", "0") == "1" and counter % 10000 == 0:
+                subprocess.run(["free"])
+            progress.update()
     outfile.write("\n\n")
     if verbose:
         sys.stderr.write(
             "Final counts of variants discarded:\nREF == ALT: %s\nWrong REF: %s\nInvalid nucleotide: %s\nUnknown contig: %s\n"
             % (ref_equals_alt, wrong_ref, invalid_nucleotide, unknown_contig)
         )
```

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv/parse_clinvar_xml.py` & `clinvar-tsv-0.6.3/clinvar_tsv/parse_clinvar_xml.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv.egg-info/PKG-INFO` & `clinvar-tsv-0.6.3/clinvar_tsv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,22 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+### [0.6.3](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.2...v0.6.3) (2023-06-22)
+
+
+### Bug Fixes
+
+* improved debugging for normalize ([#29](https://www.github.com/bihealth/clinvar-tsv/issues/29)) ([4124a34](https://www.github.com/bihealth/clinvar-tsv/commit/4124a3434294ee6736e5487b1586f9a9f0921b02))
+* memory usage in normalize command ([#31](https://www.github.com/bihealth/clinvar-tsv/issues/31)) ([33f8ac7](https://www.github.com/bihealth/clinvar-tsv/commit/33f8ac79891f1a36f788bc619e2ad728ebdabbae))
+
 ### [0.6.2](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.1...v0.6.2) (2023-06-21)
 
 
 ### Bug Fixes
 
 * failure to determine location only goes to debug level ([#22](https://www.github.com/bihealth/clinvar-tsv/issues/22)) ([76bc510](https://www.github.com/bihealth/clinvar-tsv/commit/76bc5105e6f0b26146dcaca43465c1dd59d1aee2))
 * higher verbosity in Snakemake rules ([#26](https://www.github.com/bihealth/clinvar-tsv/issues/26)) ([a3fc327](https://www.github.com/bihealth/clinvar-tsv/commit/a3fc3271a8984b39d52c8852f6fe77b05b1193c0))
```

### Comparing `clinvar-tsv-0.6.2/clinvar_tsv.egg-info/SOURCES.txt` & `clinvar-tsv-0.6.3/clinvar_tsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/setup.cfg` & `clinvar-tsv-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/setup.py` & `clinvar-tsv-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/conftest.py` & `clinvar-tsv-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/clinvar-74722873.xml` & `clinvar-tsv-0.6.3/tests/data/clinvar-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/clinvar-92148661.xml` & `clinvar-tsv-0.6.3/tests/data/clinvar-92148661.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/clinvar-in-context-74722873.xml` & `clinvar-tsv-0.6.3/tests/data/clinvar-in-context-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/clinvar-spta1.xml` & `clinvar-tsv-0.6.3/tests/data/clinvar-spta1.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/parsed-74722873.37.tsv` & `clinvar-tsv-0.6.3/tests/data/parsed-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/parsed-in-context-74722873.37.tsv` & `clinvar-tsv-0.6.3/tests/data/parsed-in-context-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/data/parsed-spta1.37.tsv` & `clinvar-tsv-0.6.3/tests/data/parsed-spta1.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/test_merge_tsvs.py` & `clinvar-tsv-0.6.3/tests/test_merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/test_parse_xml_small.py` & `clinvar-tsv-0.6.3/tests/test_parse_xml_small.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/tests/test_parse_xml_sv.py` & `clinvar-tsv-0.6.3/tests/test_parse_xml_sv.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.2/versioneer.py` & `clinvar-tsv-0.6.3/versioneer.py`

 * *Files identical despite different names*

