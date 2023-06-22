# Comparing `tmp/mavis-3.1.0.tar.gz` & `tmp/mavis-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavis-3.1.0.tar", last modified: Tue Nov 15 22:12:18 2022, max compression
+gzip compressed data, was "mavis-3.1.1.tar", last modified: Mon Mar 27 18:27:06 2023, max compression
```

## Comparing `mavis-3.1.0.tar` & `mavis-3.1.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.483460 mavis-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-15 22:12:05.000000 mavis-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-15 22:12:05.000000 mavis-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-11-15 22:12:18.483460 mavis-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-11-15 22:12:05.000000 mavis-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-15 22:12:05.000000 mavis-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-11-15 22:12:18.483460 mavis-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-15 22:12:05.000000 mavis-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.471459 mavis-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.475459 mavis-3.1.0/src/mavis/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.475459 mavis-3.1.0/src/mavis/annotate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11925 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/annotations_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     7722 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    16693 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/file_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    27596 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/fusion.py
--rw-r--r--   0 runner    (1001) docker     (121)    25046 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/genomic.py
--rw-r--r--   0 runner    (1001) docker     (121)    11654 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    16393 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/protein.py
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/splicing.py
--rw-r--r--   0 runner    (1001) docker     (121)    36347 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/annotate/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/bam/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/bam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11273 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/bam/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    18547 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/bam/cigar.py
--rw-r--r--   0 runner    (1001) docker     (121)    20835 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/bam/read.py
--rw-r--r--   0 runner    (1001) docker     (121)    10321 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/bam/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    22166 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/breakpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14974 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/cluster/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    16887 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/convert/
--rw-r--r--   0 runner    (1001) docker     (121)    11639 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/arriba.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/breakdancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/chimerascan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/cnvnator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/starfusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/straglr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/transabyss.py
--rw-r--r--   0 runner    (1001) docker     (121)    14249 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/convert/vcf.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/illustrate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    18459 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)    39328 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9304 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/illustrate/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    19220 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/interval.py
--rw-r--r--   0 runner    (1001) docker     (121)    10588 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/pairing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/pairing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/pairing/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/pairing/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    11570 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/pairing/pairing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/summary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/summary/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    14156 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/summary/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    12008 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/summary/summary.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    17945 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.479460 mavis-3.1.0/src/mavis/validate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25614 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/align.py
--rw-r--r--   0 runner    (1001) docker     (121)    18936 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/assemble.py
--rw-r--r--   0 runner    (1001) docker     (121)    21337 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17037 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/blat.py
--rw-r--r--   0 runner    (1001) docker     (121)    48050 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/call.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    16145 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/evidence.py
--rw-r--r--   0 runner    (1001) docker     (121)    30323 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/gather.py
--rw-r--r--   0 runner    (1001) docker     (121)    15678 2022-11-15 22:12:05.000000 mavis-3.1.0/src/mavis/validate/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.475459 mavis-3.1.0/src/mavis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-15 22:12:18.000000 mavis-3.1.0/src/mavis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:18.483460 mavis-3.1.0/src/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 22:12:05.000000 mavis-3.1.0/src/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-11-15 22:12:05.000000 mavis-3.1.0/src/tools/calculate_ref_alt_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)    32821 2022-11-15 22:12:05.000000 mavis-3.1.0/src/tools/convert_annotations_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-11-15 22:12:05.000000 mavis-3.1.0/src/tools/find_repeats.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19591 2022-11-15 22:12:05.000000 mavis-3.1.0/src/tools/generate_ensembl_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-27 18:26:54.000000 mavis-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-27 18:26:54.000000 mavis-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-27 18:27:06.106120 mavis-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-27 18:26:54.000000 mavis-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:26:54.000000 mavis-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-27 18:27:06.110120 mavis-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-27 18:26:54.000000 mavis-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.098120 mavis-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.102120 mavis-3.1.1/src/mavis/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.102120 mavis-3.1.1/src/mavis/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/annotations_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19204 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27596 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/genomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/splicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36346 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/annotate/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.102120 mavis-3.1.1/src/mavis/bam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/bam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/bam/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/bam/cigar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/bam/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/bam/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/breakpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.102120 mavis-3.1.1/src/mavis/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/cluster/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/mavis/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/arriba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/breakdancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/chimerascan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/cnvnator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/starfusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/straglr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/transabyss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/convert/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/mavis/illustrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39328 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/illustrate/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/mavis/pairing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/pairing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/pairing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/pairing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/pairing/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/mavis/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/summary/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/summary/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/summary/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17961 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/mavis/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/blat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48050 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30320 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-03-27 18:26:54.000000 mavis-3.1.1/src/mavis/validate/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.102120 mavis-3.1.1/src/mavis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 18:27:06.000000 mavis-3.1.1/src/mavis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:27:06.106120 mavis-3.1.1/src/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/calculate_ref_alt_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32822 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/convert_annotations_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/convert_dgv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/find_repeats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19590 2023-03-27 18:26:54.000000 mavis-3.1.1/src/tools/generate_ensembl_json.py
```

### Comparing `mavis-3.1.0/LICENSE` & `mavis-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/PKG-INFO` & `mavis-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavis
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Structural Variant Post-Processing Package
 Home-page: https://github.com/bcgsc/mavis.git
 Download-URL: https://github.com/bcgsc/mavis/archive/v2.2.10.tar.gz
 Author: Caralyn Reisle
 Author-email: creisle@bcgsc.ca
 Maintainer: mavis
 Maintainer-email: mavis@bcgsc.ca
