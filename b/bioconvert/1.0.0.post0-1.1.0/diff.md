# Comparing `tmp/bioconvert-1.0.0.post0.tar.gz` & `tmp/bioconvert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioconvert-1.0.0.post0.tar", last modified: Tue Feb 21 18:16:57 2023, max compression
+gzip compressed data, was "bioconvert-1.1.0.tar", last modified: Thu Jun 22 15:10:42 2023, max compression
```

## Comparing `bioconvert-1.0.0.post0.tar` & `bioconvert-1.1.0.tar`

### file list

```diff
@@ -1,190 +1,343 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.734732 bioconvert-1.0.0.post0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1744 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/CONTRIBUTING.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    35141 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/COPYING
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      186 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    52931 2023-02-21 18:16:57.734732 bioconvert-1.0.0.post0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    46967 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/README.rst
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.727733 bioconvert-1.0.0.post0/bioconvert/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2238 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2918 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/abi2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2905 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/abi2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3310 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/abi2qual.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4394 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2bedgraph.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4320 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2bigwig.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3516 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2cov.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3831 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2cram.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6110 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8180 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/bam2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2817 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2json.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3970 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2sam.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3814 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2tsv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2727 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bam2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2940 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bcf2vcf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2754 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bcf2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2744 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bed2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3486 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bedgraph2bigwig.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3337 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bedgraph2cov.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2965 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bedgraph2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3457 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bigbed2bed.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3238 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bigbed2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3676 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bigwig2bedgraph.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2767 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bigwig2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3501 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bplink2plink.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3650 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bplink2vcf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3144 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/bz22gz.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3860 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/clustal2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3092 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/clustal2nexus.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3469 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/clustal2phylip.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3473 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/clustal2stockholm.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.729732 bioconvert-1.0.0.post0/bioconvert/core/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       43 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    24853 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/base.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10010 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/benchmark.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8102 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/converter.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10559 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/decorators.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2950 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/downloader.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4759 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/extensions.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11085 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/graph.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5000 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/init.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3786 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/levenshtein.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16130 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/registry.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3754 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/shell.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5587 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/core/utils.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3828 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/cram2bam.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5079 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/cram2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6151 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/cram2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3843 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/cram2sam.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5244 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/csv2tsv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4379 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/csv2xls.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.730733 bioconvert-1.0.0.post0/bioconvert/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1963 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       11 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/measles.chrom.sizes
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    25805 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/test.bigwig
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8903 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/test_SP1.fq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    15096 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/test_gfa2fasta_v1.gfa
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       20 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/test_measles.fa.fai
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6569 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/test_measles.sorted.bam
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.730733 bioconvert-1.0.0.post0/bioconvert/data/testing/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/data/testing/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3116 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/dsrc2gz.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3101 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/embl2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3105 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/embl2genbank.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3841 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2clustal.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4531 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2faa.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10893 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2fasta_agp.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3555 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5370 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2genbank.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3094 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2nexus.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4321 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2phylip.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2903 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta2twobit.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4054 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fasta_qual2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11228 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fastq2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4862 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fastq2fasta_qual.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4143 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/fastq2qual.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2979 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/genbank2embl.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4185 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/genbank2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2661 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/genbank2gff3.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4339 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gfa2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4289 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gff22gff3.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4245 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gff32gff2.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2566 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gff32gtf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3682 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gtf22gff3.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3783 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gz2bz2.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3303 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/gz2dsrc.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.730733 bioconvert-1.0.0.post0/bioconvert/io/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2801 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    19075 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/genbank.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4397 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/gff2.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4953 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/gff3.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9578 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/maf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9215 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/io/scf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3032 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/json2yaml.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2966 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/maf2sam.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.731732 bioconvert-1.0.0.post0/bioconvert/misc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      176 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1212 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/cython_fastq2fasta.pyx
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3352 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/fastq2fasta.c
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      622 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/fastq2fasta.pl
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2134 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/install_goalign.sh
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2132 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/misc/install_gotree.sh
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2940 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/newick2nexus.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3012 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/newick2phyloxml.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4030 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/nexus2clustal.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6113 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/nexus2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3442 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/nexus2newick.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2992 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/nexus2phylip.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3003 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/nexus2phyloxml.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3928 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/ods2csv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3894 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/pdb2faa.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3359 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phylip2clustal.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3973 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phylip2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2943 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phylip2nexus.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3444 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phylip2stockholm.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2984 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phylip2xmfa.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2985 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phyloxml2newick.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2953 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/phyloxml2nexus.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2957 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/plink2bplink.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3111 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/plink2vcf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2851 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/sam2bam.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3985 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/sam2cram.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14907 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/sam2paf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4962 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scf2fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5272 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scf2fastq.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.731732 bioconvert-1.0.0.post0/bioconvert/scripts/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scripts/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    23292 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scripts/converter.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2591 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scripts/init_convert.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4159 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/scripts/stats.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.731732 bioconvert-1.0.0.post0/bioconvert/simulator/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/simulator/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2541 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/simulator/fasta.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2329 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/simulator/fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2155 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/simulator/gfa.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4676 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/sra2fastq.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3407 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/stockholm2clustal.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3418 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/stockholm2phylip.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5240 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/tsv2csv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3423 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/twobit2fasta.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.731732 bioconvert-1.0.0.post0/bioconvert/utils/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/utils/__init__.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.732732 bioconvert-1.0.0.post0/bioconvert/utils/biocode/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    19802 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/annotation.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9639 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/convert_genbank_to_gff3.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    31129 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/gff.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10518 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/tbl.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    58309 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/things.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     7989 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/utils/biocode/utils.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3273 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/vcf2bcf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2846 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/vcf2bed.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2936 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/vcf2bplink.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2992 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/vcf2plink.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2685 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/vcf2wiggle.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2707 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/wig2bed.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5078 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/xls2csv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5103 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/bioconvert/xlsx2csv.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2950 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/xmfa2phylip.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3186 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/bioconvert/yaml2json.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.728732 bioconvert-1.0.0.post0/bioconvert.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    52931 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4700 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      170 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-02-21 17:02:41.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      404 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       16 2023-02-21 18:16:57.000000 bioconvert-1.0.0.post0/bioconvert.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-02-21 18:16:57.733733 bioconvert-1.0.0.post0/examples/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/README.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    28138 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/conversion.dot
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2775 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/plot_benchmark.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2783 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/plot_graph.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2847 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/plot_graph_clustered.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2839 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/plot_graph_colored.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2499 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/plot_methods.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   195516 2023-02-21 16:04:10.000000 bioconvert-1.0.0.post0/examples/test.cov
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      201 2023-02-21 16:14:28.000000 bioconvert-1.0.0.post0/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      250 2023-02-21 18:16:57.734732 bioconvert-1.0.0.post0/setup.cfg
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     3405 2023-02-21 18:16:56.000000 bioconvert-1.0.0.post0/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.196799 bioconvert-1.1.0/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       89 2022-06-08 09:19:21.000000 bioconvert-1.1.0/.coveragerc
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       98 2022-06-08 09:19:21.000000 bioconvert-1.1.0/.dockerignore
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.162799 bioconvert-1.1.0/.github/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.178799 bioconvert-1.1.0/.github/workflows/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/abi2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/abi2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/abi2qual.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2bedgraph.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2bigwig.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2cov.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2cram.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2json.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2sam.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2tsv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bam2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bcf2vcf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bcf2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bed2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bedgraph2bigwig.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bedgraph2cov.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bedgraph2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bigbed2bed.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bigbed2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bigwig2bedgraph.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bigwig2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bplink2plink.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bplink2vcf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2320 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/bz22gz.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/clustal2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/clustal2nexus.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2368 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/clustal2phylip.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2386 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/clustal2stockholm.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2309 2023-01-30 15:54:08.000000 bioconvert-1.1.0/.github/workflows/core.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/cram2bam.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/cram2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/cram2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/cram2sam.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3808 2023-01-30 15:53:49.000000 bioconvert-1.1.0/.github/workflows/create_wk.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/csv2tsv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/csv2xls.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/dsrc2gz.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/embl2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/embl2genbank.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2clustal.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2faa.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2fasta_agp.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2genbank.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2nexus.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2phylip.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta2twobit.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2380 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fasta_qual2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fastq2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2380 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fastq2fasta_qual.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/fastq2qual.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/genbank2embl.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/genbank2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/genbank2gff3.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gfa2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gff22gff3.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gff32gff2.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gff32gtf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2320 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gz2bz2.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/gz2dsrc.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-02-06 08:59:27.000000 bioconvert-1.1.0/.github/workflows/json2yaml.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/maf2sam.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-02-09 09:31:39.000000 bioconvert-1.1.0/.github/workflows/main.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/newick2nexus.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/newick2phyloxml.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2362 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/nexus2clustal.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/nexus2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/nexus2newick.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/nexus2phylip.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2368 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/nexus2phyloxml.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/ods2csv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/pdb2faa.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2368 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phylip2clustal.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phylip2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phylip2nexus.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2380 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phylip2stockholm.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phylip2xmfa.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2374 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phyloxml2newick.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2368 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/phyloxml2nexus.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/plink2bplink.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/plink2vcf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      965 2022-08-14 17:04:26.000000 bioconvert-1.1.0/.github/workflows/pypi.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/sam2bam.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/sam2cram.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/sam2paf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/scf2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/scf2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/sra2fastq.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2386 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/stockholm2clustal.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2380 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/stockholm2phylip.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/tsv2csv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2356 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/twobit2fasta.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/vcf2bcf.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/vcf2bed.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/vcf2bplink.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/vcf2plink.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2344 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/vcf2wiggle.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/wig2bed.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2326 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/xls2csv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2332 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/xlsx2csv.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2350 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/xmfa2phylip.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2338 2023-01-30 15:53:52.000000 bioconvert-1.1.0/.github/workflows/yaml2json.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1356 2022-06-08 09:19:21.000000 bioconvert-1.1.0/.gitignore
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      267 2022-08-17 07:41:02.000000 bioconvert-1.1.0/.readthedocs.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1744 2022-08-14 17:10:11.000000 bioconvert-1.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    35141 2022-06-08 09:19:21.000000 bioconvert-1.1.0/COPYING
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1193 2023-02-09 09:33:00.000000 bioconvert-1.1.0/Dockerfile
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      186 2022-06-08 09:19:21.000000 bioconvert-1.1.0/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    48444 2023-06-22 15:10:42.197800 bioconvert-1.1.0/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    47170 2023-06-22 15:10:37.000000 bioconvert-1.1.0/README.rst
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.178799 bioconvert-1.1.0/Singularity/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      132 2023-01-30 15:59:14.000000 bioconvert-1.1.0/Singularity/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1753 2023-01-30 15:59:14.000000 bioconvert-1.1.0/Singularity/Singularity
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.184799 bioconvert-1.1.0/bioconvert/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2238 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2918 2023-01-26 22:33:49.000000 bioconvert-1.1.0/bioconvert/abi2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2905 2023-01-17 14:54:58.000000 bioconvert-1.1.0/bioconvert/abi2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3310 2022-10-16 20:20:15.000000 bioconvert-1.1.0/bioconvert/abi2qual.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4394 2022-10-16 20:20:20.000000 bioconvert-1.1.0/bioconvert/bam2bedgraph.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4320 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bam2bigwig.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3516 2022-10-16 20:20:27.000000 bioconvert-1.1.0/bioconvert/bam2cov.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3831 2022-10-25 22:22:43.000000 bioconvert-1.1.0/bioconvert/bam2cram.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6110 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bam2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8180 2023-02-08 15:06:25.000000 bioconvert-1.1.0/bioconvert/bam2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2817 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bam2json.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3970 2023-01-31 21:22:36.000000 bioconvert-1.1.0/bioconvert/bam2sam.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3814 2022-10-16 20:20:58.000000 bioconvert-1.1.0/bioconvert/bam2tsv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2727 2022-10-16 20:21:03.000000 bioconvert-1.1.0/bioconvert/bam2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2940 2022-10-16 20:21:07.000000 bioconvert-1.1.0/bioconvert/bcf2vcf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2754 2022-10-16 20:21:11.000000 bioconvert-1.1.0/bioconvert/bcf2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2744 2022-10-17 19:08:58.000000 bioconvert-1.1.0/bioconvert/bed2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3486 2022-10-16 20:21:21.000000 bioconvert-1.1.0/bioconvert/bedgraph2bigwig.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3337 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bedgraph2cov.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2965 2022-10-16 20:21:34.000000 bioconvert-1.1.0/bioconvert/bedgraph2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3457 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bigbed2bed.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3238 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bigbed2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3676 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/bigwig2bedgraph.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2767 2022-10-16 21:05:33.000000 bioconvert-1.1.0/bioconvert/bigwig2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3501 2022-10-16 21:05:41.000000 bioconvert-1.1.0/bioconvert/bplink2plink.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3650 2022-10-16 21:05:45.000000 bioconvert-1.1.0/bioconvert/bplink2vcf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3144 2022-10-16 21:05:50.000000 bioconvert-1.1.0/bioconvert/bz22gz.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3860 2022-10-16 21:05:54.000000 bioconvert-1.1.0/bioconvert/clustal2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3092 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/clustal2nexus.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3469 2022-10-16 21:06:03.000000 bioconvert-1.1.0/bioconvert/clustal2phylip.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3473 2022-10-16 21:06:07.000000 bioconvert-1.1.0/bioconvert/clustal2stockholm.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.186799 bioconvert-1.1.0/bioconvert/core/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       43 2022-10-17 08:24:10.000000 bioconvert-1.1.0/bioconvert/core/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    25497 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/core/base.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11973 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/core/benchmark.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8102 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/converter.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10559 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/decorators.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2950 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/downloader.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4759 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/extensions.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11085 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/graph.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5000 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/init.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3786 2022-10-17 08:24:24.000000 bioconvert-1.1.0/bioconvert/core/levenshtein.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16130 2022-10-17 08:02:56.000000 bioconvert-1.1.0/bioconvert/core/registry.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3754 2022-10-17 12:40:39.000000 bioconvert-1.1.0/bioconvert/core/shell.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5587 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/core/utils.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3828 2022-10-16 21:06:12.000000 bioconvert-1.1.0/bioconvert/cram2bam.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5079 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/cram2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6151 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/cram2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3843 2022-10-26 21:29:32.000000 bioconvert-1.1.0/bioconvert/cram2sam.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5244 2023-02-08 15:38:00.000000 bioconvert-1.1.0/bioconvert/csv2tsv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4532 2023-06-22 14:28:18.000000 bioconvert-1.1.0/bioconvert/csv2xls.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.187799 bioconvert-1.1.0/bioconvert/data/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1963 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       11 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/measles.chrom.sizes
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    25805 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/test.bigwig
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8903 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/test_SP1.fq.gz
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    15096 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/test_gfa2fasta_v1.gfa
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       20 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/test_measles.fa.fai
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6569 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/test_measles.sorted.bam
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.187799 bioconvert-1.1.0/bioconvert/data/testing/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/data/testing/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3116 2022-10-16 21:06:37.000000 bioconvert-1.1.0/bioconvert/dsrc2gz.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3101 2022-10-16 21:06:44.000000 bioconvert-1.1.0/bioconvert/embl2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3105 2022-10-16 21:06:48.000000 bioconvert-1.1.0/bioconvert/embl2genbank.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3841 2022-10-16 21:06:52.000000 bioconvert-1.1.0/bioconvert/fasta2clustal.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4531 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/fasta2faa.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10893 2023-02-21 15:35:54.000000 bioconvert-1.1.0/bioconvert/fasta2fasta_agp.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3555 2022-10-16 21:07:03.000000 bioconvert-1.1.0/bioconvert/fasta2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5370 2022-10-16 21:07:06.000000 bioconvert-1.1.0/bioconvert/fasta2genbank.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3094 2022-10-16 21:07:11.000000 bioconvert-1.1.0/bioconvert/fasta2nexus.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4321 2022-10-16 21:07:14.000000 bioconvert-1.1.0/bioconvert/fasta2phylip.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2903 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/fasta2twobit.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4054 2022-10-16 21:07:23.000000 bioconvert-1.1.0/bioconvert/fasta_qual2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11245 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/fastq2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4862 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/fastq2fasta_qual.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4160 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/fastq2qual.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2979 2022-10-16 21:07:42.000000 bioconvert-1.1.0/bioconvert/genbank2embl.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4185 2022-10-16 21:07:46.000000 bioconvert-1.1.0/bioconvert/genbank2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2661 2022-10-16 21:07:50.000000 bioconvert-1.1.0/bioconvert/genbank2gff3.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4339 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/gfa2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4289 2022-10-16 21:07:58.000000 bioconvert-1.1.0/bioconvert/gff22gff3.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4245 2022-10-16 21:08:02.000000 bioconvert-1.1.0/bioconvert/gff32gff2.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2566 2023-02-03 07:52:15.000000 bioconvert-1.1.0/bioconvert/gff32gtf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3682 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/gtf22gff3.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3783 2023-01-30 15:09:51.000000 bioconvert-1.1.0/bioconvert/gz2bz2.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3303 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/gz2dsrc.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.188799 bioconvert-1.1.0/bioconvert/io/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/io/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2801 2022-10-17 12:40:43.000000 bioconvert-1.1.0/bioconvert/io/fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    19075 2022-10-17 12:40:43.000000 bioconvert-1.1.0/bioconvert/io/genbank.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4397 2022-10-17 12:40:43.000000 bioconvert-1.1.0/bioconvert/io/gff2.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4953 2022-10-17 12:40:43.000000 bioconvert-1.1.0/bioconvert/io/gff3.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9578 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/io/maf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9215 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/io/scf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3032 2022-10-16 21:08:22.000000 bioconvert-1.1.0/bioconvert/json2yaml.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2966 2022-10-16 21:08:26.000000 bioconvert-1.1.0/bioconvert/maf2sam.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.189799 bioconvert-1.1.0/bioconvert/misc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      176 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1212 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/cython_fastq2fasta.pyx
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3352 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/fastq2fasta.c
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      622 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/fastq2fasta.pl
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2134 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/install_goalign.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2132 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/misc/install_gotree.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2940 2022-10-25 21:28:23.000000 bioconvert-1.1.0/bioconvert/newick2nexus.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3012 2022-10-16 21:08:33.000000 bioconvert-1.1.0/bioconvert/newick2phyloxml.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4030 2022-10-16 21:08:37.000000 bioconvert-1.1.0/bioconvert/nexus2clustal.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6113 2022-10-16 21:08:41.000000 bioconvert-1.1.0/bioconvert/nexus2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3442 2022-10-16 21:08:45.000000 bioconvert-1.1.0/bioconvert/nexus2newick.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2992 2022-10-16 21:08:49.000000 bioconvert-1.1.0/bioconvert/nexus2phylip.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3003 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/nexus2phyloxml.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3928 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/ods2csv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3894 2023-03-16 11:49:13.000000 bioconvert-1.1.0/bioconvert/pdb2faa.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3359 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/phylip2clustal.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3973 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/phylip2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2943 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/phylip2nexus.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3444 2022-10-16 21:09:16.000000 bioconvert-1.1.0/bioconvert/phylip2stockholm.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2984 2022-10-16 21:09:25.000000 bioconvert-1.1.0/bioconvert/phylip2xmfa.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2985 2022-10-16 21:09:29.000000 bioconvert-1.1.0/bioconvert/phyloxml2newick.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2953 2022-10-16 21:09:34.000000 bioconvert-1.1.0/bioconvert/phyloxml2nexus.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2957 2022-10-16 21:09:37.000000 bioconvert-1.1.0/bioconvert/plink2bplink.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3111 2022-10-16 21:09:42.000000 bioconvert-1.1.0/bioconvert/plink2vcf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2851 2022-10-16 21:09:46.000000 bioconvert-1.1.0/bioconvert/sam2bam.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3985 2022-10-16 21:09:50.000000 bioconvert-1.1.0/bioconvert/sam2cram.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14907 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/sam2paf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4962 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/scf2fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5272 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/scf2fastq.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.189799 bioconvert-1.1.0/bioconvert/scripts/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-10-17 08:11:35.000000 bioconvert-1.1.0/bioconvert/scripts/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    23394 2023-06-22 14:18:16.000000 bioconvert-1.1.0/bioconvert/scripts/converter.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2591 2022-10-17 12:40:49.000000 bioconvert-1.1.0/bioconvert/scripts/init_convert.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4159 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/scripts/stats.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.190799 bioconvert-1.1.0/bioconvert/simulator/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/simulator/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2541 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/simulator/fasta.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2329 2023-02-08 15:06:25.000000 bioconvert-1.1.0/bioconvert/simulator/fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2155 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/simulator/gfa.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4676 2022-10-16 21:10:04.000000 bioconvert-1.1.0/bioconvert/sra2fastq.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3407 2022-10-16 21:10:07.000000 bioconvert-1.1.0/bioconvert/stockholm2clustal.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3418 2022-10-16 21:10:11.000000 bioconvert-1.1.0/bioconvert/stockholm2phylip.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5240 2023-02-08 15:21:17.000000 bioconvert-1.1.0/bioconvert/tsv2csv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3423 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/twobit2fasta.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.190799 bioconvert-1.1.0/bioconvert/utils/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.190799 bioconvert-1.1.0/bioconvert/utils/biocode/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      407 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/biocode/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/biocode/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    19802 2023-02-08 15:24:39.000000 bioconvert-1.1.0/bioconvert/utils/biocode/annotation.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9639 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/biocode/convert_genbank_to_gff3.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    31129 2023-02-08 15:23:30.000000 bioconvert-1.1.0/bioconvert/utils/biocode/gff.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10518 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/biocode/tbl.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    58309 2022-06-08 09:19:21.000000 bioconvert-1.1.0/bioconvert/utils/biocode/things.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     7989 2023-02-08 15:23:52.000000 bioconvert-1.1.0/bioconvert/utils/biocode/utils.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3273 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/vcf2bcf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2846 2022-10-16 21:10:27.000000 bioconvert-1.1.0/bioconvert/vcf2bed.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2936 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/vcf2bplink.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2992 2023-01-30 15:59:14.000000 bioconvert-1.1.0/bioconvert/vcf2plink.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2685 2022-10-16 21:10:38.000000 bioconvert-1.1.0/bioconvert/vcf2wiggle.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2707 2022-10-17 08:26:05.000000 bioconvert-1.1.0/bioconvert/wig2bed.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5078 2023-02-21 15:47:49.000000 bioconvert-1.1.0/bioconvert/xls2csv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5103 2023-02-09 10:12:27.000000 bioconvert-1.1.0/bioconvert/xlsx2csv.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2950 2022-10-16 21:11:13.000000 bioconvert-1.1.0/bioconvert/xmfa2phylip.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3186 2022-10-16 21:11:21.000000 bioconvert-1.1.0/bioconvert/yaml2json.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.185799 bioconvert-1.1.0/bioconvert.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    48444 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9030 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-06-08 09:28:10.000000 bioconvert-1.1.0/bioconvert.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      418 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       16 2023-06-22 15:10:42.000000 bioconvert-1.1.0/bioconvert.egg-info/top_level.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.192799 bioconvert-1.1.0/doc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4918 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/Makefile
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      704 2022-10-17 09:23:19.000000 bioconvert-1.1.0/doc/Snakefile
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4612 2023-06-22 14:18:16.000000 bioconvert-1.1.0/doc/Snakefile_benchmark
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.193799 bioconvert-1.1.0/doc/_static/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     7895 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/_static/NewickExample.svg
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    10954 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/_static/basic.css
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    45271 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/_static/benchmark_fastq2fasta.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    19017 2023-01-30 21:25:01.000000 bioconvert-1.1.0/doc/benchmark.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    20369 2023-01-30 21:25:01.000000 bioconvert-1.1.0/doc/benchmark2.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    54641 2023-01-30 21:25:01.000000 bioconvert-1.1.0/doc/benchmark_1000000.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3265 2023-06-22 14:18:16.000000 bioconvert-1.1.0/doc/benchmarking.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2936 2022-08-14 16:25:44.000000 bioconvert-1.1.0/doc/bibliography.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10591 2023-04-27 09:35:43.000000 bioconvert-1.1.0/doc/conf.py
+-rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)   218647 2023-02-21 15:40:52.000000 bioconvert-1.1.0/doc/conversion.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    48786 2022-10-31 17:08:20.000000 bioconvert-1.1.0/doc/conversion.svg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8403 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/coverage_igv.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      694 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/create_automodules_allconverters.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      268 2022-10-31 17:01:12.000000 bioconvert-1.1.0/doc/create_graph.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17936 2023-01-30 15:59:14.000000 bioconvert-1.1.0/doc/developer_guide.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      969 2023-01-30 15:59:14.000000 bioconvert-1.1.0/doc/faqs.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    89304 2022-12-28 23:02:43.000000 bioconvert-1.1.0/doc/formats.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8272 2022-06-08 09:23:10.000000 bioconvert-1.1.0/doc/glossary.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      393 2023-02-08 14:35:06.000000 bioconvert-1.1.0/doc/index.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4344 2023-06-22 14:18:16.000000 bioconvert-1.1.0/doc/installation.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    45271 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/multi_benchmark.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10221 2023-02-21 15:36:21.000000 bioconvert-1.1.0/doc/ref_converters.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1142 2022-06-08 09:23:10.000000 bioconvert-1.1.0/doc/ref_core.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      231 2022-06-08 09:23:10.000000 bioconvert-1.1.0/doc/ref_io.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      112 2022-10-26 21:22:49.000000 bioconvert-1.1.0/doc/references.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      140 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/script.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      152 2022-06-08 09:19:21.000000 bioconvert-1.1.0/doc/script2.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3845 2022-08-14 16:25:44.000000 bioconvert-1.1.0/doc/tutorial.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4891 2023-01-30 15:59:14.000000 bioconvert-1.1.0/doc/user_guide.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      661 2023-02-03 17:12:20.000000 bioconvert-1.1.0/environment.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      509 2023-01-30 15:56:47.000000 bioconvert-1.1.0/environment_rtd.yml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-22 15:10:42.196799 bioconvert-1.1.0/examples/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2022-06-08 09:19:21.000000 bioconvert-1.1.0/examples/README.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    28138 2023-02-08 15:06:05.000000 bioconvert-1.1.0/examples/conversion.dot
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   242694 2023-02-08 14:35:12.000000 bioconvert-1.1.0/examples/conversion.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2775 2022-06-08 09:19:21.000000 bioconvert-1.1.0/examples/plot_benchmark.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2783 2022-06-08 09:19:21.000000 bioconvert-1.1.0/examples/plot_graph.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2847 2022-08-14 21:36:15.000000 bioconvert-1.1.0/examples/plot_graph_clustered.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2839 2022-08-14 21:33:43.000000 bioconvert-1.1.0/examples/plot_graph_colored.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2499 2022-10-17 08:07:18.000000 bioconvert-1.1.0/examples/plot_methods.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   195516 2023-02-08 14:35:13.000000 bioconvert-1.1.0/examples/test.cov
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      215 2023-06-22 14:18:16.000000 bioconvert-1.1.0/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      250 2023-06-22 15:10:42.197800 bioconvert-1.1.0/setup.cfg
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     3409 2023-06-22 14:18:16.000000 bioconvert-1.1.0/setup.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9698 2023-02-03 17:18:03.000000 bioconvert-1.1.0/spec-file.txt
```

### Comparing `bioconvert-1.0.0.post0/CONTRIBUTING.rst` & `bioconvert-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/COPYING` & `bioconvert-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/PKG-INFO` & `bioconvert-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,608 +1,19 @@
 Metadata-Version: 2.1
 Name: bioconvert
