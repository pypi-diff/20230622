# Comparing `tmp/biaslyze-0.0.5a0.tar.gz` & `tmp/biaslyze-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaslyze-0.0.5a0.tar", max compression
+gzip compressed data, was "biaslyze-0.0.6a0.tar", max compression
```

## Comparing `biaslyze-0.0.5a0.tar` & `biaslyze-0.0.6a0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.5a0/LICENSE
--rw-r--r--   0        0        0     2878 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/README.md
--rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.5a0/biaslyze/__init__.py
--rw-r--r--   0        0        0     6931 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/_plotting.py
--rw-r--r--   0        0        0      220 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/bias_detectors/__init__.py
--rw-r--r--   0        0        0    12495 2023-06-01 13:06:40.492303 biaslyze-0.0.5a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
--rw-r--r--   0        0        0     5547 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/bias_detectors/lime_biasdetector.py
--rw-r--r--   0        0        0     1831 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/concept_detectors.py
--rw-r--r--   0        0        0    64680 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/concepts.py
--rw-r--r--   0        0        0    12925 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/results/counterfactual_detection_results.py
--rw-r--r--   0        0        0     4990 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/results/lime_detection_results.py
--rw-r--r--   0        0        0     1644 2023-06-01 13:32:30.961900 biaslyze-0.0.5a0/pyproject.toml
--rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 biaslyze-0.0.5a0/setup.py
--rw-r--r--   0        0        0     4831 1970-01-01 00:00:00.000000 biaslyze-0.0.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.6a0/LICENSE
+-rw-r--r--   0        0        0     3457 2023-06-22 11:24:11.649837 biaslyze-0.0.6a0/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.6a0/biaslyze/__init__.py
+-rw-r--r--   0        0        0     6931 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/_plotting.py
+-rw-r--r--   0        0        0      220 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/bias_detectors/__init__.py
+-rw-r--r--   0        0        0    13446 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
+-rw-r--r--   0        0        0     5547 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/bias_detectors/lime_biasdetector.py
+-rw-r--r--   0        0        0     5511 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/concept_class.py
+-rw-r--r--   0        0        0     1831 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/concept_detectors.py
+-rw-r--r--   0        0        0    64680 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/concepts.py
+-rw-r--r--   0        0        0    12924 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/results/counterfactual_detection_results.py
+-rw-r--r--   0        0        0     4990 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/results/lime_detection_results.py
+-rw-r--r--   0        0        0     2546 2023-06-22 11:25:40.997149 biaslyze-0.0.6a0/biaslyze/text_representation.py
+-rw-r--r--   0        0        0     1681 2023-06-22 11:25:13.421364 biaslyze-0.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 biaslyze-0.0.6a0/setup.py
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 biaslyze-0.0.6a0/PKG-INFO
```

### Comparing `biaslyze-0.0.5a0/LICENSE` & `biaslyze-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/README.md` & `biaslyze-0.0.6a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,180 +1,217 @@
-00000000: 2320 6269 6173 6c79 7a65 202d 2054 6865  # biaslyze - The
-00000010: 204e 4c50 2042 6961 7320 4964 656e 7469   NLP Bias Identi
-00000020: 6669 6361 7469 6f6e 2054 6f6f 6c6b 6974  fication Toolkit
-00000030: 0a0a 4269 6173 2069 7320 6f66 7465 6e20  ..Bias is often 
-00000040: 7375 6274 6c65 2061 6e64 2064 6966 6669  subtle and diffi
-00000050: 6375 6c74 2074 6f20 6465 7465 6374 2069  cult to detect i
-00000060: 6e20 4e4c 5020 6d6f 6465 6c73 2c20 6173  n NLP models, as
-00000070: 2074 6865 2070 726f 7465 6374 6564 2061   the protected a
-00000080: 7474 7269 6275 7465 7320 6172 6520 6c65  ttributes are le
-00000090: 7373 206f 6276 696f 7573 2061 6e64 2063  ss obvious and c
-000000a0: 616e 2074 616b 6520 6d61 6e79 2066 6f72  an take many for
-000000b0: 6d73 2069 6e20 6c61 6e67 7561 6765 2028  ms in language (
-000000c0: 652e 672e 2070 726f 7869 6573 2c20 646f  e.g. proxies, do
-000000d0: 7562 6c65 206d 6561 6e69 6e67 732c 2061  uble meanings, a
-000000e0: 6d62 6967 7569 7469 6573 2065 7463 2e29  mbiguities etc.)
-000000f0: 2e20 5468 6572 6566 6f72 652c 2074 6563  . Therefore, tec
-00000100: 686e 6963 616c 2062 6961 7320 7465 7374  hnical bias test
-00000110: 696e 6720 6973 2061 206b 6579 2073 7465  ing is a key ste
-00000120: 7020 696e 2061 766f 6964 696e 6720 616c  p in avoiding al
-00000130: 676f 7269 7468 6d69 6361 6c6c 7920 6d65  gorithmically me
-00000140: 6469 6174 6564 2064 6973 6372 696d 696e  diated discrimin
-00000150: 6174 696f 6e2e 2048 6f77 6576 6572 2c20  ation. However, 
-00000160: 6974 2069 7320 6375 7272 656e 746c 7920  it is currently 
-00000170: 636f 6e64 7563 7465 6420 746f 6f20 7261  conducted too ra
-00000180: 7265 6c79 2064 7565 2074 6f20 7468 6520  rely due to the 
-00000190: 6566 666f 7274 2069 6e76 6f6c 7665 642c  effort involved,
-000001a0: 206d 6973 7369 6e67 2072 6573 6f75 7263   missing resourc
-000001b0: 6573 206f 7220 6c61 636b 206f 6620 6177  es or lack of aw
-000001c0: 6172 656e 6573 7320 666f 7220 7468 6520  areness for the 
-000001d0: 7072 6f62 6c65 6d2e 0a0a 4269 6173 6c79  problem...Biasly
-000001e0: 7a65 2068 656c 7073 2074 6f20 6765 7420  ze helps to get 
-000001f0: 7374 6172 7465 6420 7769 7468 2074 6865  started with the
-00000200: 2061 6e61 6c79 7369 7320 6f66 2062 6961   analysis of bia
-00000210: 7320 7769 7468 696e 204e 4c50 206d 6f64  s within NLP mod
-00000220: 656c 7320 616e 6420 6f66 6665 7273 2061  els and offers a
-00000230: 2063 6f6e 6372 6574 6520 656e 7472 7920   concrete entry 
-00000240: 706f 696e 7420 666f 7220 6675 7274 6865  point for furthe
-00000250: 7220 696d 7061 6374 2061 7373 6573 736d  r impact assessm
-00000260: 656e 7473 2061 6e64 206d 6974 6967 6174  ents and mitigat
-00000270: 696f 6e20 6d65 6173 7572 6573 2e20 4573  ion measures. Es
-00000280: 7065 6369 616c 6c79 2066 6f72 2079 6f75  pecially for you
-00000290: 6e67 2064 6576 656c 6f70 6572 732c 2073  ng developers, s
-000002a0: 7475 6465 6e74 7320 616e 6420 7465 616d  tudents and team
-000002b0: 7320 7769 7468 206c 696d 6974 6564 2072  s with limited r
-000002c0: 6573 6f75 7263 6573 2c20 6f75 7220 746f  esources, our to
-000002d0: 6f6c 626f 7820 6f66 6665 7273 2061 206c  olbox offers a l
-000002e0: 6f77 2d65 6666 6f72 7420 6170 7072 6f61  ow-effort approa
-000002f0: 6368 2074 6f20 6269 6173 2074 6573 7469  ch to bias testi
-00000300: 6e67 2069 6e20 4e4c 5020 7573 6520 6361  ng in NLP use ca
-00000310: 7365 732e 0a0a 2323 2049 6e73 7461 6c6c  ses...## Install
-00000320: 6174 696f 6e0a 0a49 6e73 7461 6c6c 6174  ation..Installat
-00000330: 696f 6e20 6361 6e20 6265 2064 6f6e 6520  ion can be done 
-00000340: 7573 696e 6720 7079 7069 3a0a 6060 6062  using pypi:.```b
-00000350: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00000360: 6269 6173 6c79 7a65 0a60 6060 0a0a 2323  biaslyze.```..##
-00000370: 2051 7569 636b 7374 6172 740a 0a60 6060   Quickstart..```
-00000380: 7079 7468 6f6e 0a66 726f 6d20 6269 6173  python.from bias
-00000390: 6c79 7a65 2e62 6961 735f 6465 7465 6374  lyze.bias_detect
-000003a0: 6f72 7320 696d 706f 7274 2043 6f75 6e74  ors import Count
-000003b0: 6572 6661 6374 7561 6c42 6961 7344 6574  erfactualBiasDet
-000003c0: 6563 746f 720a 0a62 6961 735f 6465 7465  ector..bias_dete
-000003d0: 6374 6f72 203d 2043 6f75 6e74 6572 6661  ctor = Counterfa
-000003e0: 6374 7561 6c42 6961 7344 6574 6563 746f  ctualBiasDetecto
-000003f0: 7228 290a 0a23 2064 6574 6563 7420 6269  r()..# detect bi
-00000400: 6173 2069 6e20 7468 6520 6d6f 6465 6c20  as in the model 
-00000410: 6261 7365 6420 6f6e 2074 6865 2067 6976  based on the giv
-00000420: 656e 2074 6578 7473 0a23 2068 6572 652c  en texts.# here,
-00000430: 2063 6c66 2069 7320 6120 7363 696b 6974   clf is a scikit
-00000440: 2d6c 6561 726e 2074 6578 7420 636c 6173  -learn text clas
-00000450: 7369 6669 6361 7469 6f6e 2070 6970 656c  sification pipel
-00000460: 696e 6520 7472 6169 6e65 6420 666f 7220  ine trained for 
-00000470: 6120 6269 6e61 7279 2063 6c61 7373 6966  a binary classif
-00000480: 6963 6174 696f 6e20 7461 736b 0a64 6574  ication task.det
-00000490: 6563 7469 6f6e 5f72 6573 203d 2062 6961  ection_res = bia
-000004a0: 735f 6465 7465 6374 6f72 2e70 726f 6365  s_detector.proce
-000004b0: 7373 280a 2020 2020 7465 7874 733d 7465  ss(.    texts=te
-000004c0: 7874 732c 0a20 2020 2070 7265 6469 6374  xts,.    predict
-000004d0: 5f66 756e 633d 636c 662e 7072 6564 6963  _func=clf.predic
-000004e0: 745f 7072 6f62 610a 290a 0a23 2073 6565  t_proba.)..# see
-000004f0: 2061 2073 756d 6d61 7279 206f 6620 7468   a summary of th
-00000500: 6520 6465 7465 6374 696f 6e0a 6465 7465  e detection.dete
-00000510: 6374 696f 6e5f 7265 732e 7265 706f 7274  ction_res.report
-00000520: 2829 0a0a 2320 7669 7375 616c 697a 6520  ()..# visualize 
-00000530: 7468 6520 636f 756e 7465 7266 6163 7475  the counterfactu
-00000540: 616c 2073 636f 7265 730a 6465 7465 6374  al scores.detect
-00000550: 696f 6e5f 7265 732e 7669 7375 616c 697a  ion_res.visualiz
-00000560: 655f 636f 756e 7465 7266 6163 7475 616c  e_counterfactual
-00000570: 5f73 636f 7265 7328 636f 6e63 6570 743d  _scores(concept=
-00000580: 2272 656c 6967 696f 6e22 2c20 746f 705f  "religion", top_
-00000590: 6e3d 3130 290a 6060 600a 0a45 7861 6d70  n=10).```..Examp
-000005a0: 6c65 206f 7574 7075 743a 0a21 5b5d 2872  le output:.![](r
-000005b0: 6573 6f75 7263 6573 2f68 6174 6573 7065  esources/hatespe
-000005c0: 6563 685f 646c 5f73 636f 7265 735f 7265  ech_dl_scores_re
-000005d0: 6c69 6769 6f6e 2e70 6e67 290a 0a0a 596f  ligion.png)...Yo
-000005e0: 7520 6361 6e20 7365 6520 6120 6d6f 7265  u can see a more
-000005f0: 2064 6574 6169 6c65 6420 6578 616d 706c   detailed exampl
-00000600: 6520 696e 2074 6865 205b 7475 746f 7269  e in the [tutori
-00000610: 616c 5d28 7475 746f 7269 616c 732f 7475  al](tutorials/tu
-00000620: 746f 7269 616c 2d74 6f78 6963 2d63 6f6d  torial-toxic-com
-00000630: 6d65 6e74 732f 292e 0a0a 0a23 2320 4465  ments/)....## De
-00000640: 7665 6c6f 706d 656e 7420 7365 7475 700a  velopment setup.
-00000650: 0a2d 2046 6972 7374 2079 6f75 206e 6565  .- First you nee
-00000660: 6420 746f 2069 6e73 7461 6c6c 2070 6f65  d to install poe
-00000670: 7472 7920 746f 206d 616e 6167 6520 796f  try to manage yo
-00000680: 7572 2070 7974 686f 6e20 656e 7669 726f  ur python enviro
-00000690: 6e6d 656e 743a 2068 7474 7073 3a2f 2f70  nment: https://p
-000006a0: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-000006b0: 2f64 6f63 732f 2369 6e73 7461 6c6c 6174  /docs/#installat
-000006c0: 696f 6e0a 2d20 5275 6e20 606d 616b 6520  ion.- Run `make 
-000006d0: 696e 7374 616c 6c60 2074 6f20 696e 7374  install` to inst
-000006e0: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
-000006f0: 6369 6573 2061 6e64 2067 6574 2074 6865  cies and get the
-00000700: 2073 7061 6379 2062 6173 656d 6f64 656c   spacy basemodel
-00000710: 732e 0a2d 204e 6f77 2079 6f75 2063 616e  s..- Now you can
-00000720: 2075 7365 2060 6269 6173 6c79 7a65 6020   use `biaslyze` 
-00000730: 696e 2079 6f75 7220 6a75 7079 7465 7220  in your jupyter 
-00000740: 6e6f 7465 626f 6f6b 732e 0a0a 0a23 2323  notebooks....###
-00000750: 2041 6464 696e 6720 636f 6e63 6570 7473   Adding concepts
-00000760: 2061 6e64 206b 6579 776f 7264 730a 0a59   and keywords..Y
-00000770: 6f75 2063 616e 2061 6464 2063 6f6e 6365  ou can add conce
-00000780: 7074 7320 616e 6420 6e65 7720 6b65 7977  pts and new keyw
-00000790: 6f72 6473 2066 6f72 2065 7869 7374 696e  ords for existin
-000007a0: 6720 636f 6e63 6570 7473 2062 7920 6564  g concepts by ed
-000007b0: 6974 696e 6720 5b63 6f6e 6365 7074 732e  iting [concepts.
-000007c0: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-000007d0: 7562 2e63 6f6d 2f62 6961 736c 797a 652d  ub.com/biaslyze-
-000007e0: 6465 762f 6269 6173 6c79 7a65 2f62 6c6f  dev/biaslyze/blo
-000007f0: 622f 6b65 7977 6f72 642d 6261 7365 642d  b/keyword-based-
-00000800: 7461 7267 6574 6564 2d6c 696d 652f 6269  targeted-lime/bi
-00000810: 6173 6c79 7a65 2f63 6f6e 6365 7074 732e  aslyze/concepts.
-00000820: 7079 292e 0a0a 2323 2050 7265 7669 6577  py)...## Preview
-00000830: 2f62 7569 6c64 2074 6865 2064 6f63 756d  /build the docum
-00000840: 656e 7461 7469 6f6e 2077 6974 6820 6d6b  entation with mk
-00000850: 646f 6373 0a0a 546f 2070 7265 7669 6577  docs..To preview
-00000860: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00000870: 6f6e 2072 756e 2060 6d61 6b65 2064 6f63  on run `make doc
-00000880: 2d70 7265 7669 6577 602e 2054 6869 7320  -preview`. This 
-00000890: 7769 6c6c 206c 6175 6e63 6820 6120 7072  will launch a pr
-000008a0: 6576 6965 7720 6f66 2074 6865 2064 6f63  eview of the doc
-000008b0: 756d 656e 7461 7469 6f6e 206f 6e20 6068  umentation on `h
-000008c0: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-000008d0: 3830 3030 2f60 2e0a 546f 2062 7569 6c64  8000/`..To build
-000008e0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-000008f0: 6f6e 2068 746d 6c20 7275 6e20 606d 616b  on html run `mak
-00000900: 6520 646f 6360 2e0a 0a0a 2323 2052 756e  e doc`....## Run
-00000910: 2074 6865 2061 7574 6f6d 6174 6564 2074   the automated t
-00000920: 6573 7473 0a0a 606d 616b 6520 7465 7374  ests..`make test
-00000930: 600a 0a0a 2323 2053 7479 6c65 2067 7569  `...## Style gui
-00000940: 6465 0a0a 5765 2061 7265 2075 7369 6e67  de..We are using
-00000950: 2069 736f 7274 2061 6e64 2062 6c61 636b   isort and black
-00000960: 3a20 606d 616b 6520 7374 796c 6560 0a46  : `make style`.F
-00000970: 6f72 206c 696e 7469 6e67 2077 6520 6172  or linting we ar
-00000980: 6520 7275 6e6e 696e 6720 7275 6666 3a20  e running ruff: 
-00000990: 606d 616b 6520 6c69 6e74 600a 0a23 2320  `make lint`..## 
-000009a0: 436f 6e74 7269 6275 7469 6e67 0a0a 466f  Contributing..Fo
-000009b0: 6c6c 6f77 2074 6865 2067 6f6f 676c 6520  llow the google 
-000009c0: 7374 796c 6520 6775 6964 6520 666f 7220  style guide for 
-000009d0: 7079 7468 6f6e 3a20 6874 7470 733a 2f2f  python: https://
-000009e0: 676f 6f67 6c65 2e67 6974 6875 622e 696f  google.github.io
-000009f0: 2f73 7479 6c65 6775 6964 652f 7079 6775  /styleguide/pygu
-00000a00: 6964 652e 6874 6d6c 0a0a 5468 6973 2070  ide.html..This p
-00000a10: 726f 6a65 6374 2075 7365 7320 626c 6163  roject uses blac
-00000a20: 6b2c 2069 736f 7274 2061 6e64 2072 7566  k, isort and ruf
-00000a30: 6620 746f 2065 6e66 6f72 6365 2073 7479  f to enforce sty
-00000a40: 6c65 2e20 4170 706c 7920 6974 2062 7920  le. Apply it by 
-00000a50: 7275 6e6e 696e 6720 606d 616b 6520 7374  running `make st
-00000a60: 796c 6560 2061 6e64 2060 6d61 6b65 206c  yle` and `make l
-00000a70: 696e 7460 2e0a 0a23 2320 4163 6b6e 6f77  int`...## Acknow
-00000a80: 6c65 6467 656d 656e 7473 0a0a 2a20 4675  ledgements..* Fu
-00000a90: 6e64 6564 2066 726f 6d20 4d61 7263 6820  nded from March 
-00000aa0: 3230 3233 2075 6e74 696c 2041 7567 7573  2023 until Augus
-00000ab0: 7420 3230 3233 2062 7920 215b 6c6f 676f  t 2023 by ![logo
-00000ac0: 7320 6f66 2074 6865 2022 4275 6e64 6573  s of the "Bundes
-00000ad0: 6d69 6e69 7374 6572 6975 6d20 66c3 bc72  ministerium f..r
-00000ae0: 2042 696c 6475 6e67 2075 6e64 2046 6f72   Bildung und For
-00000af0: 7363 6875 6e67 222c 2050 726f 646f 7479  schung", Prodoty
-00000b00: 7065 2046 756e 6420 616e 6420 4f4b 464e  pe Fund and OKFN
-00000b10: 2d44 6575 7473 6368 6c61 6e64 5d28 7265  -Deutschland](re
-00000b20: 736f 7572 6365 732f 7066 5f66 756e 6469  sources/pf_fundi
-00000b30: 6e67 5f6c 6f67 6f73 2e73 7667 290a       ng_logos.svg).
+00000000: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000010: 7222 3e0a 2020 3c68 313e 6269 6173 6c79  r">.  <h1>biasly
+00000020: 7a65 202d 2054 6865 204e 4c50 2042 6961  ze - The NLP Bia
+00000030: 7320 4964 656e 7469 6669 6361 7469 6f6e  s Identification
+00000040: 2054 6f6f 6c6b 6974 3c2f 6831 3e0a 3c2f   Toolkit</h1>.</
+00000050: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
+00000060: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000070: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000080: 7562 2e63 6f6d 2f62 6961 736c 797a 652d  ub.com/biaslyze-
+00000090: 6465 762f 6269 6173 6c79 7a65 2f62 6c6f  dev/biaslyze/blo
+000000a0: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+000000b0: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+000000c0: 743d 226c 6963 656e 6365 2220 7372 633d  t="licence" src=
+000000d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000000e0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000000f0: 6963 656e 7365 2f62 6961 736c 797a 652d  icense/biaslyze-
+00000100: 6465 762f 6269 6173 6c79 7a65 223e 0a20  dev/biaslyze">. 
+00000110: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+00000120: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000130: 692e 6f72 672f 7072 6f6a 6563 742f 6269  i.org/project/bi
+00000140: 6173 6c79 7a65 2f22 3e0a 2020 2020 2020  aslyze/">.      
+00000150: 2020 3c69 6d67 2061 6c74 3d22 7079 7069    <img alt="pypi
+00000160: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000170: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000180: 7069 2f76 2f62 6961 736c 797a 6522 3e0a  pi/v/biaslyze">.
+00000190: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+000001a0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000001b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f62  pi.org/project/b
+000001c0: 6961 736c 797a 652f 223e 0a20 2020 2020  iaslyze/">.     
+000001d0: 2020 203c 696d 6720 616c 743d 2270 7970     <img alt="pyp
+000001e0: 6922 2073 7263 3d22 6874 7470 733a 2f2f  i" src="https://
+000001f0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000200: 7970 692f 7079 7665 7273 696f 6e73 2f62  ypi/pyversions/b
+00000210: 6961 736c 797a 6522 3e0a 2020 2020 3c2f  iaslyze">.    </
+00000220: 613e 0a3c 2f70 3e0a 0a0a 4269 6173 2069  a>.</p>...Bias i
+00000230: 7320 6f66 7465 6e20 7375 6274 6c65 2061  s often subtle a
+00000240: 6e64 2064 6966 6669 6375 6c74 2074 6f20  nd difficult to 
+00000250: 6465 7465 6374 2069 6e20 4e4c 5020 6d6f  detect in NLP mo
+00000260: 6465 6c73 2c20 6173 2074 6865 2070 726f  dels, as the pro
+00000270: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
+00000280: 7320 6172 6520 6c65 7373 206f 6276 696f  s are less obvio
+00000290: 7573 2061 6e64 2063 616e 2074 616b 6520  us and can take 
+000002a0: 6d61 6e79 2066 6f72 6d73 2069 6e20 6c61  many forms in la
+000002b0: 6e67 7561 6765 2028 652e 672e 2070 726f  nguage (e.g. pro
+000002c0: 7869 6573 2c20 646f 7562 6c65 206d 6561  xies, double mea
+000002d0: 6e69 6e67 732c 2061 6d62 6967 7569 7469  nings, ambiguiti
+000002e0: 6573 2065 7463 2e29 2e20 5468 6572 6566  es etc.). Theref
+000002f0: 6f72 652c 2074 6563 686e 6963 616c 2062  ore, technical b
+00000300: 6961 7320 7465 7374 696e 6720 6973 2061  ias testing is a
+00000310: 206b 6579 2073 7465 7020 696e 2061 766f   key step in avo
+00000320: 6964 696e 6720 616c 676f 7269 7468 6d69  iding algorithmi
+00000330: 6361 6c6c 7920 6d65 6469 6174 6564 2064  cally mediated d
+00000340: 6973 6372 696d 696e 6174 696f 6e2e 2048  iscrimination. H
+00000350: 6f77 6576 6572 2c20 6974 2069 7320 6375  owever, it is cu
+00000360: 7272 656e 746c 7920 636f 6e64 7563 7465  rrently conducte
+00000370: 6420 746f 6f20 7261 7265 6c79 2064 7565  d too rarely due
+00000380: 2074 6f20 7468 6520 6566 666f 7274 2069   to the effort i
+00000390: 6e76 6f6c 7665 642c 206d 6973 7369 6e67  nvolved, missing
+000003a0: 2072 6573 6f75 7263 6573 206f 7220 6c61   resources or la
+000003b0: 636b 206f 6620 6177 6172 656e 6573 7320  ck of awareness 
+000003c0: 666f 7220 7468 6520 7072 6f62 6c65 6d2e  for the problem.
+000003d0: 0a0a 4269 6173 6c79 7a65 2068 656c 7073  ..Biaslyze helps
+000003e0: 2074 6f20 6765 7420 7374 6172 7465 6420   to get started 
+000003f0: 7769 7468 2074 6865 2061 6e61 6c79 7369  with the analysi
+00000400: 7320 6f66 2062 6961 7320 7769 7468 696e  s of bias within
+00000410: 204e 4c50 206d 6f64 656c 7320 616e 6420   NLP models and 
+00000420: 6f66 6665 7273 2061 2063 6f6e 6372 6574  offers a concret
+00000430: 6520 656e 7472 7920 706f 696e 7420 666f  e entry point fo
+00000440: 7220 6675 7274 6865 7220 696d 7061 6374  r further impact
+00000450: 2061 7373 6573 736d 656e 7473 2061 6e64   assessments and
+00000460: 206d 6974 6967 6174 696f 6e20 6d65 6173   mitigation meas
+00000470: 7572 6573 2e20 4573 7065 6369 616c 6c79  ures. Especially
+00000480: 2066 6f72 2074 6561 6d73 2077 6974 6820   for teams with 
+00000490: 6c69 6d69 7465 6420 7265 736f 7572 6365  limited resource
+000004a0: 732c 206f 7572 2074 6f6f 6c62 6f78 206f  s, our toolbox o
+000004b0: 6666 6572 7320 6120 6c6f 772d 6566 666f  ffers a low-effo
+000004c0: 7274 2061 7070 726f 6163 6820 746f 2062  rt approach to b
+000004d0: 6961 7320 7465 7374 696e 6720 696e 204e  ias testing in N
+000004e0: 4c50 2075 7365 2063 6173 6573 2e0a 0a23  LP use cases...#
+000004f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
+00000500: 496e 7374 616c 6c61 7469 6f6e 2063 616e  Installation can
+00000510: 2062 6520 646f 6e65 2075 7369 6e67 2070   be done using p
+00000520: 7970 693a 0a60 6060 6261 7368 0a70 6970  ypi:.```bash.pip
+00000530: 2069 6e73 7461 6c6c 2062 6961 736c 797a   install biaslyz
+00000540: 650a 6060 600a 0a54 6865 6e20 796f 7520  e.```..Then you 
+00000550: 6e65 6564 2074 6f20 646f 776e 6c6f 6164  need to download
+00000560: 2074 6865 2072 6571 7569 7265 6420 7370   the required sp
+00000570: 6163 7920 6d6f 6465 6c73 3a0a 6060 6062  acy models:.```b
+00000580: 6173 680a 7079 7468 6f6e 202d 6d20 7370  ash.python -m sp
+00000590: 6163 7920 646f 776e 6c6f 6164 2065 6e5f  acy download en_
+000005a0: 636f 7265 5f77 6562 5f73 6d0a 6060 600a  core_web_sm.```.
+000005b0: 0a23 2320 5175 6963 6b73 7461 7274 0a0a  .## Quickstart..
+000005c0: 6060 6070 7974 686f 6e0a 6672 6f6d 2062  ```python.from b
+000005d0: 6961 736c 797a 652e 6269 6173 5f64 6574  iaslyze.bias_det
+000005e0: 6563 746f 7273 2069 6d70 6f72 7420 436f  ectors import Co
+000005f0: 756e 7465 7266 6163 7475 616c 4269 6173  unterfactualBias
+00000600: 4465 7465 6374 6f72 0a0a 6269 6173 5f64  Detector..bias_d
+00000610: 6574 6563 746f 7220 3d20 436f 756e 7465  etector = Counte
+00000620: 7266 6163 7475 616c 4269 6173 4465 7465  rfactualBiasDete
+00000630: 6374 6f72 2829 0a0a 2320 6465 7465 6374  ctor()..# detect
+00000640: 2062 6961 7320 696e 2074 6865 206d 6f64   bias in the mod
+00000650: 656c 2062 6173 6564 206f 6e20 7468 6520  el based on the 
+00000660: 6769 7665 6e20 7465 7874 730a 2320 6865  given texts.# he
+00000670: 7265 2c20 636c 6620 6973 2061 2073 6369  re, clf is a sci
+00000680: 6b69 742d 6c65 6172 6e20 7465 7874 2063  kit-learn text c
+00000690: 6c61 7373 6966 6963 6174 696f 6e20 7069  lassification pi
+000006a0: 7065 6c69 6e65 2074 7261 696e 6564 2066  peline trained f
+000006b0: 6f72 2061 2062 696e 6172 7920 636c 6173  or a binary clas
+000006c0: 7369 6669 6361 7469 6f6e 2074 6173 6b0a  sification task.
+000006d0: 6465 7465 6374 696f 6e5f 7265 7320 3d20  detection_res = 
+000006e0: 6269 6173 5f64 6574 6563 746f 722e 7072  bias_detector.pr
+000006f0: 6f63 6573 7328 0a20 2020 2074 6578 7473  ocess(.    texts
+00000700: 3d74 6578 7473 2c0a 2020 2020 7072 6564  =texts,.    pred
+00000710: 6963 745f 6675 6e63 3d63 6c66 2e70 7265  ict_func=clf.pre
+00000720: 6469 6374 5f70 726f 6261 0a29 0a0a 2320  dict_proba.)..# 
+00000730: 7365 6520 6120 7375 6d6d 6172 7920 6f66  see a summary of
+00000740: 2074 6865 2064 6574 6563 7469 6f6e 0a64   the detection.d
+00000750: 6574 6563 7469 6f6e 5f72 6573 2e72 6570  etection_res.rep
+00000760: 6f72 7428 290a 0a23 2076 6973 7561 6c69  ort()..# visuali
+00000770: 7a65 2074 6865 2063 6f75 6e74 6572 6661  ze the counterfa
+00000780: 6374 7561 6c20 7363 6f72 6573 0a64 6574  ctual scores.det
+00000790: 6563 7469 6f6e 5f72 6573 2e76 6973 7561  ection_res.visua
+000007a0: 6c69 7a65 5f63 6f75 6e74 6572 6661 6374  lize_counterfact
+000007b0: 7561 6c5f 7363 6f72 6573 2863 6f6e 6365  ual_scores(conce
+000007c0: 7074 3d22 7265 6c69 6769 6f6e 222c 2074  pt="religion", t
+000007d0: 6f70 5f6e 3d31 3029 0a60 6060 0a0a 4578  op_n=10).```..Ex
+000007e0: 616d 706c 6520 6f75 7470 7574 3a0a 215b  ample output:.![
+000007f0: 5d28 7265 736f 7572 6365 732f 6861 7465  ](resources/hate
+00000800: 7370 6565 6368 5f64 6c5f 7363 6f72 6573  speech_dl_scores
+00000810: 5f72 656c 6967 696f 6e2e 706e 6729 0a0a  _religion.png)..
+00000820: 0a59 6f75 2063 616e 2073 6565 2061 206d  .You can see a m
+00000830: 6f72 6520 6465 7461 696c 6564 2065 7861  ore detailed exa
+00000840: 6d70 6c65 2069 6e20 7468 6520 5b74 7574  mple in the [tut
+00000850: 6f72 6961 6c5d 2874 7574 6f72 6961 6c73  orial](tutorials
+00000860: 2f74 7574 6f72 6961 6c2d 746f 7869 632d  /tutorial-toxic-
+00000870: 636f 6d6d 656e 7473 2f29 2e0a 0a0a 2323  comments/)....##
+00000880: 2044 6576 656c 6f70 6d65 6e74 2073 6574   Development set
+00000890: 7570 0a0a 2d20 4669 7273 7420 796f 7520  up..- First you 
+000008a0: 6e65 6564 2074 6f20 696e 7374 616c 6c20  need to install 
+000008b0: 706f 6574 7279 2074 6f20 6d61 6e61 6765  poetry to manage
+000008c0: 2079 6f75 7220 7079 7468 6f6e 2065 6e76   your python env
+000008d0: 6972 6f6e 6d65 6e74 3a20 6874 7470 733a  ironment: https:
+000008e0: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
+000008f0: 6f72 672f 646f 6373 2f23 696e 7374 616c  org/docs/#instal
+00000900: 6c61 7469 6f6e 0a2d 2052 756e 2060 6d61  lation.- Run `ma
+00000910: 6b65 2069 6e73 7461 6c6c 6020 746f 2069  ke install` to i
+00000920: 6e73 7461 6c6c 2074 6865 2064 6570 656e  nstall the depen
+00000930: 6465 6e63 6965 7320 616e 6420 6765 7420  dencies and get 
+00000940: 7468 6520 7370 6163 7920 6261 7365 6d6f  the spacy basemo
+00000950: 6465 6c73 2e0a 2d20 4e6f 7720 796f 7520  dels..- Now you 
+00000960: 6361 6e20 7573 6520 6062 6961 736c 797a  can use `biaslyz
+00000970: 6560 2069 6e20 796f 7572 206a 7570 7974  e` in your jupyt
+00000980: 6572 206e 6f74 6562 6f6f 6b73 2e0a 0a0a  er notebooks....
+00000990: 2323 2320 4164 6469 6e67 2063 6f6e 6365  ### Adding conce
+000009a0: 7074 7320 616e 6420 6b65 7977 6f72 6473  pts and keywords
+000009b0: 0a0a 596f 7520 6361 6e20 6164 6420 636f  ..You can add co
+000009c0: 6e63 6570 7473 2061 6e64 206e 6577 206b  ncepts and new k
+000009d0: 6579 776f 7264 7320 666f 7220 6578 6973  eywords for exis
+000009e0: 7469 6e67 2063 6f6e 6365 7074 7320 6279  ting concepts by
+000009f0: 2065 6469 7469 6e67 205b 636f 6e63 6570   editing [concep
+00000a00: 7473 2e70 795d 2868 7474 7073 3a2f 2f67  ts.py](https://g
+00000a10: 6974 6875 622e 636f 6d2f 6269 6173 6c79  ithub.com/biasly
+00000a20: 7a65 2d64 6576 2f62 6961 736c 797a 652f  ze-dev/biaslyze/
+00000a30: 626c 6f62 2f6b 6579 776f 7264 2d62 6173  blob/keyword-bas
+00000a40: 6564 2d74 6172 6765 7465 642d 6c69 6d65  ed-targeted-lime
+00000a50: 2f62 6961 736c 797a 652f 636f 6e63 6570  /biaslyze/concep
+00000a60: 7473 2e70 7929 2e0a 0a23 2320 5072 6576  ts.py)...## Prev
+00000a70: 6965 772f 6275 696c 6420 7468 6520 646f  iew/build the do
+00000a80: 6375 6d65 6e74 6174 696f 6e20 7769 7468  cumentation with
+00000a90: 206d 6b64 6f63 730a 0a54 6f20 7072 6576   mkdocs..To prev
+00000aa0: 6965 7720 7468 6520 646f 6375 6d65 6e74  iew the document
+00000ab0: 6174 696f 6e20 7275 6e20 606d 616b 6520  ation run `make 
+00000ac0: 646f 632d 7072 6576 6965 7760 2e20 5468  doc-preview`. Th
+00000ad0: 6973 2077 696c 6c20 6c61 756e 6368 2061  is will launch a
+00000ae0: 2070 7265 7669 6577 206f 6620 7468 6520   preview of the 
+00000af0: 646f 6375 6d65 6e74 6174 696f 6e20 6f6e  documentation on
+00000b00: 2060 6874 7470 3a2f 2f31 3237 2e30 2e30   `http://127.0.0
+00000b10: 2e31 3a38 3030 302f 602e 0a54 6f20 6275  .1:8000/`..To bu
+00000b20: 696c 6420 7468 6520 646f 6375 6d65 6e74  ild the document
+00000b30: 6174 696f 6e20 6874 6d6c 2072 756e 2060  ation html run `
+00000b40: 6d61 6b65 2064 6f63 602e 0a0a 0a23 2320  make doc`....## 
+00000b50: 5275 6e20 7468 6520 6175 746f 6d61 7465  Run the automate
+00000b60: 6420 7465 7374 730a 0a60 6d61 6b65 2074  d tests..`make t
+00000b70: 6573 7460 0a0a 0a23 2320 5374 796c 6520  est`...## Style 
+00000b80: 6775 6964 650a 0a57 6520 6172 6520 7573  guide..We are us
+00000b90: 696e 6720 6973 6f72 7420 616e 6420 626c  ing isort and bl
+00000ba0: 6163 6b3a 2060 6d61 6b65 2073 7479 6c65  ack: `make style
+00000bb0: 600a 466f 7220 6c69 6e74 696e 6720 7765  `.For linting we
+00000bc0: 2061 7265 2072 756e 6e69 6e67 2072 7566   are running ruf
+00000bd0: 663a 2060 6d61 6b65 206c 696e 7460 0a0a  f: `make lint`..
+00000be0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000bf0: 0a46 6f6c 6c6f 7720 7468 6520 676f 6f67  .Follow the goog
+00000c00: 6c65 2073 7479 6c65 2067 7569 6465 2066  le style guide f
+00000c10: 6f72 2070 7974 686f 6e3a 2068 7474 7073  or python: https
+00000c20: 3a2f 2f67 6f6f 676c 652e 6769 7468 7562  ://google.github
+00000c30: 2e69 6f2f 7374 796c 6567 7569 6465 2f70  .io/styleguide/p
+00000c40: 7967 7569 6465 2e68 746d 6c0a 0a54 6869  yguide.html..Thi
+00000c50: 7320 7072 6f6a 6563 7420 7573 6573 2062  s project uses b
+00000c60: 6c61 636b 2c20 6973 6f72 7420 616e 6420  lack, isort and 
+00000c70: 7275 6666 2074 6f20 656e 666f 7263 6520  ruff to enforce 
+00000c80: 7374 796c 652e 2041 7070 6c79 2069 7420  style. Apply it 
+00000c90: 6279 2072 756e 6e69 6e67 2060 6d61 6b65  by running `make
+00000ca0: 2073 7479 6c65 6020 616e 6420 606d 616b   style` and `mak
+00000cb0: 6520 6c69 6e74 602e 0a0a 2323 2041 636b  e lint`...## Ack
+00000cc0: 6e6f 776c 6564 6765 6d65 6e74 730a 0a2a  nowledgements..*
+00000cd0: 2046 756e 6465 6420 6672 6f6d 204d 6172   Funded from Mar
+00000ce0: 6368 2032 3032 3320 756e 7469 6c20 4175  ch 2023 until Au
+00000cf0: 6775 7374 2032 3032 3320 6279 2021 5b6c  gust 2023 by ![l
+00000d00: 6f67 6f73 206f 6620 7468 6520 2242 756e  ogos of the "Bun
+00000d10: 6465 736d 696e 6973 7465 7269 756d 2066  desministerium f
+00000d20: c3bc 7220 4269 6c64 756e 6720 756e 6420  ..r Bildung und 
+00000d30: 466f 7273 6368 756e 6722 2c20 5072 6f64  Forschung", Prod
+00000d40: 6f74 7970 6520 4675 6e64 2061 6e64 204f  otype Fund and O
+00000d50: 4b46 4e2d 4465 7574 7363 686c 616e 645d  KFN-Deutschland]
+00000d60: 2872 6573 6f75 7263 6573 2f70 665f 6675  (resources/pf_fu
+00000d70: 6e64 696e 675f 6c6f 676f 732e 7376 6729  nding_logos.svg)
+00000d80: 0a                                       .
```

### Comparing `biaslyze-0.0.5a0/biaslyze/_plotting.py` & `biaslyze-0.0.6a0/biaslyze/_plotting.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/biaslyze/bias_detectors/counterfactual_biasdetector.py` & `biaslyze-0.0.6a0/biaslyze/bias_detectors/counterfactual_biasdetector.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import random
 from typing import Callable, List, Optional
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 from tqdm import tqdm
-import spacy
 