```

### Comparing `mavis-3.1.0/README.md` & `mavis-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/setup.cfg` & `mavis-3.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mavis
-version = 3.1.0
+version = 3.1.1
 url = https://github.com/bcgsc/mavis.git
 download_url = https://github.com/bcgsc/mavis/archive/v2.2.10.tar.gz
 description = A Structural Variant Post-Processing Package
 author_email = creisle@bcgsc.ca
 author = Caralyn Reisle
 maintainer_email = mavis@bcgsc.ca
 maintainer = mavis
@@ -21,14 +21,17 @@
 	W503
 	E203
 statistics = True
 
 [flake8]
 ignore = E501,W503,E203
 
+[isort]
+profile = black
+
 [options]
 packages = find:
 package_dir = 
 	= src
 python_requires = >=3.7
 dependency_links = []
 include_package_data = True
@@ -67,14 +70,15 @@
 	coverage>=4.2
 	pycodestyle>=2.3.1
 	pytest
 	pytest-cov
 dev = 
 	black
 	flake8
+	isort
 	twine
 	wheel
 	timeout-decorator>=0.3.3
 	coverage>=4.2
 	pycodestyle>=2.3.1
 	pytest
 	pytest-cov
```

### Comparing `mavis-3.1.0/setup.py` & `mavis-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/annotations_schema.json` & `mavis-3.1.1/src/mavis/annotate/annotations_schema.json`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/base.py` & `mavis-3.1.1/src/mavis/annotate/base.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/constants.py` & `mavis-3.1.1/src/mavis/annotate/constants.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/file_io.py` & `mavis-3.1.1/src/mavis/annotate/file_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 """
 module which holds all functions relating to loading reference files
 """
 import json
 import os
 import re
-from typing import Callable, Dict, List, Optional
+import warnings
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional
 
 import pandas as pd
 from Bio import SeqIO
 from snakemake.utils import validate as snakemake_validate
 
 from ..constants import CODON_SIZE, GIEMSA_STAIN, START_AA, STOP_AA, STRAND, translate
 from ..interval import Interval
 from ..types import ReferenceAnnotations, ReferenceGenome
-from ..util import logger
+from ..util import logger, read_bpp_from_input_file
 from .base import BioInterval, ReferenceName
 from .genomic import Exon, Gene, PreTranscript, Template, Transcript
 from .protein import Domain, Translation
 
+if TYPE_CHECKING:
+    from ..breakpoint import BreakpointPair
+
 
 def load_masking_regions(*filepaths: str) -> Dict[str, List[BioInterval]]:
     """
     reads a file of regions. The expect input format for the file is tab-delimited and
     the header should contain the following columns
-
     - chr: the chromosome
     - start: start of the region, 1-based inclusive
     - end: end of the region, 1-based inclusive
     - name: the name/label of the region
-
     For example:
-
     .. code-block:: text
-
         #chr    start       end         name
         chr20   25600000    27500000    centromere
-
     Args:
         filepath: path to the input tab-delimited file
     Returns:
         a dictionary keyed by chromosome name with values of lists of regions on the chromosome
     """
+    warnings.warn(
+        "BED file support will be deprecated in future versions.",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
     regions: Dict[str, List[BioInterval]] = {}
     for filepath in filepaths:
         df = pd.read_csv(
             filepath, sep='\t', dtype={'chr': str, 'start': int, 'end': int, 'name': str}
         )
         for col in ['chr', 'start', 'end', 'name']:
             if col not in df:
@@ -54,14 +58,75 @@
             mask_region = BioInterval(
                 reference_object=row['chr'], start=row['start'], end=row['end'], name=row['name']
             )
             regions.setdefault(mask_region.reference_object, []).append(mask_region)
     return regions
 
 
+def load_known_sv(*filepaths: str) -> Dict[str, List["BreakpointPair"]]:
+    """
+    loads a standard MAVIS or BED file input to a list of known breakpoints.
+
+    Standard BED file requirements:
+    reads a file of regions. The expect input format for the file is tab-delimited and
+    the header should contain the following columns
+
+    - chr: the chromosome
+    - start: start of the region, 1-based inclusive
+    - end: end of the region, 1-based inclusive
+    - name: the name/label of the region
+
+    For example:
+
+    .. code-block:: text
+
+        #chr    start       end         name
+        chr20   25600000    27500000    centromere
+    Args:
+        filepath: path to standard MAVIS format file
+    Returns:
+        a dictionary with {str:{BreakpointPair}}
+    """
+    regions = {}
+    for filepath in filepaths:
+        header = set(pd.read_csv(filepath, nrows=1, sep='\t').columns)
+        mavis_header = {'break1_chromosome', 'break2_chromosome'}
+        bed_header = {'chr', 'start', 'end', 'name'}
+        if mavis_header.issubset(header):
+            bpps = read_bpp_from_input_file(filepath, expand_orient=True, expand_svtype=True)
+            for bpp in bpps:
+                chr_list = [bpp.break1.chr, bpp.break2.chr]
+                regions.setdefault(tuple(chr_list), []).append(bpp)
+
+        else:
+            warnings.warn(
+                "BED file support will be deprecated in future versions.",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+
+            df = pd.read_csv(
+                filepath, sep='\t', dtype={'chr': str, 'start': int, 'end': int, 'name': str}
+            )
+            for col in bed_header:
+                if col not in df:
+                    raise KeyError(f'missing required column ({col})')
+            df['chr'] = df['chr'].apply(lambda c: ReferenceName(c))
+            for row in df.to_dict('records'):
+                known_sv_region = BioInterval(
+                    reference_object=row['chr'],
+                    start=row['start'],
+                    end=row['end'],
+                    name=row['name'],
+                )
+                regions.setdefault(known_sv_region.reference_object, []).append(known_sv_region)
+
+    return regions
+
+
 def load_annotations(
     *filepaths: str,
     reference_genome: Optional[ReferenceGenome] = None,
     best_transcripts_only: bool = False,
 ) -> Dict[str, List[Gene]]:
     """
     loads gene models from an input file. Expects a tabbed or json file.
@@ -113,15 +178,14 @@
         raise AssertionError(short_msg)
 
     genes_by_chr: ReferenceAnnotations = {}
     tx_skipped = 0
     domain_errors = 0
 
     for gene_dict in data['genes']:
-
         gene = Gene(
             chr=gene_dict['chr'],
             start=gene_dict['start'],
             end=gene_dict['end'],
             name=gene_dict['name'],
             aliases=gene_dict['aliases'],
             strand=gene_dict['strand'],
@@ -342,15 +406,15 @@
     CACHE = {}  # type: ignore
 
     LOAD_FUNCTIONS: Dict[str, Optional[Callable]] = {
         'annotations': load_annotations,
         'reference_genome': load_reference_genome,
         'masking': load_masking_regions,
         'template_metadata': load_templates,
-        'dgv_annotation': load_masking_regions,
+        'dgv_annotation': load_known_sv,
         'aligner_reference': None,
     }
     """dict: Mapping of file types (based on ENV name) to load functions"""
 
     def __init__(
         self,
         file_type: str,
```

