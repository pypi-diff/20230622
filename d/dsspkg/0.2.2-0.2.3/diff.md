# Comparing `tmp/dsspkg-0.2.2.tar.gz` & `tmp/dsspkg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsspkg-0.2.2.tar", last modified: Thu Jun 22 07:30:01 2023, max compression
+gzip compressed data, was "dsspkg-0.2.3.tar", last modified: Thu Jun 22 07:44:47 2023, max compression
```

## Comparing `dsspkg-0.2.2.tar` & `dsspkg-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:30:01.466871 dsspkg-0.2.2/
--rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.2.2/LICENSE
--rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.2.2/MANIFEST.in
--rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:30:01.466733 dsspkg-0.2.2/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      104 2023-06-22 07:29:57.000000 dsspkg-0.2.2/README.md
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:30:01.465578 dsspkg-0.2.2/dsspkg/
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.2.2/dsspkg/__init__.py
--rw-r--r--   0 danielwu   (501) staff       (20)    21056 2023-06-22 07:13:48.000000 dsspkg-0.2.2/dsspkg/data_scaling_split.py
--rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.2.2/dsspkg/dss.py
--rw-r--r--   0 danielwu   (501) staff       (20)    16651 2023-06-22 07:13:48.000000 dsspkg-0.2.2/dsspkg/dss_p.py
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:30:01.466560 dsspkg-0.2.2/dsspkg/sth/
--rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.2.2/dsspkg/sth/minus.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.2/dsspkg/sth/minus_p.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.2.2/dsspkg/sth/radio.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.2/dsspkg/sth/radio_p.pkl
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:30:01.466069 dsspkg-0.2.2/dsspkg.egg-info/
--rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:30:01.000000 dsspkg-0.2.2/dsspkg.egg-info/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 07:30:01.000000 dsspkg-0.2.2/dsspkg.egg-info/SOURCES.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 07:30:01.000000 dsspkg-0.2.2/dsspkg.egg-info/dependency_links.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 07:30:01.000000 dsspkg-0.2.2/dsspkg.egg-info/top_level.txt
--rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 07:30:01.466905 dsspkg-0.2.2/setup.cfg
--rw-r--r--   0 danielwu   (501) staff       (20)      530 2023-06-22 07:29:57.000000 dsspkg-0.2.2/setup.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:44:47.181134 dsspkg-0.2.3/
+-rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.2.3/LICENSE
+-rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.2.3/MANIFEST.in
+-rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:44:47.181001 dsspkg-0.2.3/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      104 2023-06-22 07:44:45.000000 dsspkg-0.2.3/README.md
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:44:47.179592 dsspkg-0.2.3/dsspkg/
+-rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.2.3/dsspkg/__init__.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    21616 2023-06-22 07:44:45.000000 dsspkg-0.2.3/dsspkg/data_scaling_split.py
+-rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.2.3/dsspkg/dss.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    16651 2023-06-22 07:13:48.000000 dsspkg-0.2.3/dsspkg/dss_p.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:44:47.180818 dsspkg-0.2.3/dsspkg/sth/
+-rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.2.3/dsspkg/sth/minus.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.3/dsspkg/sth/minus_p.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.2.3/dsspkg/sth/radio.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2.3/dsspkg/sth/radio_p.pkl
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 07:44:47.180313 dsspkg-0.2.3/dsspkg.egg-info/
+-rw-r--r--   0 danielwu   (501) staff       (20)      330 2023-06-22 07:44:47.000000 dsspkg-0.2.3/dsspkg.egg-info/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 07:44:47.000000 dsspkg-0.2.3/dsspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 07:44:47.000000 dsspkg-0.2.3/dsspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 07:44:47.000000 dsspkg-0.2.3/dsspkg.egg-info/top_level.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 07:44:47.181166 dsspkg-0.2.3/setup.cfg
+-rw-r--r--   0 danielwu   (501) staff       (20)      530 2023-06-22 07:44:45.000000 dsspkg-0.2.3/setup.py
```

### Comparing `dsspkg-0.2.2/LICENSE` & `dsspkg-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/data_scaling_split.py` & `dsspkg-0.2.3/dsspkg/data_scaling_split.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,18 @@
         self.vPMnXraRCSYMOfHEaErHLsoFctjUIfEKYKAHlJrCfywfKDHhkSCvsTaZJpsDmiqn = []
     def NBSBqLCOxPeuYRqSUjMZdMnYotroPKGUpsELAlCYZlUpWuDnGVGqRWNOBVOTtglD(self):
         self.vPMnXraRCSYMOfHEaErHLsoFctjUIfEKYKAHlJrCfywfKDHhkSCvsTaZJpsDmiqn = True
         self.jGPnwXxWXyajkEROyywWiCZnxMBBuLloclLpVqAorBpIWEzUgukjNgRwOJpQsFxM = 'dZzSnDIVJcMYWxpPAiOsonlwwPsdhwSbXLbhWdrGFBXsVWxnXhiSqKrlNufFXiVO'
 class wLmuqTrVgslfeyjrOtaYviJoRWXfNoatYjtNICttwpMWvVKifNtgQTjUygntDsoQ:
     def __init__(self):
         self.conn = pymysql.connect(host='localhost', port=3306, user='root', passwd='wxy980828', db="perovskites")