+from biaslyze.concept_class import Concept, load_concepts
 from biaslyze.concept_detectors import KeywordConceptDetector
-from biaslyze.concepts import CONCEPTS
 from biaslyze.results.counterfactual_detection_results import (
     CounterfactualConceptResult,
     CounterfactualDetectionResult,
     CounterfactualSample,
 )
+from biaslyze.text_representation import TextRepresentation, process_texts_with_spacy
 
 
 class CounterfactualBiasDetector:
     """Detect hints of bias by calculating counterfactual token scores for protected concepts.
 
     The counterfactual score is defined as the difference between the predicted
     probability score for the original text and the predicted probability score for the counterfactual text.
@@ -65,30 +65,35 @@
     ):
         self.use_tokenizer = use_tokenizer
         self.concept_detector = concept_detector
 
         # overwrite use_tokenizer
         self.concept_detector.use_tokenizer = self.use_tokenizer
 
+        # load the concepts
+        self.concepts = load_concepts()
+
     def process(
         self,
         texts: List[str],
         predict_func: Callable[[List[str]], List[float]],
         labels: Optional[List[str]] = None,
         concepts_to_consider: Optional[List[str]] = [],
         max_counterfactual_samples: Optional[int] = None,
+        max_counterfactual_samples_per_text: Optional[int] = None,
     ) -> List:
         """Detect potential bias in the model based on the given texts.
 
         Args:
             texts: texts to probe the model for bias.
             predict_func: Function to run the texts through the model and get probabilities as outputs.
             labels: Optional. Used to add labels to the counterfactual results.
             concepts_to_consider: If given, only the given concepts are considered.
