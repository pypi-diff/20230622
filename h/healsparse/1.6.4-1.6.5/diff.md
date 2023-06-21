# Comparing `tmp/healsparse-1.6.4.tar.gz` & `tmp/healsparse-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healsparse-1.6.4.tar", last modified: Mon Mar 27 21:25:40 2023, max compression
+gzip compressed data, was "healsparse-1.6.5.tar", last modified: Wed Jun 21 23:52:20 2023, max compression
```

## Comparing `healsparse-1.6.4.tar` & `healsparse-1.6.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.067512 healsparse-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 21:25:21.000000 healsparse-1.6.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 21:25:21.000000 healsparse-1.6.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.027511 healsparse-1.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.035512 healsparse-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-27 21:25:21.000000 healsparse-1.6.4/.github/workflows/python-package-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-27 21:25:21.000000 healsparse-1.6.4/.github/workflows/python-package-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-27 21:25:21.000000 healsparse-1.6.4/.github/workflows/python-package-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-27 21:25:21.000000 healsparse-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 21:25:21.000000 healsparse-1.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-27 21:25:21.000000 healsparse-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 21:25:21.000000 healsparse-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-27 21:25:40.071512 healsparse-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-27 21:25:21.000000 healsparse-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-27 21:25:21.000000 healsparse-1.6.4/api_changes_to_1.0.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.039512 healsparse-1.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/basic_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/concatenation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/filespec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/randoms.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 21:25:21.000000 healsparse-1.6.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.047512 healsparse-1.6.4/healsparse/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/cat_healsparse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    79336 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/healSparseMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/healSparseRandoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_coverage_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_coverage_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_map_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_map_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/io_map_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/parquet_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-03-27 21:25:21.000000 healsparse-1.6.4/healsparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.047512 healsparse-1.6.4/healsparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-27 21:25:39.000000 healsparse-1.6.4/healsparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-27 21:25:40.000000 healsparse-1.6.4/healsparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:25:39.000000 healsparse-1.6.4/healsparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-27 21:25:39.000000 healsparse-1.6.4/healsparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 21:25:39.000000 healsparse-1.6.4/healsparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-27 21:25:21.000000 healsparse-1.6.4/long_description.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 21:25:21.000000 healsparse-1.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-27 21:25:40.071512 healsparse-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-27 21:25:21.000000 healsparse-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.067512 healsparse-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_applymask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_buildmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_cat_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_coverage_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_coverage_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    29282 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_degrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_emptypixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_fracdet_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_from_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_generate_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_getset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_healpix_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_io_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_moc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47867 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_recarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_single_covpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_single_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_singlevalues.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_update_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_validarea.py
--rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-03-27 21:25:21.000000 healsparse-1.6.4/tests/test_widemasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.067512 healsparse-1.6.4/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-03-27 21:25:21.000000 healsparse-1.6.4/tutorial/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:25:40.067512 healsparse-1.6.4/ups/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 21:25:21.000000 healsparse-1.6.4/ups/healsparse.table
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 23:52:04.000000 healsparse-1.6.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 23:52:04.000000 healsparse-1.6.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.963693 healsparse-1.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.967694 healsparse-1.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 23:52:04.000000 healsparse-1.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-21 23:52:04.000000 healsparse-1.6.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-21 23:52:04.000000 healsparse-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 23:52:04.000000 healsparse-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 23:52:20.979695 healsparse-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-21 23:52:04.000000 healsparse-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-21 23:52:04.000000 healsparse-1.6.5/api_changes_to_1.0.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.971694 healsparse-1.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/basic_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/concatenation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/filespec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/randoms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.975694 healsparse-1.6.5/healsparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/cat_healsparse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79398 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseRandoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/parquet_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.975694 healsparse-1.6.5/healsparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-21 23:52:04.000000 healsparse-1.6.5/long_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 23:52:04.000000 healsparse-1.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 23:52:20.979695 healsparse-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 23:52:04.000000 healsparse-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_applymask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_buildmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_cat_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_coverage_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_coverage_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29282 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_degrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_emptypixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_fracdet_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_from_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_generate_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_getset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_healpix_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_io_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_moc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47867 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_recarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_single_covpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_single_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_singlevalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_update_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_validarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_widemasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-21 23:52:04.000000 healsparse-1.6.5/tutorial/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/ups/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 23:52:04.000000 healsparse-1.6.5/ups/healsparse.table
```

### Comparing `healsparse-1.6.4/.github/workflows/python-package-pr.yml` & `healsparse-1.6.5/.github/workflows/python-package-pr.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `healsparse-1.6.4/.github/workflows/python-package-publish.yml` & `healsparse-1.6.5/.github/workflows/python-package-publish.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/.github/workflows/python-package-push.yml` & `healsparse-1.6.5/.github/workflows/python-package-push.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/.readthedocs.yml` & `healsparse-1.6.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/LICENSE` & `healsparse-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/PKG-INFO` & `healsparse-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.6.4
+Version: 1.6.5
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and others
 Author-email: erykoff@stanford.edu
 Description-Content-Type: text/markdown
 Provides-Extra: parquet
 Provides-Extra: healpy
```

