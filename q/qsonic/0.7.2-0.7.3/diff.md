# Comparing `tmp/qsonic-0.7.2.tar.gz` & `tmp/qsonic-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.7.2.tar", last modified: Tue Jun 20 22:08:28 2023, max compression
+gzip compressed data, was "qsonic-0.7.3.tar", last modified: Wed Jun 21 22:20:31 2023, max compression
```

## Comparing `qsonic-0.7.2.tar` & `qsonic-0.7.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.300312 qsonic-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 22:08:04.000000 qsonic-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-20 22:08:28.300312 qsonic-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 22:08:04.000000 qsonic-0.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52579 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 22:08:04.000000 qsonic-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 22:08:04.000000 qsonic-0.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 22:08:28.300312 qsonic-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:08:04.000000 qsonic-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.300312 qsonic-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.965005 qsonic-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 22:20:12.000000 qsonic-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 22:20:31.965005 qsonic-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-21 22:20:12.000000 qsonic-0.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.957005 qsonic-0.7.3/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52579 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 22:20:12.000000 qsonic-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 22:20:12.000000 qsonic-0.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-21 22:20:31.965005 qsonic-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:20:12.000000 qsonic-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.965005 qsonic-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_spectrum.py
```

### Comparing `qsonic-0.7.2/LICENSE` & `qsonic-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/PKG-INFO` & `qsonic-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.2
+Version: 0.7.3
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -19,14 +19,17 @@
 ======
 
 *Lightining-fast continuum fitting*
 
 .. image:: https://img.shields.io/pypi/v/qsonic?color=blue
     :target: https://pypi.org/project/qsonic
 
+.. image:: https://img.shields.io/badge/Source-qsonic-red
+    :target: https://github.com/p-slash/qsonic
+
 .. image:: https://github.com/p-slash/qsonic/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/p-slash/qsonic/actions/workflows/testing.yml
     :alt: Tests Status
 
 .. image:: https://readthedocs.org/projects/qsonic/badge/?version=latest
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `qsonic-0.7.2/README.rst` & `qsonic-0.7.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 ======
 
 *Lightining-fast continuum fitting*
 
 .. image:: https://img.shields.io/pypi/v/qsonic?color=blue
     :target: https://pypi.org/project/qsonic
 
+.. image:: https://img.shields.io/badge/Source-qsonic-red
+    :target: https://github.com/p-slash/qsonic
+
 .. image:: https://github.com/p-slash/qsonic/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/p-slash/qsonic/actions/workflows/testing.yml
     :alt: Tests Status
 
 .. image:: https://readthedocs.org/projects/qsonic/badge/?version=latest
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `qsonic-0.7.2/py/qsonic/calibration.py` & `qsonic-0.7.3/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/catalog.py` & `qsonic-0.7.3/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/io.py` & `qsonic-0.7.3/py/qsonic/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,16 @@
     pixnum = catalog_hpx['HPXPIXEL'][0]
     fspec = f"{input_dir}/{pixnum//100}/{pixnum}/spectra-{nside}-{pixnum}.fits"
     data, idx_cat = _read_onehealpix_file(
         catalog_hpx['TARGETID'], fspec, arms_to_keep, skip_resomat)
 
     fspec = f"{input_dir}/{pixnum//100}/{pixnum}/truth-{nside}-{pixnum}.fits"
     if read_true_continuum:
-        data['cont'] = _read_true_continuum(catalog_hpx['TARGETID'], fspec)
+        data['cont'] = _read_true_continuum(
+            catalog_hpx['TARGETID'][idx_cat], fspec)
 
     if skip_resomat:
         return data, idx_cat
 
     with fitsio.FITS(fspec) as fitsfile:
         for arm in arms_to_keep:
             data['reso'][arm] = np.array(fitsfile[f'{arm}_RESOLUTION'].read())
```

### Comparing `qsonic-0.7.2/py/qsonic/masks.py` & `qsonic-0.7.3/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/mathtools.py` & `qsonic-0.7.3/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/mpi_utils.py` & `qsonic-0.7.3/py/qsonic/mpi_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,19 +28,18 @@
         Options to parse. None parses ``sys.argv``
     args_logic_fnc: Callable[[args], bool], default: True
         Logic function to check for args.
     """
     if mpi_rank == 0:
         try:
             args = parser.parse_args(options)
+            if not args_logic_fnc(args):
+                args = -1
         except SystemExit:
             args = -1
-
-        if not args_logic_fnc(args):
-            args = -1
     else:
         args = -1
 
     args = comm.bcast(args)
     if args == -1:
         exit(0)
```

### Comparing `qsonic-0.7.2/py/qsonic/picca_continuum.py` & `qsonic-0.7.3/py/qsonic/picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.7.3/py/qsonic/scripts/qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.7.3/py/qsonic/scripts/qsonic_fit.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic/spectrum.py` & `qsonic-0.7.3/py/qsonic/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.7.3/py/qsonic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.2
+Version: 0.7.3
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -19,14 +19,17 @@
 ======
 
 *Lightining-fast continuum fitting*
 
 .. image:: https://img.shields.io/pypi/v/qsonic?color=blue
     :target: https://pypi.org/project/qsonic
 
+.. image:: https://img.shields.io/badge/Source-qsonic-red
+    :target: https://github.com/p-slash/qsonic
+
 .. image:: https://github.com/p-slash/qsonic/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/p-slash/qsonic/actions/workflows/testing.yml
     :alt: Tests Status
 
 .. image:: https://readthedocs.org/projects/qsonic/badge/?version=latest
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `qsonic-0.7.2/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.7.3/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/setup.cfg` & `qsonic-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.2
+current_version = 0.7.3
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.7.2/tests/test_catalog.py` & `qsonic-0.7.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_io.py` & `qsonic-0.7.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_masks.py` & `qsonic-0.7.3/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_mathtools.py` & `qsonic-0.7.3/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_mpi_utils.py` & `qsonic-0.7.3/tests/test_mpi_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
         with pytest.raises(SystemExit):
             options = ("--input-dir indir --catalog incat -o outdir "
                        "--true-continuum").split(' ')
             qsonic.mpi_utils.mpi_parse(parser, comm, mpi_rank, options,
                                        args_logic_fnc_qsonic_fit)
 
+        with pytest.raises(SystemExit):
+            qsonic.mpi_utils.mpi_parse(parser, comm, mpi_rank, ['-h'],
+                                       args_logic_fnc_qsonic_fit)
+
     def test_mpi_fnc_bcast(self):
         matrix = np.arange(20).reshape(4, 5)
         u, s, vh = np.linalg.svd(matrix)
         result = qsonic.mpi_utils.mpi_fnc_bcast(
             np.linalg.svd, None, 0, "Error", matrix)
 
         npt.assert_allclose(result[0], u)
```

### Comparing `qsonic-0.7.2/tests/test_picca_continuum.py` & `qsonic-0.7.3/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_qsonic_calib.py` & `qsonic-0.7.3/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.2/tests/test_spectrum.py` & `qsonic-0.7.3/tests/test_spectrum.py`

 * *Files identical despite different names*