-Version: 1.0.0.post0
+Version: 1.1.0
 Summary: convert between bioinformatics formats
 Home-page: https://github.com/bioconvert/bioconvert
+Download-URL: https://github.com/bioconvert/bioconvert
 Author: The bioconvert Contributors
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: Thomas Cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: GPLv3
-Download-URL: https://github.com/bioconvert/bioconvert
-Description: Bioconvert
-        ##########
-        
-        **Bioconvert** is a collaborative project to facilitate the interconversion of life science data from one format to another.
-        
-        .. image:: https://badge.fury.io/py/bioconvert.svg
-            :target: https://pypi.python.org/pypi/bioconvert
-        
-        .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml/badge.svg?branch=main
-            :target: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/github/bioconvert/bioconvert/badge.svg?branch=main
-           :target: https://coveralls.io/github/bioconvert/bioconvert?branch=main
-        
-        .. image:: http://readthedocs.org/projects/bioconvert/badge/?version=main
-            :target: http://bioconvert.readthedocs.org/en/main/?badge=main
-            :alt: Documentation Status
-        
-        .. image::  https://img.shields.io/github/issues/bioconvert/bioconvert.svg
-            :target:  https://github.com/bioconvert/bioconvert/issues
-        
-        .. image:: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
-           :target: https://anaconda.org/bioconda/bioconvert
-        
-        .. image::  https://anaconda.org/bioconda/bioconvert/badges/version.svg
-            :target: https://anaconda.org/bioconda/bioconvert/badges/version.svg
-        
-        .. image:: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
-            :target: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
-        
-        .. image:: https://zenodo.org/badge/106598809.svg
-           :target: https://zenodo.org/badge/latestdoi/106598809
-        
-        .. image:: https://static.pepy.tech/personalized-badge/bioconvert?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/months
-            :target: https://pepy.tech/project/bioconvert
-        
-        .. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
-            :target: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
-        
-        
-        :contributions: Want to add a convertor ? Please join https://github.com/bioconvert/bioconvert/issues/1
-        
-        Overview
-        ########
-        
-        
-        Life science uses many different formats. They may be old, or with complex syntax and converting those formats may be a challenge. Bioconvert aims at providing a common tool / interface to convert life science data formats from one to another.
-        
-        Many conversion tools already exist but they may be dispersed, focused on few specific formats, difficult to install, or not optimised. With Bioconvert, we plan to cover a wide spectrum of format conversions; we will re-use existing tools when possible and provide facilities to compare different conversion tools or methods via benchmarking. New implementations are provided when considered better than existing ones.
-        
-        In Jan 2023, we had 50 formats, 100 direct conversions available.
-        
-        .. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/conversion.png
-            :width: 80%
-        
-        
-        Installation
-        ###############
-        
-        **BioConvert** is developped in Python. Please use conda or any Python environment manager to install **BioConvert** using the **pip** command::
-        
-            pip install bioconvert
-        
-        50% of the conversions should work out of the box. However, many conversions require external tools. This is why we
-        recommend to use a **conda** environment. In particular, most external tools are available on the **bioconda** channel. 
-        For instance if you want to convert a SAM file to a BAM file you would need to install **samtools** as follow::
-        
-            conda install -c bioconda samtools
-        
-        Since **bioconvert** is available on `bioconda <https://bioconda.github.io>`_ on solution that installs **BioConvert** and all its dependencies is to use conda/mamba::
-        
-            conda env create --name bioconvert mamba
-            conda activate bioconvert
-            mamba install bioconvert
-            bioconvert --help
-        
-        See the Installation section for more details and alternative solutions (docker, singularity).
-        
-        Quick Start
-        ##############
-        There are many conversions available. Type::
-        
-            bioconvert --help 
-        
-        to get a list of valid method of conversions. Taking the example of a conversion from a `FastQ` file into
-        a `FastA` file, you could do the conversion as follows::
-        
-            bioconvert fastq2fasta input.fastq output.fasta
-            bioconvert fastq2fasta input.fq    output.fasta
-            bioconvert fastq2fasta input.fq.gz output.fasta.gz
-            bioconvert fastq2fasta input.fq.gz output.fasta.bz2
-        
-        When there is no ambiguity, you can be implicit::
-        
-             bioconvert input.fastq output.fasta
-        
-        The default method of conversion is used but you may use another one. Checkout the available methods with::
-        
-            bioconvert fastq2fasta --show-methods
-        
-        For more help about a conversion, just type::
-        
-            bioconvert fastq2fasta --help
-        
-        and more generally::
-        
-            bioconvert --help
-        
-        
-        You may also call **BioConvert** from a Python shell::
-        
-            # import a converter
-            from bioconvert.fastq2fasta import FASTQ2FASTA
-        
-            # Instanciate with infile/outfile names
-            convert = FASTQ2FASTA(infile, outfile)
-        
-            # the conversion itself:
-            convert()
-        
-        
-        Available Converters
-        #######################
-        
-        
-        .. list-table:: Conversion table
-            :widths: 20 40 40
-            :header-rows: 1
-        
-            * - Converters
-              - CI testing
-              - Default method
-            * - `abi2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `abi2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `abi2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bedgraph>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml
-              - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bigwig>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cov>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml
-              - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cram>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2json>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml
-              - `BAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml
-              - `SAMBAMBA <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2tsv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bcf2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml
-              - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bed2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2bigwig>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml
-              - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2cov>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigbed2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigbed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigwig2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2bedgraph>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigwig2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bplink2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2plink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bplink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bz22gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bz22gz>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml
-              - Unix commands
-            * - `clustal2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2stockholm>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2bam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `csv2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2tsv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `csv2xls <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2xls>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml
-              - Pandas
-            * - `dsrc2gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.dsrc2gz>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml
-              - DSRC software
-            * - `embl2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `embl2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2genbank>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2faa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2fasta_agp <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fasta_agp>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml
-              - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2genbank>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2twobit <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2twobit>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml
-              - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta_qual2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta_qual2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml
-              - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fastq2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml
-              -  `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_  `available <_static/benchmark_fastq2fasta.png>`_
-            * - `fastq2fasta_qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta_qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fastq2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml
-              - `READFQ <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2embl <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2embl>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2gff3>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml
-              - `BIOCODE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gfa2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gfa2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff22gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff22gff3>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff32gff2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gff2>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff32gtf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gtf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gz2bz2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2bz2>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml
-              - pigz/pbzip2 software
-            * - `gz2dsrc <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2dsrc>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml
-              - DSRC software
-            * - `json2yaml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.json2yaml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml
-              - Python
-            * - `maf2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.maf2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `newick2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `newick2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2phyloxml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2newick>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phyloxml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `ods2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.ods2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml
-              - pyexcel library
-            * - `pdb2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.pdb2faa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2stockholm>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2xmfa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2xmfa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phyloxml2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2newick>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phyloxml2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `plink2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2bplink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `plink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2bam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2cram>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2paf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2paf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `scf2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `scf2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sra2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sra2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml
-              - `FASTQDUMP <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `stockholm2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `stockholm2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `tsv2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.tsv2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `twobit2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.twobit2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml
-              - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bplink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2plink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `wig2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.wig2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml
-              - `BEDOPS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `xls2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xls2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml
-              -
-            * - `xlsx2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xlsx2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml
-              - Pandas library
-            * - `xmfa2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xmfa2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `yaml2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.yaml2json>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml
-              - Pandas library
-        
-        
-        
-        Contributors
-        ############
-        
-        Setting up and maintaining Bioconvert has been possible thanks to users and contributors.
-        Thanks to all:
-        
-        .. image:: https://contrib.rocks/image?repo=bioconvert/bioconvert
-            :target: https://github.com/bioconvert/bioconvert/graphs/contributors
-        
-        
-        Changes
-        ########
-        
-        ========= ==============================================================================
-        Version   Description
-        ========= ==============================================================================
-        1.0.0     * Fix bam2fastq for paired data that computed useless intermediate file
-                    https://github.com/bioconvert/bioconvert/issues/325
-                  * more realistic fastq simulator
-                  * pin openpyxl to <=3.0.10 to prevent regression error in v3.1.0
-        0.6.3     * add picard method in bam2sam
-                  * Fixed all CI workflows to use mamba
-                  * drop python3.7 support and add 3.10 support
-                  * update bedops test file to fit the latest bedops 2.4.41 version
-                  * revisit logging system
-        0.6.2     * added gff3 to gtf conversion. 
-                  * Added pdb to faa conversion
-                  * Added missing --reference argument to the cram2sam conversion
-        0.6.1     * output file can be in sub-directories allowing syntax such as 
-                    'bioconvert fastq2fasta test.fastq outputs/test.fasta
-                  * fix all CI actions
-                  * add more examples as notebooks in ./examples
-                  * add a Snakefile for the paper in ./doc/Snakefile_paper
-        0.6.0     * Fix bug in bam2sam (method sambamba)
-                  * Fix graph layout
-                  * add threading in fastq2fasta (seqkit method)
-                  * multibenchmark feature added
-                  * stable version used for web interface
-        0.5.2     * Update requirements and environment.yml and add a conda spec-file.txt file
-        0.5.1     * add genbank2gff3 requirement material in bioconvert.utils.biocode
-        0.5.0     * Add CI actions for all converters
-                  * remove sniffer (now in biosniff on pypi https://pypi.org/project/biosniff/)
-                  * A complete benchmarking suite (see doc/Snakefile_benchmark file and
-                    `benchmarking`)
-                  * documentation and tests for all converters
-                  * removed the validators (we assume intputs are correct)
-        0.4.X     * (aug 2019) added nexus2fasta, cram2fasta, fasta2faa ... ; 1-to-many and 
-                    many-to-one converters are now part of the API.
-        0.3.X       may 2019. new methods abi2qual, bigbed2bed, etc. added --threads option
-        0.2.X       aug 2018. abi2fastx, bioconvert_stats tool added
-        0.1.X       major refactoring to  have subcommands with implicit/explicit mode
-        ========= ==============================================================================
-        
-        
-Keywords: NGS,bam2bed,fastq2fasta,bam2sam
+Keywords: NGS,bam2bed,fastq2fasta,bam2sam,conversion
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -614,7 +25,600 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: doc
+License-File: COPYING
+
+Bioconvert
+##########
+
+**Bioconvert** is a collaborative project to facilitate the interconversion of life science data from one format to another.
+
+.. image:: https://badge.fury.io/py/bioconvert.svg
+    :target: https://pypi.python.org/pypi/bioconvert
+
+.. image:: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml/badge.svg?branch=main
+    :target: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/bioconvert/bioconvert/badge.svg?branch=main
+   :target: https://coveralls.io/github/bioconvert/bioconvert?branch=main
+
+.. image:: http://readthedocs.org/projects/bioconvert/badge/?version=main
+    :target: http://bioconvert.readthedocs.org/en/main/?badge=main
+    :alt: Documentation Status
+
+.. image::  https://img.shields.io/github/issues/bioconvert/bioconvert.svg
+    :target:  https://github.com/bioconvert/bioconvert/issues
+
+.. image:: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
+   :target: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
+
+.. image::  https://anaconda.org/bioconda/bioconvert/badges/version.svg
+    :target: https://anaconda.org/bioconda/bioconvert
+
+.. image:: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
+    :target: https://github.com/bioconvert/bioconvert/releases
+
+.. image:: https://zenodo.org/badge/106598809.svg
+   :target: https://zenodo.org/badge/latestdoi/106598809
+
+.. image:: https://static.pepy.tech/personalized-badge/bioconvert?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/months
+    :target: https://pepy.tech/project/bioconvert
+
+.. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
+    :target: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
+
+
+:contributions: Want to add a convertor ? Please join https://github.com/bioconvert/bioconvert/issues/1
+
+Overview
+########
+
+
+Life science uses many different formats. They may be old, or with complex syntax and converting those formats may be a challenge. Bioconvert aims at providing a common tool / interface to convert life science data formats from one to another.
+
+Many conversion tools already exist but they may be dispersed, focused on few specific formats, difficult to install, or not optimised. With Bioconvert, we plan to cover a wide spectrum of format conversions; we will re-use existing tools when possible and provide facilities to compare different conversion tools or methods via benchmarking. New implementations are provided when considered better than existing ones.
+
+In Jan 2023, we had 50 formats, 100 direct conversions available.
+
+.. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/conversion.png
+    :width: 80%
+
+
+Installation
+###############
+
+**BioConvert** is developped in Python. Please use conda or any Python environment manager to install **BioConvert** using the **pip** command::
+
+    pip install bioconvert
+
+50% of the conversions should work out of the box. However, many conversions require external tools. This is why we
+recommend to use a **conda** environment. In particular, most external tools are available on the **bioconda** channel. 
+For instance if you want to convert a SAM file to a BAM file you would need to install **samtools** as follow::
+
+    conda install -c bioconda samtools
+
+Since **bioconvert** is available on `bioconda <https://bioconda.github.io>`_ on solution that installs **BioConvert** and all its dependencies is to use conda/mamba::
+
+    conda env create --name bioconvert mamba
+    conda activate bioconvert
+    mamba install bioconvert
+    bioconvert --help
+
+See the Installation section for more details and alternative solutions (docker, singularity).
+
+Quick Start
+##############
+There are many conversions available. Type::
+
+    bioconvert --help 
+
+to get a list of valid method of conversions. Taking the example of a conversion from a `FastQ` file into
+a `FastA` file, you could do the conversion as follows::
+
+    bioconvert fastq2fasta input.fastq output.fasta
+    bioconvert fastq2fasta input.fq    output.fasta
+    bioconvert fastq2fasta input.fq.gz output.fasta.gz
+    bioconvert fastq2fasta input.fq.gz output.fasta.bz2
+
+When there is no ambiguity, you can be implicit::
+
+     bioconvert input.fastq output.fasta
+
+The default method of conversion is used but you may use another one. Checkout the available methods with::
+
+    bioconvert fastq2fasta --show-methods
+
+For more help about a conversion, just type::
+
+    bioconvert fastq2fasta --help
+
+and more generally::
+
+    bioconvert --help
+
+
+You may also call **BioConvert** from a Python shell::
+
+    # import a converter
+    from bioconvert.fastq2fasta import FASTQ2FASTA
+
+    # Instanciate with infile/outfile names
+    convert = FASTQ2FASTA(infile, outfile)
+
+    # the conversion itself:
+    convert()
+
+
+Available Converters
+#######################
+
+
+.. list-table:: Conversion table
+    :widths: 20 40 40
+    :header-rows: 1
+
+    * - Converters
+      - CI testing
+      - Default method
+    * - `abi2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `abi2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `abi2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bedgraph>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml
+      - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bigwig>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cov>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml
+      - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cram>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2json>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml
+      - `BAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml
+      - `SAMBAMBA <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2tsv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bcf2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml
+      - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bed2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2bigwig>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml
+      - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2cov>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigbed2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigbed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigwig2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2bedgraph>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigwig2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bplink2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2plink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bplink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bz22gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bz22gz>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml
+      - Unix commands
+    * - `clustal2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2stockholm>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2bam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `csv2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2tsv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `csv2xls <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2xls>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml
+      - Pandas
+    * - `dsrc2gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.dsrc2gz>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml
+      - DSRC software
+    * - `embl2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `embl2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2genbank>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2faa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2fasta_agp <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fasta_agp>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml
+      - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2genbank>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2twobit <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2twobit>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml
+      - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta_qual2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta_qual2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml
+      - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fastq2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml
+      -  `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_  `available <_static/benchmark_fastq2fasta.png>`_
+    * - `fastq2fasta_qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta_qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fastq2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml
+      - `READFQ <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2embl <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2embl>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2gff3>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml
+      - `BIOCODE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gfa2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gfa2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff22gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff22gff3>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff32gff2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gff2>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff32gtf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gtf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gz2bz2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2bz2>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml
+      - pigz/pbzip2 software
+    * - `gz2dsrc <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2dsrc>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml
+      - DSRC software
+    * - `json2yaml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.json2yaml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml
+      - Python
+    * - `maf2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.maf2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `newick2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `newick2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2phyloxml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2newick>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phyloxml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `ods2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.ods2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml
+      - pyexcel library
+    * - `pdb2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.pdb2faa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2stockholm>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2xmfa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2xmfa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phyloxml2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2newick>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phyloxml2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `plink2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2bplink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `plink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2bam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2cram>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2paf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2paf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `scf2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `scf2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sra2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sra2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml
+      - `FASTQDUMP <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `stockholm2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `stockholm2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `tsv2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.tsv2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `twobit2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.twobit2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml
+      - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bplink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2plink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `wig2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.wig2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml
+      - `BEDOPS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `xls2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xls2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml
+      -
+    * - `xlsx2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xlsx2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml
+      - Pandas library
+    * - `xmfa2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xmfa2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `yaml2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.yaml2json>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml
+      - Pandas library
+
+
+
+Contributors
+############
+
+Setting up and maintaining Bioconvert has been possible thanks to users and contributors.
+Thanks to all:
+
+.. image:: https://contrib.rocks/image?repo=bioconvert/bioconvert
+    :target: https://github.com/bioconvert/bioconvert/graphs/contributors
+
+
+Changes
+########
+
+========= ==============================================================================
+Version   Description
+========= ==============================================================================
+1.1.0     * Implement ability to benchmark the CPU and memory usage (not just time)
+            benchmark incorporates CPU/memory usage
+          * add missing cython in requirements (and psutil for benchmarking)
+1.0.0     * Fix bam2fastq for paired data that computed useless intermediate file
+            https://github.com/bioconvert/bioconvert/issues/325
+          * more realistic fastq simulator
+          * pin openpyxl to <=3.0.10 to prevent regression error in v3.1.0
+0.6.3     * add picard method in bam2sam
+          * Fixed all CI workflows to use mamba
+          * drop python3.7 support and add 3.10 support
+          * update bedops test file to fit the latest bedops 2.4.41 version
+          * revisit logging system
+0.6.2     * added gff3 to gtf conversion. 
+          * Added pdb to faa conversion
+          * Added missing --reference argument to the cram2sam conversion
+0.6.1     * output file can be in sub-directories allowing syntax such as 
+            'bioconvert fastq2fasta test.fastq outputs/test.fasta
+          * fix all CI actions
+          * add more examples as notebooks in ./examples
+          * add a Snakefile for the paper in ./doc/Snakefile_paper
+0.6.0     * Fix bug in bam2sam (method sambamba)
+          * Fix graph layout
+          * add threading in fastq2fasta (seqkit method)
+          * multibenchmark feature added
+          * stable version used for web interface
+0.5.2     * Update requirements and environment.yml and add a conda spec-file.txt file
+0.5.1     * add genbank2gff3 requirement material in bioconvert.utils.biocode
+0.5.0     * Add CI actions for all converters
+          * remove sniffer (now in biosniff on pypi https://pypi.org/project/biosniff/)
+          * A complete benchmarking suite (see doc/Snakefile_benchmark file and
+            `benchmarking`)
+          * documentation and tests for all converters
+          * removed the validators (we assume intputs are correct)
+0.4.X     * (aug 2019) added nexus2fasta, cram2fasta, fasta2faa ... ; 1-to-many and 
+            many-to-one converters are now part of the API.
+0.3.X       may 2019. new methods abi2qual, bigbed2bed, etc. added --threads option
+0.2.X       aug 2018. abi2fastx, bioconvert_stats tool added
+0.1.X       major refactoring to  have subcommands with implicit/explicit mode
+========= ==============================================================================
+
```