### Comparing `mavis-3.1.0/src/mavis/annotate/fusion.py` & `mavis-3.1.1/src/mavis/annotate/fusion.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/genomic.py` & `mavis-3.1.1/src/mavis/annotate/genomic.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/main.py` & `mavis-3.1.1/src/mavis/annotate/main.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/protein.py` & `mavis-3.1.1/src/mavis/annotate/protein.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/splicing.py` & `mavis-3.1.1/src/mavis/annotate/splicing.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/annotate/variant.py` & `mavis-3.1.1/src/mavis/annotate/variant.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,14 @@
                 self.ins_seq = self.mut_seq[self.nterm_aligned :]
 
             elif not self.nterm_aligned:
                 self.del_seq = self.ref_seq[: 0 - self.cterm_aligned]
                 self.ins_seq = self.mut_seq[: 0 - self.cterm_aligned]
 
             elif len(self.ref_seq) - self.cterm_aligned + 1 <= self.nterm_aligned:
-
                 # repeat region
                 diff = len(self.mut_seq) - len(self.ref_seq)
                 if diff > 0:
                     ins_length = diff
                     del_length = 0
                 else:
                     del_length = abs(diff)
```

### Comparing `mavis-3.1.0/src/mavis/bam/cache.py` & `mavis-3.1.1/src/mavis/bam/cache.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/bam/cigar.py` & `mavis-3.1.1/src/mavis/bam/cigar.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/bam/read.py` & `mavis-3.1.1/src/mavis/bam/read.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/bam/stats.py` & `mavis-3.1.1/src/mavis/bam/stats.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/breakpoint.py` & `mavis-3.1.1/src/mavis/breakpoint.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/cluster/cluster.py` & `mavis-3.1.1/src/mavis/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/cluster/main.py` & `mavis-3.1.1/src/mavis/cluster/main.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/config.py` & `mavis-3.1.1/src/mavis/config.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/constants.py` & `mavis-3.1.1/src/mavis/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         X: sequence mismatch
 
     Note:
         descriptions are taken from the `samfile documentation <https://samtools.github.io/hts-specs/SAMv1.pdf>`_
     """
 
     M = 0
-    I = 1
+    I = 1  # noqa
     D = 2
     N = 3
     S = 4
     H = 5
     P = 6
     X = 8
     EQ = 7
@@ -382,14 +382,15 @@
     see [column descriptions](/outputs/columns)
     """
 
     tracking_id: str = 'tracking_id'
     library: str = 'library'
     cluster_id: str = 'cluster_id'
     cluster_size: str = 'cluster_size'
+    dgv: str = 'dgv'
     validation_id: str = 'validation_id'
     annotation_id: str = 'annotation_id'
     product_id: str = 'product_id'
     event_type: str = 'event_type'
     pairing: str = 'pairing'
     inferred_pairing: str = 'inferred_pairing'
     gene1: str = 'gene1'
@@ -459,14 +460,15 @@
     contig_remap_coverage: str = 'contig_remap_coverage'
     contig_remapped_read_names: str = 'contig_remapped_read_names'
     contig_remapped_reads: str = 'contig_remapped_reads'
     contig_seq: str = 'contig_seq'
     contig_strand_specific: str = 'contig_strand_specific'
     contigs_assembled: str = 'contigs_assembled'
     call_sequence_complexity: str = 'call_sequence_complexity'
+    known_sv_count: str = 'known_sv_count'
     spanning_reads: str = 'spanning_reads'
     spanning_read_names: str = 'spanning_read_names'
     flanking_median_fragment_size: str = 'flanking_median_fragment_size'
     flanking_pairs: str = 'flanking_pairs'
     flanking_pairs_compatible: str = 'flanking_pairs_compatible'
     flanking_pairs_read_names: str = 'flanking_pairs_read_names'
     flanking_pairs_compatible_read_names: str = 'flanking_pairs_compatible_read_names'
@@ -551,8 +553,10 @@
     COLUMNS.flanking_pairs,
     COLUMNS.pairing,
     COLUMNS.product_id,
     COLUMNS.spanning_reads,
     COLUMNS.tools,
     COLUMNS.tools,
     COLUMNS.tracking_id,
+    COLUMNS.dgv,
+    COLUMNS.known_sv_count,
 }