### Comparing `healsparse-1.6.4/README.md` & `healsparse-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/api_changes_to_1.0.md` & `healsparse-1.6.5/api_changes_to_1.0.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/Makefile` & `healsparse-1.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/basic_interface.rst` & `healsparse-1.6.5/docs/basic_interface.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/concatenation.rst` & `healsparse-1.6.5/docs/concatenation.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/conf.py` & `healsparse-1.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/filespec.rst` & `healsparse-1.6.5/docs/filespec.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/geometry.rst` & `healsparse-1.6.5/docs/geometry.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/index.rst` & `healsparse-1.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/install.rst` & `healsparse-1.6.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/make.bat` & `healsparse-1.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/modules.rst` & `healsparse-1.6.5/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/operations.rst` & `healsparse-1.6.5/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/docs/randoms.rst` & `healsparse-1.6.5/docs/randoms.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/__init__.py` & `healsparse-1.6.5/healsparse/__init__.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/cat_healsparse_files.py` & `healsparse-1.6.5/healsparse/cat_healsparse_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/fits_shim.py` & `healsparse-1.6.5/healsparse/fits_shim.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,18 +229,26 @@
     hdu = fits.PrimaryHDU(data=cov_index_map, header=fits.Header())
     for n in c_hdr:
         if n not in FITS_RESERVED:
             hdu.header[n] = c_hdr[n]
     hdu_list.append(hdu)
 
     if compress:
-        hdu = fits.CompImageHDU(data=sparse_map, header=fits.Header(),
-                                compression_type='GZIP_2',
-                                tile_size=(compress_tilesize, ),
-                                quantize_level=0.0)
+        try:
+            # Try new tile_shape API (astropy>=5.3).
+            hdu = fits.CompImageHDU(data=sparse_map, header=fits.Header(),
+                                    compression_type='GZIP_2',
+                                    tile_shape=(compress_tilesize, ),
+                                    quantize_level=0.0)
+        except TypeError:
+            # Fall back to old tile_size API.
+            hdu = fits.CompImageHDU(data=sparse_map, header=fits.Header(),
+                                    compression_type='GZIP_2',
+                                    tile_size=(compress_tilesize, ),
+                                    quantize_level=0.0)
     else:
         if sparse_map.dtype.fields is not None:
             hdu = fits.BinTableHDU(data=sparse_map, header=fits.Header())
         else:
             hdu = fits.ImageHDU(data=sparse_map, header=fits.Header())
 
     for n in s_hdr:
```

### Comparing `healsparse-1.6.4/healsparse/geom.py` & `healsparse-1.6.5/healsparse/geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/healSparseCoverage.py` & `healsparse-1.6.5/healsparse/healSparseCoverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/healSparseMap.py` & `healsparse-1.6.5/healsparse/healSparseMap.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         Returns
         -------
         healSparseMap : `HealSparseMap`
         """
         if cov_index_map is not None and cov_map is not None:
             raise RuntimeError('Cannot specify both cov_index_map and cov_map')
         if cov_index_map is not None:
-            import warnings
             warnings.warn("cov_index_map deprecated", DeprecationWarning)
             cov_map = HealSparseCoverage(cov_index_map, nside_sparse)
 
         if cov_map is not None and sparse_map is not None and nside_sparse is not None:
             # this is a sparse map input
             self._cov_map = cov_map
             self._sparse_map = sparse_map
@@ -1719,19 +1718,20 @@
             New map with new data type.
         """
         if self._is_rec_array:
             raise RuntimeError("Cannot convert datatype of a recarray map.")
         elif self._is_wide_mask:
             raise RuntimeError("Cannot convert datatype of a wide mask.")
 
-        new_sparse_map = self._sparse_map.astype(dtype)
-        _sentinel = check_sentinel(new_sparse_map.dtype.type, sentinel)
+        new_sparse_map = np.zeros(self._sparse_map.shape, dtype=dtype)
+        valid_pix = (self._sparse_map != self._sentinel)
+        new_sparse_map[valid_pix] = self._sparse_map[valid_pix].astype(dtype)
 