-            max_counterfactual_samples: If given, only the given number of counterfactual samples are used for each concept.
+            max_counterfactual_samples: Optional. The maximum number of counterfactual samples to return. Defaults to None, which returns all possible counterfactual samples.
+            max_counterfactual_samples_per_text: Optional. The maximum number of counterfactual samples to return per text. Defaults to None, which returns all possible counterfactual samples.
 
         Returns:
             A [CounterfactualDetectionResult](/biaslyze/results/counterfactual_detection_results/) object.
 
         Raises:
             ValueError: If texts or predict_func is not given.
         """
@@ -101,149 +106,158 @@
         if max_counterfactual_samples:
             if (not isinstance(max_counterfactual_samples, int)) or (
                 max_counterfactual_samples < 1
             ):
                 raise ValueError(
                     "max_counterfactual_samples must be a positive integer."
                 )
+        if max_counterfactual_samples_per_text:
+            if (not isinstance(max_counterfactual_samples_per_text, int)) or (
+                max_counterfactual_samples_per_text < 1
+            ):
+                raise ValueError(
+                    "max_counterfactual_samples_per_text must be a positive integer."
+                )
 
         # find bias relevant texts
         detected_texts = self.concept_detector.detect(texts)
 
+        # limit the number of counterfactual samples per text if max_counterfactual_samples is given
+        if max_counterfactual_samples:
+            max_counterfactual_samples_per_text = max_counterfactual_samples // len(
+                detected_texts
+            )
+
         results = []
-        for concept, concept_keywords in CONCEPTS.items():
-            if concepts_to_consider and concept not in concepts_to_consider:
+        for concept in self.concepts:
+            if concepts_to_consider and concept.name not in concepts_to_consider:
                 continue
-            logger.info(f"Processing concept {concept}...")
+            logger.info(f"Processing concept {concept.name}...")
             score_dict = dict()
 
             counterfactual_samples = _extract_counterfactual_concept_samples(
                 texts=detected_texts,
                 concept=concept,
-                tokenizer=self.concept_detector._tokenizer,
                 labels=labels,
+                n_texts=max_counterfactual_samples_per_text,
             )
             if not counterfactual_samples:
                 logger.warning(f"No samples containing {concept} found. Skipping.")
                 continue
 
             # calculate counterfactual scores for each keyword
-            for keyword in tqdm(concept_keywords):
+            for keyword in tqdm(concept.keywords):
                 # get the counterfactual scores
                 counterfactual_scores = _calculate_counterfactual_scores(
-                    bias_keyword=keyword.get("keyword"),
+                    bias_keyword=keyword.text,
                     predict_func=predict_func,
                     samples=counterfactual_samples,
-                    max_counterfactual_samples=max_counterfactual_samples,
                 )
                 # add to score dict
-                score_dict[keyword.get("keyword")] = counterfactual_scores
+                score_dict[keyword.text] = counterfactual_scores
                 # add scores to samples
                 original_keyword_samples = [
                     sample
                     for sample in counterfactual_samples
-                    if (sample.keyword == keyword.get("keyword"))
+                    if (sample.keyword == keyword.text)
                     and (sample.keyword == sample.orig_keyword)
                 ]
                 for score, sample in zip(
                     counterfactual_scores, original_keyword_samples
                 ):
                     sample.score = score
 
-            score_df = pd.DataFrame(score_dict)
+            # create a dataframe from the score dict, allow for different lengths of scores
+            score_df = pd.DataFrame(
+                dict([(k, pd.Series(v)) for k, v in score_dict.items()])
+            )
+            # score_df = pd.DataFrame(score_dict)
             # remove words with exactly the same score
             omitted_keywords = score_df.loc[
                 :, score_df.T.duplicated().T
             ].columns.tolist()
             score_df = score_df.loc[:, ~score_df.T.duplicated().T]
+
             results.append(
                 CounterfactualConceptResult(
-                    concept=concept,
+                    concept=concept.name,
                     scores=score_df,
                     omitted_keywords=omitted_keywords,
                     counterfactual_samples=counterfactual_samples,
                 )
             )
             logger.info("DONE")
 
         return CounterfactualDetectionResult(concept_results=results)
 
 
 def _extract_counterfactual_concept_samples(
-    concept: str,
+    concept: Concept,
     texts: List[str],
-    tokenizer: spacy.tokenizer.Tokenizer,
     labels: Optional[List[str]] = None,
+    n_texts: Optional[int] = None,
 ) -> List[CounterfactualSample]:
     """Extract counterfactual samples for a given concept from a list of texts.
 
     A counterfactual sample is defined as a text where a keyword of the
     given concept is replaced by another keyword of the same concept.
 
     Args:
         concept: The concept to extract counterfactual samples for.
         texts: The texts to extract counterfactual samples from.
         tokenizer: The tokenizer to use for tokenization.
         labels: Optional. Used to add labels to the counterfactual results.
+        n_texts: Optional. The number of counterfactual texts to return. Defaults to None, which returns all possible counterfactual texts.
+
+    Returns:
+        A list of CounterfactualSample objects.
     """
     counterfactual_samples = []
     original_texts = []
-    text_representations = tokenizer.pipe(texts)
-    concept_keywords = set([keyword.get("keyword") for keyword in CONCEPTS[concept]])
+    text_representations: List[TextRepresentation] = process_texts_with_spacy(texts)
     for idx, (text, text_representation) in tqdm(
         enumerate(zip(texts, text_representations)), total=len(texts)
     ):
-        present_keywords = list(
-            keyword
-            for keyword in concept_keywords
-            if keyword in (token.text.lower() for token in text_representation)
-        )
+        present_keywords = concept.get_present_keywords(text_representation)
         if present_keywords:
             original_texts.append(text)
             for orig_keyword in present_keywords:
-                for concept_keyword in concept_keywords:
-                    resampled_text = "".join(
-                        [
-                            concept_keyword + token.whitespace_
-                            if token.text.lower() == orig_keyword.lower()
-                            else token.text + token.whitespace_
-                            for token in text_representation
-                        ]
-                    )
+                counterfactual_texts = concept.get_counterfactual_texts(
+                    orig_keyword, text_representation, n_texts=n_texts
+                )
+                for counterfactual_text, counterfactual_keyword in counterfactual_texts:
                     counterfactual_samples.append(
                         CounterfactualSample(
-                            text=resampled_text,
-                            orig_keyword=orig_keyword,
-                            keyword=concept_keyword,
-                            concept=concept,
+                            text=counterfactual_text,
+                            orig_keyword=orig_keyword.text,
+                            keyword=counterfactual_keyword.text,
+                            concept=concept.name,
                             tokenized=text_representation,
                             label=labels[idx] if labels else None,
                             source_text=text,
                         )
                     )
     logger.info(
-        f"Extracted {len(counterfactual_samples)} counterfactual sample texts for concept {concept} from {len(original_texts)} original texts."
+        f"Extracted {len(counterfactual_samples)} counterfactual sample texts for concept {concept.name} from {len(original_texts)} original texts."
     )
     return counterfactual_samples
 
 
 def _calculate_counterfactual_scores(
     bias_keyword: str,
     predict_func: Callable,
     samples: List[CounterfactualSample],
-    max_counterfactual_samples: int = None,
     positive_classes: Optional[List] = None,
 ) -> np.ndarray:
     """Calculate the counterfactual score for a bias keyword given samples.
 
     Args:
         bias_keyword: The keyword to calculate the counterfactual score for.
         predict_func: Function to run the texts through the model and get probabilities as outputs.
         samples: A list of CounterfactualSample objects.
-        max_counterfactual_samples: The maximum number of counterfactual samples to use.
         positive_classes: A list of classes that are considered positive.
 
     TODO: If `positive_classes` is given, all other classes are considered non-positive and positive and negative outcomes are compared.
     TODO: introduce neutral classes.
 
     Returns:
         A numpy array of differences between the original predictions and the predictions for the counterfactual samples.
@@ -258,21 +272,22 @@
         sample.source_text for sample in samples if (sample.keyword == bias_keyword)
     ]
     counterfactual_texts = [
         sample.text for sample in samples if (sample.keyword == bias_keyword)
     ]
 
     # if max_counterfactual_samples is given, only use a random sample of the counterfactual texts