### Comparing `bioconvert-1.0.0.post0/README.rst` & `bioconvert-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     :target: http://bioconvert.readthedocs.org/en/main/?badge=main
     :alt: Documentation Status
 
 .. image::  https://img.shields.io/github/issues/bioconvert/bioconvert.svg
     :target:  https://github.com/bioconvert/bioconvert/issues
 
 .. image:: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
-   :target: https://anaconda.org/bioconda/bioconvert
+   :target: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
 
 .. image::  https://anaconda.org/bioconda/bioconvert/badges/version.svg
-    :target: https://anaconda.org/bioconda/bioconvert/badges/version.svg
+    :target: https://anaconda.org/bioconda/bioconvert
 
 .. image:: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
-    :target: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
+    :target: https://github.com/bioconvert/bioconvert/releases
 
 .. image:: https://zenodo.org/badge/106598809.svg
    :target: https://zenodo.org/badge/latestdoi/106598809
 
 .. image:: https://static.pepy.tech/personalized-badge/bioconvert?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/months
     :target: https://pepy.tech/project/bioconvert
 
@@ -545,14 +545,17 @@
 
 Changes
 ########
 
 ========= ==============================================================================
 Version   Description
 ========= ==============================================================================
+1.1.0     * Implement ability to benchmark the CPU and memory usage (not just time)
+            benchmark incorporates CPU/memory usage
+          * add missing cython in requirements (and psutil for benchmarking)
 1.0.0     * Fix bam2fastq for paired data that computed useless intermediate file
             https://github.com/bioconvert/bioconvert/issues/325
           * more realistic fastq simulator
           * pin openpyxl to <=3.0.10 to prevent regression error in v3.1.0
 0.6.3     * add picard method in bam2sam
           * Fixed all CI workflows to use mamba
           * drop python3.7 support and add 3.10 support
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/__init__.py` & `bioconvert-1.1.0/bioconvert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "1.0.0"
 import pkg_resources
 
 try:
     version = pkg_resources.require("bioconvert")[0].version
 except:
     version = __version__
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/abi2fasta.py` & `bioconvert-1.1.0/bioconvert/abi2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/abi2fastq.py` & `bioconvert-1.1.0/bioconvert/abi2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/abi2qual.py` & `bioconvert-1.1.0/bioconvert/abi2qual.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2bedgraph.py` & `bioconvert-1.1.0/bioconvert/bam2bedgraph.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2bigwig.py` & `bioconvert-1.1.0/bioconvert/bam2bigwig.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2cov.py` & `bioconvert-1.1.0/bioconvert/bam2cov.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2cram.py` & `bioconvert-1.1.0/bioconvert/bam2cram.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2fasta.py` & `bioconvert-1.1.0/bioconvert/bam2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2fastq.py` & `bioconvert-1.1.0/bioconvert/bam2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2json.py` & `bioconvert-1.1.0/bioconvert/bam2json.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2sam.py` & `bioconvert-1.1.0/bioconvert/bam2sam.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2tsv.py` & `bioconvert-1.1.0/bioconvert/bam2tsv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bam2wiggle.py` & `bioconvert-1.1.0/bioconvert/bam2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bcf2vcf.py` & `bioconvert-1.1.0/bioconvert/bcf2vcf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bcf2wiggle.py` & `bioconvert-1.1.0/bioconvert/bcf2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bed2wiggle.py` & `bioconvert-1.1.0/bioconvert/bed2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bedgraph2bigwig.py` & `bioconvert-1.1.0/bioconvert/bedgraph2bigwig.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bedgraph2cov.py` & `bioconvert-1.1.0/bioconvert/bedgraph2cov.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bedgraph2wiggle.py` & `bioconvert-1.1.0/bioconvert/bedgraph2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bigbed2bed.py` & `bioconvert-1.1.0/bioconvert/bigbed2bed.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bigbed2wiggle.py` & `bioconvert-1.1.0/bioconvert/bigbed2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bigwig2bedgraph.py` & `bioconvert-1.1.0/bioconvert/bigwig2bedgraph.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bigwig2wiggle.py` & `bioconvert-1.1.0/bioconvert/bigwig2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bplink2plink.py` & `bioconvert-1.1.0/bioconvert/bplink2plink.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bplink2vcf.py` & `bioconvert-1.1.0/bioconvert/bplink2vcf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/bz22gz.py` & `bioconvert-1.1.0/bioconvert/bz22gz.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/clustal2fasta.py` & `bioconvert-1.1.0/bioconvert/clustal2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/clustal2nexus.py` & `bioconvert-1.1.0/bioconvert/clustal2nexus.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/clustal2phylip.py` & `bioconvert-1.1.0/bioconvert/clustal2phylip.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/clustal2stockholm.py` & `bioconvert-1.1.0/bioconvert/clustal2stockholm.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/base.py` & `bioconvert-1.1.0/bioconvert/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,17 @@
     # default method should be provided
     _default_method = None
     _is_compressor = False
     # Can be overriden and if True, new argument --thread is added automatically
     _threading = False
     _extra_arguments = ""
 