-        invalid_pix = (self._sparse_map == self._sentinel)
-        new_sparse_map[invalid_pix] = _sentinel
+        _sentinel = check_sentinel(new_sparse_map.dtype.type, sentinel)
+        new_sparse_map[~valid_pix] = _sentinel
 
         return HealSparseMap(cov_map=self._cov_map, sparse_map=new_sparse_map,
                              nside_sparse=self.nside_sparse, sentinel=_sentinel)
 
     def __add__(self, other):
         """
         Add a constant.
```

### Comparing `healsparse-1.6.4/healsparse/healSparseRandoms.py` & `healsparse-1.6.5/healsparse/healSparseRandoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_coverage.py` & `healsparse-1.6.5/healsparse/io_coverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_coverage_fits.py` & `healsparse-1.6.5/healsparse/io_coverage_fits.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_coverage_parquet.py` & `healsparse-1.6.5/healsparse/io_coverage_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_map.py` & `healsparse-1.6.5/healsparse/io_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_map_fits.py` & `healsparse-1.6.5/healsparse/io_map_fits.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_map_healpix.py` & `healsparse-1.6.5/healsparse/io_map_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/io_map_parquet.py` & `healsparse-1.6.5/healsparse/io_map_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/operations.py` & `healsparse-1.6.5/healsparse/operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/parquet_shim.py` & `healsparse-1.6.5/healsparse/parquet_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse/utils.py` & `healsparse-1.6.5/healsparse/utils.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/healsparse.egg-info/PKG-INFO` & `healsparse-1.6.5/healsparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.6.4
+Version: 1.6.5
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and others
 Author-email: erykoff@stanford.edu
 Description-Content-Type: text/markdown
 Provides-Extra: parquet
 Provides-Extra: healpy
```

### Comparing `healsparse-1.6.4/healsparse.egg-info/SOURCES.txt` & `healsparse-1.6.5/healsparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/long_description.md` & `healsparse-1.6.5/long_description.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/setup.py` & `healsparse-1.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_applymask.py` & `healsparse-1.6.5/tests/test_applymask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_astype.py` & `healsparse-1.6.5/tests/test_astype.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_buildmaps.py` & `healsparse-1.6.5/tests/test_buildmaps.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_cat_files.py` & `healsparse-1.6.5/tests/test_cat_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_coverage_map.py` & `healsparse-1.6.5/tests/test_coverage_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_coverage_mask.py` & `healsparse-1.6.5/tests/test_coverage_mask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_degrade.py` & `healsparse-1.6.5/tests/test_degrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_emptypixels.py` & `healsparse-1.6.5/tests/test_emptypixels.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_fits_shim.py` & `healsparse-1.6.5/tests/test_fits_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_fracdet_map.py` & `healsparse-1.6.5/tests/test_fracdet_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_from_healpix.py` & `healsparse-1.6.5/tests/test_from_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_generate_healpix.py` & `healsparse-1.6.5/tests/test_generate_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_geom.py` & `healsparse-1.6.5/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_getset.py` & `healsparse-1.6.5/tests/test_getset.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_healSparseCoverage.py` & `healsparse-1.6.5/tests/test_healSparseCoverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_healpix_io.py` & `healsparse-1.6.5/tests/test_healpix_io.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_io.py` & `healsparse-1.6.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_io_parquet.py` & `healsparse-1.6.5/tests/test_io_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_lookup.py` & `healsparse-1.6.5/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_metadata.py` & `healsparse-1.6.5/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_moc.py` & `healsparse-1.6.5/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_operations.py` & `healsparse-1.6.5/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_randoms.py` & `healsparse-1.6.5/tests/test_randoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_recarray.py` & `healsparse-1.6.5/tests/test_recarray.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_single_covpix.py` & `healsparse-1.6.5/tests/test_single_covpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_single_datatypes.py` & `healsparse-1.6.5/tests/test_single_datatypes.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_singlevalues.py` & `healsparse-1.6.5/tests/test_singlevalues.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_update_values.py` & `healsparse-1.6.5/tests/test_update_values.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_upgrade.py` & `healsparse-1.6.5/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_validarea.py` & `healsparse-1.6.5/tests/test_validarea.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tests/test_widemasks.py` & `healsparse-1.6.5/tests/test_widemasks.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.4/tutorial/quickstart.ipynb` & `healsparse-1.6.5/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

