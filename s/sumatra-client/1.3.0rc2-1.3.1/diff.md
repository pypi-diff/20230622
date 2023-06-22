# Comparing `tmp/sumatra-client-1.3.0rc2.tar.gz` & `tmp/sumatra-client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumatra-client-1.3.0rc2.tar", last modified: Mon Jun  5 22:15:32 2023, max compression
+gzip compressed data, was "sumatra-client-1.3.1.tar", last modified: Thu Jun 22 16:40:28 2023, max compression
```

## Comparing `sumatra-client-1.3.0rc2.tar` & `sumatra-client-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.029421 sumatra-client-1.3.0rc2/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.0rc2/LICENSE
--rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-06-05 22:15:32.029652 sumatra-client-1.3.0rc2/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.0rc2/README.md
--rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.0rc2/pyproject.toml
--rw-r--r--   0 kuhlmann   (501) staff       (20)      827 2023-06-05 22:15:32.031018 sumatra-client-1.3.0rc2/setup.cfg
--rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc2/setup.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.020199 sumatra-client-1.3.0rc2/sumatra_client/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc2/sumatra_client/__init__.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc2/sumatra_client/admin.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     9612 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/auth.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.028133 sumatra-client-1.3.0rc2/sumatra_client/certs/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     1574 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/cert1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)     3749 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/chain1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)     5323 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/fullchain1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)      241 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/privkey1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc2/sumatra_client/cli.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-05-19 19:17:38.000000 sumatra-client-1.3.0rc2/sumatra_client/client.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-06-05 21:56:45.000000 sumatra-client-1.3.0rc2/sumatra_client/config.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-05-18 18:11:52.000000 sumatra-client-1.3.0rc2/sumatra_client/workspace.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.025477 sumatra-client-1.3.0rc2/sumatra_client.egg-info/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)      646 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/SOURCES.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/dependency_links.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/entry_points.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/not-zip-safe
--rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/requires.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/top_level.txt
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.028921 sumatra-client-1.3.0rc2/tests/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc2/tests/test_config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.741750 sumatra-client-1.3.1/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.1/LICENSE
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-06-22 16:40:28.741972 sumatra-client-1.3.1/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.1/README.md
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.1/pyproject.toml
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      824 2023-06-22 16:40:28.743060 sumatra-client-1.3.1/setup.cfg
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.1/setup.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.732729 sumatra-client-1.3.1/sumatra_client/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/__init__.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/admin.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     9612 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/auth.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.740563 sumatra-client-1.3.1/sumatra_client/certs/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     1574 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/cert1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     3749 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/certs/chain1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5323 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/fullchain1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      241 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/privkey1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/cli.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/client.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/config.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/workspace.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.737386 sumatra-client-1.3.1/sumatra_client.egg-info/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      646 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/entry_points.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.1/sumatra_client.egg-info/not-zip-safe
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/requires.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/top_level.txt
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.741243 sumatra-client-1.3.1/tests/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.1/tests/test_config.py
```

### Comparing `sumatra-client-1.3.0rc2/PKG-INFO` & `sumatra-client-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.0rc2
+Version: 1.3.1
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.0rc2/setup.cfg` & `sumatra-client-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumatra-client
-version = 1.3.0rc2
+version = 1.3.1
 author = Sumatra
 author_email = support@sumatra.ai
 url = https://sumatra.ai
 description = Sumatra Python Client and CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Sumatra Proprietary