```

### Comparing `mavis-3.1.0/src/mavis/convert/__init__.py` & `mavis-3.1.1/src/mavis/convert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,31 +85,26 @@
         SUPPORTED_TOOL.DELLY,
         SUPPORTED_TOOL.MANTA,
         SUPPORTED_TOOL.PINDEL,
         SUPPORTED_TOOL.VCF,
         SUPPORTED_TOOL.BREAKSEQ,
         SUPPORTED_TOOL.STRELKA,
     ]:
-
         std_row.update(row)
 
     elif file_type == SUPPORTED_TOOL.CHIMERASCAN:
-
         std_row.update(_parse_chimerascan(row))
 
     elif file_type == SUPPORTED_TOOL.CNVNATOR:
-
         std_row.update(_parse_cnvnator(row))
 
     elif file_type == SUPPORTED_TOOL.STARFUSION:
-
         std_row.update(_parse_starfusion(row))
 
     elif file_type == SUPPORTED_TOOL.DEFUSE:
-
         std_row[COLUMNS.break1_orientation] = (
             ORIENT.LEFT if row['genomic_strand1'] == STRAND.POS else ORIENT.RIGHT
         )
         std_row[COLUMNS.break2_orientation] = (
             ORIENT.LEFT if row['genomic_strand2'] == STRAND.POS else ORIENT.RIGHT
         )
         std_row.update(
@@ -122,38 +117,34 @@
         )
         if TRACKING_COLUMN in row:
             std_row[TRACKING_COLUMN] = row[TRACKING_COLUMN]
         else:
             std_row[TRACKING_COLUMN] = '{}-{}'.format(file_type, row['cluster_id'])
 
     elif file_type == SUPPORTED_TOOL.TA:
-
         std_row.update(_parse_transabyss(row))
 
     elif file_type == SUPPORTED_TOOL.BREAKDANCER:
-
         std_row.update(
             {
                 COLUMNS.event_type: row['Type'],
                 COLUMNS.break1_chromosome: row['Chr1'],
                 COLUMNS.break2_chromosome: row['Chr2'],
                 COLUMNS.break1_position_start: row['Pos1'],
                 COLUMNS.break2_position_start: row['Pos2'],
             }
         )
         std_row.update(
             {k: v for k, v in row.items() if k not in {'Type', 'Chr1', 'Chr2', 'Pos1', 'Pos2'}}
         )
 
     elif file_type == SUPPORTED_TOOL.ARRIBA:
-
         std_row.update(_parse_arriba(row))
 
     elif file_type == SUPPORTED_TOOL.STRAGLR:
-
         std_row.update(_parse_straglr(row))
 
     else:
         raise NotImplementedError('unsupported file type', file_type)
 
     if stranded:
         std_row[COLUMNS.break1_strand] = STRAND.expand(std_row[COLUMNS.break1_strand])
```

### Comparing `mavis-3.1.0/src/mavis/convert/arriba.py` & `mavis-3.1.1/src/mavis/convert/arriba.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from ..constants import COLUMNS, ORIENT, STRAND
-
-from .constants import TRACKING_COLUMN, SUPPORTED_TOOL
+from ..constants import COLUMNS, ORIENT
 
 
 def get_orient(string):
     if string == "downstream":
         return ORIENT.LEFT
     elif string == "upstream":
         return ORIENT.RIGHT
```

### Comparing `mavis-3.1.0/src/mavis/convert/breakdancer.py` & `mavis-3.1.1/src/mavis/convert/breakdancer.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/chimerascan.py` & `mavis-3.1.1/src/mavis/convert/chimerascan.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/cnvnator.py` & `mavis-3.1.1/src/mavis/convert/cnvnator.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/constants.py` & `mavis-3.1.1/src/mavis/convert/constants.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/starfusion.py` & `mavis-3.1.1/src/mavis/convert/starfusion.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/straglr.py` & `mavis-3.1.1/src/mavis/convert/straglr.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/convert/transabyss.py` & `mavis-3.1.1/src/mavis/convert/transabyss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 
 from ..constants import COLUMNS
