# Comparing `tmp/bioat-0.1.5.4.tar.gz` & `tmp/bioat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.1.5.4.tar", max compression
+gzip compressed data, was "bioat-0.2.1.tar", max compression
```

## Comparing `bioat-0.1.5.4.tar` & `bioat-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.1.5.4/LICENSE
--rw-r--r--   0        0        0      852 2023-05-09 16:09:06.000000 bioat-0.1.5.4/README.md
--rw-r--r--   0        0        0     1112 2023-05-11 14:58:52.861266 bioat-0.1.5.4/pyproject.toml
--rw-r--r--   0        0        0      471 2023-04-01 11:15:49.201131 bioat-0.1.5.4/src/bioat/__init__.py
--rw-r--r--   0        0        0      508 2023-04-02 12:41:49.000000 bioat-0.1.5.4/src/bioat/about.py
--rw-r--r--   0        0        0    13627 2023-05-08 15:34:47.326510 bioat-0.1.5.4/src/bioat/bam.py
--rw-r--r--   0        0        0     1452 2023-05-11 14:31:32.618474 bioat-0.1.5.4/src/bioat/cli.py
--rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.1.5.4/src/bioat/detect_seq.py
--rw-r--r--   0        0        0       63 2022-10-12 10:34:44.000000 bioat-0.1.5.4/src/bioat/exceptions.py
--rw-r--r--   0        0        0    11016 2023-03-13 04:00:08.114588 bioat-0.1.5.4/src/bioat/fastx.py
--rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.1.5.4/src/bioat/genome.py
--rw-r--r--   0        0        0     5895 2023-04-10 17:00:56.000000 bioat-0.1.5.4/src/bioat/hic.py
--rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.1.5.4/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.1.5.4/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.1.5.4/src/bioat/lib/libalignment.py
--rwxr-xr-x   0        0        0    77022 2023-05-11 14:29:19.339453 bioat-0.1.5.4/src/bioat/lib/libcircos.py
--rw-r--r--   0        0        0     4439 2023-05-11 14:58:22.968190 bioat-0.1.5.4/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     6543 2023-04-13 15:00:50.900126 bioat-0.1.5.4/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.1.5.4/src/bioat/lib/libdetect_seq.py
--rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.1.5.4/src/bioat/lib/libplot.py
--rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.1.5.4/src/bioat/lib/libsnakemake.py
--rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.1.5.4/src/bioat/logger.py
--rw-r--r--   0        0        0      668 2023-04-07 16:11:22.000000 bioat-0.1.5.4/src/bioat/mgi.py
--rw-r--r--   0        0        0     5745 2023-05-07 15:13:15.000000 bioat-0.1.5.4/src/bioat/system.py
--rw-r--r--   0        0        0     3245 2023-04-07 08:00:16.234706 bioat-0.1.5.4/src/bioat/table.py
--rw-r--r--   0        0        0    27399 2023-04-13 16:49:11.000000 bioat-0.1.5.4/src/bioat/targeted_deep_sequencing.py
--rw-r--r--   0        0        0      384 2023-05-11 14:58:47.076113 bioat-0.1.5.4/src/bioat/version.py
--rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 bioat-0.1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.2.1/LICENSE
+-rw-r--r--   0        0        0      915 2023-05-26 06:22:16.476980 bioat-0.2.1/README.md
+-rw-r--r--   0        0        0     1115 2023-06-22 16:05:25.282500 bioat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      637 2023-06-22 06:29:42.769242 bioat-0.2.1/src/bioat/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-17 10:35:36.080629 bioat-0.2.1/src/bioat/__main__.py
+-rw-r--r--   0        0        0      508 2023-05-26 06:02:39.222570 bioat-0.2.1/src/bioat/about.py
+-rw-r--r--   0        0        0    13916 2023-06-17 12:05:22.520338 bioat-0.2.1/src/bioat/bamtools.py
+-rw-r--r--   0        0        0      738 2023-06-17 09:21:50.061008 bioat-0.2.1/src/bioat/bedtools.py
+-rw-r--r--   0        0        0     1833 2023-06-17 10:35:16.669568 bioat-0.2.1/src/bioat/cli.py
+-rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.2.1/src/bioat/detect_seq.py
+-rw-r--r--   0        0        0      151 2023-06-22 06:29:35.418689 bioat-0.2.1/src/bioat/exceptions.py
+-rw-r--r--   0        0        0    11024 2023-05-26 05:45:47.350133 bioat-0.2.1/src/bioat/fastxtools.py
+-rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.2.1/src/bioat/genome.py
+-rw-r--r--   0        0        0     5940 2023-06-17 09:21:44.490936 bioat-0.2.1/src/bioat/hictools.py
+-rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.2.1/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.2.1/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.2.1/src/bioat/lib/libalignment.py
+-rwxr-xr-x   0        0        0    77022 2023-05-11 14:29:19.339453 bioat-0.2.1/src/bioat/lib/libcircos.py
+-rw-r--r--   0        0        0     4458 2023-06-22 12:43:55.714188 bioat-0.2.1/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     6571 2023-06-17 09:16:08.912240 bioat-0.2.1/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0      793 2023-05-26 06:06:17.851659 bioat-0.2.1/src/bioat/lib/libdataclasses.py
+-rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.2.1/src/bioat/lib/libdetect_seq.py
+-rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.2.1/src/bioat/lib/libplot.py
+-rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.2.1/src/bioat/lib/libsnakemake.py
+-rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.2.1/src/bioat/logger.py
+-rw-r--r--   0        0        0      717 2023-06-17 09:22:39.495970 bioat-0.2.1/src/bioat/mgitools.py
+-rw-r--r--   0        0        0     5748 2023-05-26 05:47:35.184115 bioat-0.2.1/src/bioat/systemtools.py
+-rw-r--r--   0        0        0     3280 2023-06-17 09:26:06.543411 bioat-0.2.1/src/bioat/tabletools.py
+-rw-r--r--   0        0        0    81594 2023-06-22 15:47:38.145193 bioat-0.2.1/src/bioat/target_seq.py
+-rw-r--r--   0        0        0      519 2023-06-22 16:04:13.593669 bioat-0.2.1/src/bioat/version.py
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 bioat-0.2.1/PKG-INFO
```

### Comparing `bioat-0.1.5.4/LICENSE` & `bioat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/README.md` & `bioat-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 > author: [赵华男 | ZHAO Hua-nan](https://scholar.google.com/citations?user=ojSVoWQAAAAJ&hl=en)
 >
 > email: hermanzhaozzzz@gmail.com
 >
 > [Zhihu](https://www.zhihu.com/people/hymanzhaozzzz) | [BLOG](http://zhaohuanan.cc)
 
 ## Introduction
-A python command line toolkit for Bioinformatics and data science!
+A python **package** & **command line toolkit** for Bioinformatics and data science!
 
-**\<under development\>**
+**\<under development\>!!**
 
 ## Installation
 ```shell
 # supported platform: Linux / MacOS (intel & arm64) / WSL on Windows
 pip install --upgrade bioat
 ```
 
@@ -28,10 +28,11 @@
 # check information about bioat
 bioat about
 
 # example usage
 bioat bam remove_clip --help
 samtools view -h test_sorted_n.bam | bioat bam remove_clip | tail
 ```
+[circos plot](docs/demo_circos-plot.ipynb)
 
 ## known trouble
 - sometimes, pysam dependent foo.lib can be absent, just `brew install foo.lib` to fix it.
```

### Comparing `bioat-0.1.5.4/pyproject.toml` & `bioat-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioat"
-version = "0.1.5.4"
+version = "0.2.1"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 homepage = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 # README file(s) are used as the package description
 readme = "README.md"
@@ -23,15 +23,15 @@
 pandarallel = "^1.6.4"
 matplotlib = "^3.7.1"
 tabulate = "^0.9.0"
 scipy = "^1.8.0"
 statsmodels = "^0.13.5"
 
 [tool.poetry.scripts]
-bioat = "bioat.cli:main"
+bioat = "bioat.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
 
 # ...and can be installed only when explicitly requested
 [tool.poetry.group.docs]
```

### Comparing `bioat-0.1.5.4/src/bioat/bam.py` & `bioat-0.2.1/src/bioat/bamtools.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,27 @@
 import logging
 import gzip
 import os
 import sys
 import string
 import random
 import pysam
+from io import TextIOWrapper
 from multiprocessing import Process
+from signal import signal, SIGPIPE, SIG_DFL
 from bioat.logger import set_logging_level
 
+# from bioat.lib.libdataclasses import Bam
+
+signal(SIGPIPE, SIG_DFL)
+
+
+class BamTools:
+    """Bam toolbox."""
 
-class Bam:
     def __init__(self):
         pass
 
     def mpileup_to_table(
             self,
             mpileup: str,
             output: str = sys.stdout,
@@ -153,28 +161,28 @@
         # merge output files
         logger.debug("Merging files...")
         _merge_out_bmat(temp_filename_list=temp_filename_list, output=output, remove_temp=remove_temp)
         logger.debug("Done!...")
 
     def remove_clip(
             self,
-            input: str = 'stdin',
-            output: str = 'stdout',
+            input: str = sys.stdin,
+            output: str = sys.stdout,
             threads: int = 1,
             output_fmt: str = 'SAM',
             remove_as_paired: bool = True,
             max_clip: int = 0,
             log_level: str = 'INFO'
     ):
         """Remove softclip reads in BAM file.
 
-        :param input: BAM file sorted by coordinate with soft/hard clip reads, pipe stdin is supported
+        :param input: BAM file sorted by queryname with soft/hard clip reads, pipe stdin is supported
 
                         [samtools view -h foo_sort_name.bam | bioat bam remove_clip <flags>]
-        :param output: BAM file sorted by coordinate without soft/hard clip reads, pipe stdout is supported
+        :param output: BAM file sorted by queryname without soft/hard clip reads, pipe stdout is supported
 
                         [bioat bam remove_clip <flags> | wc -l]
                         [bioat bam remove_clip <flags> | samtools view ....]
         :param threads: threads used by pysam and samtools core
         :param output_format: BAM, SAM
         :param remove_as_paired: True, False. remove single clip(False) / clip and its pair read(True)
         :param max_clip: the maximum clips allowed per read
@@ -182,22 +190,23 @@
         """
         set_logging_level(level=log_level)
         # set logger
         lib_name = __name__
         function_name = sys._getframe().f_code.co_name
         logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
 
-        if sys.stdin.isatty():  # not stdin
+        save = pysam.set_verbosity(0)  # https://github.com/pysam-developers/pysam/issues/939
+
+        if isinstance(input, str):  # not stdin
             bam_in = pysam.AlignmentFile(input, "r", threads=threads, check_sq=False)
-        else:  # stdin
+        elif isinstance(input, TextIOWrapper):  # stdin
             bam_in = pysam.AlignmentFile("-", "r", threads=threads, check_sq=False)
-
-        # fix output
-        if output == 'stdout':
-            output = sys.stdout
+        else:
+            exit(1)
+        pysam.set_verbosity(save)
 
         try:
             so = bam_in.header['HD']['SO']
         except KeyError:
             so = None
 
         if so:
```

### Comparing `bioat-0.1.5.4/src/bioat/detect_seq.py` & `bioat-0.2.1/src/bioat/detect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/fastx.py` & `bioat-0.2.1/src/bioat/fastxtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 import gzip
 import sys
 from Bio import SeqIO
 from tqdm import tqdm
 
-class Fastx():
+class FastxTools:
     def __init__(self, file=None, iterable=True):
         self.file = file
         self.iterable = iterable
         self.fastx = None
 
     # def __load_fastx_list(self) -> list:
     #     """
@@ -295,9 +295,9 @@
                 continue
             else:
                 f.write('\n'.join(read) + '\n')
         f.close()
 
 
 if __name__ == '__main__':
-    # fastx = Fastx(file='../../data/random_l-180_n-100_hg38_minus-test.fa')
+    # fastx = FastxTools(file='../../data/random_l-180_n-100_hg38_minus-test.fa')
     pass
```

### Comparing `bioat-0.1.5.4/src/bioat/genome.py` & `bioat-0.2.1/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/hic.py` & `bioat-0.2.1/src/bioat/hictools.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     pandarallel.initialize(
         progress_bar=False,
         use_memory_fs=False,
         verbose=1
     )
 
 
-class HiC:
+class HiCTools:
+    """Hi-C toolbox."""
+
     def __init__(self):
         pass
 
     @profile
     def get_effective_resolutions(
             self,
             genome_index,
@@ -35,15 +37,15 @@
             log_level: str = 'INFO'
     ):
         """Get deepest resolution of cis-interation.
 
         输入为result文件，输出为matrix的大致resolution.
 
         :param genome_index: genome.fa.fai
-        :param valid_pairs: rm_dup_pairs.allValidPairs by HiC-Pro
+        :param valid_pairs: rm_dup_pairs.allValidPairs by HiCTools-Pro
         :param output: table_output, TSV file
         :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
         """
         set_logging_level(level=log_level)
         # set logger
         lib_name = __name__
         function_name = sys._getframe().f_code.co_name
@@ -53,15 +55,15 @@
         df_chromosome = pd.read_csv(
             genome_index,
             sep='\t',
             usecols=[0, 1],
             names=['chromosome', 'length'],
             index_col='chromosome',
         )
-        # load sample valid pairs by HiC-Pro after remove duplication and filter.
+        # load sample valid pairs by HiCTools-Pro after remove duplication and filter.
         reader = pd.read_csv(
             valid_pairs,
             sep='\t',
             header=None,
             names=[
                 'read_name', 'chr_A', 'start_A', 'strand_A', 'chr_B', 'start_B', 'strand_B', 'insert_size',
                 'fragment_name_A', 'fragment_name_B', 'mapQ_A', 'mapQ_B', 'allele_specific_info'
@@ -148,15 +150,15 @@
             del s_bin_idx_count1, s_bin_idx_count2, df_bin_interaction_count
             gc.collect()
         output.close()
 
 
 if __name__ == '__main__':
     a = time.time()
-    hic = HiC()
+    hic = HiCTools()
     hic.get_effective_resolutions(
         genome_index="/Volumes/zhaohn_HD/Bio/1.database/db_genomes/genome_fa/genome_ucsc_hg38/genome_ucsc_hg38.fa.fai",
         valid_pairs="../../data/hic/test.rm_dup_pairs.allValidPairs",
         output="/Users/zhaohuanan/Downloads/testout"
     )
     a = time.time() - a
     # print(f'\n{a:.3f}s')
```

### Comparing `bioat-0.1.5.4/src/bioat/lib/_dev_tools.py` & `bioat-0.2.1/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/lib/libalignment.py` & `bioat-0.2.1/src/bioat/lib/libalignment.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/lib/libcircos.py` & `bioat-0.2.1/src/bioat/lib/libcircos.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/lib/libcolor.py` & `bioat-0.2.1/src/bioat/lib/libcolor.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,27 +119,28 @@
         <color_list>
     """
     # set logger
     lib_name = __name__
     function_name = sys._getframe().f_code.co_name
     logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
 
-    supported_fmt = ('HEX', 'RGB')
     return_fmt = return_fmt.upper()
+    supported_fmt = ('HEX', 'RGB')
+
     if return_fmt not in supported_fmt:
         logger.critical(
             f'not supported color format: {return_fmt}\n'
             f'supported_fmt = {supported_fmt}'
         )
     low_color = np.array(low_color_RGB)
     high_color = np.array(high_color_RGB)
 
     color_list = []
     for index in range(0, length_out + 1):
-        rgb_color = low_color + (high_color - low_color) // length_out * index
+        rgb_color = [abs(i) for i in low_color + (high_color - low_color) // length_out * index]
         if return_fmt == "HEX":
             color_list.append(convert_rgb_to_hex(tuple(rgb_color)))
         else:
             color_list.append(tuple(rgb_color))
 
     return color_list
```

### Comparing `bioat-0.1.5.4/src/bioat/lib/libcrispr.py` & `bioat-0.2.1/src/bioat/lib/libcrispr.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import sys
 
 import pandas as pd
 from Bio.Seq import Seq
 from Bio.Align import PairwiseAligner
 from bioat.lib.libalignment import get_alignment_info
 
-"""TARGET_REGIONS_LIB.
+# TARGET_REGIONS_LIB
+#     for target_seq alignment
+#
+# bioat target_seq region_heatmap test_sorted.mpileup.info.tsv test.pdf --get_built_in_target_region
+#
+# INFO:root:You can use <key> in built-in <target_regions> to represent your target_region:
+#         <key>   <target_region>
+#         EMX1    GAGTCCGAGCAGAAGAAGAA^NGG^
+#         HEK3    GGCCCAGACTGAGCACGTGA^NGG^
+#         HEK4    GGCACTGCGGCTGGAGGTGG^NGG^
+#         ...
 
-bioat targeted_deep_sequencing region_heatmap test_sorted.mpileup.info.tsv test.pdf --get_built_in_target_region
-
-INFO:root:You can use <key> in built-in <target_regions> to represent your target_region:
-        <key>   <target_region>
-        EMX1    GAGTCCGAGCAGAAGAAGAA^NGG^
-        HEK3    GGCCCAGACTGAGCACGTGA^NGG^
-        HEK4    GGCACTGCGGCTGGAGGTGG^NGG^
-        ...
-"""
 TARGET_SEQ_LIB = {
     "EMX1": "GAGTCCGAGCAGAAGAAGAA^NGG^",
     "HEK3": "GGCCCAGACTGAGCACGTGA^NGG^",
     "HEK4": "GGCACTGCGGCTGGAGGTGG^NGG^",
     "RNF2": "GTCATCTTAGTCATTACCTG^NGG^",
     "VEGFA": "GACCCCCTCCACCCCGCCTC^NGG^",
     "CDKN2A": "^TTTA^GCCCCAATAATCCCCACATGTCA",
```

### Comparing `bioat-0.1.5.4/src/bioat/lib/libdetect_seq.py` & `bioat-0.2.1/src/bioat/lib/libdetect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/lib/libplot.py` & `bioat-0.2.1/src/bioat/lib/libplot.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/logger.py` & `bioat-0.2.1/src/bioat/logger.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.4/src/bioat/mgi.py` & `bioat-0.2.1/src/bioat/mgitools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd
 
 
-class Mgi():
+class MgiTools():
+    """Raw MGI sequencing data toolbox."""
+
     def __init__(self):
         pass
 
     def parse_md5(self, file: str):
         """Read mgi-like md5 file and convert to a normal md5 file.
 
         :param file: file name of a mgi-like md5 file.
```

### Comparing `bioat-0.1.5.4/src/bioat/system.py` & `bioat-0.2.1/src/bioat/systemtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import
 # from bioat.api.internet_speed import main as speedtest
 
 
-class System():
+class SystemTools:
     def __init__(self):
         # self.test_internet_speed = speedtest()
         pass
 
 #     def __convert_size(self, size, mode='b') -> float:
 #         """将单位为Byte的数字转为其它单位
 #
```

### Comparing `bioat-0.1.5.4/src/bioat/table.py` & `bioat-0.2.1/src/bioat/tabletools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sys
 import pandas as pd
 
 
-class Table():
+class TableTools:
+    """To integrate tables."""
+
     def __init__(self):
         pass
 
     def merge(
             self,
             inputs,
             tags,
```

### Comparing `bioat-0.1.5.4/PKG-INFO` & `bioat-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.1.5.4
+Version: 0.2.1
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
 Requires-Python: >=3.8.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -33,17 +33,17 @@
 > author: [赵华男 | ZHAO Hua-nan](https://scholar.google.com/citations?user=ojSVoWQAAAAJ&hl=en)
 >
 > email: hermanzhaozzzz@gmail.com
 >
 > [Zhihu](https://www.zhihu.com/people/hymanzhaozzzz) | [BLOG](http://zhaohuanan.cc)
 
 ## Introduction
-A python command line toolkit for Bioinformatics and data science!
+A python **package** & **command line toolkit** for Bioinformatics and data science!
 
-**\<under development\>**
+**\<under development\>!!**
 
 ## Installation
 ```shell
 # supported platform: Linux / MacOS (intel & arm64) / WSL on Windows
 pip install --upgrade bioat
 ```
 
@@ -57,11 +57,12 @@
 # check information about bioat
 bioat about
 
 # example usage
 bioat bam remove_clip --help
 samtools view -h test_sorted_n.bam | bioat bam remove_clip | tail
 ```
+[circos plot](docs/demo_circos-plot.ipynb)
 
 ## known trouble
 - sometimes, pysam dependent foo.lib can be absent, just `brew install foo.lib` to fix it.
```

