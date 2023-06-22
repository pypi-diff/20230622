# Comparing `tmp/pmx_biobb-4.0.1.tar.gz` & `tmp/pmx_biobb-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-4.0.1.tar", last modified: Wed Jun 21 11:24:50 2023, max compression
+gzip compressed data, was "dist/pmx_biobb-4.0.2.tar", last modified: Thu Jun 22 15:07:11 2023, max compression
```

## Comparing `pmx_biobb-4.0.1.tar` & `pmx_biobb-4.0.2.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/
--rw-r--r--   0 pau        (501) staff       (20)     7651 2023-06-14 14:42:12.000000 pmx_biobb-4.0.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)       95 2023-06-19 13:37:17.000000 pmx_biobb-4.0.1/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     2087 2023-06-19 13:29:31.000000 pmx_biobb-4.0.1/README.rst
--rw-r--r--   0 pau        (501) staff       (20)      194 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2108 2023-06-21 11:22:47.000000 pmx_biobb-4.0.1/setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/
--rw-r--r--   0 pau        (501) staff       (20)      459 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/_version.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/
--rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/bbdep.pkl
--rw-r--r--   0 pau        (501) staff       (20)     1786 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/blosum62_new.mat
--rw-r--r--   0 pau        (501) staff       (20)   144604 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/bp.pkl
--rw-r--r--   0 pau        (501) staff       (20)   149219 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/bp_amber.pkl
--rw-r--r--   0 pau        (501) staff       (20)   148935 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/bp_charmm.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9416 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      951 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)      661 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am
--rw-r--r--   0 pau        (501) staff       (20)    12694 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       84 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2060 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1519 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      181 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)     6253 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)      244 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1660 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9612 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    88617 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    47717 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     1208 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2882 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)        0 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/lipids.hdb
--rw-r--r--   0 pau        (501) staff       (20)    48593 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp
--rw-r--r--   0 pau        (501) staff       (20)       70 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)      164 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      126 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)     9712 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      910 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      916 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1369 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1419 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1576 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     2237 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      306 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm36mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     3940 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/elements.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)      343 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45/xlateat.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    21524 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5335 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      130 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    45478 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7972 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129919 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4978 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)     7476 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129937 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    82367 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)      435 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2734 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     2079 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.arn
--rw-r--r--   0 pau        (501) staff       (20)     1134 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8979 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1397 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      198 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.r2b
--rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5220 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd
--rw-r--r--   0 pau        (501) staff       (20)   283035 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   123173 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1339 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp
--rw-r--r--   0 pau        (501) staff       (20)      619 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      625 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1026 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1242 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      221 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)    70529 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/data/rna.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx/extensions/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/
--rw-r--r--   0 pau        (501) staff       (20)    13896 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/Energy.c
--rw-r--r--   0 pau        (501) staff       (20)    15145 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/Geometry.c
--rw-r--r--   0 pau        (501) staff       (20)    20514 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/Geometry.h
--rw-r--r--   0 pau        (501) staff       (20)     2086 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/cpp_test.cpp
--rw-r--r--   0 pau        (501) staff       (20)     3939 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/init.c
--rw-r--r--   0 pau        (501) staff       (20)     4662 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/pmx.h
--rw-r--r--   0 pau        (501) staff       (20)    17556 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/pmx/wrap_Geometry.c
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/
--rw-r--r--   0 pau        (501) staff       (20)     8847 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/trr2xtc.c
--rw-r--r--   0 pau        (501) staff       (20)    64408 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile.c
--rw-r--r--   0 pau        (501) staff       (20)    23730 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile.h
--rw-r--r--   0 pau        (501) staff       (20)    13474 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c
--rw-r--r--   0 pau        (501) staff       (20)    14744 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_trr.c
--rw-r--r--   0 pau        (501) staff       (20)     2364 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_trr.h
--rw-r--r--   0 pau        (501) staff       (20)     3629 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c
--rw-r--r--   0 pau        (501) staff       (20)     2255 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/scripts/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/
--rwxr-xr-x   0 pau        (501) staff       (20)    68373 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/atoms_to_morph.py
--rwxr-xr-x   0 pau        (501) staff       (20)    79997 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/atoms_to_morph_rdkit2018.py
--rwxr-xr-x   0 pau        (501) staff       (20)    22630 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/build_mst_graph.py
--rwxr-xr-x   0 pau        (501) staff       (20)    50443 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/make_hybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2495 2023-06-19 14:09:16.000000 pmx_biobb-4.0.1/src/pmx/scripts/ligands/one_ff_file.py
--rw-r--r--   0 pau        (501) staff       (20)    19712 2023-06-19 13:29:35.000000 pmx_biobb-4.0.1/src/pmx/scripts/md_setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-21 11:24:50.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    11807 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-19 14:00:41.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       29 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2023-06-21 11:24:49.000000 pmx_biobb-4.0.1/src/pmx_biobb.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)    65963 2023-06-21 11:22:44.000000 pmx_biobb-4.0.1/versioneer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/
+-rw-r--r--   0 pau        (501) staff       (20)     7651 2023-06-14 14:42:12.000000 pmx_biobb-4.0.2/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)       95 2023-06-19 13:37:17.000000 pmx_biobb-4.0.2/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     2087 2023-06-19 13:29:31.000000 pmx_biobb-4.0.2/README.rst
+-rw-r--r--   0 pau        (501) staff       (20)      194 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     2154 2023-06-22 15:03:05.000000 pmx_biobb-4.0.2/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)      459 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/_version.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/
+-rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bbdep.pkl
+-rw-r--r--   0 pau        (501) staff       (20)     1786 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/blosum62_new.mat
+-rw-r--r--   0 pau        (501) staff       (20)   144604 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   149219 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp_amber.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   148935 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp_charmm.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9416 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      951 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)      661 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am
+-rw-r--r--   0 pau        (501) staff       (20)    12694 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)     3873 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/atommass.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2060 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1519 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      181 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)     6253 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)      244 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1660 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9612 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    88617 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)    47717 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1208 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2882 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1767 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)    48593 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)       70 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/mutres.arn
+-rw-r--r--   0 pau        (501) staff       (20)      164 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      126 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)     9712 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      910 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      916 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1369 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1419 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1576 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2237 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      306 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm36mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3940 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/elements.dat
+-rw-r--r--   0 pau        (501) staff       (20)    29266 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/spc216.gro
+-rw-r--r--   0 pau        (501) staff       (20)      343 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/specbond.dat
+-rw-r--r--   0 pau        (501) staff       (20)      447 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/xlateat.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    21524 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     5335 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      130 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)    45478 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7972 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129919 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     4978 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7476 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129937 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    82367 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp
+-rw-r--r--   0 pau        (501) staff       (20)      435 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2734 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2079 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.arn
+-rw-r--r--   0 pau        (501) staff       (20)     1134 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8979 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb
+-rw-r--r--   0 pau        (501) staff       (20)     1397 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      198 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.r2b
+-rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5220 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd
+-rw-r--r--   0 pau        (501) staff       (20)   283035 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   123173 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     1339 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp
+-rw-r--r--   0 pau        (501) staff       (20)      619 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      625 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1026 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1242 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      221 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)    70529 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/rna.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)    13896 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Energy.c
+-rw-r--r--   0 pau        (501) staff       (20)    15145 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.c
+-rw-r--r--   0 pau        (501) staff       (20)    20514 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.h
+-rw-r--r--   0 pau        (501) staff       (20)     2086 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/cpp_test.cpp
+-rw-r--r--   0 pau        (501) staff       (20)     3939 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/init.c
+-rw-r--r--   0 pau        (501) staff       (20)     4662 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/pmx.h
+-rw-r--r--   0 pau        (501) staff       (20)    17556 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/wrap_Geometry.c
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/
+-rw-r--r--   0 pau        (501) staff       (20)     8847 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/trr2xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)    64408 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.c
+-rw-r--r--   0 pau        (501) staff       (20)    23730 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.h
+-rw-r--r--   0 pau        (501) staff       (20)    13474 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c
+-rw-r--r--   0 pau        (501) staff       (20)    14744 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.c
+-rw-r--r--   0 pau        (501) staff       (20)     2364 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.h
+-rw-r--r--   0 pau        (501) staff       (20)     3629 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)     2255 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/scripts/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/
+-rwxr-xr-x   0 pau        (501) staff       (20)    68373 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    79997 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph_rdkit2018.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    22630 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/build_mst_graph.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    50443 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/make_hybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2495 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/one_ff_file.py
+-rw-r--r--   0 pau        (501) staff       (20)    19712 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/scripts/md_setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    11807 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-19 14:00:41.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       29 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)    65963 2023-06-22 15:03:05.000000 pmx_biobb-4.0.2/versioneer.py
```

### Comparing `pmx_biobb-4.0.1/LICENSE` & `pmx_biobb-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/PKG-INFO` & `pmx_biobb-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx_biobb
-Version: 4.0.1
+Version: 4.0.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.0.1/README.rst` & `pmx_biobb-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/setup.py` & `pmx_biobb-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                   )
 extensions = [pmx, xdrio]
 
 # -----
 # Setup
 # -----
 setup(name='pmx_biobb',
-      version='4.0.1',
+      version='4.0.2',
       cmdclass=versioneer.get_cmdclass(),
       description='Toolkit for free-energy calculation setup/analysis '
                   'and biomolecular structure handling',
       long_description=readme(),
       classifiers=[
         'Programming Language :: Python',
         'Intended Audience :: Science/Research',
@@ -58,9 +58,13 @@
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       ext_modules=extensions,
       tests_require=['pytest'],
       install_requires=['numpy', 'scipy', 'matplotlib', 'rdkit'],
       python_requires=">=3.7",
-      entry_points={'console_scripts': ['pmx = pmx.scripts.cli:entry_point']},
+      entry_points={
+          "console_scripts": [
+              "pmx = pmx.scripts.cli:entry_point"
+          ]
+        },
       )
```

### Comparing `pmx_biobb-4.0.1/src/pmx/data/bbdep.pkl` & `pmx_biobb-4.0.2/src/pmx/data/bbdep.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/blosum62_new.mat` & `pmx_biobb-4.0.2/src/pmx/data/blosum62_new.mat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/bp.pkl` & `pmx_biobb-4.0.2/src/pmx/data/bp.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/bp_amber.pkl` & `pmx_biobb-4.0.2/src/pmx/data/bp_amber.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/bp_charmm.pkl` & `pmx_biobb-4.0.2/src/pmx/data/bp_charmm.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/atommass.dat` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/atommass.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/elements.dat` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/elements.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45/spc216.gro` & `pmx_biobb-4.0.2/src/pmx/data/mutff45/spc216.gro`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp` & `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/data/rna.pkl` & `pmx_biobb-4.0.2/src/pmx/data/rna.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/Energy.c` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Energy.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/Geometry.c` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/Geometry.h` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/cpp_test.cpp` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/cpp_test.cpp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/init.c` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/init.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/pmx.h` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/pmx.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/pmx/wrap_Geometry.c` & `pmx_biobb-4.0.2/src/pmx/extensions/pmx/wrap_Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/trr2xtc.c` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/trr2xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile.c` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile.h` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_trr.c` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_trr.h` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h` & `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/ligands/atoms_to_morph.py` & `pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/ligands/atoms_to_morph_rdkit2018.py` & `pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph_rdkit2018.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/ligands/build_mst_graph.py` & `pmx_biobb-4.0.2/src/pmx/scripts/ligands/build_mst_graph.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/ligands/make_hybrid.py` & `pmx_biobb-4.0.2/src/pmx/scripts/ligands/make_hybrid.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/ligands/one_ff_file.py` & `pmx_biobb-4.0.2/src/pmx/scripts/ligands/one_ff_file.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx/scripts/md_setup.py` & `pmx_biobb-4.0.2/src/pmx/scripts/md_setup.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/src/pmx_biobb.egg-info/PKG-INFO` & `pmx_biobb-4.0.2/src/pmx_biobb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx-biobb
-Version: 4.0.1
+Version: 4.0.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.0.1/src/pmx_biobb.egg-info/SOURCES.txt` & `pmx_biobb-4.0.2/src/pmx_biobb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.1/versioneer.py` & `pmx_biobb-4.0.2/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,26 +734,26 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 4.0.1
+    1: no tags. git_describe was just HEX. 4.0.2
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "4.0.1" %% (pieces["distance"],
+        rendered = "4.0.2" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
@@ -1235,26 +1235,26 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 4.0.1
+    1: no tags. git_describe was just HEX. 4.0.2
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "4.0.1"
+        rendered = "4.0.2"
 
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
 
@@ -1395,15 +1395,15 @@
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available."""
 
-    return {"version": "4.0.1", "full-revisionid": None,
+    return {"version": "4.0.2", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
```

