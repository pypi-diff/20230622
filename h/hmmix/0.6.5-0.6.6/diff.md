# Comparing `tmp/hmmix-0.6.5.tar.gz` & `tmp/hmmix-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmix-0.6.5.tar", last modified: Mon Feb 27 21:30:38 2023, max compression
+gzip compressed data, was "dist/hmmix-0.6.6.tar", last modified: Thu Jun 22 21:00:18 2023, max compression
```

## Comparing `hmmix-0.6.5.tar` & `hmmix-0.6.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-02-27 21:30:38.780398 hmmix-0.6.5/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.6.5/LICENSE.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-02-27 21:30:38.776398 hmmix-0.6.5/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34092 2023-02-27 21:20:22.000000 hmmix-0.6.5/README.md
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2023-02-27 21:30:38.780398 hmmix-0.6.5/setup.cfg
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2023-02-27 21:25:36.000000 hmmix-0.6.5/setup.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-02-27 21:30:38.776398 hmmix-0.6.5/src/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8853 2022-10-25 01:10:48.000000 hmmix-0.6.5/src/bcf_vcf.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    15167 2022-10-25 01:10:13.000000 hmmix-0.6.5/src/helper_functions.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    13669 2023-02-27 21:19:11.000000 hmmix-0.6.5/src/hmm_functions.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-02-27 21:30:38.776398 hmmix-0.6.5/src/hmmix.egg-info/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/SOURCES.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/dependency_links.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       37 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/entry_points.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/requires.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2023-02-27 21:30:38.000000 hmmix-0.6.5/src/hmmix.egg-info/top_level.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    16030 2023-02-27 21:25:43.000000 hmmix-0.6.5/src/main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.6.5/src/make_mutationrate.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4281 2022-10-25 01:10:46.000000 hmmix-0.6.5/src/make_test_data.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-02-27 21:30:38.776398 hmmix-0.6.5/test/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2725 2022-05-26 04:20:02.000000 hmmix-0.6.5/test/test.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.6.5/test/test2.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.6.5/test/test_main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.6.5/test/testfred.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.6.6/LICENSE.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-22 21:00:18.000000 hmmix-0.6.6/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34092 2023-02-27 21:20:22.000000 hmmix-0.6.6/README.md
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2023-06-22 21:00:18.000000 hmmix-0.6.6/setup.cfg
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2023-06-22 19:56:41.000000 hmmix-0.6.6/setup.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2023-06-22 20:59:26.000000 hmmix-0.6.6/src/bcf_vcf.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    15245 2023-06-22 20:45:50.000000 hmmix-0.6.6/src/helper_functions.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    13669 2023-03-03 06:04:46.000000 hmmix-0.6.6/src/hmm_functions.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34626 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/entry_points.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/requires.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2023-06-22 21:00:18.000000 hmmix-0.6.6/src/hmmix.egg-info/top_level.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    16030 2023-06-22 20:45:54.000000 hmmix-0.6.6/src/main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.6.6/src/make_mutationrate.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4281 2022-10-25 01:10:46.000000 hmmix-0.6.6/src/make_test_data.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-06-22 21:00:18.000000 hmmix-0.6.6/test/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2725 2022-05-26 04:20:02.000000 hmmix-0.6.6/test/test.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.6.6/test/test2.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.6.6/test/test_main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.6.6/test/testfred.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hmmix-0.6.5/LICENSE.txt` & `hmmix-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/PKG-INFO` & `hmmix-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.6.5
+Version: 0.6.6
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hmmix-0.6.5/README.md` & `hmmix-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/setup.py` & `hmmix-0.6.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='hmmix', 
-    version = '0.6.5',
+    version = '0.6.6',
     description='Find introgressed segments',
     py_modules=['bcf_vcf', 'helper_functions', 'hmm_functions', 'main', 'make_mutationrate', 'make_test_data'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `hmmix-0.6.5/src/bcf_vcf.py` & `hmmix-0.6.6/src/bcf_vcf.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
             # If reference genome is provided then remove positions where the reference and ancestral differ AND which is not found in the outgroup
             if reffile is not None and ancestralfile is not None:
                 print('Find fixed derived sites')
                 refgenome_allele = load_fasta(reffile)
 
                 for index, (refbase, ancbase) in enumerate(zip(refgenome_allele, ancestral_allele)):
-                    if ancbase in 'ACGT' and refbase in 'ACGT':
+                    if ancbase in ['A','C','G','T']  and refbase in ['A','C','G','T'] :
                         if refbase != ancbase and variants_seen[index] == 0:
                             print(chrom, index + 1, f'{refbase}:100', f'{ancbase}:0', ancbase, sep = '\t', file = out)
 
     # Sort outgroup file
     print('Sorting outgroup file')
     positions_to_sort = defaultdict(lambda: defaultdict(str))
     with open(outputfile + '.unsorted') as data, open(outputfile, 'w') as out:
@@ -124,53 +124,48 @@
 
     for vcffile, ancestralfile in zip(vcffiles, ancestralfiles):
 
         if ancestralfile is not None:
             ancestral_allele = load_fasta(ancestralfile)
 
         if bedfile is not None:
-            command = f'bcftools view -m2 -M2 -v snps -s {individuals_for_bcf} -T {bedfile} {vcffile} | vcftools --vcf - --exclude-positions {outgroupfile} --recode --stdout'
+            command = f'bcftools view -v snps -s {individuals_for_bcf} -T {bedfile} {vcffile} | bcftools norm -m +any | vcftools --vcf - --exclude-positions {outgroupfile} --recode --stdout'
         else:
-            command = f'bcftools view -m2 -M2 -v snps -s {individuals_for_bcf} {vcffile} | vcftools --vcf - --exclude-positions {outgroupfile} --recode --stdout'
+            command = f'bcftools view -v snps -s {individuals_for_bcf} {vcffile} | bcftools norm -m +any | vcftools --vcf - --exclude-positions {outgroupfile} --recode --stdout'
 
         print('Running command:')
         print(command, '\n\n')
 
         for index, line in enumerate(os.popen(command)):
 
             if line.startswith('#CHROM'):
                 individuals_in_vcffile = line.strip().split()[9:]
 
             if not line.startswith('#'):
 
                 chrom, pos, _, ref_allele, alt_allele = line.strip().split()[0:5]
                 pos = int(pos)
                 genotypes = [x.split(':')[0] for x in line.strip().split()[9:]]
+                all_bases = [ref_allele] + alt_allele.split(',')
 
-                if ref_allele in 'ACGT' and alt_allele in 'ACGT':
+                if ref_allele in ['A','C','G','T']:
 
-                    for original_genotype, individual in zip(genotypes, individuals_in_vcffile):
-                        ref_count = original_genotype.count('0')
-                        alt_count = original_genotype.count('1')     
-                        genotype = convert_to_bases(original_genotype, ref_allele, alt_allele)   
+                    for original_genotype, individual in zip(genotypes, individuals_in_vcffile):  
+                        genotype = convert_to_bases(original_genotype, all_bases)   
 
                         if ancestralfile is not None:
                             # With ancestral information look for derived alleles
                             ancestral_base = ancestral_allele[pos-1]
-                            if ancestral_base in [ref_allele, alt_allele]:
-
-                                derived_count = genotype.count(alt_allele) if ancestral_base == ref_allele else genotype.count(ref_allele)
-                                if derived_count > 0:
-                                    print(chrom, pos, ancestral_base, genotype, sep = '\t', file = outfile_handler[individual])
+                            if ancestral_base in all_bases and genotype.count(ancestral_base) != 2 and genotype != 'NN':
+                                print(chrom, pos, ancestral_base, genotype, sep = '\t', file = outfile_handler[individual])
 
                         else:
                             # If no ancestral information is provided only include heterozygous variants
-                            if alt_count * ref_count > 0:
-                                ancestral_base = ref_allele
-                                print(chrom, pos, ancestral_base, genotype, sep = '\t', file = outfile_handler[individual])
+                            if genotype[0] != genotype[1]:
+                                print(chrom, pos, ref_allele, genotype, sep = '\t', file = outfile_handler[individual])
                 
 
                 if index % 100000 == 0:
                     print(f'at line {index} at chrom {chrom} and position {pos}')
 
     # Clean log files generated by vcf and bcf tools
     clean_files('out.log')
```

### Comparing `hmmix-0.6.5/src/helper_functions.py` & `hmmix-0.6.6/src/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,27 +338,28 @@
                     flattened_list.append(position)
             else:
                 flattened_list.append(bin)
 
     return ','.join(flattened_list)
 
 
-def convert_to_bases(genotype, ref, alt):
+def convert_to_bases(genotype, both_bases):
 
     return_genotype = 'NN'
-    both_bases = ref + alt
-
     separator = None
+    
     if '/' in genotype or '|' in genotype:
         separator = '|' if '|' in genotype else '/'
-    
+
         base1, base2 = [x for x in genotype.split(separator)]
         if base1.isnumeric() and base2.isnumeric():
             base1, base2 = int(base1), int(base2)
-            return_genotype = both_bases[base1] + both_bases[base2]
+
+            if both_bases[base1] in ['A','C','G','T'] and both_bases[base2] in ['A','C','G','T']:
+                return_genotype = both_bases[base1] + both_bases[base2]
 
     return return_genotype
 
 
 
 
 # Check which type of input we are dealing with
```

### Comparing `hmmix-0.6.5/src/hmm_functions.py` & `hmmix-0.6.6/src/hmm_functions.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/src/hmmix.egg-info/PKG-INFO` & `hmmix-0.6.6/src/hmmix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.6.5
+Version: 0.6.6
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hmmix-0.6.5/src/main.py` & `hmmix-0.6.6/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output
 from bcf_vcf import make_out_group, make_ingroup_obs
 from make_test_data import create_test_data
 from make_mutationrate import make_mutation_rate
 from helper_functions import Load_observations_weights_mutrates, handle_individuals_input, handle_infiles, combined_files
 
 
-VERSION = '0.6.5'
+VERSION = '0.6.6'
 
 
 def print_script_usage():
     toprint = f'''
 Script for identifying introgressed archaic segments (version: {VERSION})
 
 > Turorial:
```

### Comparing `hmmix-0.6.5/src/make_mutationrate.py` & `hmmix-0.6.6/src/make_mutationrate.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/src/make_test_data.py` & `hmmix-0.6.6/src/make_test_data.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/test/test.py` & `hmmix-0.6.6/test/test.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/test/test2.py` & `hmmix-0.6.6/test/test2.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.5/test/test_main.py` & `hmmix-0.6.6/test/test_main.py`

 * *Files identical despite different names*

