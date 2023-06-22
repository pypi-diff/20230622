# Comparing `tmp/dsspkg-0.2.4.tar.gz` & `tmp/dsspkg-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsspkg-0.2.4.tar", last modified: Thu Jun 22 07:50:32 2023, max compression
+gzip compressed data, was "dsspkg-0.2.5.tar", last modified: Thu Jun 22 07:54:34 2023, max compression
```

## Comparing `dsspkg-0.2.4.tar` & `dsspkg-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:50:32.880769 dsspkg-0.2.4/
--rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.2.4/LICENSE
--rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.2.4/MANIFEST.in
--rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:50:32.880517 dsspkg-0.2.4/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      104 2023-06-22 07:50:29.000000 dsspkg-0.2.4/README.md
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:50:32.878891 dsspkg-0.2.4/dsspkg/
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.2.4/dsspkg/__init__.py
--rw-r--r--   0 danielwu   (501) staff       (20)    21616 2023-06-22 07:44:45.000000 dsspkg-0.2.4/dsspkg/data_scaling_split.py
--rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.2.4/dsspkg/dss.py
--rw-r--r--   0 danielwu   (501) staff       (20)    16651 2023-06-22 07:13:48.000000 dsspkg-0.2.4/dsspkg/dss_p.py
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:50:32.880321 dsspkg-0.2.4/dsspkg/sth/
--rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.2.4/dsspkg/sth/minus.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.4/dsspkg/sth/minus_p.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.2.4/dsspkg/sth/radio.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.4/dsspkg/sth/radio_p.pkl
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:50:32.879351 dsspkg-0.2.4/dsspkg.egg-info/
--rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:50:32.000000 dsspkg-0.2.4/dsspkg.egg-info/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 07:50:32.000000 dsspkg-0.2.4/dsspkg.egg-info/SOURCES.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 07:50:32.000000 dsspkg-0.2.4/dsspkg.egg-info/dependency_links.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 07:50:32.000000 dsspkg-0.2.4/dsspkg.egg-info/top_level.txt
--rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 07:50:32.880840 dsspkg-0.2.4/setup.cfg
--rw-r--r--   0 danielwu   (501) staff       (20)      560 2023-06-22 07:50:29.000000 dsspkg-0.2.4/setup.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:54:34.988726 dsspkg-0.2.5/
+-rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.2.5/LICENSE
+-rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.2.5/MANIFEST.in
+-rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:54:34.988537 dsspkg-0.2.5/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      104 2023-06-22 07:54:14.000000 dsspkg-0.2.5/README.md
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:54:34.987366 dsspkg-0.2.5/dsspkg/
+-rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.2.5/dsspkg/__init__.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    21616 2023-06-22 07:44:45.000000 dsspkg-0.2.5/dsspkg/data_scaling_split.py
+-rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.2.5/dsspkg/dss.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    16942 2023-06-22 07:54:03.000000 dsspkg-0.2.5/dsspkg/dss_p.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:54:34.988321 dsspkg-0.2.5/dsspkg/sth/
+-rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.2.5/dsspkg/sth/minus.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.5/dsspkg/sth/minus_p.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.2.5/dsspkg/sth/radio.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.5/dsspkg/sth/radio_p.pkl
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:54:34.987859 dsspkg-0.2.5/dsspkg.egg-info/
+-rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:54:34.000000 dsspkg-0.2.5/dsspkg.egg-info/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 07:54:34.000000 dsspkg-0.2.5/dsspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 07:54:34.000000 dsspkg-0.2.5/dsspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 07:54:34.000000 dsspkg-0.2.5/dsspkg.egg-info/top_level.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 07:54:34.988775 dsspkg-0.2.5/setup.cfg
+-rw-r--r--   0 danielwu   (501) staff       (20)      560 2023-06-22 07:54:14.000000 dsspkg-0.2.5/setup.py
```

### Comparing `dsspkg-0.2.4/LICENSE` & `dsspkg-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/data_scaling_split.py` & `dsspkg-0.2.5/dsspkg/data_scaling_split.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/dss.py` & `dsspkg-0.2.5/dsspkg/dss.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/dss_p.py` & `dsspkg-0.2.5/dsspkg/dss_p.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pickle
+import os
 BhYmCCIUbpbUizBLuMmqVfNjDRpvIGkSayekLWJbnPAKGQGuYkgRjvcRgvJLkANf = 'rqOHNAMZjoQLTZwvrgPTvqXxSkcVRzDjeKjhpByKrfkCHzDslCPPMnGdiAhygQhI'
 RSWLnoIsuZaXfmGgEPnaFdzivcEvkdFaOcoNggtxqQahIxltsskHSNrEwCoHnLvg = 'aEtTVceCeYWTTpvNRxMkwCGswehlIZnxCQRJCVWifQkyNxhMbamTbSGqulhLBDJn'
 latndTTYClYqBOuKqUIUVmikStPPBLtQmgDOIQgpAYHREdQZFucESCsqGFBYIYLD = 'xcSkmbEsEggJmQkKAHlMWXZAeWPElaLNtNuTqWuLyxMIZtQXtXpfXdAboNTlQwIq'
 UPkQFvjFcbLoYdoYmWnIKcSBGUybQrhnsOfreYLDyEgxAvfvpxuIryebuudgaUxV = 'dXuKBBaWWxTBFBHcCpEdZqjRsMXsOwBGrfgstxIZuJjHOolPSPKetgudSGRtkbar'
 BWsVsdrTrFpPfGmaNCzyLEukHrlLzLvFZzFbHwmvbaXGavwjyuqHavbahnjddlqx = 'kiEhexALXIgPvNYvEOngyGOIQdbQBXHpMvuMkpWLHxHrWxEcEumiudqBNFMVMIEQ'
 SeNYuMNTMWMSBpgtVjEsDMMiryblZAAFAjJjiKukCGKxigpqmHIVcsFHzLBOvypC = 'FAvPbdsdSBiFmMVQGtTwfeDgwDLqjSEBuYzHBSyauWwLbXjLNzNNhDBPlNhbxEBM'
 if latndTTYClYqBOuKqUIUVmikStPPBLtQmgDOIQgpAYHREdQZFucESCsqGFBYIYLD == UPkQFvjFcbLoYdoYmWnIKcSBGUybQrhnsOfreYLDyEgxAvfvpxuIryebuudgaUxV:
@@ -38,15 +39,19 @@
 class nxvcNfbRPmURCsTmliTcPqUQXJgtouLhtBZqKYcxKXARgeQlLgfgoOWiOQQbvEpE:
     def __init__(self):
         pass
         ekYLZiouqidpdcOSqPeReRjrvuSexINgFuySZOBBrCLJBTZfyoSmmeOiUrMEFcko = 'elUILWNnbpZesTMuecejgoLpnMkzEoPlnfdHfzFFjJzoYvJxmLCIgDsrGzASXbLc'
     def aFcbVogSJsJSyduTNWMqDpEwRWTEoNYvNPgaAWPSfjMHmLHgiVWHPRVucToSMtGH(self):
         ljIVReQvmCyXxoElAjTByjrQIoavehXPfuIsIlMpjzvQBLjJiNLkEzGsUZIJUkiP = pd.read_csv('./data/unkonwn.csv')
         FmewbOVncCxYmBtIzPkOoIoSzOGEULXveuqSrJgsaTvrwwWLCXbsmYbZkFftaWjg = ljIVReQvmCyXxoElAjTByjrQIoavehXPfuIsIlMpjzvQBLjJiNLkEzGsUZIJUkiP.drop(columns=['A-site', 'B-site', 'X-site', 'defect', 'element_first', 'element_second'])
-        with open('sth/radio_p.pkl', 'rb') as f:
+
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/radio_p.pkl')
+        with open(data_path, 'rb') as f:
             FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku = 'FxVAzwfSYJgUhUHpqsVQqAqIVigkkoimyNzeCilbuTORuVZIQJPlniThczYfHLxZ'
             fyHsgOdbymWbROqfGCdKkvbftrsFMpTNlnjzIGduhBnhaNOAYbWUNeWnhkPHYFce = 'gQtYhHNSyYlgqSGxoxdjdTvVTHglTVPYEBblzwkLBcMuSgdsAsxHvyOgqKPDFcdN'
             sOYGSVgchciEYXLkNononsQpivkcZWzBQcqxXPwsozaPHFDijATRtdcTxoutTPcN = 'YokrfKTntctpRLaJTvQRmIfMWsndlpbqqwofhdwwAxJHasFqCnEkftBudHUeRtwW'
             yRmLBPezRBGRFBtJphAQLwdlkxZVlhmadQtLTgfFuzgaSFbsjyCcwOPwAcAsPyMF = 'GrAktvihKsecvLkQaSezoGnCaRnqOuSeDuuOppUuINEiFezDUfuBUgAAsYRNlBIo'
             RJyNeuUrPJwoYAWgcPhLLOUIxQSjKMwFmlmBMFARfRUPZBzSyEFPfEjgcVpbswah = 'sTVlMbtVInsgyhWGZIuUqQnbyeIVXMRLTcNduzwwRDpFhzXTeruOxExZZONFFpVe'
             YmKnGieVDxBeKHdhsgrlsoHOkxlGFpzTEKDAIUZaqQGhhriROOOmIqQRYupTkMSX = 'HkKPwYGQwZNsFCBaBMgAKNPdxOxOLDddhnEoJAdOGtpFjuJLwIdaHbywLYBLjpvj'
             if FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku != yRmLBPezRBGRFBtJphAQLwdlkxZVlhmadQtLTgfFuzgaSFbsjyCcwOPwAcAsPyMF:
@@ -62,15 +67,18 @@
                 if sOYGSVgchciEYXLkNononsQpivkcZWzBQcqxXPwsozaPHFDijATRtdcTxoutTPcN == FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku:
                     for YmKnGieVDxBeKHdhsgrlsoHOkxlGFpzTEKDAIUZaqQGhhriROOOmIqQRYupTkMSX in FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku:
                         if YmKnGieVDxBeKHdhsgrlsoHOkxlGFpzTEKDAIUZaqQGhhriROOOmIqQRYupTkMSX == sOYGSVgchciEYXLkNononsQpivkcZWzBQcqxXPwsozaPHFDijATRtdcTxoutTPcN:
                             sOYGSVgchciEYXLkNononsQpivkcZWzBQcqxXPwsozaPHFDijATRtdcTxoutTPcN = FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku
                         else:
                             sOYGSVgchciEYXLkNononsQpivkcZWzBQcqxXPwsozaPHFDijATRtdcTxoutTPcN = RJyNeuUrPJwoYAWgcPhLLOUIxQSjKMwFmlmBMFARfRUPZBzSyEFPfEjgcVpbswah
             CeeIVbsiHzrSzHtftHukyBHHMnFjdlmqDgklzOTztrIlXGrcNfbdNSJKvlfDtOdf = pickle.load(f)
-        with open('sth/minus_p.pkl', 'rb') as f:
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/minus_p.pkl')
+        with open(data_path, 'rb') as f:
             lGXYOABaNRMGswZuaayIHeKkoyTuQNqprMPaPZFWqHBSfeTDoqLlREMQYFHlIBXX = 'FFrFMfKksEFhRQLHgHfYOOhEWjDQFujyZyQdHwZYDZLUoXycdyolEJDhiGOVFgJT'
             paZKsscAoSpBiOOVHYouWaiuLQMjnCCCjKfXcZBnGLmrhDPRrSdPaDeuVFoEKbXl = 'wNMZBEFeEsQqMAaCCfPuJeldQSAVulbiYzrziXZvWEmXoxSUbnPVxXttELOupZnk'
             cHLPWLcklOXZlwIRoQJfERWbcsovjVoZtLDUdYqZKhETfnKiLmJjQLOzjcsjRYep = 'XpOivwPVwkSTWURIBOrMrxajYchdVHPUyJzAFCnVkXUcVptoQrbgUJdtOVTQMNpR'
             zlbrcAzsNyRTwHkUCuwgZRfFGiHArSTtdrpwlHxhNooUolXPgQzdFCmSbAvUDlgx = 'FXfXSTYyhjuPbPNWGkkCXjAwpjPqknhtAnqbLvNWDTwuXrXDArYQksUSSpJVAtyb'
             NELVbqnddGpQSrGlgXsOGTRuFTMVBQHDUsRIynSkcwYmxqfgRoWfMjcsfSkhamWU = 'DCFEguplBCaiDvOZnQwRzKUZEQauDtRyqTNaRfYQjczrAVhjIwzMLJpsOdlWuBEG'
             zQCOOmvXjOiKgRkGQknoDCvZRdTcHBuCyBwahSUPjVxQAWKgzEWoKnjSXwYjRYCf = 'fbEYKeWNDsiKHPqHDIfkZzGnroRDZmdqAEfwRTFrFadkBEyOdYJchnafUQgZnmVf'
             if lGXYOABaNRMGswZuaayIHeKkoyTuQNqprMPaPZFWqHBSfeTDoqLlREMQYFHlIBXX != zlbrcAzsNyRTwHkUCuwgZRfFGiHArSTtdrpwlHxhNooUolXPgQzdFCmSbAvUDlgx:
```

### Comparing `dsspkg-0.2.4/dsspkg/sth/minus.pkl` & `dsspkg-0.2.5/dsspkg/sth/minus.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/sth/minus_p.pkl` & `dsspkg-0.2.5/dsspkg/sth/minus_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/sth/radio.pkl` & `dsspkg-0.2.5/dsspkg/sth/radio.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/dsspkg/sth/radio_p.pkl` & `dsspkg-0.2.5/dsspkg/sth/radio_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.4/setup.py` & `dsspkg-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dsspkg",   # 包名字
-    version="0.2.4",
+    version="0.2.5",
     description="A data splitting and scaling package",
     long_description=long_description,  # 将说明文件设置为README.md
     long_description_content_type="text/markdown",
     packages=find_packages(),   # 默认从当前目录下搜索包
     author="DW",
     author_email="prwe98@gmail.com",
     python_requires='>=3.10',
```