+    # do we lose information when performing the conversion ? 
+    _loss = False
+
     # Used for the benchmarking only
     others = {}
 
     # threads to be used by default if argument is required in a method
     # this will be overriden if _threading set to True and therefore --threads
     # set by the user. It is feed back into Bioconvert class
     threads = min([4, os.cpu_count()])
@@ -298,17 +301,14 @@
 
 
         if method_name not in self.available_methods:
             msg = "Methods available are {}".format(self.available_methods)
             _log.error(msg)
             raise ValueError(msg)
 
-
-
-
         _log.info("{}> Executing {} method ".format(self.name, method_name))
         # reference to the method requested
         method_reference = getattr(self, "_method_{}".format(method_name))
 
         # call the method itself
 
         t1 = time.time()
@@ -317,17 +317,21 @@
         if isinstance(self.outfile, (tuple, list)):
             output_file = Path(self.outfile[0])
         else:
             output_file = Path(self.outfile)
         output_file.parent.mkdir(parents=True, exist_ok=True)
 
         method_reference(*args, **kwargs)
+
         t2 = time.time()
         _log.info("Took {} seconds ".format(t2 - t1))
 
+        if self._loss:
+            _log.warning(f"There is a loss of information in the conversion {self.name}")
+
     @property
     def name(self):
         """
         The name of the class
         """
         return type(self).__name__
 