```

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/admin.py` & `sumatra-client-1.3.1/sumatra_client/admin.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/auth.py` & `sumatra-client-1.3.1/sumatra_client/auth.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/certs/chain1.pem` & `sumatra-client-1.3.1/sumatra_client/certs/chain1.pem`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/certs/fullchain1.pem` & `sumatra-client-1.3.1/sumatra_client/certs/fullchain1.pem`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
 00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4945  FICATE-----.MIIE
 00000020: 5844 4343 4130 5367 4177 4942 4167 4953  XDCCA0SgAwIBAgIS
-00000030: 4179 6f67 6e6e 6e6e 5176 4745 564f 4951  AyognnnnQvGEVOIQ
-00000040: 4e32 7835 3036 7668 4d41 3047 4353 7147  N2x506vhMA0GCSqG
+00000030: 4246 3449 7767 3531 794f 4442 6a4f 6368  BF4Iwg51yODBjOch
+00000040: 536a 706d 5276 2f63 4d41 3047 4353 7147  SjpmRv/cMA0GCSqG
 00000050: 5349 6233 4451 4542 4377 5541 0a4d 4449  SIb3DQEBCwUA.MDI
 00000060: 7843 7a41 4a42 674e 5642 4159 5441 6c56  xCzAJBgNVBAYTAlV
 00000070: 544d 5259 7746 4159 4456 5151 4b45 7731  TMRYwFAYDVQQKEw1
 00000080: 4d5a 5851 6e63 7942 4662 6d4e 7965 5842  MZXQncyBFbmNyeXB
 00000090: 304d 5173 7743 5159 4456 5151 440a 4577  0MQswCQYDVQQD.Ew
-000000a0: 4a53 4d7a 4165 4677 3079 4d7a 4130 4d44  JSMzAeFw0yMzA0MD
-000000b0: 5978 4e44 4135 4e44 6861 4677 3079 4d7a  YxNDA5NDhaFw0yMz
-000000c0: 4133 4d44 5578 4e44 4135 4e44 6461 4d42  A3MDUxNDA5NDdaMB
+000000a0: 4a53 4d7a 4165 4677 3079 4d7a 4132 4d54  JSMzAeFw0yMzA2MT
+000000b0: 5578 4e44 4179 4d7a 6461 4677 3079 4d7a  UxNDAyMzdaFw0yMz
+000000c0: 4135 4d54 4d78 4e44 4179 4d7a 5a61 4d42  A5MTMxNDAyMzZaMB
 000000d0: 7778 476a 4159 4267 4e56 4241 4d54 0a45  wxGjAYBgNVBAMT.E
 000000e0: 5777 774c 6d78 795a 4335 7a64 5731 6864  WwwLmxyZC5zdW1hd
 000000f0: 484a 684c 6d46 704d 466b 7745 7759 484b  HJhLmFpMFkwEwYHK
 00000100: 6f5a 497a 6a30 4341 5159 494b 6f5a 497a  oZIzj0CAQYIKoZIz
-00000110: 6a30 4441 5163 4451 6741 452f 494b 610a  j0DAQcDQgAE/IKa.
-00000120: 4c4c 7851 6e73 5639 7244 6463 6658 686d  LLxQnsV9rDdcfXhm
-00000130: 5a50 5233 5832 2b4c 6d54 664d 4779 5856  ZPR3X2+LmTfMGyXV
-00000140: 7178 7a6b 6b31 2b70 426c 3745 7a32 644a  qxzkk1+pBl7Ez2dJ
-00000150: 4336 3032 434f 6266 4172 656a 3134 515a  C602CObfArej14QZ
-00000160: 0a5a 4d2b 6932 5a75 7841 746d 522b 6d52  .ZM+i2ZuxAtmR+mR
-00000170: 4947 364f 4341 6b73 7767 674a 484d 4134  IG6OCAkswggJHMA4
+00000110: 6a30 4441 5163 4451 6741 4545 7359 640a  j0DAQcDQgAEEsYd.
+00000120: 6e52 4f46 466d 6772 6c42 6967 7662 6e48  nROFFmgrlBigvbnH
+00000130: 452f 364f 4c59 576b 5179 3458 6535 704f  E/6OLYWkQy4Xe5pO
+00000140: 7a4d 7962 4636 5349 4475 5344 347a 4b46  zMybF6SIDuSD4zKF
+00000150: 7159 424c 626b 5a37 4a5a 5236 426b 3652  qYBLbkZ7JZR6Bk6R
+00000160: 0a5a 6279 7264 514d 6249 6970 304e 3138  .ZbyrdQMbIip0N18
+00000170: 6d61 364f 4341 6b73 7767 674a 484d 4134  ma6OCAkswggJHMA4
 00000180: 4741 3155 6444 7745 422f 7751 4541 7749  GA1UdDwEB/wQEAwI
 00000190: 4867 4441 6442 674e 5648 5355 4546 6a41  HgDAdBgNVHSUEFjA
 000001a0: 550a 4267 6772 4267 4546 4251 6344 4151  U.BggrBgEFBQcDAQ
 000001b0: 5949 4b77 5942 4251 5548 4177 4977 4441  YIKwYBBQUHAwIwDA
 000001c0: 5944 5652 3054 4151 482f 4241 4977 4144  YDVR0TAQH/BAIwAD
-000001d0: 4164 4267 4e56 4851 3445 4667 5155 4d44  AdBgNVHQ4EFgQUMD
-000001e0: 4874 0a58 4f6b 2b63 7834 4377 4f6d 4779  Ht.XOk+cx4CwOmGy
-000001f0: 3334 7645 4474 2b6a 4c6f 7748 7759 4456  34vEDt+jLowHwYDV
+000001d0: 4164 4267 4e56 4851 3445 4667 5155 344c  AdBgNVHQ4EFgQU4L
+000001e0: 764d 0a31 6932 5274 4d6d 626d 6730 4766  vM.1i2RtMmbmg0Gf
+000001f0: 4946 5a31 6e70 7759 7563 7748 7759 4456  IFZ1npwYucwHwYDV
 00000200: 5230 6a42 4267 7746 6f41 5546 4336 7a46  R0jBBgwFoAUFC6zF
 00000210: 3764 5956 7375 7555 416c 4135 682b 766e  7dYVsuuUAlA5h+vn
 00000220: 5973 550a 7773 5977 5651 5949 4b77 5942  YsU.wsYwVQYIKwYB
 00000230: 4251 5548 4151 4545 5354 4248 4d43 4547  BQUHAQEESTBHMCEG
 00000240: 4343 7347 4151 5546 427a 4142 6868 566f  CCsGAQUFBzABhhVo
 00000250: 6448 5277 4f69 3876 636a 4d75 6279 3573  dHRwOi8vcjMuby5s
 00000260: 5a57 356a 0a63 6935 7663 6d63 7749 6759  ZW5j.ci5vcmcwIgY
@@ -47,58 +47,58 @@
 000002e0: 4577 4e77 594c 0a4b 7759 4242 4147 4333  EwNwYL.KwYBBAGC3
 000002f0: 784d 4241 5145 774b 4441 6d42 6767 7242  xMBAQEwKDAmBggrB
 00000300: 6745 4642 5163 4341 5259 6161 4852 3063  gEFBQcCARYaaHR0c
 00000310: 446f 764c 324e 7763 7935 735a 5852 7a5a  DovL2Nwcy5sZXRzZ
 00000320: 5735 6a63 6e6c 770a 6443 3576 636d 6377  W5jcnlw.dC5vcmcw
 00000330: 6767 4544 4267 6f72 4267 4545 4164 5a35  ggEDBgorBgEEAdZ5
 00000340: 4167 5143 4249 4830 4249 4878 414f 3841  AgQCBIH0BIHxAO8A
-00000350: 6467 4333 5076 736b 3335 784e 756e 5879  dgC3Pvsk35xNunXy
-00000360: 4f63 5736 5750 5273 0a58 6678 437a 3371  OcW6WPRs.XfxCz3q
-00000370: 664e 6353 6548 516d 424a 6532 306d 5141  fNcSeHQmBJe20mQA
-00000380: 4141 5964 5848 6549 5441 4141 4541 7742  AAYdXHeITAAAEAwB
-00000390: 484d 4555 4349 4342 6675 5456 3241 7266  HMEUCICBfuTV2Arf
-000003a0: 4c4d 6e64 3854 586b 300a 7a71 5141 3250  LMnd8TXk0.zqQA2P
-000003b0: 4d77 6b59 6662 5448 7230 7256 5256 555a  MwkYfbTHr0rVRVUZ
-000003c0: 6566 4169 4541 6d33 3972 594f 6a6b 6452  efAiEAm39rYOjkdR
-000003d0: 5655 2b49 4a4f 7044 7757 625a 6868 5653  VU+IJOpDwWbZhhVS
-000003e0: 5173 4e35 5367 524d 2b69 0a41 4d57 6e4e  QsN5SgRM+i.AMWnN
-000003f0: 7763 4164 5143 7439 3737 3666 5038 5179  wcAdQCt9776fP8Qy
-00000400: 4975 6450 5a77 6550 6868 7174 4763 7058  IudPZwePhhqtGcpX
-00000410: 632b 7844 4354 4b68 5959 3036 3979 4369  c+xDCTKhYY069yCi
-00000420: 6741 4141 5964 5848 6549 340a 4141 4145  gAAAYdXHeI4.AAAE
-00000430: 4177 4247 4d45 5143 4945 7035 5330 3030  AwBGMEQCIEp5S000
-00000440: 4e6f 704f 7349 3245 766a 3165 5442 6173  NopOsI2Evj1eTBas
-00000450: 4c38 5a46 7471 6e65 754f 7947 6c4d 5339  L8ZFtqneuOyGlMS9
-00000460: 416d 737a 4169 414c 4233 6d63 0a52 782b  AmszAiALB3mc.Rx+
-00000470: 4c6c 5675 797a 2f39 5741 324e 4d6d 716d  LlVuyz/9WA2NMmqm
-00000480: 4459 6150 4252 624d 6277 332f 6770 5270  DYaPBRbMbw3/gpRp
-00000490: 474f 6a41 4e42 676b 7168 6b69 4739 7730  GOjANBgkqhkiG9w0
-000004a0: 4241 5173 4641 414f 4341 5145 410a 6771  BAQsFAAOCAQEA.gq
-000004b0: 4764 7435 7966 467a 5a77 5750 5473 5977  Gdt5yfFzZwWPTsYw
-000004c0: 6d4d 4f6f 7550 5435 5364 4d57 4933 4a79  mMOouPT5SdMWI3Jy
-000004d0: 7934 6971 4a73 726c 4675 5777 6e42 624b  y4iqJsrlFuWwnBbK
-000004e0: 314b 764c 5651 4241 324f 316c 6a30 0a2b  1KvLVQBA2O1lj0.+
-000004f0: 6d51 3547 5a4f 4c32 7837 3550 394e 6a31  mQ5GZOL2x75P9Nj1
-00000500: 6957 6962 304d 385a 2f34 5470 5347 6630  iWib0M8Z/4TpSGf0
-00000510: 5361 6d62 495a 5452 435a 434d 6c72 4e2b  SambIZTRCZCMlrN+
-00000520: 336a 6f4c 716b 4531 6979 3533 6230 530a  3joLqkE1iy53b0S.
-00000530: 5970 7971 4965 3456 4b43 7436 3552 6f61  YpyqIe4VKCt65Roa
-00000540: 3553 6b68 345a 5251 6758 474e 6545 6957  5Skh4ZRQgXGNeEiW
-00000550: 7674 4745 4376 4364 744d 434b 6858 5361  vtGECvCdtMCKhXSa
-00000560: 3557 412b 4b68 6848 6b42 4c61 7459 7245  5WA+KhhHkBLatYrE
-00000570: 0a49 2b64 4a48 7a45 2f66 5041 554c 4f6e  .I+dJHzE/fPAULOn
-00000580: 544e 5954 6a30 6d4a 4173 386c 396b 7a43  TNYTj0mJAs8l9kzC
-00000590: 4330 6278 726c 5375 6244 4e37 5245 5078  C0bxrlSubDN7REPx
-000005a0: 3447 3749 4b44 3145 4f61 3875 3776 6567  4G7IKD1EOa8u7veg
-000005b0: 490a 4555 5348 5a6a 7232 5275 5173 7434  I.EUSHZjr2RuQst4
-000005c0: 2b6c 762f 7275 3154 5038 6f50 6661 6350  +lv/ru1TP8oPfacP
-000005d0: 5971 396e 3469 515a 432b 6177 5845 3678  Yq9n4iQZC+awXE6x
-000005e0: 6c32 4656 6756 524e 6233 6f71 752b 6171  l2FVgVRNb3oqu+aq
-000005f0: 5a46 0a48 654f 4f35 705a 3769 6970 414e  ZF.HeOO5pZ7iipAN
-00000600: 7578 5758 6d70 6a36 413d 3d0a 2d2d 2d2d  uxWXmpj6A==.----
+00000350: 6451 4236 4d6f 7855 324c 6374 7469 4471  dQB6MoxU2LcttiDq
+00000360: 4f4f 4253 4875 6d45 0a46 6e41 7945 3456  OOBSHumE.FnAyE4V
+00000370: 4e4f 3949 7277 5470 586f 314c 7255 6741  NO9IrwTpXo1LrUgA
+00000380: 4141 5969 2f6c 4858 4241 4141 4541 7742  AAYi/lHXBAAAEAwB
+00000390: 474d 4551 4349 4144 2b63 6d32 3965 4b65  GMEQCIAD+cm29eKe
+000003a0: 5476 7648 5631 4a55 360a 4f36 416f 7556  TvvHV1JU6.O6AouV
+000003b0: 4d79 4e72 5277 6b70 4e38 4d58 3033 7851  MyNrRwkpN8MX03xQ
+000003c0: 7266 4169 4245 394b 6579 507a 7264 6368  rfAiBE9KeyPzrdch
+000003d0: 3257 7741 6e2b 7169 614b 4279 4761 4d6e  2WwAn+qiaKByGaMn
+000003e0: 4744 686d 6c4b 6576 6f61 0a36 6171 452f  GDhmlKevoa.6aqE/
+000003f0: 7742 3241 4f67 2b30 4e6f 2b39 5159 314d  wB2AOg+0No+9QY1M
+00000400: 7564 584b 4c79 4a61 386b 4430 3876 5245  udXKLyJa8kD08vRE
+00000410: 5776 7336 326e 6864 3331 7442 7231 7541  Wvs62nhd31tBr1uA
+00000420: 4141 4269 4c2b 5564 6159 410a 4141 5144  AABiL+UdaYA.AAQD
+00000430: 4145 6377 5251 4968 414a 6e4b 3342 566c  AEcwRQIhAJnK3BVl
+00000440: 6754 5639 4a47 6d48 4f75 2f68 4742 6b79  gTV9JGmHOu/hGBky
+00000450: 3777 6863 6b46 3432 6a56 2f75 4678 734c  7whckF42jV/uFxsL
+00000460: 3774 4756 4169 4150 4238 5836 0a6e 6962  7tGVAiAPB8X6.nib
+00000470: 6675 6373 3452 716e 5951 486b 5a77 7771  fucs4RqnYQHkZwwq
+00000480: 656e 3152 545a 316e 5a6b 5065 776d 6774  en1RTZ1nZkPewmgt
+00000490: 2f72 4441 4e42 676b 7168 6b69 4739 7730  /rDANBgkqhkiG9w0
+000004a0: 4241 5173 4641 414f 4341 5145 410a 4972  BAQsFAAOCAQEA.Ir
+000004b0: 6f55 3769 6447 537a 6357 565a 7247 3279  oU7idGSzcWVZrG2y
+000004c0: 3367 552f 4959 4236 5544 384b 384c 7734  3gU/IYB6UD8K8Lw4
+000004d0: 5845 5270 486a 5751 5762 556e 6579 486c  XERpHjWQWbUneyHl
+000004e0: 3737 6853 306b 6959 4a44 3639 3065 0a6c  77hS0kiYJD690e.l
+000004f0: 452f 3830 7637 4755 6c31 5877 702f 5654  E/80v7GUl1Xwp/VT
+00000500: 7564 7748 4a59 754e 7942 446f 6e77 346d  udwHJYuNyBDonw4m
+00000510: 3734 7237 2f6b 6132 6864 6142 546e 7042  74r7/ka2hdaBTnpB
+00000520: 4649 476d 5a62 6865 3432 4244 674d 340a  FIGmZbhe42BDgM4.
+00000530: 5a33 7762 4b43 6670 796a 4b44 3969 7a75  Z3wbKCfpyjKD9izu
+00000540: 664d 6839 4a67 7736 6f73 7277 4752 502f  fMh9Jgw6osrwGRP/
+00000550: 4737 6276 726e 4943 324a 2b4a 6641 5573  G7bvrnIC2J+JfAUs
+00000560: 3461 5772 5767 3165 4775 7941 664b 3643  4aWrWg1eGuyAfK6C
+00000570: 0a61 6145 3532 674b 4a54 7269 3031 4459  .aaE52gKJTri01DY
+00000580: 6843 6e6b 7876 3335 7652 7768 7477 4868  hCnkxv35vRwhtwHh
+00000590: 6d52 4866 6d4d 6a6d 2b65 6f32 5a31 3748  mRHfmMjm+eo2Z17H
+000005a0: 7149 526d 6f37 2b78 4d41 5647 2b48 4152  qIRmo7+xMAVG+HAR
+000005b0: 300a 4446 4a65 6f53 3939 646a 332f 7946  0.DFJeoS99dj3/yF
+000005c0: 3959 4d35 7a7a 6930 3752 7a30 2b76 566f  9YM5zzi07Rz0+vVo
+000005d0: 6f74 7364 4e68 5965 7a48 7861 3942 516c  otsdNhYezHxa9BQl
+000005e0: 435a 6272 6f52 3345 544c 6775 6559 4453  CZbroR3ETLgueYDS
+000005f0: 5a62 0a53 7164 4c79 4732 7638 4d59 634b  Zb.SqdLyG2v8MYcK
+00000600: 3551 4338 6175 5946 513d 3d0a 2d2d 2d2d  5QC8auYFQ==.----
 00000610: 2d45 4e44 2043 4552 5449 4649 4341 5445  -END CERTIFICATE
 00000620: 2d2d 2d2d 2d0a 2d2d 2d2d 2d42 4547 494e  -----.-----BEGIN
 00000630: 2043 4552 5449 4649 4341 5445 2d2d 2d2d   CERTIFICATE----
 00000640: 2d0a 4d49 4946 466a 4343 4176 3667 4177  -.MIIFFjCCAv6gAw
 00000650: 4942 4167 4952 414a 4572 4345 7250 4442  IBAgIRAJErCErPDB
 00000660: 696e 552f 6257 4c69 576e 5831 6f77 4451  inU/bWLiWnX1owDQ
 00000670: 594a 4b6f 5a49 6876 634e 4151 454c 4251  YJKoZIhvcNAQELBQ
```

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/cli.py` & `sumatra-client-1.3.1/sumatra_client/cli.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/client.py` & `sumatra-client-1.3.1/sumatra_client/client.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/config.py` & `sumatra-client-1.3.1/sumatra_client/config.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client/workspace.py` & `sumatra-client-1.3.1/sumatra_client/workspace.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/sumatra_client.egg-info/PKG-INFO` & `sumatra-client-1.3.1/sumatra_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.0rc2
+Version: 1.3.1
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.0rc2/sumatra_client.egg-info/SOURCES.txt` & `sumatra-client-1.3.1/sumatra_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc2/tests/test_config.py` & `sumatra-client-1.3.1/tests/test_config.py`

 * *Files identical despite different names*