-        with open('sth/radio.pkl', 'rb') as f:
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/radio.pkl')
+        with open(data_path, 'rb') as f:
             VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs = 'VUXzkbNrwzqDgeOhLFyhQepSYmTXJgjteuLmmcsMirziAfbJwmvGZAMIxvBEStzP'
             ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm = 'VqTRfjMJtOVEgprRLzxOaBoGIszJkXLyYTAKoZuGetRKxpScDoyiTROEsAQrkzUl'
             MLsIuCjQmTmYjYPQonluLCMOPtILeLoqJBlDmLOrACutkuPMsUyVFTNslxOrxLSB = 'qfTcURkKMurWgwxbluRHisPvObIwgwhjCbVRgHblWTVtWPyXwYvWBjgvlJjMnWaw'
             ayhDtGdqCwnIwSKAkChffLayEhjqYUEdfkJtlxoMbKuiFVgBOYJGdYCTdRinYHMZ = 'eMQNtWfzNnukJxywlnaRUKxFAMngaQSBiuoQOwmTyOFCZmnjGwlPMUmmzYZWGoFc'
             if ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm == VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs:
                 for VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs in ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm:
                     if ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm == ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm:
@@ -83,26 +86,32 @@
                             elif MLsIuCjQmTmYjYPQonluLCMOPtILeLoqJBlDmLOrACutkuPMsUyVFTNslxOrxLSB == ayhDtGdqCwnIwSKAkChffLayEhjqYUEdfkJtlxoMbKuiFVgBOYJGdYCTdRinYHMZ:
                                 ayhDtGdqCwnIwSKAkChffLayEhjqYUEdfkJtlxoMbKuiFVgBOYJGdYCTdRinYHMZ = VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs
                             else:
                                 VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs = ayhDtGdqCwnIwSKAkChffLayEhjqYUEdfkJtlxoMbKuiFVgBOYJGdYCTdRinYHMZ
             else:
                 VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs = ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm
             self.radio = pickle.load(f)
-        with open('sth/minus.pkl', 'rb') as f:
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/minus.pkl')
+        with open(data_path, 'rb') as f:
             FKcQIikQfKsDoCMprGaRziivYFzqnRnqTbQZpWReJLDjuksTuRupbBPCIGRfqGGC = 'qYfJyXLEqqXIgtixpLYyaQFXcGKTNTyHZuEVcINoknXtshRzSkIbqBbjmrQVCWAD'
             mqAazlzGkYyDzkKZBJyDoFmflBrqfgcUEyGPKlYtJqmmfdgHNqpVNaLcNbNJrHJP = 'pmepQSOzZXMUGErMPZfSypfRctKGhedVoXRlBzzIdUmDPOFCnxGerPlAPGqaqqhg'
             NEfwRdLvEqVGudlGsrjlHifYTBWbUmLIocGAlAovCYswSINtaQIxhXqYzInLsuPY = 'ZUoGysPtBoRldgQFJnFLhOQDlVANEdxoyhGNsYtfrfUzVQDyUGwAcLfRTaBWlGqq'
             if FKcQIikQfKsDoCMprGaRziivYFzqnRnqTbQZpWReJLDjuksTuRupbBPCIGRfqGGC == mqAazlzGkYyDzkKZBJyDoFmflBrqfgcUEyGPKlYtJqmmfdgHNqpVNaLcNbNJrHJP:
                 NEfwRdLvEqVGudlGsrjlHifYTBWbUmLIocGAlAovCYswSINtaQIxhXqYzInLsuPY = 'ZUoGysPtBoRldgQFJnFLhOQDlVANEdxoyhGNsYtfrfUzVQDyUGwAcLfRTaBWlGqq'
                 NEfwRdLvEqVGudlGsrjlHifYTBWbUmLIocGAlAovCYswSINtaQIxhXqYzInLsuPY = FKcQIikQfKsDoCMprGaRziivYFzqnRnqTbQZpWReJLDjuksTuRupbBPCIGRfqGGC
             else:
                 NEfwRdLvEqVGudlGsrjlHifYTBWbUmLIocGAlAovCYswSINtaQIxhXqYzInLsuPY = 'ZUoGysPtBoRldgQFJnFLhOQDlVANEdxoyhGNsYtfrfUzVQDyUGwAcLfRTaBWlGqq'
                 NEfwRdLvEqVGudlGsrjlHifYTBWbUmLIocGAlAovCYswSINtaQIxhXqYzInLsuPY = 'qYfJyXLEqqXIgtixpLYyaQFXcGKTNTyHZuEVcINoknXtshRzSkIbqBbjmrQVCWAD'
             self.minus = pickle.load(f)