-    if max_counterfactual_samples:
-        original_texts, counterfactual_texts = zip(
-            *random.sample(
-                list(zip(original_texts, counterfactual_texts)),
-                max_counterfactual_samples,
-            )
-        )
+    # if max_counterfactual_samples:
+    #     original_texts, counterfactual_texts = zip(
+    #         *random.sample(
+    #             list(zip(original_texts, counterfactual_texts)),
+    #             max_counterfactual_samples,
+    #         )
+    #     )
+
     # predict the scores for the original texts and the counterfactual texts
     original_scores = predict_func(original_texts)
     predicted_scores = predict_func(counterfactual_texts)
 
     # check if the model is a binary classifier
     if (not positive_classes) and (len(original_scores[0]) != 2):
         raise NotImplementedError(
```

### Comparing `biaslyze-0.0.5a0/biaslyze/bias_detectors/lime_biasdetector.py` & `biaslyze-0.0.6a0/biaslyze/bias_detectors/lime_biasdetector.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/biaslyze/concept_detectors.py` & `biaslyze-0.0.6a0/biaslyze/concept_detectors.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/biaslyze/concepts.py` & `biaslyze-0.0.6a0/biaslyze/concepts.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/biaslyze/results/counterfactual_detection_results.py` & `biaslyze-0.0.6a0/biaslyze/results/counterfactual_detection_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                 all_samples.append(sample)
                 # calculate the median score and change the sign
                 # this means that the score represents the median change in prediction if the keyword is replaced
                 # with a concept keyword.
                 all_scores.append(-1 * np.median(score.tolist()))
         if all_samples == []:
             raise ValueError(
-                f"No results found. Please make sure that the concepts are in the results."
+                "No results found. Please make sure that the concepts are in the results."
             )
 
         dashboard = _plot_histogram_dashboard(
             texts=[sample.text for sample in all_samples],
             concepts=[sample.concept for sample in all_samples],
             scores=all_scores,
             keywords=[sample.keyword for sample in all_samples],
```

### Comparing `biaslyze-0.0.5a0/biaslyze/results/lime_detection_results.py` & `biaslyze-0.0.6a0/biaslyze/results/lime_detection_results.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.5a0/pyproject.toml` & `biaslyze-0.0.6a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biaslyze"
-version = "0.0.5-alpha"
+version = "0.0.6-alpha"
 description = "The NLP Bias Identification Toolkit"
 authors = [
     "Tobias Sterbak & Stina Lohmüller <hello@biaslyze.org>",
 ]
 maintainers = [
     "Tobias Sterbak <hello@tobiassterbak.com>",
     "Stina Lohmüller <slohmueller@posteo.de>",
@@ -46,14 +46,15 @@
 nvidia-cusparse-cu11 = "^11.7.5.86"
 nvidia-nccl-cu11 = "^2.16.5"
 nvidia-nvtx-cu11 = "^11.8.86"
 triton = "^2.0.0.post1"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.1.1"
+material-plausible-plugin = "^0.2.0"
 mkgendocs = "^0.9.2"
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.254"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `biaslyze-0.0.5a0/setup.py` & `biaslyze-0.0.6a0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,222 +61,259 @@
 000003c0: 3d32 2e30 2e30 2e70 6f73 7431 2c3c 332e  =2.0.0.post1,<3.
 000003d0: 302e 3027 2c0a 2027 756d 6170 2d6c 6561  0.0',. 'umap-lea
 000003e0: 726e 3e3d 302e 352e 332c 3c30 2e36 2e30  rn>=0.5.3,<0.6.0
 000003f0: 275d 0a0a 7365 7475 705f 6b77 6172 6773  ']..setup_kwargs
 00000400: 203d 207b 0a20 2020 2027 6e61 6d65 273a   = {.    'name':
 00000410: 2027 6269 6173 6c79 7a65 272c 0a20 2020   'biaslyze',.   
 00000420: 2027 7665 7273 696f 6e27 3a20 2730 2e30   'version': '0.0
-00000430: 2e35 6130 272c 0a20 2020 2027 6465 7363  .5a0',.    'desc
+00000430: 2e36 6130 272c 0a20 2020 2027 6465 7363  .6a0',.    'desc
 00000440: 7269 7074 696f 6e27 3a20 2754 6865 204e  ription': 'The N
 00000450: 4c50 2042 6961 7320 4964 656e 7469 6669  LP Bias Identifi
 00000460: 6361 7469 6f6e 2054 6f6f 6c6b 6974 272c  cation Toolkit',
 00000470: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-00000480: 6970 7469 6f6e 273a 2027 2320 6269 6173  iption': '# bias
-00000490: 6c79 7a65 202d 2054 6865 204e 4c50 2042  lyze - The NLP B
-000004a0: 6961 7320 4964 656e 7469 6669 6361 7469  ias Identificati
-000004b0: 6f6e 2054 6f6f 6c6b 6974 5c6e 5c6e 4269  on Toolkit\n\nBi
-000004c0: 6173 2069 7320 6f66 7465 6e20 7375 6274  as is often subt
-000004d0: 6c65 2061 6e64 2064 6966 6669 6375 6c74  le and difficult
-000004e0: 2074 6f20 6465 7465 6374 2069 6e20 4e4c   to detect in NL
-000004f0: 5020 6d6f 6465 6c73 2c20 6173 2074 6865  P models, as the
-00000500: 2070 726f 7465 6374 6564 2061 7474 7269   protected attri
-00000510: 6275 7465 7320 6172 6520 6c65 7373 206f  butes are less o
-00000520: 6276 696f 7573 2061 6e64 2063 616e 2074  bvious and can t
-00000530: 616b 6520 6d61 6e79 2066 6f72 6d73 2069  ake many forms i
-00000540: 6e20 6c61 6e67 7561 6765 2028 652e 672e  n language (e.g.
-00000550: 2070 726f 7869 6573 2c20 646f 7562 6c65   proxies, double
-00000560: 206d 6561 6e69 6e67 732c 2061 6d62 6967   meanings, ambig
-00000570: 7569 7469 6573 2065 7463 2e29 2e20 5468  uities etc.). Th
-00000580: 6572 6566 6f72 652c 2074 6563 686e 6963  erefore, technic
-00000590: 616c 2062 6961 7320 7465 7374 696e 6720  al bias testing 
-000005a0: 6973 2061 206b 6579 2073 7465 7020 696e  is a key step in
-000005b0: 2061 766f 6964 696e 6720 616c 676f 7269   avoiding algori
-000005c0: 7468 6d69 6361 6c6c 7920 6d65 6469 6174  thmically mediat
-000005d0: 6564 2064 6973 6372 696d 696e 6174 696f  ed discriminatio
-000005e0: 6e2e 2048 6f77 6576 6572 2c20 6974 2069  n. However, it i
-000005f0: 7320 6375 7272 656e 746c 7920 636f 6e64  s currently cond
-00000600: 7563 7465 6420 746f 6f20 7261 7265 6c79  ucted too rarely
-00000610: 2064 7565 2074 6f20 7468 6520 6566 666f   due to the effo
-00000620: 7274 2069 6e76 6f6c 7665 642c 206d 6973  rt involved, mis
-00000630: 7369 6e67 2072 6573 6f75 7263 6573 206f  sing resources o
-00000640: 7220 6c61 636b 206f 6620 6177 6172 656e  r lack of awaren
-00000650: 6573 7320 666f 7220 7468 6520 7072 6f62  ess for the prob
-00000660: 6c65 6d2e 5c6e 5c6e 4269 6173 6c79 7a65  lem.\n\nBiaslyze
-00000670: 2068 656c 7073 2074 6f20 6765 7420 7374   helps to get st
-00000680: 6172 7465 6420 7769 7468 2074 6865 2061  arted with the a
-00000690: 6e61 6c79 7369 7320 6f66 2062 6961 7320  nalysis of bias 
-000006a0: 7769 7468 696e 204e 4c50 206d 6f64 656c  within NLP model
-000006b0: 7320 616e 6420 6f66 6665 7273 2061 2063  s and offers a c
-000006c0: 6f6e 6372 6574 6520 656e 7472 7920 706f  oncrete entry po
-000006d0: 696e 7420 666f 7220 6675 7274 6865 7220  int for further 
-000006e0: 696d 7061 6374 2061 7373 6573 736d 656e  impact assessmen
-000006f0: 7473 2061 6e64 206d 6974 6967 6174 696f  ts and mitigatio
-00000700: 6e20 6d65 6173 7572 6573 2e20 4573 7065  n measures. Espe
-00000710: 6369 616c 6c79 2066 6f72 2079 6f75 6e67  cially for young
-00000720: 2064 6576 656c 6f70 6572 732c 2073 7475   developers, stu
-00000730: 6465 6e74 7320 616e 6420 7465 616d 7320  dents and teams 
-00000740: 7769 7468 206c 696d 6974 6564 2072 6573  with limited res
-00000750: 6f75 7263 6573 2c20 6f75 7220 746f 6f6c  ources, our tool
-00000760: 626f 7820 6f66 6665 7273 2061 206c 6f77  box offers a low
-00000770: 2d65 6666 6f72 7420 6170 7072 6f61 6368  -effort approach
-00000780: 2074 6f20 6269 6173 2074 6573 7469 6e67   to bias testing
-00000790: 2069 6e20 4e4c 5020 7573 6520 6361 7365   in NLP use case
-000007a0: 732e 5c6e 5c6e 2323 2049 6e73 7461 6c6c  s.\n\n## Install
-000007b0: 6174 696f 6e5c 6e5c 6e49 6e73 7461 6c6c  ation\n\nInstall
-000007c0: 6174 696f 6e20 6361 6e20 6265 2064 6f6e  ation can be don
-000007d0: 6520 7573 696e 6720 7079 7069 3a5c 6e60  e using pypi:\n`
-000007e0: 6060 6261 7368 5c6e 7069 7020 696e 7374  ``bash\npip inst
-000007f0: 616c 6c20 6269 6173 6c79 7a65 5c6e 6060  all biaslyze\n``
-00000800: 605c 6e5c 6e23 2320 5175 6963 6b73 7461  `\n\n## Quicksta
-00000810: 7274 5c6e 5c6e 6060 6070 7974 686f 6e5c  rt\n\n```python\
-00000820: 6e66 726f 6d20 6269 6173 6c79 7a65 2e62  nfrom biaslyze.b
-00000830: 6961 735f 6465 7465 6374 6f72 7320 696d  ias_detectors im
-00000840: 706f 7274 2043 6f75 6e74 6572 6661 6374  port Counterfact
-00000850: 7561 6c42 6961 7344 6574 6563 746f 725c  ualBiasDetector\
-00000860: 6e5c 6e62 6961 735f 6465 7465 6374 6f72  n\nbias_detector
-00000870: 203d 2043 6f75 6e74 6572 6661 6374 7561   = Counterfactua
-00000880: 6c42 6961 7344 6574 6563 746f 7228 295c  lBiasDetector()\
-00000890: 6e5c 6e23 2064 6574 6563 7420 6269 6173  n\n# detect bias
-000008a0: 2069 6e20 7468 6520 6d6f 6465 6c20 6261   in the model ba
-000008b0: 7365 6420 6f6e 2074 6865 2067 6976 656e  sed on the given
-000008c0: 2074 6578 7473 5c6e 2320 6865 7265 2c20   texts\n# here, 
-000008d0: 636c 6620 6973 2061 2073 6369 6b69 742d  clf is a scikit-
-000008e0: 6c65 6172 6e20 7465 7874 2063 6c61 7373  learn text class
-000008f0: 6966 6963 6174 696f 6e20 7069 7065 6c69  ification pipeli
-00000900: 6e65 2074 7261 696e 6564 2066 6f72 2061  ne trained for a
-00000910: 2062 696e 6172 7920 636c 6173 7369 6669   binary classifi
-00000920: 6361 7469 6f6e 2074 6173 6b5c 6e64 6574  cation task\ndet
-00000930: 6563 7469 6f6e 5f72 6573 203d 2062 6961  ection_res = bia
-00000940: 735f 6465 7465 6374 6f72 2e70 726f 6365  s_detector.proce
-00000950: 7373 285c 6e20 2020 2074 6578 7473 3d74  ss(\n    texts=t
-00000960: 6578 7473 2c5c 6e20 2020 2070 7265 6469  exts,\n    predi
-00000970: 6374 5f66 756e 633d 636c 662e 7072 6564  ct_func=clf.pred
-00000980: 6963 745f 7072 6f62 615c 6e29 5c6e 5c6e  ict_proba\n)\n\n
-00000990: 2320 7365 6520 6120 7375 6d6d 6172 7920  # see a summary 
-000009a0: 6f66 2074 6865 2064 6574 6563 7469 6f6e  of the detection
-000009b0: 5c6e 6465 7465 6374 696f 6e5f 7265 732e  \ndetection_res.
-000009c0: 7265 706f 7274 2829 5c6e 5c6e 2320 7669  report()\n\n# vi
-000009d0: 7375 616c 697a 6520 7468 6520 636f 756e  sualize the coun
-000009e0: 7465 7266 6163 7475 616c 2073 636f 7265  terfactual score
-000009f0: 735c 6e64 6574 6563 7469 6f6e 5f72 6573  s\ndetection_res
-00000a00: 2e76 6973 7561 6c69 7a65 5f63 6f75 6e74  .visualize_count
-00000a10: 6572 6661 6374 7561 6c5f 7363 6f72 6573  erfactual_scores
-00000a20: 2863 6f6e 6365 7074 3d22 7265 6c69 6769  (concept="religi
-00000a30: 6f6e 222c 2074 6f70 5f6e 3d31 3029 5c6e  on", top_n=10)\n
-00000a40: 6060 605c 6e5c 6e45 7861 6d70 6c65 206f  ```\n\nExample o
-00000a50: 7574 7075 743a 5c6e 215b 5d28 7265 736f  utput:\n![](reso
-00000a60: 7572 6365 732f 6861 7465 7370 6565 6368  urces/hatespeech
-00000a70: 5f64 6c5f 7363 6f72 6573 5f72 656c 6967  _dl_scores_relig
-00000a80: 696f 6e2e 706e 6729 5c6e 5c6e 5c6e 596f  ion.png)\n\n\nYo
-00000a90: 7520 6361 6e20 7365 6520 6120 6d6f 7265  u can see a more
-00000aa0: 2064 6574 6169 6c65 6420 6578 616d 706c   detailed exampl
-00000ab0: 6520 696e 2074 6865 205b 7475 746f 7269  e in the [tutori
-00000ac0: 616c 5d28 7475 746f 7269 616c 732f 7475  al](tutorials/tu
-00000ad0: 746f 7269 616c 2d74 6f78 6963 2d63 6f6d  torial-toxic-com
-00000ae0: 6d65 6e74 732f 292e 5c6e 5c6e 5c6e 2323  ments/).\n\n\n##
-00000af0: 2044 6576 656c 6f70 6d65 6e74 2073 6574   Development set
-00000b00: 7570 5c6e 5c6e 2d20 4669 7273 7420 796f  up\n\n- First yo
-00000b10: 7520 6e65 6564 2074 6f20 696e 7374 616c  u need to instal
-00000b20: 6c20 706f 6574 7279 2074 6f20 6d61 6e61  l poetry to mana
-00000b30: 6765 2079 6f75 7220 7079 7468 6f6e 2065  ge your python e
-00000b40: 6e76 6972 6f6e 6d65 6e74 3a20 6874 7470  nvironment: http
-00000b50: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
-00000b60: 792e 6f72 672f 646f 6373 2f23 696e 7374  y.org/docs/#inst
-00000b70: 616c 6c61 7469 6f6e 5c6e 2d20 5275 6e20  allation\n- Run 
-00000b80: 606d 616b 6520 696e 7374 616c 6c60 2074  `make install` t
-00000b90: 6f20 696e 7374 616c 6c20 7468 6520 6465  o install the de
-00000ba0: 7065 6e64 656e 6369 6573 2061 6e64 2067  pendencies and g
-00000bb0: 6574 2074 6865 2073 7061 6379 2062 6173  et the spacy bas
-00000bc0: 656d 6f64 656c 732e 5c6e 2d20 4e6f 7720  emodels.\n- Now 
-00000bd0: 796f 7520 6361 6e20 7573 6520 6062 6961  you can use `bia
-00000be0: 736c 797a 6560 2069 6e20 796f 7572 206a  slyze` in your j
-00000bf0: 7570 7974 6572 206e 6f74 6562 6f6f 6b73  upyter notebooks
-00000c00: 2e5c 6e5c 6e5c 6e23 2323 2041 6464 696e  .\n\n\n### Addin
-00000c10: 6720 636f 6e63 6570 7473 2061 6e64 206b  g concepts and k
-00000c20: 6579 776f 7264 735c 6e5c 6e59 6f75 2063  eywords\n\nYou c
-00000c30: 616e 2061 6464 2063 6f6e 6365 7074 7320  an add concepts 
-00000c40: 616e 6420 6e65 7720 6b65 7977 6f72 6473  and new keywords
-00000c50: 2066 6f72 2065 7869 7374 696e 6720 636f   for existing co
-00000c60: 6e63 6570 7473 2062 7920 6564 6974 696e  ncepts by editin
-00000c70: 6720 5b63 6f6e 6365 7074 732e 7079 5d28  g [concepts.py](
-00000c80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c90: 6f6d 2f62 6961 736c 797a 652d 6465 762f  om/biaslyze-dev/
-00000ca0: 6269 6173 6c79 7a65 2f62 6c6f 622f 6b65  biaslyze/blob/ke
-00000cb0: 7977 6f72 642d 6261 7365 642d 7461 7267  yword-based-targ
-00000cc0: 6574 6564 2d6c 696d 652f 6269 6173 6c79  eted-lime/biasly
-00000cd0: 7a65 2f63 6f6e 6365 7074 732e 7079 292e  ze/concepts.py).
-00000ce0: 5c6e 5c6e 2323 2050 7265 7669 6577 2f62  \n\n## Preview/b
-00000cf0: 7569 6c64 2074 6865 2064 6f63 756d 656e  uild the documen
-00000d00: 7461 7469 6f6e 2077 6974 6820 6d6b 646f  tation with mkdo
-00000d10: 6373 5c6e 5c6e 546f 2070 7265 7669 6577  cs\n\nTo preview
-00000d20: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00000d30: 6f6e 2072 756e 2060 6d61 6b65 2064 6f63  on run `make doc
-00000d40: 2d70 7265 7669 6577 602e 2054 6869 7320  -preview`. This 
-00000d50: 7769 6c6c 206c 6175 6e63 6820 6120 7072  will launch a pr
-00000d60: 6576 6965 7720 6f66 2074 6865 2064 6f63  eview of the doc
-00000d70: 756d 656e 7461 7469 6f6e 206f 6e20 6068  umentation on `h
-00000d80: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00000d90: 3830 3030 2f60 2e5c 6e54 6f20 6275 696c  8000/`.\nTo buil
-00000da0: 6420 7468 6520 646f 6375 6d65 6e74 6174  d the documentat
-00000db0: 696f 6e20 6874 6d6c 2072 756e 2060 6d61  ion html run `ma
-00000dc0: 6b65 2064 6f63 602e 5c6e 5c6e 5c6e 2323  ke doc`.\n\n\n##
-00000dd0: 2052 756e 2074 6865 2061 7574 6f6d 6174   Run the automat
-00000de0: 6564 2074 6573 7473 5c6e 5c6e 606d 616b  ed tests\n\n`mak
-00000df0: 6520 7465 7374 605c 6e5c 6e5c 6e23 2320  e test`\n\n\n## 
-00000e00: 5374 796c 6520 6775 6964 655c 6e5c 6e57  Style guide\n\nW
-00000e10: 6520 6172 6520 7573 696e 6720 6973 6f72  e are using isor
-00000e20: 7420 616e 6420 626c 6163 6b3a 2060 6d61  t and black: `ma
-00000e30: 6b65 2073 7479 6c65 605c 6e46 6f72 206c  ke style`\nFor l
-00000e40: 696e 7469 6e67 2077 6520 6172 6520 7275  inting we are ru
-00000e50: 6e6e 696e 6720 7275 6666 3a20 606d 616b  nning ruff: `mak
-00000e60: 6520 6c69 6e74 605c 6e5c 6e23 2320 436f  e lint`\n\n## Co
-00000e70: 6e74 7269 6275 7469 6e67 5c6e 5c6e 466f  ntributing\n\nFo
-00000e80: 6c6c 6f77 2074 6865 2067 6f6f 676c 6520  llow the google 
-00000e90: 7374 796c 6520 6775 6964 6520 666f 7220  style guide for 
-00000ea0: 7079 7468 6f6e 3a20 6874 7470 733a 2f2f  python: https://
-00000eb0: 676f 6f67 6c65 2e67 6974 6875 622e 696f  google.github.io
-00000ec0: 2f73 7479 6c65 6775 6964 652f 7079 6775  /styleguide/pygu
-00000ed0: 6964 652e 6874 6d6c 5c6e 5c6e 5468 6973  ide.html\n\nThis
-00000ee0: 2070 726f 6a65 6374 2075 7365 7320 626c   project uses bl
-00000ef0: 6163 6b2c 2069 736f 7274 2061 6e64 2072  ack, isort and r
-00000f00: 7566 6620 746f 2065 6e66 6f72 6365 2073  uff to enforce s
-00000f10: 7479 6c65 2e20 4170 706c 7920 6974 2062  tyle. Apply it b
-00000f20: 7920 7275 6e6e 696e 6720 606d 616b 6520  y running `make 
-00000f30: 7374 796c 6560 2061 6e64 2060 6d61 6b65  style` and `make
-00000f40: 206c 696e 7460 2e5c 6e5c 6e23 2320 4163   lint`.\n\n## Ac
-00000f50: 6b6e 6f77 6c65 6467 656d 656e 7473 5c6e  knowledgements\n
-00000f60: 5c6e 2a20 4675 6e64 6564 2066 726f 6d20  \n* Funded from 
-00000f70: 4d61 7263 6820 3230 3233 2075 6e74 696c  March 2023 until
-00000f80: 2041 7567 7573 7420 3230 3233 2062 7920   August 2023 by 
-00000f90: 215b 6c6f 676f 7320 6f66 2074 6865 2022  ![logos of the "
-00000fa0: 4275 6e64 6573 6d69 6e69 7374 6572 6975  Bundesministeriu
-00000fb0: 6d20 66c3 bc72 2042 696c 6475 6e67 2075  m f..r Bildung u
-00000fc0: 6e64 2046 6f72 7363 6875 6e67 222c 2050  nd Forschung", P
-00000fd0: 726f 646f 7479 7065 2046 756e 6420 616e  rodotype Fund an
-00000fe0: 6420 4f4b 464e 2d44 6575 7473 6368 6c61  d OKFN-Deutschla
-00000ff0: 6e64 5d28 7265 736f 7572 6365 732f 7066  nd](resources/pf
-00001000: 5f66 756e 6469 6e67 5f6c 6f67 6f73 2e73  _funding_logos.s
-00001010: 7667 295c 6e27 2c0a 2020 2020 2761 7574  vg)\n',.    'aut
-00001020: 686f 7227 3a20 2754 6f62 6961 7320 5374  hor': 'Tobias St
-00001030: 6572 6261 6b20 2620 5374 696e 6120 4c6f  erbak & Stina Lo
-00001040: 686d c3bc 6c6c 6572 272c 0a20 2020 2027  hm..ller',.    '
-00001050: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
-00001060: 6865 6c6c 6f40 6269 6173 6c79 7a65 2e6f  hello@biaslyze.o
-00001070: 7267 272c 0a20 2020 2027 6d61 696e 7461  rg',.    'mainta
-00001080: 696e 6572 273a 2027 546f 6269 6173 2053  iner': 'Tobias S
-00001090: 7465 7262 616b 272c 0a20 2020 2027 6d61  terbak',.    'ma
-000010a0: 696e 7461 696e 6572 5f65 6d61 696c 273a  intainer_email':
-000010b0: 2027 6865 6c6c 6f40 746f 6269 6173 7374   'hello@tobiasst
-000010c0: 6572 6261 6b2e 636f 6d27 2c0a 2020 2020  erbak.com',.    
-000010d0: 2775 726c 273a 2027 6874 7470 733a 2f2f  'url': 'https://
-000010e0: 6269 6173 6c79 7a65 2e6f 7267 272c 0a20  biaslyze.org',. 
-000010f0: 2020 2027 7061 636b 6167 6573 273a 2070     'packages': p
-00001100: 6163 6b61 6765 732c 0a20 2020 2027 7061  ackages,.    'pa
-00001110: 636b 6167 655f 6461 7461 273a 2070 6163  ckage_data': pac
-00001120: 6b61 6765 5f64 6174 612c 0a20 2020 2027  kage_data,.    '
-00001130: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00001140: 273a 2069 6e73 7461 6c6c 5f72 6571 7569  ': install_requi
-00001150: 7265 732c 0a20 2020 2027 7079 7468 6f6e  res,.    'python
-00001160: 5f72 6571 7569 7265 7327 3a20 273e 3d33  _requires': '>=3
-00001170: 2e31 302c 3c33 2e31 3127 2c0a 7d0a 0a0a  .10,<3.11',.}...
-00001180: 7365 7475 7028 2a2a 7365 7475 705f 6b77  setup(**setup_kw
-00001190: 6172 6773 290a                           args).
+00000480: 6970 7469 6f6e 273a 2027 5c6e 3c70 2061  iption': '\n<p a
+00000490: 6c69 676e 3d22 6365 6e74 6572 223e 5c6e  lign="center">\n
+000004a0: 2020 3c68 313e 6269 6173 6c79 7a65 202d    <h1>biaslyze -
+000004b0: 2054 6865 204e 4c50 2042 6961 7320 4964   The NLP Bias Id
+000004c0: 656e 7469 6669 6361 7469 6f6e 2054 6f6f  entification Too
+000004d0: 6c6b 6974 3c2f 6831 3e5c 6e3c 2f70 3e5c  lkit</h1>\n</p>\
+000004e0: 6e5c 6e3c 7020 616c 6967 6e3d 2263 656e  n\n<p align="cen
+000004f0: 7465 7222 3e5c 6e20 2020 203c 6120 6872  ter">\n    <a hr
+00000500: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000510: 7562 2e63 6f6d 2f62 6961 736c 797a 652d  ub.com/biaslyze-
+00000520: 6465 762f 6269 6173 6c79 7a65 2f62 6c6f  dev/biaslyze/blo
+00000530: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+00000540: 5c6e 2020 2020 2020 2020 3c69 6d67 2061  \n        <img a
+00000550: 6c74 3d22 6c69 6365 6e63 6522 2073 7263  lt="licence" src
+00000560: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000570: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000580: 6c69 6365 6e73 652f 6269 6173 6c79 7a65  license/biaslyze
+00000590: 2d64 6576 2f62 6961 736c 797a 6522 3e5c  -dev/biaslyze">\
+000005a0: 6e20 2020 203c 2f61 3e5c 6e20 2020 203c  n    </a>\n    <
+000005b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000005c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000005d0: 2f62 6961 736c 797a 652f 223e 5c6e 2020  /biaslyze/">\n  
+000005e0: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
+000005f0: 7079 7069 2220 7372 633d 2268 7474 7073  pypi" src="https
+00000600: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000610: 6f2f 7079 7069 2f76 2f62 6961 736c 797a  o/pypi/v/biaslyz
+00000620: 6522 3e5c 6e20 2020 203c 2f61 3e5c 6e20  e">\n    </a>\n 
+00000630: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000640: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000650: 6a65 6374 2f62 6961 736c 797a 652f 223e  ject/biaslyze/">
+00000660: 5c6e 2020 2020 2020 2020 3c69 6d67 2061  \n        <img a
+00000670: 6c74 3d22 7079 7069 2220 7372 633d 2268  lt="pypi" src="h
+00000680: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000690: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+000006a0: 7369 6f6e 732f 6269 6173 6c79 7a65 223e  sions/biaslyze">
+000006b0: 5c6e 2020 2020 3c2f 613e 5c6e 3c2f 703e  \n    </a>\n</p>
+000006c0: 5c6e 5c6e 5c6e 4269 6173 2069 7320 6f66  \n\n\nBias is of
+000006d0: 7465 6e20 7375 6274 6c65 2061 6e64 2064  ten subtle and d
+000006e0: 6966 6669 6375 6c74 2074 6f20 6465 7465  ifficult to dete
+000006f0: 6374 2069 6e20 4e4c 5020 6d6f 6465 6c73  ct in NLP models
+00000700: 2c20 6173 2074 6865 2070 726f 7465 6374  , as the protect
+00000710: 6564 2061 7474 7269 6275 7465 7320 6172  ed attributes ar
+00000720: 6520 6c65 7373 206f 6276 696f 7573 2061  e less obvious a
+00000730: 6e64 2063 616e 2074 616b 6520 6d61 6e79  nd can take many
+00000740: 2066 6f72 6d73 2069 6e20 6c61 6e67 7561   forms in langua
+00000750: 6765 2028 652e 672e 2070 726f 7869 6573  ge (e.g. proxies
+00000760: 2c20 646f 7562 6c65 206d 6561 6e69 6e67  , double meaning
+00000770: 732c 2061 6d62 6967 7569 7469 6573 2065  s, ambiguities e
+00000780: 7463 2e29 2e20 5468 6572 6566 6f72 652c  tc.). Therefore,
+00000790: 2074 6563 686e 6963 616c 2062 6961 7320   technical bias 
+000007a0: 7465 7374 696e 6720 6973 2061 206b 6579  testing is a key
+000007b0: 2073 7465 7020 696e 2061 766f 6964 696e   step in avoidin
+000007c0: 6720 616c 676f 7269 7468 6d69 6361 6c6c  g algorithmicall
+000007d0: 7920 6d65 6469 6174 6564 2064 6973 6372  y mediated discr
+000007e0: 696d 696e 6174 696f 6e2e 2048 6f77 6576  imination. Howev
+000007f0: 6572 2c20 6974 2069 7320 6375 7272 656e  er, it is curren
+00000800: 746c 7920 636f 6e64 7563 7465 6420 746f  tly conducted to
+00000810: 6f20 7261 7265 6c79 2064 7565 2074 6f20  o rarely due to 
+00000820: 7468 6520 6566 666f 7274 2069 6e76 6f6c  the effort invol
+00000830: 7665 642c 206d 6973 7369 6e67 2072 6573  ved, missing res
+00000840: 6f75 7263 6573 206f 7220 6c61 636b 206f  ources or lack o
+00000850: 6620 6177 6172 656e 6573 7320 666f 7220  f awareness for 
+00000860: 7468 6520 7072 6f62 6c65 6d2e 5c6e 5c6e  the problem.\n\n
+00000870: 4269 6173 6c79 7a65 2068 656c 7073 2074  Biaslyze helps t
+00000880: 6f20 6765 7420 7374 6172 7465 6420 7769  o get started wi
+00000890: 7468 2074 6865 2061 6e61 6c79 7369 7320  th the analysis 
+000008a0: 6f66 2062 6961 7320 7769 7468 696e 204e  of bias within N
+000008b0: 4c50 206d 6f64 656c 7320 616e 6420 6f66  LP models and of
+000008c0: 6665 7273 2061 2063 6f6e 6372 6574 6520  fers a concrete 
+000008d0: 656e 7472 7920 706f 696e 7420 666f 7220  entry point for 
+000008e0: 6675 7274 6865 7220 696d 7061 6374 2061  further impact a
+000008f0: 7373 6573 736d 656e 7473 2061 6e64 206d  ssessments and m
+00000900: 6974 6967 6174 696f 6e20 6d65 6173 7572  itigation measur
+00000910: 6573 2e20 4573 7065 6369 616c 6c79 2066  es. Especially f
+00000920: 6f72 2074 6561 6d73 2077 6974 6820 6c69  or teams with li
+00000930: 6d69 7465 6420 7265 736f 7572 6365 732c  mited resources,
+00000940: 206f 7572 2074 6f6f 6c62 6f78 206f 6666   our toolbox off
+00000950: 6572 7320 6120 6c6f 772d 6566 666f 7274  ers a low-effort
+00000960: 2061 7070 726f 6163 6820 746f 2062 6961   approach to bia
+00000970: 7320 7465 7374 696e 6720 696e 204e 4c50  s testing in NLP
+00000980: 2075 7365 2063 6173 6573 2e5c 6e5c 6e23   use cases.\n\n#
+00000990: 2320 496e 7374 616c 6c61 7469 6f6e 5c6e  # Installation\n
+000009a0: 5c6e 496e 7374 616c 6c61 7469 6f6e 2063  \nInstallation c
+000009b0: 616e 2062 6520 646f 6e65 2075 7369 6e67  an be done using
+000009c0: 2070 7970 693a 5c6e 6060 6062 6173 685c   pypi:\n```bash\
+000009d0: 6e70 6970 2069 6e73 7461 6c6c 2062 6961  npip install bia
+000009e0: 736c 797a 655c 6e60 6060 5c6e 5c6e 5468  slyze\n```\n\nTh
+000009f0: 656e 2079 6f75 206e 6565 6420 746f 2064  en you need to d
+00000a00: 6f77 6e6c 6f61 6420 7468 6520 7265 7175  ownload the requ
+00000a10: 6972 6564 2073 7061 6379 206d 6f64 656c  ired spacy model
+00000a20: 733a 5c6e 6060 6062 6173 685c 6e70 7974  s:\n```bash\npyt
+00000a30: 686f 6e20 2d6d 2073 7061 6379 2064 6f77  hon -m spacy dow
+00000a40: 6e6c 6f61 6420 656e 5f63 6f72 655f 7765  nload en_core_we
+00000a50: 625f 736d 5c6e 6060 605c 6e5c 6e23 2320  b_sm\n```\n\n## 
+00000a60: 5175 6963 6b73 7461 7274 5c6e 5c6e 6060  Quickstart\n\n``
+00000a70: 6070 7974 686f 6e5c 6e66 726f 6d20 6269  `python\nfrom bi
+00000a80: 6173 6c79 7a65 2e62 6961 735f 6465 7465  aslyze.bias_dete
+00000a90: 6374 6f72 7320 696d 706f 7274 2043 6f75  ctors import Cou
+00000aa0: 6e74 6572 6661 6374 7561 6c42 6961 7344  nterfactualBiasD
+00000ab0: 6574 6563 746f 725c 6e5c 6e62 6961 735f  etector\n\nbias_
+00000ac0: 6465 7465 6374 6f72 203d 2043 6f75 6e74  detector = Count
+00000ad0: 6572 6661 6374 7561 6c42 6961 7344 6574  erfactualBiasDet
+00000ae0: 6563 746f 7228 295c 6e5c 6e23 2064 6574  ector()\n\n# det
+00000af0: 6563 7420 6269 6173 2069 6e20 7468 6520  ect bias in the 
+00000b00: 6d6f 6465 6c20 6261 7365 6420 6f6e 2074  model based on t
+00000b10: 6865 2067 6976 656e 2074 6578 7473 5c6e  he given texts\n
+00000b20: 2320 6865 7265 2c20 636c 6620 6973 2061  # here, clf is a
+00000b30: 2073 6369 6b69 742d 6c65 6172 6e20 7465   scikit-learn te
+00000b40: 7874 2063 6c61 7373 6966 6963 6174 696f  xt classificatio
+00000b50: 6e20 7069 7065 6c69 6e65 2074 7261 696e  n pipeline train
+00000b60: 6564 2066 6f72 2061 2062 696e 6172 7920  ed for a binary 
+00000b70: 636c 6173 7369 6669 6361 7469 6f6e 2074  classification t
+00000b80: 6173 6b5c 6e64 6574 6563 7469 6f6e 5f72  ask\ndetection_r
+00000b90: 6573 203d 2062 6961 735f 6465 7465 6374  es = bias_detect
+00000ba0: 6f72 2e70 726f 6365 7373 285c 6e20 2020  or.process(\n   
+00000bb0: 2074 6578 7473 3d74 6578 7473 2c5c 6e20   texts=texts,\n 
+00000bc0: 2020 2070 7265 6469 6374 5f66 756e 633d     predict_func=
+00000bd0: 636c 662e 7072 6564 6963 745f 7072 6f62  clf.predict_prob
+00000be0: 615c 6e29 5c6e 5c6e 2320 7365 6520 6120  a\n)\n\n# see a 
+00000bf0: 7375 6d6d 6172 7920 6f66 2074 6865 2064  summary of the d
+00000c00: 6574 6563 7469 6f6e 5c6e 6465 7465 6374  etection\ndetect
+00000c10: 696f 6e5f 7265 732e 7265 706f 7274 2829  ion_res.report()
+00000c20: 5c6e 5c6e 2320 7669 7375 616c 697a 6520  \n\n# visualize 
+00000c30: 7468 6520 636f 756e 7465 7266 6163 7475  the counterfactu
+00000c40: 616c 2073 636f 7265 735c 6e64 6574 6563  al scores\ndetec
+00000c50: 7469 6f6e 5f72 6573 2e76 6973 7561 6c69  tion_res.visuali
+00000c60: 7a65 5f63 6f75 6e74 6572 6661 6374 7561  ze_counterfactua
+00000c70: 6c5f 7363 6f72 6573 2863 6f6e 6365 7074  l_scores(concept
+00000c80: 3d22 7265 6c69 6769 6f6e 222c 2074 6f70  ="religion", top
+00000c90: 5f6e 3d31 3029 5c6e 6060 605c 6e5c 6e45  _n=10)\n```\n\nE
+00000ca0: 7861 6d70 6c65 206f 7574 7075 743a 5c6e  xample output:\n
+00000cb0: 215b 5d28 7265 736f 7572 6365 732f 6861  ![](resources/ha
+00000cc0: 7465 7370 6565 6368 5f64 6c5f 7363 6f72  tespeech_dl_scor
+00000cd0: 6573 5f72 656c 6967 696f 6e2e 706e 6729  es_religion.png)
+00000ce0: 5c6e 5c6e 5c6e 596f 7520 6361 6e20 7365  \n\n\nYou can se
+00000cf0: 6520 6120 6d6f 7265 2064 6574 6169 6c65  e a more detaile
+00000d00: 6420 6578 616d 706c 6520 696e 2074 6865  d example in the
+00000d10: 205b 7475 746f 7269 616c 5d28 7475 746f   [tutorial](tuto
+00000d20: 7269 616c 732f 7475 746f 7269 616c 2d74  rials/tutorial-t
+00000d30: 6f78 6963 2d63 6f6d 6d65 6e74 732f 292e  oxic-comments/).
+00000d40: 5c6e 5c6e 5c6e 2323 2044 6576 656c 6f70  \n\n\n## Develop
+00000d50: 6d65 6e74 2073 6574 7570 5c6e 5c6e 2d20  ment setup\n\n- 
+00000d60: 4669 7273 7420 796f 7520 6e65 6564 2074  First you need t
+00000d70: 6f20 696e 7374 616c 6c20 706f 6574 7279  o install poetry
+00000d80: 2074 6f20 6d61 6e61 6765 2079 6f75 7220   to manage your 
+00000d90: 7079 7468 6f6e 2065 6e76 6972 6f6e 6d65  python environme
+00000da0: 6e74 3a20 6874 7470 733a 2f2f 7079 7468  nt: https://pyth
+00000db0: 6f6e 2d70 6f65 7472 792e 6f72 672f 646f  on-poetry.org/do
+00000dc0: 6373 2f23 696e 7374 616c 6c61 7469 6f6e  cs/#installation
+00000dd0: 5c6e 2d20 5275 6e20 606d 616b 6520 696e  \n- Run `make in
+00000de0: 7374 616c 6c60 2074 6f20 696e 7374 616c  stall` to instal
+00000df0: 6c20 7468 6520 6465 7065 6e64 656e 6369  l the dependenci
+00000e00: 6573 2061 6e64 2067 6574 2074 6865 2073  es and get the s
+00000e10: 7061 6379 2062 6173 656d 6f64 656c 732e  pacy basemodels.
+00000e20: 5c6e 2d20 4e6f 7720 796f 7520 6361 6e20  \n- Now you can 
+00000e30: 7573 6520 6062 6961 736c 797a 6560 2069  use `biaslyze` i
+00000e40: 6e20 796f 7572 206a 7570 7974 6572 206e  n your jupyter n
+00000e50: 6f74 6562 6f6f 6b73 2e5c 6e5c 6e5c 6e23  otebooks.\n\n\n#
+00000e60: 2323 2041 6464 696e 6720 636f 6e63 6570  ## Adding concep
+00000e70: 7473 2061 6e64 206b 6579 776f 7264 735c  ts and keywords\
+00000e80: 6e5c 6e59 6f75 2063 616e 2061 6464 2063  n\nYou can add c
+00000e90: 6f6e 6365 7074 7320 616e 6420 6e65 7720  oncepts and new 
+00000ea0: 6b65 7977 6f72 6473 2066 6f72 2065 7869  keywords for exi
+00000eb0: 7374 696e 6720 636f 6e63 6570 7473 2062  sting concepts b
+00000ec0: 7920 6564 6974 696e 6720 5b63 6f6e 6365  y editing [conce
+00000ed0: 7074 732e 7079 5d28 6874 7470 733a 2f2f  pts.py](https://
+00000ee0: 6769 7468 7562 2e63 6f6d 2f62 6961 736c  github.com/biasl
+00000ef0: 797a 652d 6465 762f 6269 6173 6c79 7a65  yze-dev/biaslyze
+00000f00: 2f62 6c6f 622f 6b65 7977 6f72 642d 6261  /blob/keyword-ba
+00000f10: 7365 642d 7461 7267 6574 6564 2d6c 696d  sed-targeted-lim
+00000f20: 652f 6269 6173 6c79 7a65 2f63 6f6e 6365  e/biaslyze/conce
+00000f30: 7074 732e 7079 292e 5c6e 5c6e 2323 2050  pts.py).\n\n## P
+00000f40: 7265 7669 6577 2f62 7569 6c64 2074 6865  review/build the
+00000f50: 2064 6f63 756d 656e 7461 7469 6f6e 2077   documentation w
+00000f60: 6974 6820 6d6b 646f 6373 5c6e 5c6e 546f  ith mkdocs\n\nTo
+00000f70: 2070 7265 7669 6577 2074 6865 2064 6f63   preview the doc
+00000f80: 756d 656e 7461 7469 6f6e 2072 756e 2060  umentation run `
+00000f90: 6d61 6b65 2064 6f63 2d70 7265 7669 6577  make doc-preview
+00000fa0: 602e 2054 6869 7320 7769 6c6c 206c 6175  `. This will lau
+00000fb0: 6e63 6820 6120 7072 6576 6965 7720 6f66  nch a preview of
+00000fc0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00000fd0: 6f6e 206f 6e20 6068 7474 703a 2f2f 3132  on on `http://12
+00000fe0: 372e 302e 302e 313a 3830 3030 2f60 2e5c  7.0.0.1:8000/`.\
+00000ff0: 6e54 6f20 6275 696c 6420 7468 6520 646f  nTo build the do
+00001000: 6375 6d65 6e74 6174 696f 6e20 6874 6d6c  cumentation html
+00001010: 2072 756e 2060 6d61 6b65 2064 6f63 602e   run `make doc`.
+00001020: 5c6e 5c6e 5c6e 2323 2052 756e 2074 6865  \n\n\n## Run the
+00001030: 2061 7574 6f6d 6174 6564 2074 6573 7473   automated tests
+00001040: 5c6e 5c6e 606d 616b 6520 7465 7374 605c  \n\n`make test`\
+00001050: 6e5c 6e5c 6e23 2320 5374 796c 6520 6775  n\n\n## Style gu
+00001060: 6964 655c 6e5c 6e57 6520 6172 6520 7573  ide\n\nWe are us
+00001070: 696e 6720 6973 6f72 7420 616e 6420 626c  ing isort and bl
+00001080: 6163 6b3a 2060 6d61 6b65 2073 7479 6c65  ack: `make style
+00001090: 605c 6e46 6f72 206c 696e 7469 6e67 2077  `\nFor linting w
+000010a0: 6520 6172 6520 7275 6e6e 696e 6720 7275  e are running ru
+000010b0: 6666 3a20 606d 616b 6520 6c69 6e74 605c  ff: `make lint`\
+000010c0: 6e5c 6e23 2320 436f 6e74 7269 6275 7469  n\n## Contributi
+000010d0: 6e67 5c6e 5c6e 466f 6c6c 6f77 2074 6865  ng\n\nFollow the
+000010e0: 2067 6f6f 676c 6520 7374 796c 6520 6775   google style gu
+000010f0: 6964 6520 666f 7220 7079 7468 6f6e 3a20  ide for python: 
+00001100: 6874 7470 733a 2f2f 676f 6f67 6c65 2e67  https://google.g
+00001110: 6974 6875 622e 696f 2f73 7479 6c65 6775  ithub.io/stylegu
+00001120: 6964 652f 7079 6775 6964 652e 6874 6d6c  ide/pyguide.html
+00001130: 5c6e 5c6e 5468 6973 2070 726f 6a65 6374  \n\nThis project
+00001140: 2075 7365 7320 626c 6163 6b2c 2069 736f   uses black, iso
+00001150: 7274 2061 6e64 2072 7566 6620 746f 2065  rt and ruff to e
+00001160: 6e66 6f72 6365 2073 7479 6c65 2e20 4170  nforce style. Ap
+00001170: 706c 7920 6974 2062 7920 7275 6e6e 696e  ply it by runnin
+00001180: 6720 606d 616b 6520 7374 796c 6560 2061  g `make style` a
+00001190: 6e64 2060 6d61 6b65 206c 696e 7460 2e5c  nd `make lint`.\
+000011a0: 6e5c 6e23 2320 4163 6b6e 6f77 6c65 6467  n\n## Acknowledg
+000011b0: 656d 656e 7473 5c6e 5c6e 2a20 4675 6e64  ements\n\n* Fund
+000011c0: 6564 2066 726f 6d20 4d61 7263 6820 3230  ed from March 20
+000011d0: 3233 2075 6e74 696c 2041 7567 7573 7420  23 until August 
+000011e0: 3230 3233 2062 7920 215b 6c6f 676f 7320  2023 by ![logos 
+000011f0: 6f66 2074 6865 2022 4275 6e64 6573 6d69  of the "Bundesmi
+00001200: 6e69 7374 6572 6975 6d20 66c3 bc72 2042  nisterium f..r B
+00001210: 696c 6475 6e67 2075 6e64 2046 6f72 7363  ildung und Forsc
+00001220: 6875 6e67 222c 2050 726f 646f 7479 7065  hung", Prodotype
+00001230: 2046 756e 6420 616e 6420 4f4b 464e 2d44   Fund and OKFN-D
+00001240: 6575 7473 6368 6c61 6e64 5d28 7265 736f  eutschland](reso
+00001250: 7572 6365 732f 7066 5f66 756e 6469 6e67  urces/pf_funding
+00001260: 5f6c 6f67 6f73 2e73 7667 295c 6e27 2c0a  _logos.svg)\n',.
+00001270: 2020 2020 2761 7574 686f 7227 3a20 2754      'author': 'T
+00001280: 6f62 6961 7320 5374 6572 6261 6b20 2620  obias Sterbak & 
+00001290: 5374 696e 6120 4c6f 686d c3bc 6c6c 6572  Stina Lohm..ller
+000012a0: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
+000012b0: 6d61 696c 273a 2027 6865 6c6c 6f40 6269  mail': 'hello@bi
+000012c0: 6173 6c79 7a65 2e6f 7267 272c 0a20 2020  aslyze.org',.   
+000012d0: 2027 6d61 696e 7461 696e 6572 273a 2027   'maintainer': '
+000012e0: 546f 6269 6173 2053 7465 7262 616b 272c  Tobias Sterbak',
+000012f0: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
+00001300: 5f65 6d61 696c 273a 2027 6865 6c6c 6f40  _email': 'hello@
+00001310: 746f 6269 6173 7374 6572 6261 6b2e 636f  tobiassterbak.co
+00001320: 6d27 2c0a 2020 2020 2775 726c 273a 2027  m',.    'url': '
+00001330: 6874 7470 733a 2f2f 6269 6173 6c79 7a65  https://biaslyze
+00001340: 2e6f 7267 272c 0a20 2020 2027 7061 636b  .org',.    'pack
+00001350: 6167 6573 273a 2070 6163 6b61 6765 732c  ages': packages,
+00001360: 0a20 2020 2027 7061 636b 6167 655f 6461  .    'package_da
+00001370: 7461 273a 2070 6163 6b61 6765 5f64 6174  ta': package_dat
+00001380: 612c 0a20 2020 2027 696e 7374 616c 6c5f  a,.    'install_
+00001390: 7265 7175 6972 6573 273a 2069 6e73 7461  requires': insta
+000013a0: 6c6c 5f72 6571 7569 7265 732c 0a20 2020  ll_requires,.   
+000013b0: 2027 7079 7468 6f6e 5f72 6571 7569 7265   'python_require
+000013c0: 7327 3a20 273e 3d33 2e31 302c 3c33 2e31  s': '>=3.10,<3.1
+000013d0: 3127 2c0a 7d0a 0a0a 7365 7475 7028 2a2a  1',.}...setup(**
+000013e0: 7365 7475 705f 6b77 6172 6773 290a       setup_kwargs).
```

### Comparing `biaslyze-0.0.5a0/PKG-INFO` & `biaslyze-0.0.6a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6269 6173  : 2.1.Name: bias
 00000020: 6c79 7a65 0a56 6572 7369 6f6e 3a20 302e  lyze.Version: 0.
-00000030: 302e 3561 300a 5375 6d6d 6172 793a 2054  0.5a0.Summary: T
+00000030: 302e 3661 300a 5375 6d6d 6172 793a 2054  0.6a0.Summary: T
 00000040: 6865 204e 4c50 2042 6961 7320 4964 656e  he NLP Bias Iden
 00000050: 7469 6669 6361 7469 6f6e 2054 6f6f 6c6b  tification Toolk
 00000060: 6974 0a48 6f6d 652d 7061 6765 3a20 6874  it.Home-page: ht
 00000070: 7470 733a 2f2f 6269 6173 6c79 7a65 2e6f  tps://biaslyze.o
 00000080: 7267 0a4c 6963 656e 7365 3a20 4253 442d  rg.License: BSD-
 00000090: 332d 436c 6175 7365 0a4b 6579 776f 7264  3-Clause.Keyword
 000000a0: 733a 204e 4c50 2c62 6961 732c 6574 6869  s: NLP,bias,ethi
@@ -116,187 +116,224 @@
 00000730: 6f6a 6563 742d 5552 4c3a 2052 6570 6f73  oject-URL: Repos
 00000740: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
 00000750: 6974 6875 622e 636f 6d2f 6269 6173 6c79  ithub.com/biasly
 00000760: 7a65 2d64 6576 2f62 6961 736c 797a 652f  ze-dev/biaslyze/
 00000770: 6973 7375 6573 0a44 6573 6372 6970 7469  issues.Descripti
 00000780: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 00000790: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-000007a0: 2320 6269 6173 6c79 7a65 202d 2054 6865  # biaslyze - The
-000007b0: 204e 4c50 2042 6961 7320 4964 656e 7469   NLP Bias Identi
-000007c0: 6669 6361 7469 6f6e 2054 6f6f 6c6b 6974  fication Toolkit
-000007d0: 0a0a 4269 6173 2069 7320 6f66 7465 6e20  ..Bias is often 
-000007e0: 7375 6274 6c65 2061 6e64 2064 6966 6669  subtle and diffi
-000007f0: 6375 6c74 2074 6f20 6465 7465 6374 2069  cult to detect i
-00000800: 6e20 4e4c 5020 6d6f 6465 6c73 2c20 6173  n NLP models, as
-00000810: 2074 6865 2070 726f 7465 6374 6564 2061   the protected a
-00000820: 7474 7269 6275 7465 7320 6172 6520 6c65  ttributes are le
-00000830: 7373 206f 6276 696f 7573 2061 6e64 2063  ss obvious and c
-00000840: 616e 2074 616b 6520 6d61 6e79 2066 6f72  an take many for
-00000850: 6d73 2069 6e20 6c61 6e67 7561 6765 2028  ms in language (
-00000860: 652e 672e 2070 726f 7869 6573 2c20 646f  e.g. proxies, do
-00000870: 7562 6c65 206d 6561 6e69 6e67 732c 2061  uble meanings, a
-00000880: 6d62 6967 7569 7469 6573 2065 7463 2e29  mbiguities etc.)
-00000890: 2e20 5468 6572 6566 6f72 652c 2074 6563  . Therefore, tec
-000008a0: 686e 6963 616c 2062 6961 7320 7465 7374  hnical bias test
-000008b0: 696e 6720 6973 2061 206b 6579 2073 7465  ing is a key ste
-000008c0: 7020 696e 2061 766f 6964 696e 6720 616c  p in avoiding al
-000008d0: 676f 7269 7468 6d69 6361 6c6c 7920 6d65  gorithmically me
-000008e0: 6469 6174 6564 2064 6973 6372 696d 696e  diated discrimin
-000008f0: 6174 696f 6e2e 2048 6f77 6576 6572 2c20  ation. However, 
-00000900: 6974 2069 7320 6375 7272 656e 746c 7920  it is currently 
-00000910: 636f 6e64 7563 7465 6420 746f 6f20 7261  conducted too ra
-00000920: 7265 6c79 2064 7565 2074 6f20 7468 6520  rely due to the 
-00000930: 6566 666f 7274 2069 6e76 6f6c 7665 642c  effort involved,
-00000940: 206d 6973 7369 6e67 2072 6573 6f75 7263   missing resourc
-00000950: 6573 206f 7220 6c61 636b 206f 6620 6177  es or lack of aw
-00000960: 6172 656e 6573 7320 666f 7220 7468 6520  areness for the 
-00000970: 7072 6f62 6c65 6d2e 0a0a 4269 6173 6c79  problem...Biasly
-00000980: 7a65 2068 656c 7073 2074 6f20 6765 7420  ze helps to get 
-00000990: 7374 6172 7465 6420 7769 7468 2074 6865  started with the
-000009a0: 2061 6e61 6c79 7369 7320 6f66 2062 6961   analysis of bia
-000009b0: 7320 7769 7468 696e 204e 4c50 206d 6f64  s within NLP mod
-000009c0: 656c 7320 616e 6420 6f66 6665 7273 2061  els and offers a
-000009d0: 2063 6f6e 6372 6574 6520 656e 7472 7920   concrete entry 
-000009e0: 706f 696e 7420 666f 7220 6675 7274 6865  point for furthe
-000009f0: 7220 696d 7061 6374 2061 7373 6573 736d  r impact assessm
-00000a00: 656e 7473 2061 6e64 206d 6974 6967 6174  ents and mitigat
-00000a10: 696f 6e20 6d65 6173 7572 6573 2e20 4573  ion measures. Es
-00000a20: 7065 6369 616c 6c79 2066 6f72 2079 6f75  pecially for you
-00000a30: 6e67 2064 6576 656c 6f70 6572 732c 2073  ng developers, s
-00000a40: 7475 6465 6e74 7320 616e 6420 7465 616d  tudents and team
-00000a50: 7320 7769 7468 206c 696d 6974 6564 2072  s with limited r
-00000a60: 6573 6f75 7263 6573 2c20 6f75 7220 746f  esources, our to
-00000a70: 6f6c 626f 7820 6f66 6665 7273 2061 206c  olbox offers a l
-00000a80: 6f77 2d65 6666 6f72 7420 6170 7072 6f61  ow-effort approa
-00000a90: 6368 2074 6f20 6269 6173 2074 6573 7469  ch to bias testi
-00000aa0: 6e67 2069 6e20 4e4c 5020 7573 6520 6361  ng in NLP use ca
-00000ab0: 7365 732e 0a0a 2323 2049 6e73 7461 6c6c  ses...## Install
-00000ac0: 6174 696f 6e0a 0a49 6e73 7461 6c6c 6174  ation..Installat
-00000ad0: 696f 6e20 6361 6e20 6265 2064 6f6e 6520  ion can be done 
-00000ae0: 7573 696e 6720 7079 7069 3a0a 6060 6062  using pypi:.```b
-00000af0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00000b00: 6269 6173 6c79 7a65 0a60 6060 0a0a 2323  biaslyze.```..##
-00000b10: 2051 7569 636b 7374 6172 740a 0a60 6060   Quickstart..```
-00000b20: 7079 7468 6f6e 0a66 726f 6d20 6269 6173  python.from bias
-00000b30: 6c79 7a65 2e62 6961 735f 6465 7465 6374  lyze.bias_detect
-00000b40: 6f72 7320 696d 706f 7274 2043 6f75 6e74  ors import Count
-00000b50: 6572 6661 6374 7561 6c42 6961 7344 6574  erfactualBiasDet
-00000b60: 6563 746f 720a 0a62 6961 735f 6465 7465  ector..bias_dete
-00000b70: 6374 6f72 203d 2043 6f75 6e74 6572 6661  ctor = Counterfa
-00000b80: 6374 7561 6c42 6961 7344 6574 6563 746f  ctualBiasDetecto
-00000b90: 7228 290a 0a23 2064 6574 6563 7420 6269  r()..# detect bi
-00000ba0: 6173 2069 6e20 7468 6520 6d6f 6465 6c20  as in the model 
-00000bb0: 6261 7365 6420 6f6e 2074 6865 2067 6976  based on the giv
-00000bc0: 656e 2074 6578 7473 0a23 2068 6572 652c  en texts.# here,
-00000bd0: 2063 6c66 2069 7320 6120 7363 696b 6974   clf is a scikit
-00000be0: 2d6c 6561 726e 2074 6578 7420 636c 6173  -learn text clas
-00000bf0: 7369 6669 6361 7469 6f6e 2070 6970 656c  sification pipel
-00000c00: 696e 6520 7472 6169 6e65 6420 666f 7220  ine trained for 
-00000c10: 6120 6269 6e61 7279 2063 6c61 7373 6966  a binary classif
-00000c20: 6963 6174 696f 6e20 7461 736b 0a64 6574  ication task.det
-00000c30: 6563 7469 6f6e 5f72 6573 203d 2062 6961  ection_res = bia
-00000c40: 735f 6465 7465 6374 6f72 2e70 726f 6365  s_detector.proce
-00000c50: 7373 280a 2020 2020 7465 7874 733d 7465  ss(.    texts=te
-00000c60: 7874 732c 0a20 2020 2070 7265 6469 6374  xts,.    predict
-00000c70: 5f66 756e 633d 636c 662e 7072 6564 6963  _func=clf.predic
-00000c80: 745f 7072 6f62 610a 290a 0a23 2073 6565  t_proba.)..# see
-00000c90: 2061 2073 756d 6d61 7279 206f 6620 7468   a summary of th
-00000ca0: 6520 6465 7465 6374 696f 6e0a 6465 7465  e detection.dete
-00000cb0: 6374 696f 6e5f 7265 732e 7265 706f 7274  ction_res.report
-00000cc0: 2829 0a0a 2320 7669 7375 616c 697a 6520  ()..# visualize 
-00000cd0: 7468 6520 636f 756e 7465 7266 6163 7475  the counterfactu
-00000ce0: 616c 2073 636f 7265 730a 6465 7465 6374  al scores.detect
-00000cf0: 696f 6e5f 7265 732e 7669 7375 616c 697a  ion_res.visualiz
-00000d00: 655f 636f 756e 7465 7266 6163 7475 616c  e_counterfactual
-00000d10: 5f73 636f 7265 7328 636f 6e63 6570 743d  _scores(concept=
-00000d20: 2272 656c 6967 696f 6e22 2c20 746f 705f  "religion", top_
-00000d30: 6e3d 3130 290a 6060 600a 0a45 7861 6d70  n=10).```..Examp
-00000d40: 6c65 206f 7574 7075 743a 0a21 5b5d 2872  le output:.![](r
-00000d50: 6573 6f75 7263 6573 2f68 6174 6573 7065  esources/hatespe
-00000d60: 6563 685f 646c 5f73 636f 7265 735f 7265  ech_dl_scores_re
-00000d70: 6c69 6769 6f6e 2e70 6e67 290a 0a0a 596f  ligion.png)...Yo
-00000d80: 7520 6361 6e20 7365 6520 6120 6d6f 7265  u can see a more
-00000d90: 2064 6574 6169 6c65 6420 6578 616d 706c   detailed exampl
-00000da0: 6520 696e 2074 6865 205b 7475 746f 7269  e in the [tutori
-00000db0: 616c 5d28 7475 746f 7269 616c 732f 7475  al](tutorials/tu
-00000dc0: 746f 7269 616c 2d74 6f78 6963 2d63 6f6d  torial-toxic-com
-00000dd0: 6d65 6e74 732f 292e 0a0a 0a23 2320 4465  ments/)....## De
-00000de0: 7665 6c6f 706d 656e 7420 7365 7475 700a  velopment setup.
-00000df0: 0a2d 2046 6972 7374 2079 6f75 206e 6565  .- First you nee
-00000e00: 6420 746f 2069 6e73 7461 6c6c 2070 6f65  d to install poe
-00000e10: 7472 7920 746f 206d 616e 6167 6520 796f  try to manage yo
-00000e20: 7572 2070 7974 686f 6e20 656e 7669 726f  ur python enviro
-00000e30: 6e6d 656e 743a 2068 7474 7073 3a2f 2f70  nment: https://p
-00000e40: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-00000e50: 2f64 6f63 732f 2369 6e73 7461 6c6c 6174  /docs/#installat
-00000e60: 696f 6e0a 2d20 5275 6e20 606d 616b 6520  ion.- Run `make 
-00000e70: 696e 7374 616c 6c60 2074 6f20 696e 7374  install` to inst
-00000e80: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
-00000e90: 6369 6573 2061 6e64 2067 6574 2074 6865  cies and get the
-00000ea0: 2073 7061 6379 2062 6173 656d 6f64 656c   spacy basemodel
-00000eb0: 732e 0a2d 204e 6f77 2079 6f75 2063 616e  s..- Now you can
-00000ec0: 2075 7365 2060 6269 6173 6c79 7a65 6020   use `biaslyze` 
-00000ed0: 696e 2079 6f75 7220 6a75 7079 7465 7220  in your jupyter 
-00000ee0: 6e6f 7465 626f 6f6b 732e 0a0a 0a23 2323  notebooks....###
-00000ef0: 2041 6464 696e 6720 636f 6e63 6570 7473   Adding concepts
-00000f00: 2061 6e64 206b 6579 776f 7264 730a 0a59   and keywords..Y
-00000f10: 6f75 2063 616e 2061 6464 2063 6f6e 6365  ou can add conce
-00000f20: 7074 7320 616e 6420 6e65 7720 6b65 7977  pts and new keyw
-00000f30: 6f72 6473 2066 6f72 2065 7869 7374 696e  ords for existin
-00000f40: 6720 636f 6e63 6570 7473 2062 7920 6564  g concepts by ed
-00000f50: 6974 696e 6720 5b63 6f6e 6365 7074 732e  iting [concepts.
-00000f60: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00000f70: 7562 2e63 6f6d 2f62 6961 736c 797a 652d  ub.com/biaslyze-
-00000f80: 6465 762f 6269 6173 6c79 7a65 2f62 6c6f  dev/biaslyze/blo
-00000f90: 622f 6b65 7977 6f72 642d 6261 7365 642d  b/keyword-based-
-00000fa0: 7461 7267 6574 6564 2d6c 696d 652f 6269  targeted-lime/bi
-00000fb0: 6173 6c79 7a65 2f63 6f6e 6365 7074 732e  aslyze/concepts.
-00000fc0: 7079 292e 0a0a 2323 2050 7265 7669 6577  py)...## Preview
-00000fd0: 2f62 7569 6c64 2074 6865 2064 6f63 756d  /build the docum
-00000fe0: 656e 7461 7469 6f6e 2077 6974 6820 6d6b  entation with mk
-00000ff0: 646f 6373 0a0a 546f 2070 7265 7669 6577  docs..To preview
-00001000: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00001010: 6f6e 2072 756e 2060 6d61 6b65 2064 6f63  on run `make doc
-00001020: 2d70 7265 7669 6577 602e 2054 6869 7320  -preview`. This 
-00001030: 7769 6c6c 206c 6175 6e63 6820 6120 7072  will launch a pr
-00001040: 6576 6965 7720 6f66 2074 6865 2064 6f63  eview of the doc
-00001050: 756d 656e 7461 7469 6f6e 206f 6e20 6068  umentation on `h
-00001060: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00001070: 3830 3030 2f60 2e0a 546f 2062 7569 6c64  8000/`..To build
-00001080: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00001090: 6f6e 2068 746d 6c20 7275 6e20 606d 616b  on html run `mak
-000010a0: 6520 646f 6360 2e0a 0a0a 2323 2052 756e  e doc`....## Run
-000010b0: 2074 6865 2061 7574 6f6d 6174 6564 2074   the automated t
-000010c0: 6573 7473 0a0a 606d 616b 6520 7465 7374  ests..`make test
-000010d0: 600a 0a0a 2323 2053 7479 6c65 2067 7569  `...## Style gui
-000010e0: 6465 0a0a 5765 2061 7265 2075 7369 6e67  de..We are using
-000010f0: 2069 736f 7274 2061 6e64 2062 6c61 636b   isort and black
-00001100: 3a20 606d 616b 6520 7374 796c 6560 0a46  : `make style`.F
-00001110: 6f72 206c 696e 7469 6e67 2077 6520 6172  or linting we ar
-00001120: 6520 7275 6e6e 696e 6720 7275 6666 3a20  e running ruff: 
-00001130: 606d 616b 6520 6c69 6e74 600a 0a23 2320  `make lint`..## 
-00001140: 436f 6e74 7269 6275 7469 6e67 0a0a 466f  Contributing..Fo
-00001150: 6c6c 6f77 2074 6865 2067 6f6f 676c 6520  llow the google 
-00001160: 7374 796c 6520 6775 6964 6520 666f 7220  style guide for 
-00001170: 7079 7468 6f6e 3a20 6874 7470 733a 2f2f  python: https://
-00001180: 676f 6f67 6c65 2e67 6974 6875 622e 696f  google.github.io
-00001190: 2f73 7479 6c65 6775 6964 652f 7079 6775  /styleguide/pygu
-000011a0: 6964 652e 6874 6d6c 0a0a 5468 6973 2070  ide.html..This p
-000011b0: 726f 6a65 6374 2075 7365 7320 626c 6163  roject uses blac
-000011c0: 6b2c 2069 736f 7274 2061 6e64 2072 7566  k, isort and ruf
-000011d0: 6620 746f 2065 6e66 6f72 6365 2073 7479  f to enforce sty
-000011e0: 6c65 2e20 4170 706c 7920 6974 2062 7920  le. Apply it by 
-000011f0: 7275 6e6e 696e 6720 606d 616b 6520 7374  running `make st
-00001200: 796c 6560 2061 6e64 2060 6d61 6b65 206c  yle` and `make l
-00001210: 696e 7460 2e0a 0a23 2320 4163 6b6e 6f77  int`...## Acknow
-00001220: 6c65 6467 656d 656e 7473 0a0a 2a20 4675  ledgements..* Fu
-00001230: 6e64 6564 2066 726f 6d20 4d61 7263 6820  nded from March 
-00001240: 3230 3233 2075 6e74 696c 2041 7567 7573  2023 until Augus
-00001250: 7420 3230 3233 2062 7920 215b 6c6f 676f  t 2023 by ![logo
-00001260: 7320 6f66 2074 6865 2022 4275 6e64 6573  s of the "Bundes
-00001270: 6d69 6e69 7374 6572 6975 6d20 66c3 bc72  ministerium f..r
-00001280: 2042 696c 6475 6e67 2075 6e64 2046 6f72   Bildung und For
-00001290: 7363 6875 6e67 222c 2050 726f 646f 7479  schung", Prodoty
-000012a0: 7065 2046 756e 6420 616e 6420 4f4b 464e  pe Fund and OKFN
-000012b0: 2d44 6575 7473 6368 6c61 6e64 5d28 7265  -Deutschland](re
-000012c0: 736f 7572 6365 732f 7066 5f66 756e 6469  sources/pf_fundi
-000012d0: 6e67 5f6c 6f67 6f73 2e73 7667 290a 0a    ng_logos.svg)..
+000007a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000007b0: 7222 3e0a 2020 3c68 313e 6269 6173 6c79  r">.  <h1>biasly
+000007c0: 7a65 202d 2054 6865 204e 4c50 2042 6961  ze - The NLP Bia
+000007d0: 7320 4964 656e 7469 6669 6361 7469 6f6e  s Identification
+000007e0: 2054 6f6f 6c6b 6974 3c2f 6831 3e0a 3c2f   Toolkit</h1>.</
+000007f0: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
+00000800: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000810: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000820: 7562 2e63 6f6d 2f62 6961 736c 797a 652d  ub.com/biaslyze-
+00000830: 6465 762f 6269 6173 6c79 7a65 2f62 6c6f  dev/biaslyze/blo
+00000840: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+00000850: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+00000860: 743d 226c 6963 656e 6365 2220 7372 633d  t="licence" src=
+00000870: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000880: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000890: 6963 656e 7365 2f62 6961 736c 797a 652d  icense/biaslyze-
+000008a0: 6465 762f 6269 6173 6c79 7a65 223e 0a20  dev/biaslyze">. 
+000008b0: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+000008c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000008d0: 692e 6f72 672f 7072 6f6a 6563 742f 6269  i.org/project/bi
+000008e0: 6173 6c79 7a65 2f22 3e0a 2020 2020 2020  aslyze/">.      
+000008f0: 2020 3c69 6d67 2061 6c74 3d22 7079 7069    <img alt="pypi
+00000900: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000910: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000920: 7069 2f76 2f62 6961 736c 797a 6522 3e0a  pi/v/biaslyze">.
+00000930: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+00000940: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000950: 7069 2e6f 7267 2f70 726f 6a65 6374 2f62  pi.org/project/b
+00000960: 6961 736c 797a 652f 223e 0a20 2020 2020  iaslyze/">.     
+00000970: 2020 203c 696d 6720 616c 743d 2270 7970     <img alt="pyp
+00000980: 6922 2073 7263 3d22 6874 7470 733a 2f2f  i" src="https://
+00000990: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000009a0: 7970 692f 7079 7665 7273 696f 6e73 2f62  ypi/pyversions/b
+000009b0: 6961 736c 797a 6522 3e0a 2020 2020 3c2f  iaslyze">.    </
+000009c0: 613e 0a3c 2f70 3e0a 0a0a 4269 6173 2069  a>.</p>...Bias i
+000009d0: 7320 6f66 7465 6e20 7375 6274 6c65 2061  s often subtle a
+000009e0: 6e64 2064 6966 6669 6375 6c74 2074 6f20  nd difficult to 
+000009f0: 6465 7465 6374 2069 6e20 4e4c 5020 6d6f  detect in NLP mo
+00000a00: 6465 6c73 2c20 6173 2074 6865 2070 726f  dels, as the pro
+00000a10: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
+00000a20: 7320 6172 6520 6c65 7373 206f 6276 696f  s are less obvio
+00000a30: 7573 2061 6e64 2063 616e 2074 616b 6520  us and can take 
+00000a40: 6d61 6e79 2066 6f72 6d73 2069 6e20 6c61  many forms in la
+00000a50: 6e67 7561 6765 2028 652e 672e 2070 726f  nguage (e.g. pro
+00000a60: 7869 6573 2c20 646f 7562 6c65 206d 6561  xies, double mea
+00000a70: 6e69 6e67 732c 2061 6d62 6967 7569 7469  nings, ambiguiti
+00000a80: 6573 2065 7463 2e29 2e20 5468 6572 6566  es etc.). Theref
+00000a90: 6f72 652c 2074 6563 686e 6963 616c 2062  ore, technical b
+00000aa0: 6961 7320 7465 7374 696e 6720 6973 2061  ias testing is a
+00000ab0: 206b 6579 2073 7465 7020 696e 2061 766f   key step in avo
+00000ac0: 6964 696e 6720 616c 676f 7269 7468 6d69  iding algorithmi
+00000ad0: 6361 6c6c 7920 6d65 6469 6174 6564 2064  cally mediated d
+00000ae0: 6973 6372 696d 696e 6174 696f 6e2e 2048  iscrimination. H
+00000af0: 6f77 6576 6572 2c20 6974 2069 7320 6375  owever, it is cu
+00000b00: 7272 656e 746c 7920 636f 6e64 7563 7465  rrently conducte
+00000b10: 6420 746f 6f20 7261 7265 6c79 2064 7565  d too rarely due
+00000b20: 2074 6f20 7468 6520 6566 666f 7274 2069   to the effort i
+00000b30: 6e76 6f6c 7665 642c 206d 6973 7369 6e67  nvolved, missing
+00000b40: 2072 6573 6f75 7263 6573 206f 7220 6c61   resources or la
+00000b50: 636b 206f 6620 6177 6172 656e 6573 7320  ck of awareness 
+00000b60: 666f 7220 7468 6520 7072 6f62 6c65 6d2e  for the problem.
+00000b70: 0a0a 4269 6173 6c79 7a65 2068 656c 7073  ..Biaslyze helps
+00000b80: 2074 6f20 6765 7420 7374 6172 7465 6420   to get started 
+00000b90: 7769 7468 2074 6865 2061 6e61 6c79 7369  with the analysi
+00000ba0: 7320 6f66 2062 6961 7320 7769 7468 696e  s of bias within
+00000bb0: 204e 4c50 206d 6f64 656c 7320 616e 6420   NLP models and 
+00000bc0: 6f66 6665 7273 2061 2063 6f6e 6372 6574  offers a concret
+00000bd0: 6520 656e 7472 7920 706f 696e 7420 666f  e entry point fo
+00000be0: 7220 6675 7274 6865 7220 696d 7061 6374  r further impact
+00000bf0: 2061 7373 6573 736d 656e 7473 2061 6e64   assessments and
+00000c00: 206d 6974 6967 6174 696f 6e20 6d65 6173   mitigation meas
+00000c10: 7572 6573 2e20 4573 7065 6369 616c 6c79  ures. Especially
+00000c20: 2066 6f72 2074 6561 6d73 2077 6974 6820   for teams with 
+00000c30: 6c69 6d69 7465 6420 7265 736f 7572 6365  limited resource
+00000c40: 732c 206f 7572 2074 6f6f 6c62 6f78 206f  s, our toolbox o
+00000c50: 6666 6572 7320 6120 6c6f 772d 6566 666f  ffers a low-effo
+00000c60: 7274 2061 7070 726f 6163 6820 746f 2062  rt approach to b
+00000c70: 6961 7320 7465 7374 696e 6720 696e 204e  ias testing in N
+00000c80: 4c50 2075 7365 2063 6173 6573 2e0a 0a23  LP use cases...#
+00000c90: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
+00000ca0: 496e 7374 616c 6c61 7469 6f6e 2063 616e  Installation can
+00000cb0: 2062 6520 646f 6e65 2075 7369 6e67 2070   be done using p
+00000cc0: 7970 693a 0a60 6060 6261 7368 0a70 6970  ypi:.```bash.pip
+00000cd0: 2069 6e73 7461 6c6c 2062 6961 736c 797a   install biaslyz
+00000ce0: 650a 6060 600a 0a54 6865 6e20 796f 7520  e.```..Then you 
+00000cf0: 6e65 6564 2074 6f20 646f 776e 6c6f 6164  need to download
+00000d00: 2074 6865 2072 6571 7569 7265 6420 7370   the required sp
+00000d10: 6163 7920 6d6f 6465 6c73 3a0a 6060 6062  acy models:.```b
+00000d20: 6173 680a 7079 7468 6f6e 202d 6d20 7370  ash.python -m sp
+00000d30: 6163 7920 646f 776e 6c6f 6164 2065 6e5f  acy download en_
+00000d40: 636f 7265 5f77 6562 5f73 6d0a 6060 600a  core_web_sm.```.
+00000d50: 0a23 2320 5175 6963 6b73 7461 7274 0a0a  .## Quickstart..
+00000d60: 6060 6070 7974 686f 6e0a 6672 6f6d 2062  ```python.from b
+00000d70: 6961 736c 797a 652e 6269 6173 5f64 6574  iaslyze.bias_det
+00000d80: 6563 746f 7273 2069 6d70 6f72 7420 436f  ectors import Co
+00000d90: 756e 7465 7266 6163 7475 616c 4269 6173  unterfactualBias
+00000da0: 4465 7465 6374 6f72 0a0a 6269 6173 5f64  Detector..bias_d
+00000db0: 6574 6563 746f 7220 3d20 436f 756e 7465  etector = Counte
+00000dc0: 7266 6163 7475 616c 4269 6173 4465 7465  rfactualBiasDete
+00000dd0: 6374 6f72 2829 0a0a 2320 6465 7465 6374  ctor()..# detect
+00000de0: 2062 6961 7320 696e 2074 6865 206d 6f64   bias in the mod
+00000df0: 656c 2062 6173 6564 206f 6e20 7468 6520  el based on the 
+00000e00: 6769 7665 6e20 7465 7874 730a 2320 6865  given texts.# he
+00000e10: 7265 2c20 636c 6620 6973 2061 2073 6369  re, clf is a sci
+00000e20: 6b69 742d 6c65 6172 6e20 7465 7874 2063  kit-learn text c
+00000e30: 6c61 7373 6966 6963 6174 696f 6e20 7069  lassification pi
+00000e40: 7065 6c69 6e65 2074 7261 696e 6564 2066  peline trained f
+00000e50: 6f72 2061 2062 696e 6172 7920 636c 6173  or a binary clas
+00000e60: 7369 6669 6361 7469 6f6e 2074 6173 6b0a  sification task.
+00000e70: 6465 7465 6374 696f 6e5f 7265 7320 3d20  detection_res = 
+00000e80: 6269 6173 5f64 6574 6563 746f 722e 7072  bias_detector.pr
+00000e90: 6f63 6573 7328 0a20 2020 2074 6578 7473  ocess(.    texts
+00000ea0: 3d74 6578 7473 2c0a 2020 2020 7072 6564  =texts,.    pred
+00000eb0: 6963 745f 6675 6e63 3d63 6c66 2e70 7265  ict_func=clf.pre
+00000ec0: 6469 6374 5f70 726f 6261 0a29 0a0a 2320  dict_proba.)..# 
+00000ed0: 7365 6520 6120 7375 6d6d 6172 7920 6f66  see a summary of
+00000ee0: 2074 6865 2064 6574 6563 7469 6f6e 0a64   the detection.d
+00000ef0: 6574 6563 7469 6f6e 5f72 6573 2e72 6570  etection_res.rep
+00000f00: 6f72 7428 290a 0a23 2076 6973 7561 6c69  ort()..# visuali
+00000f10: 7a65 2074 6865 2063 6f75 6e74 6572 6661  ze the counterfa
+00000f20: 6374 7561 6c20 7363 6f72 6573 0a64 6574  ctual scores.det
+00000f30: 6563 7469 6f6e 5f72 6573 2e76 6973 7561  ection_res.visua
+00000f40: 6c69 7a65 5f63 6f75 6e74 6572 6661 6374  lize_counterfact
+00000f50: 7561 6c5f 7363 6f72 6573 2863 6f6e 6365  ual_scores(conce
+00000f60: 7074 3d22 7265 6c69 6769 6f6e 222c 2074  pt="religion", t
+00000f70: 6f70 5f6e 3d31 3029 0a60 6060 0a0a 4578  op_n=10).```..Ex
+00000f80: 616d 706c 6520 6f75 7470 7574 3a0a 215b  ample output:.![
+00000f90: 5d28 7265 736f 7572 6365 732f 6861 7465  ](resources/hate
+00000fa0: 7370 6565 6368 5f64 6c5f 7363 6f72 6573  speech_dl_scores
+00000fb0: 5f72 656c 6967 696f 6e2e 706e 6729 0a0a  _religion.png)..
+00000fc0: 0a59 6f75 2063 616e 2073 6565 2061 206d  .You can see a m
+00000fd0: 6f72 6520 6465 7461 696c 6564 2065 7861  ore detailed exa
+00000fe0: 6d70 6c65 2069 6e20 7468 6520 5b74 7574  mple in the [tut
+00000ff0: 6f72 6961 6c5d 2874 7574 6f72 6961 6c73  orial](tutorials
+00001000: 2f74 7574 6f72 6961 6c2d 746f 7869 632d  /tutorial-toxic-
+00001010: 636f 6d6d 656e 7473 2f29 2e0a 0a0a 2323  comments/)....##
+00001020: 2044 6576 656c 6f70 6d65 6e74 2073 6574   Development set
+00001030: 7570 0a0a 2d20 4669 7273 7420 796f 7520  up..- First you 
+00001040: 6e65 6564 2074 6f20 696e 7374 616c 6c20  need to install 
+00001050: 706f 6574 7279 2074 6f20 6d61 6e61 6765  poetry to manage
+00001060: 2079 6f75 7220 7079 7468 6f6e 2065 6e76   your python env
+00001070: 6972 6f6e 6d65 6e74 3a20 6874 7470 733a  ironment: https:
+00001080: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
+00001090: 6f72 672f 646f 6373 2f23 696e 7374 616c  org/docs/#instal
+000010a0: 6c61 7469 6f6e 0a2d 2052 756e 2060 6d61  lation.- Run `ma
+000010b0: 6b65 2069 6e73 7461 6c6c 6020 746f 2069  ke install` to i
+000010c0: 6e73 7461 6c6c 2074 6865 2064 6570 656e  nstall the depen
+000010d0: 6465 6e63 6965 7320 616e 6420 6765 7420  dencies and get 
+000010e0: 7468 6520 7370 6163 7920 6261 7365 6d6f  the spacy basemo
+000010f0: 6465 6c73 2e0a 2d20 4e6f 7720 796f 7520  dels..- Now you 
+00001100: 6361 6e20 7573 6520 6062 6961 736c 797a  can use `biaslyz
+00001110: 6560 2069 6e20 796f 7572 206a 7570 7974  e` in your jupyt
+00001120: 6572 206e 6f74 6562 6f6f 6b73 2e0a 0a0a  er notebooks....
+00001130: 2323 2320 4164 6469 6e67 2063 6f6e 6365  ### Adding conce
+00001140: 7074 7320 616e 6420 6b65 7977 6f72 6473  pts and keywords
+00001150: 0a0a 596f 7520 6361 6e20 6164 6420 636f  ..You can add co
+00001160: 6e63 6570 7473 2061 6e64 206e 6577 206b  ncepts and new k
+00001170: 6579 776f 7264 7320 666f 7220 6578 6973  eywords for exis
+00001180: 7469 6e67 2063 6f6e 6365 7074 7320 6279  ting concepts by
+00001190: 2065 6469 7469 6e67 205b 636f 6e63 6570   editing [concep
+000011a0: 7473 2e70 795d 2868 7474 7073 3a2f 2f67  ts.py](https://g
+000011b0: 6974 6875 622e 636f 6d2f 6269 6173 6c79  ithub.com/biasly
+000011c0: 7a65 2d64 6576 2f62 6961 736c 797a 652f  ze-dev/biaslyze/
+000011d0: 626c 6f62 2f6b 6579 776f 7264 2d62 6173  blob/keyword-bas
+000011e0: 6564 2d74 6172 6765 7465 642d 6c69 6d65  ed-targeted-lime
+000011f0: 2f62 6961 736c 797a 652f 636f 6e63 6570  /biaslyze/concep
+00001200: 7473 2e70 7929 2e0a 0a23 2320 5072 6576  ts.py)...## Prev
+00001210: 6965 772f 6275 696c 6420 7468 6520 646f  iew/build the do
+00001220: 6375 6d65 6e74 6174 696f 6e20 7769 7468  cumentation with
+00001230: 206d 6b64 6f63 730a 0a54 6f20 7072 6576   mkdocs..To prev
+00001240: 6965 7720 7468 6520 646f 6375 6d65 6e74  iew the document
+00001250: 6174 696f 6e20 7275 6e20 606d 616b 6520  ation run `make 
+00001260: 646f 632d 7072 6576 6965 7760 2e20 5468  doc-preview`. Th
+00001270: 6973 2077 696c 6c20 6c61 756e 6368 2061  is will launch a
+00001280: 2070 7265 7669 6577 206f 6620 7468 6520   preview of the 
+00001290: 646f 6375 6d65 6e74 6174 696f 6e20 6f6e  documentation on
+000012a0: 2060 6874 7470 3a2f 2f31 3237 2e30 2e30   `http://127.0.0
+000012b0: 2e31 3a38 3030 302f 602e 0a54 6f20 6275  .1:8000/`..To bu
+000012c0: 696c 6420 7468 6520 646f 6375 6d65 6e74  ild the document
+000012d0: 6174 696f 6e20 6874 6d6c 2072 756e 2060  ation html run `
+000012e0: 6d61 6b65 2064 6f63 602e 0a0a 0a23 2320  make doc`....## 
+000012f0: 5275 6e20 7468 6520 6175 746f 6d61 7465  Run the automate
+00001300: 6420 7465 7374 730a 0a60 6d61 6b65 2074  d tests..`make t
+00001310: 6573 7460 0a0a 0a23 2320 5374 796c 6520  est`...## Style 
+00001320: 6775 6964 650a 0a57 6520 6172 6520 7573  guide..We are us
+00001330: 696e 6720 6973 6f72 7420 616e 6420 626c  ing isort and bl
+00001340: 6163 6b3a 2060 6d61 6b65 2073 7479 6c65  ack: `make style
+00001350: 600a 466f 7220 6c69 6e74 696e 6720 7765  `.For linting we
+00001360: 2061 7265 2072 756e 6e69 6e67 2072 7566   are running ruf
+00001370: 663a 2060 6d61 6b65 206c 696e 7460 0a0a  f: `make lint`..
+00001380: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00001390: 0a46 6f6c 6c6f 7720 7468 6520 676f 6f67  .Follow the goog
+000013a0: 6c65 2073 7479 6c65 2067 7569 6465 2066  le style guide f
+000013b0: 6f72 2070 7974 686f 6e3a 2068 7474 7073  or python: https
+000013c0: 3a2f 2f67 6f6f 676c 652e 6769 7468 7562  ://google.github
+000013d0: 2e69 6f2f 7374 796c 6567 7569 6465 2f70  .io/styleguide/p
+000013e0: 7967 7569 6465 2e68 746d 6c0a 0a54 6869  yguide.html..Thi
+000013f0: 7320 7072 6f6a 6563 7420 7573 6573 2062  s project uses b
+00001400: 6c61 636b 2c20 6973 6f72 7420 616e 6420  lack, isort and 
+00001410: 7275 6666 2074 6f20 656e 666f 7263 6520  ruff to enforce 
+00001420: 7374 796c 652e 2041 7070 6c79 2069 7420  style. Apply it 
+00001430: 6279 2072 756e 6e69 6e67 2060 6d61 6b65  by running `make
+00001440: 2073 7479 6c65 6020 616e 6420 606d 616b   style` and `mak
+00001450: 6520 6c69 6e74 602e 0a0a 2323 2041 636b  e lint`...## Ack
+00001460: 6e6f 776c 6564 6765 6d65 6e74 730a 0a2a  nowledgements..*
+00001470: 2046 756e 6465 6420 6672 6f6d 204d 6172   Funded from Mar
+00001480: 6368 2032 3032 3320 756e 7469 6c20 4175  ch 2023 until Au
+00001490: 6775 7374 2032 3032 3320 6279 2021 5b6c  gust 2023 by ![l
+000014a0: 6f67 6f73 206f 6620 7468 6520 2242 756e  ogos of the "Bun
+000014b0: 6465 736d 696e 6973 7465 7269 756d 2066  desministerium f
+000014c0: c3bc 7220 4269 6c64 756e 6720 756e 6420  ..r Bildung und 
+000014d0: 466f 7273 6368 756e 6722 2c20 5072 6f64  Forschung", Prod
+000014e0: 6f74 7970 6520 4675 6e64 2061 6e64 204f  otype Fund and O
+000014f0: 4b46 4e2d 4465 7574 7363 686c 616e 645d  KFN-Deutschland]
+00001500: 2872 6573 6f75 7263 6573 2f70 665f 6675  (resources/pf_fu
+00001510: 6e64 696e 675f 6c6f 676f 732e 7376 6729  nding_logos.svg)
+00001520: 0a0a                                     ..
```