-
 from .constants import SUPPORTED_TOOL, TRACKING_COLUMN
 
 
 def convert_row(row):
     """
     transforms the transabyss output into the common format for expansion.
     Maps the input column names to column names which MAVIS can read
```

### Comparing `mavis-3.1.0/src/mavis/convert/vcf.py` & `mavis-3.1.1/src/mavis/convert/vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import gzip
 import logging
 import re
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Tuple
-from ..interval import Interval
+
 import pandas as pd
 
+from ..interval import Interval
+
 try:
     # TypedDict added to typing package directly in later versions
     from typing import TypedDict
 except ImportError:
     from typing_extensions import TypedDict
 
 from ..constants import COLUMNS, ORIENT, SVTYPE
@@ -331,15 +333,14 @@
         return info
 
     df['info'] = df['INFO'].apply(parse_info)
     df['alts'] = df['ALT'].apply(lambda a: a.split(','))
 
     rows = []
     for _, row in df.iterrows():
-
         rows.append(
             VcfRecordType(
                 id=row['ID'],
                 pos=row['POS'],
                 info=VcfInfoType(row['info']),
                 chrom=row['CHROM'],
                 ref=row['REF'],
```

### Comparing `mavis-3.1.0/src/mavis/illustrate/constants.py` & `mavis-3.1.1/src/mavis/illustrate/constants.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/illustrate/diagram.py` & `mavis-3.1.1/src/mavis/illustrate/diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """
 This is the primary module responsible for generating svg visualizations
 
 """
 from typing import Iterable, List, Optional
 
+from svgwrite import Drawing
+
 from mavis.annotate.genomic import Gene, Template
 from mavis.annotate.variant import Annotation
 from mavis.types import ReferenceGenome
-from svgwrite import Drawing
 
 from ..annotate.genomic import IntergenicRegion
 from ..interval import Interval
 from .constants import DiagramSettings
-from .elements import draw_exon_track, draw_genes, draw_template, draw_ustranscript, draw_vmarker
+from .elements import (
+    draw_exon_track,
+    draw_genes,
+    draw_template,
+    draw_ustranscript,
+    draw_vmarker,
+)
 from .scatter import ScatterPlot, draw_scatter
 from .util import LabelMapping, generate_interval_mapping
 
 # draw gene level view
 # draw gene box
 HEX_WHITE = '#FFFFFF'
 HEX_BLACK = '#000000'
```

### Comparing `mavis-3.1.0/src/mavis/illustrate/elements.py` & `mavis-3.1.1/src/mavis/illustrate/elements.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/illustrate/scatter.py` & `mavis-3.1.1/src/mavis/illustrate/scatter.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/illustrate/util.py` & `mavis-3.1.1/src/mavis/illustrate/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from colour import Color
 import svgwrite
+from colour import Color
 
 from ..error import DrawingFitError
 from ..interval import Interval, IntervalMapping
 
-
 MIN_PIXEL_ACCURACY = 1
 
 
 def dynamic_label_color(color):
     """
     calculates the luminance of a color and determines if a black or white label will be more contrasting
     """
@@ -207,15 +206,14 @@
         s = max(intergenic_unit(len(ifrom)), 0)
         ito = Interval(pos, pos + min_inter_width + s)
         mapping.append((ifrom, ito))
         pos = ito.end
 
     for i, curr in enumerate(intervals):
         if i > 0 and intervals[i - 1].end + 1 < curr.start:  # add between the intervals
-
             prev = intervals[i - 1]
             ifrom = Interval(prev.end + 1, curr.start - 1)
             s = max(intergenic_unit(len(ifrom)), 0)
             ito = Interval(pos, pos + min_inter_width + s)
             mapping.append((ifrom, ito))
             pos = ito.end
```

### Comparing `mavis-3.1.0/src/mavis/interval.py` & `mavis-3.1.1/src/mavis/interval.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/main.py` & `mavis-3.1.1/src/mavis/main.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/overlay.py` & `mavis-3.1.1/src/mavis/overlay.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/pairing/main.py` & `mavis-3.1.1/src/mavis/pairing/main.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/pairing/pairing.py` & `mavis-3.1.1/src/mavis/pairing/pairing.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,17 @@
                             Breakpoint(
                                 breakpoint.chr,
                                 curr.acceptor,
                                 strand=breakpoint.strand,
                                 orient=breakpoint.orient,
                             )
                         )
-            except AttributeError:  # for introns that are smaller than this ignore (covered by exon check)
+            except (
+                AttributeError
+            ):  # for introns that are smaller than this ignore (covered by exon check)
                 pass
 
     if not tbreaks:
         raise AssertionError('could not predict breakpoint')
     return sorted(tbreaks)
 
 
@@ -150,17 +152,26 @@
     max_distance = max(
         distances[event1.data.get(COLUMNS.call_method, CALL_METHOD.CONTIG)],
         distances[event2.data.get(COLUMNS.call_method, CALL_METHOD.CONTIG)],
     )
     return max_distance
 
 
-def equivalent(event1: BreakpointPair, event2: BreakpointPair, distances=None) -> bool:
+def equivalent(
+    event1: BreakpointPair, event2: BreakpointPair, distances=None, matching_event_type=True
+) -> bool:
     """
     compares two events by breakpoint position to see if they are equivalent
+
+    Args:
+        - event1: first BreakpointPair to be compared
+        - event2: second BreakpointPair to be compared
+        - distances: distance between two BreakpointPairs to be considered equivalent
+        - matching_event_type: specificies whether event type must match
+
     """
 
     max_distance = comparison_distance(event1, event2, distances)
 
     if not _equivalent_events(event1, event2):
         return False
     seqlen = sum(
@@ -171,18 +182,19 @@
     )
     max_distance += seqlen
     # location comparison
     if any(
         [
             abs(Interval.dist(event1.break1, event2.break1)) > max_distance,
             abs(Interval.dist(event1.break2, event2.break2)) > max_distance,
-            event1.data[COLUMNS.event_type] != event2.data[COLUMNS.event_type],
         ]
     ):
         return False
+    if matching_event_type and event1.event_type != event2.event_type:
+        return False
     return True
 
 
 def pair_by_distance(
     calls: List[BreakpointPair], distances, against_self: bool = False
 ) -> Dict[str, Set[str]]:
     """
```

### Comparing `mavis-3.1.0/src/mavis/summary/main.py` & `mavis-3.1.1/src/mavis/summary/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,24 +272,25 @@
         COLUMNS.contig_remapped_reads,
         COLUMNS.tracking_id,
         COLUMNS.supplementary_call,
         COLUMNS.protein_synon,
         COLUMNS.cdna_synon,
         COLUMNS.net_size,
         COLUMNS.assumed_untemplated,
-        'dgv',
+        COLUMNS.dgv,
+        COLUMNS.known_sv_count,
     }
 
     rows = []
     for lib in bpps_by_library:
         logger.info(f'annotating dgv for {lib}')
         if not dgv_annotation.is_empty():
             annotate_dgv(
-                bpps_by_library[lib], dgv_annotation.content, distance=10
-            )  # TODO make distance a parameter
+                bpps_by_library[lib], dgv_annotation.content, config['summary.cluster_radius']
+            )
         logger.info(f'adding pairing states for {lib}')
         for row in bpps_by_library[lib]:
             # in case no pairing was done, add default (applicable to single library summaries)
             row.data.setdefault(COLUMNS.inferred_pairing, '')
             row.data.setdefault(COLUMNS.pairing, '')
             row.data.setdefault(COLUMNS.library, lib)
             # filter pairing ids based on what is still kept?