-        with open('sth/radio_p.pkl', 'rb') as f:
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/radio_p.pkl')
+        with open(data_path, 'rb') as f:
             NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa = 'yKpGEliZjVnJGVuCcCBnIuuNYmhWPBRyKBxyHPSsJGzIvniwHmFTaOoVFjsBNnXE'
             bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ = 'auGeQeHKCvYKivsQnLglFjUjtvSmsMEmucgNhyQEWQPkNwXBPpnweqWdHaLLrvfO'
             jYYcoQHyYBIbbLAoiLuXKgxxBosgKMHRecVRKSNcWFfcDRcpkdXMggRoxzxRYeRb = 'zGjZJpEscCFuAnilQBWwVDLoAkVvSeRNpempLFRfyIApNJlyWMLKIxxsVRHBNmlU'
             wamaYyKCuccqfSIkQOuTsXNNMVOLFphGIyDyShOSKNwyAazGzswxOIzYvTZwUZjo = 'JgpBcqIekIEUiWssJPqNeVpwJYaYCPTZvweONYfJRiJSfuOiWRTEWMBXNOBwwRSg'
             if bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ == NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa:
                 for NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa in bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ:
                     if bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ == bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ:
@@ -125,15 +134,18 @@
                             elif jYYcoQHyYBIbbLAoiLuXKgxxBosgKMHRecVRKSNcWFfcDRcpkdXMggRoxzxRYeRb == wamaYyKCuccqfSIkQOuTsXNNMVOLFphGIyDyShOSKNwyAazGzswxOIzYvTZwUZjo:
                                 wamaYyKCuccqfSIkQOuTsXNNMVOLFphGIyDyShOSKNwyAazGzswxOIzYvTZwUZjo = NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa
                             else:
                                 NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa = wamaYyKCuccqfSIkQOuTsXNNMVOLFphGIyDyShOSKNwyAazGzswxOIzYvTZwUZjo
             else:
                 NmdeqMREyVgHOuTsVyhwWfwTWCOqKXFfkeMNgmDzOmcUpxJxGqicanOcSZnzZxSa = bXbCMuqtMcbvzAGhJbMWOPgonHDRJGsdvXYCtrjZBPxzzRlJbuiNbLxvUWoXeUgJ
             self.radio_p = pickle.load(f)
-        with open('sth/minus_p.pkl', 'rb') as f:
+        basepath = os.path.abspath(__file__)
+        folder = os.path.dirname(basepath)
+        data_path = os.path.join(folder, 'sth/minus_p.pkl')
+        with open(data_path, 'rb') as f:
             ehMYTZEYCdVUeXNYxqlSJwzBafFaEMUMARlMLOVmevzdwrnVcohNUVwXiFXVMJkU = 'mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             JKEpciSvuproDpifMfVOhufoHStTLXBQMWbgsxzQuGbRNfniwLDmephkRLaEUxoS = 'nTqtCZvJCWzfwrwOOsvaVGPPyoHvofDJSGgzSkjBcwUTBWveExbZjaCZyIiuyVAW mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             self.minus_p = pickle.load(f)
     def RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo(self):
         GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_sql(sql='select * from perovskites_processed', con=self.conn)
         TmbqfbqnVquxMXmLHSnEjOWmgBSkoVjlVGDqAQUorFHyqCjhUgJlFOcbXYCdGcKR = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC['transition_energy_level']
         TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC.drop(
```

### Comparing `dsspkg-0.2.2/dsspkg/dss.py` & `dsspkg-0.2.3/dsspkg/dss.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/dss_p.py` & `dsspkg-0.2.3/dsspkg/dss_p.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/sth/minus.pkl` & `dsspkg-0.2.3/dsspkg/sth/minus.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/sth/minus_p.pkl` & `dsspkg-0.2.3/dsspkg/sth/minus_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/sth/radio.pkl` & `dsspkg-0.2.3/dsspkg/sth/radio.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/dsspkg/sth/radio_p.pkl` & `dsspkg-0.2.3/dsspkg/sth/radio_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.2.2/setup.py` & `dsspkg-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dsspkg",   # 包名字
-    version="0.2.2",
+    version="0.2.3",
     description="A data splitting and scaling package",
     long_description=long_description,  # 将说明文件设置为README.md
     long_description_content_type="text/markdown",
     packages=find_packages(),   # 默认从当前目录下搜索包
     author="DW",
     author_email="prwe98@gmail.com",
     python_requires='>=3.10',
```