@@ -404,33 +408,43 @@
 
         if process_.returncode != 0:
             if not ignore_errors:
                 raise RuntimeError(errors)
         else:
             return output
 
-    def boxplot_benchmark(
+    def compute_benchmark(
         self,
         N=5,
-        rerun=True,
         to_exclude=[],
-        to_include=[],
-        rot_xticks=90,
-        boxplot_args={},
+        to_include=[]
     ):
-        """Simple wrapper to call :class:`Benchmark` and plot the results
+        """Simple wrapper to call :class:`Benchmark` 
+
+        This function computes the benchmark
 
         see :class:`~bioconvert.core.benchmark.Benchmark` for details.
 
         """
         if to_include == "all":
             to_include = []
 
         self._benchmark = Benchmark(self, N=N, to_exclude=to_exclude, to_include=to_include)
-        data = self._benchmark.plot(rerun=rerun, rot_xticks=rot_xticks, boxplot_args=boxplot_args)
+        self._benchmark.run_methods()
+
+
+    def boxplot_benchmark(self,
+        rot_xticks=90,
+        boxplot_args={},
+        mode="time"):
+        """
+        This function plots the benchmark computed in :meth:`compute_benchmark`
+
+        """
+        data = self._benchmark.plot(rerun=False, rot_xticks=rot_xticks, boxplot_args=boxplot_args, mode=mode)
         return data
 
     def _get_default_method(self):
         if self._default_method is None:
             return self.available_methods[0]
         else:
             return self._default_method
@@ -567,14 +581,21 @@
                 "--benchmark-save-image",
             ],
             action="store_true",
             help="Save results as an image (using the same tag as from --benchmark-tag)",
         )
         yield ConvArg(
             names=[
+                "--benchmark-mode",
+            ],
+            default="time",
+            help="Set the mode of the benchmark, which can be time, CPU or memory. Defaults to time)",
+        )
+        yield ConvArg(
+            names=[
                 "-M",
                 "--benchmark-methods",
             ],
             default="all",
             nargs="+",
             type=str,
             help="Methods to include. Provide list as space-separated method names. Use -s  to get the full list.",
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/benchmark.py` & `bioconvert-1.1.0/bioconvert/core/benchmark.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,27 @@
 #                                                                         #
 # Repository: https://github.com/bioconvert/bioconvert                    #
 # Documentation: http://bioconvert.readthedocs.io                         #
 ###########################################################################
 """Tools for benchmarking"""
 
 import statistics
+import threading
+import time
 
 import colorlog
 import matplotlib.pyplot as plt
 import pandas as pd
 import pylab
 import statsmodels.api
 import statsmodels.formula.api
 import statsmodels.stats.multitest
 from bioconvert.core.utils import Timer
 from tqdm import tqdm
+import psutil
 
 _log = colorlog.getLogger(__name__)
 
 
 __all__ = ["Benchmark", "plot_multi_benchmark_max"]
 
 
@@ -76,69 +79,115 @@
         else:
             self.to_exclude = to_exclude
         if to_include is None:
             self.to_include = []
         else:
             self.to_include = to_include
 
+        # CPU and memory usage
+        self.cpu_percent = []
+        self.memory_usage = []
+
     def run_methods(self):
         """Runs the benchmarks, and stores the timings in *self.results*."""
-        results = {}
+        results = {"time": {}, "CPU": {}, "memory": {}}
         methods = self.converter.available_methods[:]  # a copy !
 
         if self.to_include:
             methods = [x for x in methods if x in self.to_include]
         elif self.to_exclude:
             methods = [x for x in methods if x not in self.to_exclude]
 
         for method in methods:
             times = []
+            CPUs = []
+            MEMs = []
+
             for i in tqdm(range(self.N), desc="Evaluating method {}".format(method)):
                 with Timer(times):
                     # Need to get all extra arguments for specify method e.g Bam2BIGWIG.uscs method
                     kwargs = {"method": method}
                     for k, v in self.converter.others.items():
                         kwargs[k] = v
+
+                    # start monitoring CPU and Memory usage
+                    self.stop_monitoring = False
+
+                    # reset CPU and memory usage before monitoring
+                    self.cpu_percent = []
+                    self.memory_usage = []
+
+                    # start monitoring
+                    monitor_thread = threading.Thread(target=self.monitor_usage)
+                    monitor_thread.start()
+
+                    # the actual computation
                     self.converter(**kwargs)
-            results[method] = times
+
+                    # stop monitoring
+                    self.stop_monitoring = True
+                    monitor_thread.join()
+
+                    # gather information
+                    L = len(self.cpu_percent)
+                    CPUs.append(sum(self.cpu_percent) / L)
+                    MEMs.append(sum(self.memory_usage) / L)
+            results["CPU"][method] = CPUs
+            results["memory"][method] = MEMs
+            results["time"][method] = times
+
         self.results = results
 
-    def plot(self, rerun=False, ylabel="Time (seconds)", rot_xticks=0, boxplot_args={}):
+    def monitor_usage(self):
+        while not self.stop_monitoring:
+            # Retrieve CPU and memory usage
+            cpu_percent = psutil.cpu_percent()
+            memory_usage = psutil.virtual_memory().percent
+
+            # Adjust the sleep time as per your requirement
+            time.sleep(0.05)
+            self.cpu_percent.append(cpu_percent)
+            self.memory_usage.append(memory_usage)
+
+    def plot(self, rerun=False, ylabel="Time (seconds)", rot_xticks=0, boxplot_args={}, mode="time"):
         """Plots the benchmark results, running the benchmarks
         if needed or if *rerun* is True.
 
         :param rot_xlabel: rotation of the xticks function
         :param boxplot_args: dictionary with any of the pylab.boxplot arguments
+        :param mode: either time, CPU or memory
         :return: dataframe with all results
         """
 
         if self.results is None or rerun is True:
             self.run_methods()
 
-        # an alias.
-        data = self.results.copy()
+
+        assert mode in ["time", "CPU", "memory"], f"mode must be time, CPU or memory; {mode} provided"
+        data = self.results[mode].copy()
+
 
         methods = sorted(data, key=lambda x: pylab.mean(data[x]))
         pylab.boxplot([data[x] for x in methods], **boxplot_args)
         # pylab.xticks([1+this for this in range(len(methods))], methods)
         if "vert" in boxplot_args and boxplot_args["vert"] is False:
             pylab.yticks(*zip(*enumerate(methods, start=1)), rotation=rot_xticks)
             pylab.xlabel(ylabel)
         else:
             pylab.xticks(*zip(*enumerate(methods, start=1)), rotation=rot_xticks)
             pylab.ylabel(ylabel)
             pylab.xlim([0, len(methods) + 1])
-
         pylab.grid(True)
         pylab.tight_layout()
 
-        return data
+        # make sure it does not change with a copy
+        return self.results.copy()
 
 
-def plot_multi_benchmark_max(path_json, output_filename="multi_benchmark.png", min_ylim=0):
+def plot_multi_benchmark_max(path_json, output_filename="multi_benchmark.png", min_ylim=0, mode=None):
     """Plotting function for the Snakefile_benchmark to be found in the doc
 
     The json file looks like::
 
 
         {
           "awk":{
@@ -160,16 +209,25 @@
             "3":2
           }
         }
 
     Number of benchmark is infered from field 'Benchmark'.
 
     """
-    # open and read JSON file
-    df = pd.read_json(path_json)
+
+
+    # for back compatibility with 1.0.0
+
+    if mode is None:
+        # open and read JSON file
+        df = pd.read_json(path_json)
+    else:
+        with open(path_json, "r") as fin:
+            dd = json.loads(fin.read())
+            df = pd.DataFrame(dd[mode])
 
     # how many runs per method ?
     N = len(df["Benchmark"]) / len(df["Benchmark"].unique())
     N = len(df["Benchmark"]) / N
 
     # Retrieving method names
     methods = list(df)
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/converter.py` & `bioconvert-1.1.0/bioconvert/core/converter.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/decorators.py` & `bioconvert-1.1.0/bioconvert/core/decorators.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/downloader.py` & `bioconvert-1.1.0/bioconvert/core/downloader.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/extensions.py` & `bioconvert-1.1.0/bioconvert/core/extensions.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/graph.py` & `bioconvert-1.1.0/bioconvert/core/graph.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/init.py` & `bioconvert-1.1.0/bioconvert/core/init.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/levenshtein.py` & `bioconvert-1.1.0/bioconvert/core/levenshtein.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/registry.py` & `bioconvert-1.1.0/bioconvert/core/registry.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/shell.py` & `bioconvert-1.1.0/bioconvert/core/shell.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/core/utils.py` & `bioconvert-1.1.0/bioconvert/core/utils.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/cram2bam.py` & `bioconvert-1.1.0/bioconvert/cram2bam.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/cram2fasta.py` & `bioconvert-1.1.0/bioconvert/cram2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/cram2fastq.py` & `bioconvert-1.1.0/bioconvert/cram2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/cram2sam.py` & `bioconvert-1.1.0/bioconvert/cram2sam.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/csv2tsv.py` & `bioconvert-1.1.0/bioconvert/csv2tsv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/csv2xls.py` & `bioconvert-1.1.0/bioconvert/csv2xls.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,20 @@
 
         writer = pd.ExcelWriter(self.outfile, engine="openpyxl")
         pd.read_csv(self.infile, sep=in_sep, header="infer",).to_excel(
             excel_writer=writer,
             sheet_name=sheet_name,
             index=False,
         )
-        writer.save()
+
+        # depends on pandas/pyexcel version. need to cope with the two cases
+        try:
+            writer.save()
+        except AttributeError:
+            writer._save()
 
     @classmethod
     def get_additional_arguments(cls):
         yield ConvArg(
             names=[
                 "--sheet-name",
             ],
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/data/README.rst` & `bioconvert-1.1.0/bioconvert/data/README.rst`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/data/test.bigwig` & `bioconvert-1.1.0/bioconvert/data/test.bigwig`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/data/test_SP1.fq.gz` & `bioconvert-1.1.0/bioconvert/data/test_SP1.fq.gz`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/data/test_gfa2fasta_v1.gfa` & `bioconvert-1.1.0/bioconvert/data/test_gfa2fasta_v1.gfa`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/data/test_measles.sorted.bam` & `bioconvert-1.1.0/bioconvert/data/test_measles.sorted.bam`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/dsrc2gz.py` & `bioconvert-1.1.0/bioconvert/dsrc2gz.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/embl2fasta.py` & `bioconvert-1.1.0/bioconvert/embl2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/embl2genbank.py` & `bioconvert-1.1.0/bioconvert/embl2genbank.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2clustal.py` & `bioconvert-1.1.0/bioconvert/fasta2clustal.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2faa.py` & `bioconvert-1.1.0/bioconvert/fasta2faa.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2fasta_agp.py` & `bioconvert-1.1.0/bioconvert/fasta2fasta_agp.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2fastq.py` & `bioconvert-1.1.0/bioconvert/fasta2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2genbank.py` & `bioconvert-1.1.0/bioconvert/fasta2genbank.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2nexus.py` & `bioconvert-1.1.0/bioconvert/fasta2nexus.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2phylip.py` & `bioconvert-1.1.0/bioconvert/fasta2phylip.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta2twobit.py` & `bioconvert-1.1.0/bioconvert/fasta2twobit.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fasta_qual2fastq.py` & `bioconvert-1.1.0/bioconvert/fasta_qual2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fastq2fasta.py` & `bioconvert-1.1.0/bioconvert/fastq2fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     # use readfq for now because pure python are fast enough
     # for production, could use seqtk which seems the fastest method
     # though. Make sure that the default handles also the compresssion
     # input_ext = extensions.extensions.fastq
     # output_ext =  extensions.fasta
     #: default value
     _default_method = "bioconvert"
+    _loss = True
     _threading = True  # not used but required for the main benchmark
 
     def __init__(self, infile, outfile):
         """
         :param str infile: The path to the input FASTA file.
         :param str outfile: The path to the output file.
         """
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/fastq2fasta_qual.py` & `bioconvert-1.1.0/bioconvert/fastq2fasta_qual.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/fastq2qual.py` & `bioconvert-1.1.0/bioconvert/fastq2qual.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     """Convert :term:`FASTQ` to :term:`QUAL`"""
 
     # use readfq for now because pure python are fast enough
     # for production, could use seqtk which seems the fastest method though
     # Make sure that the default handles also the compresssion
     #: Default value
     _default_method = "readfq"
+    _loss = True
 
     # (https://raw.githubusercontent.com/lh3/readfq/master/readfq.py)
     @staticmethod
     def _readfq(fp):  # this is a generator function
         last = None  # this is a buffer keeping the last unprocessed line
         while True:  # mimic closure; is it a bad idea?
             if not last:  # the first record or a record following a fastq
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/genbank2embl.py` & `bioconvert-1.1.0/bioconvert/genbank2embl.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/genbank2fasta.py` & `bioconvert-1.1.0/bioconvert/genbank2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/genbank2gff3.py` & `bioconvert-1.1.0/bioconvert/genbank2gff3.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gfa2fasta.py` & `bioconvert-1.1.0/bioconvert/gfa2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gff22gff3.py` & `bioconvert-1.1.0/bioconvert/gff22gff3.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gff32gff2.py` & `bioconvert-1.1.0/bioconvert/gff32gff2.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gff32gtf.py` & `bioconvert-1.1.0/bioconvert/gff32gtf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gtf22gff3.py` & `bioconvert-1.1.0/bioconvert/gtf22gff3.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gz2bz2.py` & `bioconvert-1.1.0/bioconvert/gz2bz2.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/gz2dsrc.py` & `bioconvert-1.1.0/bioconvert/gz2dsrc.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/fasta.py` & `bioconvert-1.1.0/bioconvert/io/fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/genbank.py` & `bioconvert-1.1.0/bioconvert/io/genbank.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/gff2.py` & `bioconvert-1.1.0/bioconvert/io/gff2.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/gff3.py` & `bioconvert-1.1.0/bioconvert/io/gff3.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/maf.py` & `bioconvert-1.1.0/bioconvert/io/maf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/io/scf.py` & `bioconvert-1.1.0/bioconvert/io/scf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/json2yaml.py` & `bioconvert-1.1.0/bioconvert/json2yaml.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/maf2sam.py` & `bioconvert-1.1.0/bioconvert/maf2sam.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/misc/cython_fastq2fasta.pyx` & `bioconvert-1.1.0/bioconvert/misc/cython_fastq2fasta.pyx`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/misc/fastq2fasta.c` & `bioconvert-1.1.0/bioconvert/misc/fastq2fasta.c`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/misc/fastq2fasta.pl` & `bioconvert-1.1.0/bioconvert/misc/fastq2fasta.pl`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/misc/install_goalign.sh` & `bioconvert-1.1.0/bioconvert/misc/install_goalign.sh`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/misc/install_gotree.sh` & `bioconvert-1.1.0/bioconvert/misc/install_gotree.sh`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/newick2nexus.py` & `bioconvert-1.1.0/bioconvert/newick2nexus.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/newick2phyloxml.py` & `bioconvert-1.1.0/bioconvert/newick2phyloxml.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/nexus2clustal.py` & `bioconvert-1.1.0/bioconvert/nexus2clustal.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/nexus2fasta.py` & `bioconvert-1.1.0/bioconvert/nexus2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/nexus2newick.py` & `bioconvert-1.1.0/bioconvert/nexus2newick.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/nexus2phylip.py` & `bioconvert-1.1.0/bioconvert/nexus2phylip.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/nexus2phyloxml.py` & `bioconvert-1.1.0/bioconvert/nexus2phyloxml.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/ods2csv.py` & `bioconvert-1.1.0/bioconvert/ods2csv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/pdb2faa.py` & `bioconvert-1.1.0/bioconvert/pdb2faa.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phylip2clustal.py` & `bioconvert-1.1.0/bioconvert/phylip2clustal.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phylip2fasta.py` & `bioconvert-1.1.0/bioconvert/phylip2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phylip2nexus.py` & `bioconvert-1.1.0/bioconvert/phylip2nexus.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phylip2stockholm.py` & `bioconvert-1.1.0/bioconvert/phylip2stockholm.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phylip2xmfa.py` & `bioconvert-1.1.0/bioconvert/phylip2xmfa.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phyloxml2newick.py` & `bioconvert-1.1.0/bioconvert/phyloxml2newick.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/phyloxml2nexus.py` & `bioconvert-1.1.0/bioconvert/phyloxml2nexus.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/plink2bplink.py` & `bioconvert-1.1.0/bioconvert/plink2bplink.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/plink2vcf.py` & `bioconvert-1.1.0/bioconvert/plink2vcf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/sam2bam.py` & `bioconvert-1.1.0/bioconvert/sam2bam.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/sam2cram.py` & `bioconvert-1.1.0/bioconvert/sam2cram.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/sam2paf.py` & `bioconvert-1.1.0/bioconvert/sam2paf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/scf2fasta.py` & `bioconvert-1.1.0/bioconvert/scf2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/scf2fastq.py` & `bioconvert-1.1.0/bioconvert/scf2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/scripts/converter.py` & `bioconvert-1.1.0/bioconvert/scripts/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,22 +601,26 @@
             "method",
             "show_methods",
             "converter",
             "raise_exception",
             "batch",
             "benchmark",
             "benchmark_N",
+            "benchmark_mode",
             "benchmark_methods",
         ]:
             bioconv.converter.others[k] = v
 
     if args.benchmark:
-        results = bioconv.converter.boxplot_benchmark(N=args.benchmark_N, to_include=args.benchmark_methods)
+
+        bioconv.converter.compute_benchmark(N=args.benchmark_N, to_include=args.benchmark_methods)
         import pylab
 
+        results = bioconv.converter.boxplot_benchmark(mode=args.benchmark_mode)
+
         json_file = Path(f"{args.benchmark_tag}.json")
         json_file.parent.mkdir(parents=True, exist_ok=True)
 
         if args.benchmark_save_image:
             pylab.savefig(f"{args.benchmark_tag}.png", dpi=200)
             logger.info(f"File {args.benchmark_tag}.png created")
```

### Comparing `bioconvert-1.0.0.post0/bioconvert/scripts/init_convert.py` & `bioconvert-1.1.0/bioconvert/scripts/init_convert.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/scripts/stats.py` & `bioconvert-1.1.0/bioconvert/scripts/stats.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/simulator/fasta.py` & `bioconvert-1.1.0/bioconvert/simulator/fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/simulator/fastq.py` & `bioconvert-1.1.0/bioconvert/simulator/fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/simulator/gfa.py` & `bioconvert-1.1.0/bioconvert/simulator/gfa.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/sra2fastq.py` & `bioconvert-1.1.0/bioconvert/sra2fastq.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/stockholm2clustal.py` & `bioconvert-1.1.0/bioconvert/stockholm2clustal.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/stockholm2phylip.py` & `bioconvert-1.1.0/bioconvert/stockholm2phylip.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/tsv2csv.py` & `bioconvert-1.1.0/bioconvert/tsv2csv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/twobit2fasta.py` & `bioconvert-1.1.0/bioconvert/twobit2fasta.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/annotation.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/annotation.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/convert_genbank_to_gff3.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/convert_genbank_to_gff3.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/gff.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/gff.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/tbl.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/tbl.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/things.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/things.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/utils/biocode/utils.py` & `bioconvert-1.1.0/bioconvert/utils/biocode/utils.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/vcf2bcf.py` & `bioconvert-1.1.0/bioconvert/vcf2bcf.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/vcf2bed.py` & `bioconvert-1.1.0/bioconvert/vcf2bed.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/vcf2bplink.py` & `bioconvert-1.1.0/bioconvert/vcf2bplink.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/vcf2plink.py` & `bioconvert-1.1.0/bioconvert/vcf2plink.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/vcf2wiggle.py` & `bioconvert-1.1.0/bioconvert/vcf2wiggle.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/wig2bed.py` & `bioconvert-1.1.0/bioconvert/wig2bed.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/xls2csv.py` & `bioconvert-1.1.0/bioconvert/xls2csv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/xlsx2csv.py` & `bioconvert-1.1.0/bioconvert/xlsx2csv.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/xmfa2phylip.py` & `bioconvert-1.1.0/bioconvert/xmfa2phylip.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert/yaml2json.py` & `bioconvert-1.1.0/bioconvert/yaml2json.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/bioconvert.egg-info/PKG-INFO` & `bioconvert-1.1.0/bioconvert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,608 +1,19 @@
 Metadata-Version: 2.1
 Name: bioconvert
-Version: 1.0.0.post0
+Version: 1.1.0
 Summary: convert between bioinformatics formats
 Home-page: https://github.com/bioconvert/bioconvert
+Download-URL: https://github.com/bioconvert/bioconvert
 Author: The bioconvert Contributors
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: Thomas Cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: GPLv3
-Download-URL: https://github.com/bioconvert/bioconvert
-Description: Bioconvert
-        ##########
-        
-        **Bioconvert** is a collaborative project to facilitate the interconversion of life science data from one format to another.
-        
-        .. image:: https://badge.fury.io/py/bioconvert.svg
-            :target: https://pypi.python.org/pypi/bioconvert
-        
-        .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml/badge.svg?branch=main
-            :target: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/github/bioconvert/bioconvert/badge.svg?branch=main
-           :target: https://coveralls.io/github/bioconvert/bioconvert?branch=main
-        
-        .. image:: http://readthedocs.org/projects/bioconvert/badge/?version=main
-            :target: http://bioconvert.readthedocs.org/en/main/?badge=main
-            :alt: Documentation Status
-        
-        .. image::  https://img.shields.io/github/issues/bioconvert/bioconvert.svg
-            :target:  https://github.com/bioconvert/bioconvert/issues
-        
-        .. image:: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
-           :target: https://anaconda.org/bioconda/bioconvert
-        
-        .. image::  https://anaconda.org/bioconda/bioconvert/badges/version.svg
-            :target: https://anaconda.org/bioconda/bioconvert/badges/version.svg
-        
-        .. image:: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
-            :target: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
-        
-        .. image:: https://zenodo.org/badge/106598809.svg
-           :target: https://zenodo.org/badge/latestdoi/106598809
-        
-        .. image:: https://static.pepy.tech/personalized-badge/bioconvert?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/months
-            :target: https://pepy.tech/project/bioconvert
-        
-        .. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
-            :target: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
-        
-        
-        :contributions: Want to add a convertor ? Please join https://github.com/bioconvert/bioconvert/issues/1
-        
-        Overview
-        ########
-        
-        
-        Life science uses many different formats. They may be old, or with complex syntax and converting those formats may be a challenge. Bioconvert aims at providing a common tool / interface to convert life science data formats from one to another.
-        
-        Many conversion tools already exist but they may be dispersed, focused on few specific formats, difficult to install, or not optimised. With Bioconvert, we plan to cover a wide spectrum of format conversions; we will re-use existing tools when possible and provide facilities to compare different conversion tools or methods via benchmarking. New implementations are provided when considered better than existing ones.
-        
-        In Jan 2023, we had 50 formats, 100 direct conversions available.
-        
-        .. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/conversion.png
-            :width: 80%
-        
-        
-        Installation
-        ###############
-        
-        **BioConvert** is developped in Python. Please use conda or any Python environment manager to install **BioConvert** using the **pip** command::
-        
-            pip install bioconvert
-        
-        50% of the conversions should work out of the box. However, many conversions require external tools. This is why we
-        recommend to use a **conda** environment. In particular, most external tools are available on the **bioconda** channel. 
-        For instance if you want to convert a SAM file to a BAM file you would need to install **samtools** as follow::
-        
-            conda install -c bioconda samtools
-        
-        Since **bioconvert** is available on `bioconda <https://bioconda.github.io>`_ on solution that installs **BioConvert** and all its dependencies is to use conda/mamba::
-        
-            conda env create --name bioconvert mamba
-            conda activate bioconvert
-            mamba install bioconvert
-            bioconvert --help
-        
-        See the Installation section for more details and alternative solutions (docker, singularity).
-        
-        Quick Start
-        ##############
-        There are many conversions available. Type::
-        
-            bioconvert --help 
-        
-        to get a list of valid method of conversions. Taking the example of a conversion from a `FastQ` file into
-        a `FastA` file, you could do the conversion as follows::
-        
-            bioconvert fastq2fasta input.fastq output.fasta
-            bioconvert fastq2fasta input.fq    output.fasta
-            bioconvert fastq2fasta input.fq.gz output.fasta.gz
-            bioconvert fastq2fasta input.fq.gz output.fasta.bz2
-        
-        When there is no ambiguity, you can be implicit::
-        
-             bioconvert input.fastq output.fasta
-        
-        The default method of conversion is used but you may use another one. Checkout the available methods with::
-        
-            bioconvert fastq2fasta --show-methods
-        
-        For more help about a conversion, just type::
-        
-            bioconvert fastq2fasta --help
-        
-        and more generally::
-        
-            bioconvert --help
-        
-        
-        You may also call **BioConvert** from a Python shell::
-        
-            # import a converter
-            from bioconvert.fastq2fasta import FASTQ2FASTA
-        
-            # Instanciate with infile/outfile names
-            convert = FASTQ2FASTA(infile, outfile)
-        
-            # the conversion itself:
-            convert()
-        
-        
-        Available Converters
-        #######################
-        
-        
-        .. list-table:: Conversion table
-            :widths: 20 40 40
-            :header-rows: 1
-        
-            * - Converters
-              - CI testing
-              - Default method
-            * - `abi2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `abi2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `abi2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bedgraph>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml
-              - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bigwig>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cov>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml
-              - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cram>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2json>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml
-              - `BAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml
-              - `SAMBAMBA <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2tsv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bam2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bcf2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml
-              - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bed2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2bigwig>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml
-              - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2cov>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bedgraph2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigbed2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigbed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigwig2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2bedgraph>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bigwig2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bplink2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2plink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bplink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `bz22gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bz22gz>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml
-              - Unix commands
-            * - `clustal2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `clustal2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2stockholm>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2bam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `cram2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `csv2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2tsv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `csv2xls <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2xls>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml
-              - Pandas
-            * - `dsrc2gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.dsrc2gz>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml
-              - DSRC software
-            * - `embl2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `embl2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2genbank>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2faa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2fasta_agp <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fasta_agp>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml
-              - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2genbank>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta2twobit <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2twobit>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml
-              - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fasta_qual2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta_qual2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml
-              - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fastq2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml
-              -  `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_  `available <_static/benchmark_fastq2fasta.png>`_
-            * - `fastq2fasta_qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta_qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `fastq2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2qual>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml
-              - `READFQ <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2embl <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2embl>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `genbank2gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2gff3>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml
-              - `BIOCODE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gfa2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gfa2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff22gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff22gff3>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff32gff2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gff2>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gff32gtf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gtf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `gz2bz2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2bz2>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml
-              - pigz/pbzip2 software
-            * - `gz2dsrc <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2dsrc>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml
-              - DSRC software
-            * - `json2yaml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.json2yaml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml
-              - Python
-            * - `maf2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.maf2sam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `newick2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `newick2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2phyloxml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2newick>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `nexus2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phyloxml>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `ods2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.ods2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml
-              - pyexcel library
-            * - `pdb2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.pdb2faa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml
-              - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2stockholm>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phylip2xmfa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2xmfa>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phyloxml2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2newick>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `phyloxml2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2nexus>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml
-              - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `plink2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2bplink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `plink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2vcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2bam>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2cram>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml
-              - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sam2paf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2paf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `scf2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `scf2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `sra2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sra2fastq>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml
-              - `FASTQDUMP <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `stockholm2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2clustal>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `stockholm2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `tsv2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.tsv2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `twobit2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.twobit2fasta>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml
-              - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bcf>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml
-              - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml
-              - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bplink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2plink>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml
-              - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `vcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2wiggle>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml
-              - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `wig2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.wig2bed>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml
-              - `BEDOPS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `xls2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xls2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml
-              -
-            * - `xlsx2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xlsx2csv>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml
-              - Pandas library
-            * - `xmfa2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xmfa2phylip>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml
-              - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
-            * - `yaml2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.yaml2json>`_
-              - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml/badge.svg
-                    :target: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml
-              - Pandas library
-        
-        
-        
-        Contributors
-        ############
-        
-        Setting up and maintaining Bioconvert has been possible thanks to users and contributors.
-        Thanks to all:
-        
-        .. image:: https://contrib.rocks/image?repo=bioconvert/bioconvert
-            :target: https://github.com/bioconvert/bioconvert/graphs/contributors
-        
-        
-        Changes
-        ########
-        
-        ========= ==============================================================================
-        Version   Description
-        ========= ==============================================================================
-        1.0.0     * Fix bam2fastq for paired data that computed useless intermediate file
-                    https://github.com/bioconvert/bioconvert/issues/325
-                  * more realistic fastq simulator
-                  * pin openpyxl to <=3.0.10 to prevent regression error in v3.1.0
-        0.6.3     * add picard method in bam2sam
-                  * Fixed all CI workflows to use mamba
-                  * drop python3.7 support and add 3.10 support
-                  * update bedops test file to fit the latest bedops 2.4.41 version
-                  * revisit logging system
-        0.6.2     * added gff3 to gtf conversion. 
-                  * Added pdb to faa conversion
-                  * Added missing --reference argument to the cram2sam conversion
-        0.6.1     * output file can be in sub-directories allowing syntax such as 
-                    'bioconvert fastq2fasta test.fastq outputs/test.fasta
-                  * fix all CI actions
-                  * add more examples as notebooks in ./examples
-                  * add a Snakefile for the paper in ./doc/Snakefile_paper
-        0.6.0     * Fix bug in bam2sam (method sambamba)
-                  * Fix graph layout
-                  * add threading in fastq2fasta (seqkit method)
-                  * multibenchmark feature added
-                  * stable version used for web interface
-        0.5.2     * Update requirements and environment.yml and add a conda spec-file.txt file
-        0.5.1     * add genbank2gff3 requirement material in bioconvert.utils.biocode
-        0.5.0     * Add CI actions for all converters
-                  * remove sniffer (now in biosniff on pypi https://pypi.org/project/biosniff/)
-                  * A complete benchmarking suite (see doc/Snakefile_benchmark file and
-                    `benchmarking`)
-                  * documentation and tests for all converters
-                  * removed the validators (we assume intputs are correct)
-        0.4.X     * (aug 2019) added nexus2fasta, cram2fasta, fasta2faa ... ; 1-to-many and 
-                    many-to-one converters are now part of the API.
-        0.3.X       may 2019. new methods abi2qual, bigbed2bed, etc. added --threads option
-        0.2.X       aug 2018. abi2fastx, bioconvert_stats tool added
-        0.1.X       major refactoring to  have subcommands with implicit/explicit mode
-        ========= ==============================================================================
-        
-        
-Keywords: NGS,bam2bed,fastq2fasta,bam2sam
+Keywords: NGS,bam2bed,fastq2fasta,bam2sam,conversion
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -614,7 +25,600 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: doc
+License-File: COPYING
+
+Bioconvert
+##########
+
+**Bioconvert** is a collaborative project to facilitate the interconversion of life science data from one format to another.
+
+.. image:: https://badge.fury.io/py/bioconvert.svg
+    :target: https://pypi.python.org/pypi/bioconvert
+
+.. image:: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml/badge.svg?branch=main
+    :target: https://github.com/bioconvert/bioconvert/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/bioconvert/bioconvert/badge.svg?branch=main
+   :target: https://coveralls.io/github/bioconvert/bioconvert?branch=main
+
+.. image:: http://readthedocs.org/projects/bioconvert/badge/?version=main
+    :target: http://bioconvert.readthedocs.org/en/main/?badge=main
+    :alt: Documentation Status
+
+.. image::  https://img.shields.io/github/issues/bioconvert/bioconvert.svg
+    :target:  https://github.com/bioconvert/bioconvert/issues
+
+.. image:: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
+   :target: https://anaconda.org/bioconda/bioconvert/badges/platforms.svg
+
+.. image::  https://anaconda.org/bioconda/bioconvert/badges/version.svg
+    :target: https://anaconda.org/bioconda/bioconvert
+
+.. image:: https://anaconda.org/bioconda/bioconvert/badges/downloads.svg
+    :target: https://github.com/bioconvert/bioconvert/releases
+
+.. image:: https://zenodo.org/badge/106598809.svg
+   :target: https://zenodo.org/badge/latestdoi/106598809
+
+.. image:: https://static.pepy.tech/personalized-badge/bioconvert?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/months
+    :target: https://pepy.tech/project/bioconvert
+
+.. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
+    :target: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/_static/logo_300x200.png
+
+
+:contributions: Want to add a convertor ? Please join https://github.com/bioconvert/bioconvert/issues/1
+
+Overview
+########
+
+
+Life science uses many different formats. They may be old, or with complex syntax and converting those formats may be a challenge. Bioconvert aims at providing a common tool / interface to convert life science data formats from one to another.
+
+Many conversion tools already exist but they may be dispersed, focused on few specific formats, difficult to install, or not optimised. With Bioconvert, we plan to cover a wide spectrum of format conversions; we will re-use existing tools when possible and provide facilities to compare different conversion tools or methods via benchmarking. New implementations are provided when considered better than existing ones.
+
+In Jan 2023, we had 50 formats, 100 direct conversions available.
+
+.. image:: https://raw.githubusercontent.com/bioconvert/bioconvert/main/doc/conversion.png
+    :width: 80%
+
+
+Installation
+###############
+
+**BioConvert** is developped in Python. Please use conda or any Python environment manager to install **BioConvert** using the **pip** command::
+
+    pip install bioconvert
+
+50% of the conversions should work out of the box. However, many conversions require external tools. This is why we
+recommend to use a **conda** environment. In particular, most external tools are available on the **bioconda** channel. 
+For instance if you want to convert a SAM file to a BAM file you would need to install **samtools** as follow::
+
+    conda install -c bioconda samtools
+
+Since **bioconvert** is available on `bioconda <https://bioconda.github.io>`_ on solution that installs **BioConvert** and all its dependencies is to use conda/mamba::
+
+    conda env create --name bioconvert mamba
+    conda activate bioconvert
+    mamba install bioconvert
+    bioconvert --help
+
+See the Installation section for more details and alternative solutions (docker, singularity).
+
+Quick Start
+##############
+There are many conversions available. Type::
+
+    bioconvert --help 
+
+to get a list of valid method of conversions. Taking the example of a conversion from a `FastQ` file into
+a `FastA` file, you could do the conversion as follows::
+
+    bioconvert fastq2fasta input.fastq output.fasta
+    bioconvert fastq2fasta input.fq    output.fasta
+    bioconvert fastq2fasta input.fq.gz output.fasta.gz
+    bioconvert fastq2fasta input.fq.gz output.fasta.bz2
+
+When there is no ambiguity, you can be implicit::
+
+     bioconvert input.fastq output.fasta
+
+The default method of conversion is used but you may use another one. Checkout the available methods with::
+
+    bioconvert fastq2fasta --show-methods
+
+For more help about a conversion, just type::
+
+    bioconvert fastq2fasta --help
+
+and more generally::
+
+    bioconvert --help
+
+
+You may also call **BioConvert** from a Python shell::
+
+    # import a converter
+    from bioconvert.fastq2fasta import FASTQ2FASTA
+
+    # Instanciate with infile/outfile names
+    convert = FASTQ2FASTA(infile, outfile)
+
+    # the conversion itself:
+    convert()
+
+
+Available Converters
+#######################
+
+
+.. list-table:: Conversion table
+    :widths: 20 40 40
+    :header-rows: 1
+
+    * - Converters
+      - CI testing
+      - Default method
+    * - `abi2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `abi2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2fastq.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `abi2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.abi2qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/abi2qual.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bedgraph>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bedgraph.yml
+      - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2bigwig>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2bigwig.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cov>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cov.yml
+      - `BEDTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2cram>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2cram.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fasta.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2fastq.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2json>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2json.yml
+      - `BAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2sam.yml
+      - `SAMBAMBA <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2tsv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2tsv.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bam2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bam2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bam2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bcf2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2vcf.yml
+      - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bcf2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bcf2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bed2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bed2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2bigwig <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2bigwig>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2bigwig.yml
+      - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2cov <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2cov>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2cov.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bedgraph2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bedgraph2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bedgraph2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigbed2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2bed.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigbed2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigbed2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigbed2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigwig2bedgraph <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2bedgraph>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2bedgraph.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bigwig2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bigwig2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bigwig2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bplink2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2plink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2plink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bplink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bplink2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bplink2vcf.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `bz22gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.bz22gz>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/bz22gz.yml
+      - Unix commands
+    * - `clustal2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `clustal2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.clustal2stockholm>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/clustal2stockholm.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2bam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2bam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fasta.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2fastq.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `cram2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.cram2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/cram2sam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `csv2tsv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2tsv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2tsv.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `csv2xls <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.csv2xls>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/csv2xls.yml
+      - Pandas
+    * - `dsrc2gz <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.dsrc2gz>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/dsrc2gz.yml
+      - DSRC software
+    * - `embl2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `embl2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.embl2genbank>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/embl2genbank.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2faa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2faa.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2fasta_agp <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fasta_agp>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fasta_agp.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2fastq.yml
+      - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2genbank <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2genbank>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2genbank.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta2twobit <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta2twobit>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta2twobit.yml
+      - `UCSC <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fasta_qual2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fasta_qual2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fasta_qual2fastq.yml
+      - `PYSAM <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fastq2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta.yml
+      -  `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_  `available <_static/benchmark_fastq2fasta.png>`_
+    * - `fastq2fasta_qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2fasta_qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2fasta_qual.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `fastq2qual <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.fastq2qual>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/fastq2qual.yml
+      - `READFQ <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2embl <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2embl>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2embl.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `genbank2gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.genbank2gff3>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/genbank2gff3.yml
+      - `BIOCODE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gfa2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gfa2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gfa2fasta.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff22gff3 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff22gff3>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff22gff3.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff32gff2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gff2>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gff2.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gff32gtf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gff32gtf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gff32gtf.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `gz2bz2 <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2bz2>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2bz2.yml
+      - pigz/pbzip2 software
+    * - `gz2dsrc <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.gz2dsrc>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/gz2dsrc.yml
+      - DSRC software
+    * - `json2yaml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.json2yaml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/json2yaml.yml
+      - Python
+    * - `maf2sam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.maf2sam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/maf2sam.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `newick2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2nexus.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `newick2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.newick2phyloxml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/newick2phyloxml.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2clustal.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2newick>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2newick.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phylip.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `nexus2phyloxml <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.nexus2phyloxml>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/nexus2phyloxml.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `ods2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.ods2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/ods2csv.yml
+      - pyexcel library
+    * - `pdb2faa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.pdb2faa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/pdb2faa.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2fasta.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2nexus.yml
+      - `GOALIGN <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2stockholm <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2stockholm>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2stockholm.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phylip2xmfa <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phylip2xmfa>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phylip2xmfa.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phyloxml2newick <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2newick>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2newick.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `phyloxml2nexus <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.phyloxml2nexus>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/phyloxml2nexus.yml
+      - `GOTREE <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `plink2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2bplink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2bplink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `plink2vcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.plink2vcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/plink2vcf.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2bam <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2bam>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2bam.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2cram <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2cram>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2cram.yml
+      - `SAMTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sam2paf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sam2paf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sam2paf.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `scf2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fasta.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `scf2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.scf2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/scf2fastq.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `sra2fastq <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.sra2fastq>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/sra2fastq.yml
+      - `FASTQDUMP <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `stockholm2clustal <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2clustal>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2clustal.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `stockholm2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.stockholm2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/stockholm2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `tsv2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.tsv2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/tsv2csv.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `twobit2fasta <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.twobit2fasta>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/twobit2fasta.yml
+      - `DEEPTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bcf <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bcf>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bcf.yml
+      - `BCFTOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bed.yml
+      - `BIOCONVERT <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2bplink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2bplink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2bplink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2plink <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2plink>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2plink.yml
+      - `PLINK <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `vcf2wiggle <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.vcf2wiggle>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/vcf2wiggle.yml
+      - `WIGGLETOOLS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `wig2bed <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.wig2bed>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/wig2bed.yml
+      - `BEDOPS <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `xls2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xls2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xls2csv.yml
+      -
+    * - `xlsx2csv <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xlsx2csv>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xlsx2csv.yml
+      - Pandas library
+    * - `xmfa2phylip <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.xmfa2phylip>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/xmfa2phylip.yml
+      - `BIOPYTHON <https://bioconvert.readthedocs.io/en/main/bibliography.html>`_
+    * - `yaml2json <https://bioconvert.readthedocs.io/en/main/ref_converters.html#module-bioconvert.yaml2json>`_
+      - .. image:: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml/badge.svg
+            :target: https://github.com/bioconvert/bioconvert/actions/workflows/yaml2json.yml
+      - Pandas library
+
+
+
+Contributors
+############
+
+Setting up and maintaining Bioconvert has been possible thanks to users and contributors.
+Thanks to all:
+
+.. image:: https://contrib.rocks/image?repo=bioconvert/bioconvert
+    :target: https://github.com/bioconvert/bioconvert/graphs/contributors
+
+
+Changes
+########
+
+========= ==============================================================================
+Version   Description
+========= ==============================================================================
+1.1.0     * Implement ability to benchmark the CPU and memory usage (not just time)
+            benchmark incorporates CPU/memory usage
+          * add missing cython in requirements (and psutil for benchmarking)
+1.0.0     * Fix bam2fastq for paired data that computed useless intermediate file
+            https://github.com/bioconvert/bioconvert/issues/325
+          * more realistic fastq simulator
+          * pin openpyxl to <=3.0.10 to prevent regression error in v3.1.0
+0.6.3     * add picard method in bam2sam
+          * Fixed all CI workflows to use mamba
+          * drop python3.7 support and add 3.10 support
+          * update bedops test file to fit the latest bedops 2.4.41 version
+          * revisit logging system
+0.6.2     * added gff3 to gtf conversion. 
+          * Added pdb to faa conversion
+          * Added missing --reference argument to the cram2sam conversion
+0.6.1     * output file can be in sub-directories allowing syntax such as 
+            'bioconvert fastq2fasta test.fastq outputs/test.fasta
+          * fix all CI actions
+          * add more examples as notebooks in ./examples
+          * add a Snakefile for the paper in ./doc/Snakefile_paper
+0.6.0     * Fix bug in bam2sam (method sambamba)
+          * Fix graph layout
+          * add threading in fastq2fasta (seqkit method)
+          * multibenchmark feature added
+          * stable version used for web interface
+0.5.2     * Update requirements and environment.yml and add a conda spec-file.txt file
+0.5.1     * add genbank2gff3 requirement material in bioconvert.utils.biocode
+0.5.0     * Add CI actions for all converters
+          * remove sniffer (now in biosniff on pypi https://pypi.org/project/biosniff/)
+          * A complete benchmarking suite (see doc/Snakefile_benchmark file and
+            `benchmarking`)
+          * documentation and tests for all converters
+          * removed the validators (we assume intputs are correct)
+0.4.X     * (aug 2019) added nexus2fasta, cram2fasta, fasta2faa ... ; 1-to-many and 
+            many-to-one converters are now part of the API.
+0.3.X       may 2019. new methods abi2qual, bigbed2bed, etc. added --threads option
+0.2.X       aug 2018. abi2fastx, bioconvert_stats tool added
+0.1.X       major refactoring to  have subcommands with implicit/explicit mode
+========= ==============================================================================
+
```

### Comparing `bioconvert-1.0.0.post0/examples/conversion.dot` & `bioconvert-1.1.0/examples/conversion.dot`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/plot_benchmark.py` & `bioconvert-1.1.0/examples/plot_benchmark.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/plot_graph.py` & `bioconvert-1.1.0/examples/plot_graph.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/plot_graph_clustered.py` & `bioconvert-1.1.0/examples/plot_graph_clustered.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/plot_graph_colored.py` & `bioconvert-1.1.0/examples/plot_graph_colored.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/plot_methods.py` & `bioconvert-1.1.0/examples/plot_methods.py`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/examples/test.cov` & `bioconvert-1.1.0/examples/test.cov`

 * *Files identical despite different names*

### Comparing `bioconvert-1.0.0.post0/setup.py` & `bioconvert-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 _MAJOR = 1
-_MINOR = 0
+_MINOR = 1
 _MICRO = 0
-version = "%d.%d.%d" % (_MAJOR, _MINOR, _MICRO) + "post0"
+version = "%d.%d.%d" % (_MAJOR, _MINOR, _MICRO)
 release = "%d.%d" % (_MAJOR, _MINOR)
 
 metainfo = {
     "authors": {"Cokelaer": ("Thomas Cokelaer", "thomas.cokelaer@pasteur.fr"),},
     "version": version,
     "license": "GPLv3",
     "download_url": "https://github.com/bioconvert/bioconvert",
     "url": "https://github.com/bioconvert/bioconvert",
     "description": "convert between bioinformatics formats",
     "platforms": ["Linux", "Unix", "MacOsX", "Windows"],
-    "keywords": ["NGS", "bam2bed", "fastq2fasta", "bam2sam"],
+    "keywords": ["NGS", "bam2bed", "fastq2fasta", "bam2sam", "conversion"],
     "classifiers": [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

