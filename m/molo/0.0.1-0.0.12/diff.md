# Comparing `tmp/molo-0.0.1.tar.gz` & `tmp/molo-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molo-0.0.1.tar", last modified: Thu Jun 22 08:45:03 2023, max compression
+gzip compressed data, was "molo-0.0.12.tar", last modified: Thu Jun 22 09:39:40 2023, max compression
```

## Comparing `molo-0.0.1.tar` & `molo-0.0.12.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:45:03.774278 molo-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-22 06:51:47.000000 molo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      438 2023-06-22 08:45:03.774278 molo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-06-22 06:52:37.000000 molo-0.0.1/README.md
--rw-rw-rw-   0        0        0      111 2023-06-22 06:48:25.000000 molo-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      517 2023-06-22 08:45:03.783278 molo-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 08:45:03.742280 molo-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 08:45:03.770279 molo-0.0.1/src/molo.egg-info/
--rw-rw-rw-   0        0        0      438 2023-06-22 08:45:03.000000 molo-0.0.1/src/molo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-22 08:45:03.000000 molo-0.0.1/src/molo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:45:03.000000 molo-0.0.1/src/molo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 08:45:03.000000 molo-0.0.1/src/molo.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 08:45:03.773279 molo-0.0.1/src/mypackage/
--rw-rw-rw-   0        0        0        3 2023-06-22 06:44:00.000000 molo-0.0.1/src/mypackage/__init__.py
--rw-rw-rw-   0        0        0       50 2023-06-22 06:46:00.000000 molo-0.0.1/src/mypackage/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 09:39:40.321441 molo-0.0.12/
+-rw-rw-rw-   0        0        0     1094 2023-06-22 06:51:47.000000 molo-0.0.12/LICENSE
+-rw-rw-rw-   0        0        0      439 2023-06-22 09:39:40.322440 molo-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-06-22 06:52:37.000000 molo-0.0.12/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-22 06:48:25.000000 molo-0.0.12/pyproject.toml
+-rw-rw-rw-   0        0        0      518 2023-06-22 09:39:40.324441 molo-0.0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 09:39:40.273444 molo-0.0.12/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 09:39:40.297443 molo-0.0.12/src/molo.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-06-22 09:39:40.000000 molo-0.0.12/src/molo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-22 09:39:40.000000 molo-0.0.12/src/molo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 09:39:40.000000 molo-0.0.12/src/molo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 09:39:40.000000 molo-0.0.12/src/molo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 09:39:40.320441 molo-0.0.12/src/mypackage/
+-rw-rw-rw-   0        0        0        3 2023-06-22 06:44:00.000000 molo-0.0.12/src/mypackage/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-06-22 06:46:00.000000 molo-0.0.12/src/mypackage/main.py
+-rw-rw-rw-   0        0        0      930 2023-06-22 09:38:12.000000 molo-0.0.12/src/mypackage/print.py
```

### Comparing `molo-0.0.1/LICENSE` & `molo-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `molo-0.0.1/setup.cfg` & `molo-0.0.12/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6c 6f0d 0a76 6572 7369 6f6e   = molo..version
-00000020: 203d 2030 2e30 2e31 0d0a 6175 7468 6f72   = 0.0.1..author
-00000030: 203d 2050 7261 6e61 765f 530d 0a61 7574   = Pranav_S..aut
-00000040: 686f 725f 656d 6169 6c20 3d20 7072 616e  hor_email = pran
-00000050: 6176 7340 6472 6e67 7069 742e 6163 2e69  avs@drngpit.ac.i
-00000060: 6e0d 0a64 6573 6372 6970 7469 6f6e 203d  n..description =
-00000070: 2041 2073 6d61 6c6c 2065 7861 6d70 6c65   A small example
-00000080: 2070 6163 6b61 6765 0d0a 6c6f 6e67 5f64   package..long_d
-00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000a0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000c0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000d0: 7874 2f6d 6172 6b64 6f77 6e0d 0a63 6c61  xt/markdown..cla
-000000e0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000000f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000100: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000110: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000120: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000130: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000140: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000150: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000160: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000170: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000180: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000190: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000001a0: 6571 7569 7265 7320 3d20 3e3d 332e 360d  equires = >=3.6.
-000001b0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000001c0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000001d0: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-000001e0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000001f0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000200: 300d 0a0d 0a                             0....
+00000020: 203d 2030 2e30 2e31 320d 0a61 7574 686f   = 0.0.12..autho
+00000030: 7220 3d20 5072 616e 6176 5f53 0d0a 6175  r = Pranav_S..au
+00000040: 7468 6f72 5f65 6d61 696c 203d 2070 7261  thor_email = pra
+00000050: 6e61 7673 4064 726e 6770 6974 2e61 632e  navs@drngpit.ac.
+00000060: 696e 0d0a 6465 7363 7269 7074 696f 6e20  in..description 
+00000070: 3d20 4120 736d 616c 6c20 6578 616d 706c  = A small exampl
+00000080: 6520 7061 636b 6167 650d 0a6c 6f6e 675f  e package..long_
+00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000a0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+000000b0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+000000c0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+000000d0: 6578 742f 6d61 726b 646f 776e 0d0a 636c  ext/markdown..cl
+000000e0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+000000f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000100: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000110: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000120: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000130: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000140: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000150: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000160: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000170: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000180: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
+00000190: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+000001a0: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
+000001b0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000001c0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+000001d0: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
+000001e0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000001f0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000200: 2030 0d0a 0d0a                            0....
```