```

### Comparing `mavis-3.1.0/src/mavis/summary/summary.py` & `mavis-3.1.1/src/mavis/summary/summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from typing import Dict, List
+from itertools import chain
+from typing import Dict, List, Tuple, Union
 
-from ..annotate.genomic import Transcript
+from ..annotate.genomic import BioInterval, Transcript
 from ..breakpoint import Breakpoint, BreakpointPair
+from ..cluster.cluster import merge_breakpoint_pairs
 from ..constants import CALL_METHOD, COLUMNS, DISEASE_STATUS, PROTOCOL, SVTYPE
 from ..interval import Interval
 from ..pairing.pairing import pair_by_distance, product_key
 from ..util import get_connected_components
 from .constants import PAIRING_STATE
 
 
@@ -56,14 +58,15 @@
 
 
 def filter_by_call_method(bpp_list):
     """
     Filters a set of breakpoint pairs to returns the call with the most evidence.
     Prefers contig evidence over spanning over split over flanking, etc.
     """
+
     # ranking scores of the methods (more is better)
     def sort_key(bpp):
         key = [
             bpp.data.get(col, 0) if bpp.data.get(col, 0) is not None else 0
             for col in [
                 'contig_remapped_reads',
                 'contig_alignment_score',
@@ -186,53 +189,131 @@
             for key in component:
                 pairs.extend(mapping[key])
             grouped_calls.append(group_events(pairs))
             removed_calls.extend(pairs)
     return grouped_calls, removed_calls
 
 
-def annotate_dgv(bpps, dgv_regions_by_reference_name, distance=0):
+def annotate_with_dgv_bpp(
+    bpps: List[BreakpointPair],
+    dgv_regions_list: List[BreakpointPair],
+    input_cluster_radius: int,
+):
     """
-    given a list of bpps and a dgv reference, annotate the events that are within the set distance of both breakpoints
+    Given a list of breakpoint pairs (bpps) and bpps from another reference set, annotate the events that are within the set distance of both breakpoints
 
     Args:
-        bpps (list) : the list of BreakpointPair objects
-        dgv_regions_by_reference_name (dict) : the dgv reference regions file loaded by load_masking_regions
-        distance (int) : the minimum distance required to match a dgv event with a breakpoint
+        bpps: the list of BreakpointPair objects
+        dgv_regions_list: the dgv reference regions specified by the MAVIS input file represented as BreakpointPairs
+        input_cluster_radius: Distance used in matching input SVs to reference SVs through clusterind, defined by summary.cluster_radius in the configuration file
+    """
+    bpps_copy = bpps.copy()
+    for variant in bpps:
+        variant.data[COLUMNS.dgv] = False
+        variant.data[COLUMNS.known_sv_count] = 0
+    for variant in dgv_regions_list:
+        variant.data[COLUMNS.dgv] = True
+        variant.data[COLUMNS.known_sv_count] = 0
+    bpps_copy.extend(dgv_regions_list)
+
+    clusters = merge_breakpoint_pairs(
+        bpps_copy, cluster_radius=input_cluster_radius
+    )  # all breakpoint pairs (bpps + dgv)
+
+    flag_col = '_is_variant'
+    for variant in bpps:
+        variant.data[flag_col] = True
+        variant.data[COLUMNS.dgv] = ''
+        variant.data[COLUMNS.known_sv_count] = 0
+
+    for clustered_bpp_key, clustered_bpp_val in clusters.items():
+        dgv_tracking_ids = [
+            bpp.tracking_id for bpp in clustered_bpp_val if bpp.data.get(flag_col) is not True
+        ]
+        dgv_field = ';'.join(sorted(dgv_tracking_ids))
+        variant_bpp = [bpp for bpp in clustered_bpp_val if bpp.data.get(flag_col) is True]
+        for variant in variant_bpp:
+            variant.data[COLUMNS.dgv] = dgv_field
+            variant.data[COLUMNS.known_sv_count] = len(dgv_tracking_ids)
+
+    for bpp in bpps:
+        if flag_col in bpp.data:
+            del bpp.data[flag_col]
+
+
+def annotate_with_dgv_bed(
+    bpps: List[BreakpointPair],
+    dgv_regions_by_reference_name: Dict[Tuple[str], List[BioInterval]],
+    input_cluster_radius: int,
+):
+    """
+    Given a list of breakpoint pairs (bpps) and bpps from another reference set, annotate the events that are within the set distance of both breakpoints
+
+    Args:
+        bpps: the list of BreakpointPair objects
+        dgv_regions_by_reference_name: the dgv reference regions specified by the bed input file represented as BioIntervals
+        input_cluster_radius: Distance used in matching input SVs to reference SVs through clusterind, defined by summary.cluster_radius in the configuration file
     """
     for chrom in dgv_regions_by_reference_name:
         dgv_regions_by_reference_name[chrom] = sorted(
             dgv_regions_by_reference_name[chrom], key=lambda x: x.start
         )
-
     lowest_resolution = max([len(b.break1) for b in bpps])  # only need start res
-
+    for bpp in bpps:
+        bpp.data[COLUMNS.dgv] = []
+        bpp.data[COLUMNS.known_sv_count] = 0
     # only look at the bpps that dgv events could pair to, Intrachromosomal
     for bpp in [
         b for b in bpps if not b.interchromosomal and b.break1.chr in dgv_regions_by_reference_name
     ]:
-        bpp.data['dgv'] = []
         for dgv_region in dgv_regions_by_reference_name[bpp.break1.chr]:
             dist = abs(Interval.dist(Interval(dgv_region.start), bpp.break1))
-            if dist > lowest_resolution + distance:
+            if dist > lowest_resolution + input_cluster_radius:
                 continue
             elif (
-                dist > distance
-                or abs(Interval.dist(Interval(dgv_region.end), bpp.break2)) > distance
+                dist > input_cluster_radius
+                or abs(Interval.dist(Interval(dgv_region.end), bpp.break2)) > input_cluster_radius
             ):
                 continue
             refname = dgv_region.reference_object
             try:
                 refname = dgv_region.reference_object.name
             except AttributeError:
                 pass
-            bpp.data['dgv'].append(
+            bpp.data[COLUMNS.dgv].append(
                 '{}({}:{}-{})'.format(dgv_region.name, refname, dgv_region.start, dgv_region.end)
             )
-        bpp.data['dgv'] = ';'.join(bpp.data['dgv'])
+        bpp.data[COLUMNS.known_sv_count] = len(bpp.data[COLUMNS.dgv])
+        bpp.data[COLUMNS.dgv] = ';'.join(bpp.data[COLUMNS.dgv])
+
+
+def annotate_dgv(
+    bpps: List[BreakpointPair],
+    dgv_regions_by_reference_name: Dict[Tuple[str], Union[List[BreakpointPair], List[BioInterval]]],
+    input_cluster_radius: int,
+):
+    """
+    Given a list of breakpoint pairs (bpps) and bpps from another reference set, annotate the events that are within the set distance of both breakpoints
+
+    Args:
+        bpps: the list of BreakpointPair objects
+        dgv_regions_by_reference_name: tuple of strings of chr name and its associated list of BreakpointPair/BioInterval objects specified by the MAVIS input file
+        input_cluster_radius: Distance used in matching input SVs to reference SVs through clusterind, defined by summary.cluster_radius in the configuration file
+    """
+
+    if not dgv_regions_by_reference_name:
+        pass
+
+    elif isinstance(list(dgv_regions_by_reference_name.values())[0][0], BreakpointPair):
+        annotate_with_dgv_bpp(
+            bpps, list(chain(*dgv_regions_by_reference_name.values())), input_cluster_radius
+        )
+
+    else:
+        annotate_with_dgv_bed(bpps, dgv_regions_by_reference_name, input_cluster_radius)
 
 
 def get_pairing_state(
     current_protocol,
     current_disease_state,
     other_protocol,
     other_disease_state,
```

### Comparing `mavis-3.1.0/src/mavis/util.py` & `mavis-3.1.1/src/mavis/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,17 @@
 def mkdirp(dirname):
     """
     Make a directory or path of directories. Suppresses the error that is normally raised when the directory already exists
     """
     logger.info(f"creating output directory: '{dirname}'")
     try:
         os.makedirs(dirname)
-    except OSError as exc:  # Python >2.5: http://stackoverflow.com/questions/600268/mkdir-p-functionality-in-python
+    except (
+        OSError
+    ) as exc:  # Python >2.5: http://stackoverflow.com/questions/600268/mkdir-p-functionality-in-python
         if exc.errno == errno.EEXIST and os.path.isdir(dirname):
             pass
         else:
             raise exc
     return dirname
```

### Comparing `mavis-3.1.0/src/mavis/validate/align.py` & `mavis-3.1.1/src/mavis/validate/align.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 from typing import TYPE_CHECKING, Dict, List
 
 import pysam
 
 from ..bam import cigar as _cigar
 from ..bam import read as _read
 from ..breakpoint import Breakpoint, BreakpointPair, classify_breakpoint_pair
-from ..constants import CIGAR, ORIENT, STRAND, SVTYPE, MavisNamespace, reverse_complement
+from ..constants import (
+    CIGAR,
+    ORIENT,
+    STRAND,
+    SVTYPE,
+    MavisNamespace,
+    reverse_complement,
+)
 from ..interval import Interval
 from ..types import ReferenceGenome
 from ..util import logger
 
 if TYPE_CHECKING:
     from ..bam.cache import BamCache
```

### Comparing `mavis-3.1.0/src/mavis/validate/assemble.py` & `mavis-3.1.1/src/mavis/validate/assemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,14 @@
     # initial data cleaning
     assembly.trim_forks_by_freq(min_edge_trim_weight)
     assembly.trim_tails_by_freq(min_edge_trim_weight)
     assembly.trim_noncutting_paths_by_freq(min_edge_trim_weight)
 
     path_scores = {}
     for component in digraph_connected_components(assembly):
-
         # pull the path scores
         path_scores.update(
             pull_contigs_from_component(
                 assembly.subgraph(component).copy(),
                 component,
                 min_edge_trim_weight=min_edge_trim_weight,
                 assembly_max_paths=assembly_max_paths,
```

### Comparing `mavis-3.1.0/src/mavis/validate/base.py` & `mavis-3.1.1/src/mavis/validate/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 import pysam
 from mavis_config import DEFAULTS
 
 from ..bam import cigar as _cigar
 from ..bam import read as _read
 from ..bam.cache import BamCache
 from ..breakpoint import Breakpoint, BreakpointPair, classify_breakpoint_pair
-from ..constants import COLUMNS, ORIENT, PYSAM_READ_FLAGS, STRAND, SVTYPE, reverse_complement
+from ..constants import (
+    COLUMNS,
+    ORIENT,
+    PYSAM_READ_FLAGS,
+    STRAND,
+    SVTYPE,
+    reverse_complement,
+)
 from ..error import NotSpecifiedError
 from ..interval import Interval
 from ..util import logger
 from .assemble import Contig, assemble
 
 
 class Evidence(BreakpointPair):
```

### Comparing `mavis-3.1.0/src/mavis/validate/blat.py` & `mavis-3.1.1/src/mavis/validate/blat.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/validate/call.py` & `mavis-3.1.1/src/mavis/validate/call.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/validate/evidence.py` & `mavis-3.1.1/src/mavis/validate/evidence.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis/validate/gather.py` & `mavis-3.1.1/src/mavis/validate/gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,14 @@
         strand1 = _read.sequenced_strand(read, evidence_bpp.strand_determining_read)
         strand2 = _read.sequenced_strand(mate, evidence_bpp.strand_determining_read)
 
         if strand1 != evidence_bpp.break1.strand or strand2 != evidence_bpp.break2.strand:
             return False
 
     for event_type in evidence_bpp.putative_event_types():
-
         # check that the pair orientation is correct
         if not _read.orientation_supports_type(read, event_type):
             continue
 
         # check that the fragment size is reasonable
         fragment_size = evidence_bpp.compute_fragment_size(read, mate)
 
@@ -514,19 +513,17 @@
         if strand != evidence_bpp.break1.strand and strand != evidence_bpp.break2.strand:
             return False
 
     combined = evidence_bpp.inner_window1 & evidence_bpp.inner_window2
     read_interval = Interval(read.reference_start + 1, read.reference_end)
 
     if Interval.overlaps(combined, read_interval):
-
         if not read.has_tag(PYSAM_READ_FLAGS.RECOMPUTED_CIGAR) or not read.get_tag(
             PYSAM_READ_FLAGS.RECOMPUTED_CIGAR
         ):
-
             read = evidence_bpp.standardize_read(read)
         # in the correct position, now determine if it can support the event types
         for event_type in evidence_bpp.putative_event_types():
             if event_type in [SVTYPE.DUP, SVTYPE.INS]:
                 if CIGAR.I in [c[0] for c in read.cigar]:
                     evidence_bpp.spanning_reads.add(read)
                     return True
```

### Comparing `mavis-3.1.0/src/mavis/validate/main.py` & `mavis-3.1.1/src/mavis/validate/main.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/mavis.egg-info/PKG-INFO` & `mavis-3.1.1/src/mavis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavis
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Structural Variant Post-Processing Package
 Home-page: https://github.com/bcgsc/mavis.git
 Download-URL: https://github.com/bcgsc/mavis/archive/v2.2.10.tar.gz
 Author: Caralyn Reisle
 Author-email: creisle@bcgsc.ca
 Maintainer: mavis
 Maintainer-email: mavis@bcgsc.ca
```

### Comparing `mavis-3.1.0/src/mavis.egg-info/SOURCES.txt` & `mavis-3.1.1/src/mavis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,9 +73,10 @@
 src/mavis/validate/constants.py
 src/mavis/validate/evidence.py
 src/mavis/validate/gather.py
 src/mavis/validate/main.py
 src/tools/__init__.py
 src/tools/calculate_ref_alt_counts.py
 src/tools/convert_annotations_format.py
+src/tools/convert_dgv.py
 src/tools/find_repeats.py
 src/tools/generate_ensembl_json.py
```

### Comparing `mavis-3.1.0/src/mavis.egg-info/requires.txt` & `mavis-3.1.1/src/mavis.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 [deploy]
 twine
 wheel
 
 [dev]
 black
 flake8
+isort
 twine
 wheel
 timeout-decorator>=0.3.3
 coverage>=4.2
 pycodestyle>=2.3.1
 pytest
 pytest-cov
```

### Comparing `mavis-3.1.0/src/tools/calculate_ref_alt_counts.py` & `mavis-3.1.1/src/tools/calculate_ref_alt_counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """
 import argparse
 import logging
 import statistics as stats
 
 import pysam
+
 from mavis.annotate.file_io import load_reference_genome
 from mavis.constants import SVTYPE
 from mavis.util import logger, output_tabbed_file, read_inputs
 from mavis.validate.call import EventCall
 
 
 def get_read_length(bam_cache, sample_cap=20):
@@ -86,14 +87,17 @@
     else:
         raise ValueError("Cannot determine ref and alt counts for non dup/ins/del event types")
     all_reads = bam_cache.fetch(
         bpp.break1.chr, bpp.break1.start - read_length, bpp.break2.end + read_length
     )
 
     for read in all_reads:
+        if read.is_duplicate or read.is_unmapped or read.is_qcfail:
+            continue
+
         # compare the actual sequence
         ref_align = ref_sequence in read.seq
         alt_align = alt_sequence in read.seq
 
         if ref_align and alt_align:
             multimap_reads.add(read)
```

### Comparing `mavis-3.1.0/src/tools/convert_annotations_format.py` & `mavis-3.1.1/src/tools/convert_annotations_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import json
 import logging
 import re
 from typing import Dict, Tuple
 
 import pandas as pd
+
 from mavis.annotate.file_io import parse_annotations_json
 
 PANDAS_DEFAULT_NA_VALUES = [
     '-1.#IND',
     '1.#QNAN',
     '1.#IND',
     '-1.#QNAN',
```

### Comparing `mavis-3.1.0/src/tools/find_repeats.py` & `mavis-3.1.1/src/tools/find_repeats.py`

 * *Files identical despite different names*

### Comparing `mavis-3.1.0/src/tools/generate_ensembl_json.py` & `mavis-3.1.1/src/tools/generate_ensembl_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,14 @@
         best_file (str): path to file of "best transcripts"
         alias_file (str): path to file with gene aliases
     """
 
     def __init__(
         self, release, species, output, best_file=None, alias_file=None, custom_cache=None
     ):
-
         self.annotation = {}
 
         self.custom_cache = custom_cache
         self.cache_prefix = None
         self.gen_time = get_date()
         self.release = release
         self.species = species
```

