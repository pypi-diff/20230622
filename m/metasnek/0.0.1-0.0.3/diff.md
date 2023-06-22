# Comparing `tmp/metasnek-0.0.1.tar.gz` & `tmp/metasnek-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasnek-0.0.1.tar", last modified: Tue Jun 13 02:54:04 2023, max compression
+gzip compressed data, was "metasnek-0.0.3.tar", last modified: Thu Jun 22 01:31:22 2023, max compression
```

## Comparing `metasnek-0.0.1.tar` & `metasnek-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:54:04.472032 metasnek-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 02:53:52.000000 metasnek-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 02:53:52.000000 metasnek-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 02:54:04.472032 metasnek-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 02:53:52.000000 metasnek-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 02:53:52.000000 metasnek-0.0.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:54:04.472032 metasnek-0.0.1/metasnek/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-13 02:53:52.000000 metasnek-0.0.1/metasnek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-06-13 02:53:52.000000 metasnek-0.0.1/metasnek/fastq_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:54:04.472032 metasnek-0.0.1/metasnek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 02:54:04.000000 metasnek-0.0.1/metasnek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 02:54:04.000000 metasnek-0.0.1/metasnek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:54:04.000000 metasnek-0.0.1/metasnek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 02:54:04.000000 metasnek-0.0.1/metasnek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:54:04.472032 metasnek-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-13 02:53:52.000000 metasnek-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 01:31:13.000000 metasnek-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 01:31:13.000000 metasnek-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-22 01:31:22.862733 metasnek-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-22 01:31:13.000000 metasnek-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 01:31:13.000000 metasnek-0.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/metasnek/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 01:31:13.000000 metasnek-0.0.3/metasnek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-22 01:31:13.000000 metasnek-0.0.3/metasnek/fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/metasnek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:31:22.862733 metasnek-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-22 01:31:13.000000 metasnek-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-22 01:31:13.000000 metasnek-0.0.3/tests/test_fastq_finder.py
```

### Comparing `metasnek-0.0.1/LICENSE` & `metasnek-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.1/metasnek/fastq_finder.py` & `metasnek-0.0.3/metasnek/fastq_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 import glob
 import csv
 import re
 
 
 def parse_directory(file_list):
     """Pairs samples from a list of files.
@@ -10,43 +11,43 @@
     Args:
         file_list (list): A list of file paths.
 
     Returns:
         tuple: A tuple containing two sets:
             - paired_files: A set of tuples with the sample name, unpaired file path, and paired file path.
             - unpaired_files: A set of tuples with the sample name and unpaired file path.
-
     """
 
     paired_files = set()
     unpaired_files = set()
 
     for file in file_list:
         file_path, file_ext = os.path.splitext(file)
-        file_name = os.path.basename(file_path)
+        file_name = os.path.basename(file)
         file_ext = file_ext.lower()
 
         pattern = r"\.(fasta|fastq)(\.gz)?$"
-        if re.search(pattern,file_name,re.IGNORECASE):
-            paired_file = None
-            unpaired_file = None
-            sample_name = None
+        if re.search(pattern, file_name, re.IGNORECASE):
+            R1_file = None
+            R2_file = None
 
             if "_R1" in file_name:
                 sample_name = file_name.rsplit("_R1", 1)[0]
-                paired_file = file_path.replace("_R1", "_R2") + file_ext
-                unpaired_file = file
+                R2_file = file_path.replace("_R1", "_R2") + file_ext
+                R1_file = file
             elif "_R2" in file_name:
                 sample_name = file_name.rsplit("_R2", 1)[0]
-                unpaired_file = file_path.replace("_R2", "_R1") + file_ext
-                paired_file = file
-
-            if paired_file and paired_file in file_list:
-                paired_files.add((sample_name, unpaired_file, paired_file))
+                R1_file = file_path.replace("_R2", "_R1") + file_ext
+                R2_file = file
+            if R1_file and R2_file and R1_file in file_list and R2_file in file_list:
+                paired_files.add((sample_name, R1_file, R2_file))
             else:
+                sample_name = re.split(r"\.(fasta|fastq)(\.gz)?$", file_name)[0]
+                if "_R1" in sample_name or "_R2" in sample_name:
+                    warnings.warn(f"Orphaned paired read detected: {file_name}", Warning)
                 unpaired_files.add((sample_name, file))
 
     return paired_files, unpaired_files
 
 
 def parse_tsv_file(file_path):
     """Parses a 3-column TSV file of sample names and sequencing reads (column 3 is optional)
@@ -54,15 +55,14 @@
     Args:
         file_path (str): Path to the TSV file.
 
     Returns:
         tuple: A tuple containing two lists:
             - paired_reads: A list of tuples with the sample name, R1 file, and R2 file (if available).
             - unpaired_reads: A list of tuples with the sample name and R1 file (for unpaired reads).
-
     """
 
     paired_reads = set()
     unpaired_reads = set()
 
     with open(file_path, 'r') as tsv_file:
         reader = csv.reader(tsv_file, delimiter='\t')
@@ -119,16 +119,18 @@
     """Converts paired and unpaired reads to a single dictionary.
 
     Args:
         paired_reads (set): A list of tuples with sample name, R1 file, and R2 file (if available).
         unpaired_reads (set): A list of tuples with sample name and R1 file (for unpaired reads).
 
     Returns:
-        dict: A dictionary containing the sample name as the key and a dictionary with 'R1' and 'R2' keys.
-
+        dict:
+            - sample name (dict):
+                - R1 (str): filepath of R1 reads file
+                - R2 (str): filepath of R2 reads file or None for unpaired
     """
 
     reads_dictionary = {}
 
     for sample_name, r1_file, r2_file in paired_reads:
         if sample_name not in reads_dictionary:
             reads_dictionary[sample_name] = {'R1': r1_file, 'R2': r2_file}
@@ -157,21 +159,17 @@
     return sample_dictionary
 
 
 def write_samples_tsv(dictionary, output_file):
     """Write the samples dictionary to a TSV file
 
     Args:
-        dictionary (dict):
-             - key (str): sample name
-             - value (dict):
-                - R1 (str): filepath of R1 file
-                - R2 (str): filepath of R2 file, or None for unpaired reads
+        dictionary:
+            - sample name (dict):
+                - R1 (str): filepath of R1 reads file
+                - R2 (str): filepath of R2 reads file or None for unpaired
         output_file (str): filepath of output file for writing
-
-    Returns:
-
     """
 
     with open(output_file, "w") as out:
         for sample in dictionary.keys():
             out.write(f"{sample}\t{dictionary[sample]['R1']}\t{dictionary[sample]['R2']}\n")
```

### Comparing `metasnek-0.0.1/setup.py` & `metasnek-0.0.3/setup.py`

 * *Files identical despite different names*

