# Comparing `tmp/dsspkg-0.3.tar.gz` & `tmp/dsspkg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsspkg-0.3.tar", last modified: Thu Jun 22 08:01:59 2023, max compression
+gzip compressed data, was "dsspkg-0.3.1.tar", last modified: Thu Jun 22 08:26:31 2023, max compression
```

## Comparing `dsspkg-0.3.tar` & `dsspkg-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:01:59.209128 dsspkg-0.3/
--rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.3/LICENSE
--rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.3/MANIFEST.in
--rw-r--r--   0 danielwu   (501) staff       (20)      326 2023-06-22 08:01:59.208981 dsspkg-0.3/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      102 2023-06-22 08:01:58.000000 dsspkg-0.3/README.md
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:01:59.207109 dsspkg-0.3/dsspkg/
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.3/dsspkg/__init__.py
--rw-r--r--   0 danielwu   (501) staff       (20)    21660 2023-06-22 08:01:31.000000 dsspkg-0.3/dsspkg/data_scaling_split.py
--rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.3/dsspkg/dss.py
--rw-r--r--   0 danielwu   (501) staff       (20)    16942 2023-06-22 07:54:03.000000 dsspkg-0.3/dsspkg/dss_p.py
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:01:59.208767 dsspkg-0.3/dsspkg/sth/
--rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.3/dsspkg/sth/minus.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3/dsspkg/sth/minus_p.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.3/dsspkg/sth/radio.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3/dsspkg/sth/radio_p.pkl
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:01:59.207846 dsspkg-0.3/dsspkg.egg-info/
--rw-r--r--   0 danielwu   (501) staff       (20)      326 2023-06-22 08:01:59.000000 dsspkg-0.3/dsspkg.egg-info/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 08:01:59.000000 dsspkg-0.3/dsspkg.egg-info/SOURCES.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 08:01:59.000000 dsspkg-0.3/dsspkg.egg-info/dependency_links.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 08:01:59.000000 dsspkg-0.3/dsspkg.egg-info/top_level.txt
--rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 08:01:59.209163 dsspkg-0.3/setup.cfg
--rw-r--r--   0 danielwu   (501) staff       (20)      558 2023-06-22 08:01:58.000000 dsspkg-0.3/setup.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.753914 dsspkg-0.3.1/
+-rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.3.1/LICENSE
+-rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.3.1/MANIFEST.in
+-rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:26:31.753774 dsspkg-0.3.1/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      340 2023-06-22 08:26:23.000000 dsspkg-0.3.1/README.md
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.752022 dsspkg-0.3.1/dsspkg/
+-rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.3.1/dsspkg/__init__.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    21574 2023-06-22 08:19:50.000000 dsspkg-0.3.1/dsspkg/data_scaling_split.py
+-rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.3.1/dsspkg/dss.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    16942 2023-06-22 07:54:03.000000 dsspkg-0.3.1/dsspkg/dss_p.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.753573 dsspkg-0.3.1/dsspkg/sth/
+-rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.3.1/dsspkg/sth/minus.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.1/dsspkg/sth/minus_p.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.3.1/dsspkg/sth/radio.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.1/dsspkg/sth/radio_p.pkl
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.752692 dsspkg-0.3.1/dsspkg.egg-info/
+-rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/top_level.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 08:26:31.753950 dsspkg-0.3.1/setup.cfg
+-rw-r--r--   0 danielwu   (501) staff       (20)      560 2023-06-22 08:26:23.000000 dsspkg-0.3.1/setup.py
```

### Comparing `dsspkg-0.3/LICENSE` & `dsspkg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/data_scaling_split.py` & `dsspkg-0.3.1/dsspkg/data_scaling_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.jGPnwXxWXyajkEROyywWiCZnxMBBuLloclLpVqAorBpIWEzUgukjNgRwOJpQsFxM = 'UclLxyAtKosjHEKZbAOfRBqZdGyfwiifIjxYPhFeoAeTWmVhnOsAwEYJqbKBDXYc'
         self.vPMnXraRCSYMOfHEaErHLsoFctjUIfEKYKAHlJrCfywfKDHhkSCvsTaZJpsDmiqn = []
     def NBSBqLCOxPeuYRqSUjMZdMnYotroPKGUpsELAlCYZlUpWuDnGVGqRWNOBVOTtglD(self):
         self.vPMnXraRCSYMOfHEaErHLsoFctjUIfEKYKAHlJrCfywfKDHhkSCvsTaZJpsDmiqn = True
         self.jGPnwXxWXyajkEROyywWiCZnxMBBuLloclLpVqAorBpIWEzUgukjNgRwOJpQsFxM = 'dZzSnDIVJcMYWxpPAiOsonlwwPsdhwSbXLbhWdrGFBXsVWxnXhiSqKrlNufFXiVO'
 class wLmuqTrVgslfeyjrOtaYviJoRWXfNoatYjtNICttwpMWvVKifNtgQTjUygntDsoQ:
     def __init__(self):
-        self.conn = pymysql.connect(host='localhost', port=3306, user='root', passwd='wxy980828', db="perovskites")
+        # self.conn = pymysql.connect(host='localhost', port=3306, user='root', passwd='wxy980828', db="perovskites")
         basepath = os.path.abspath(__file__)
         folder = os.path.dirname(basepath)
         data_path = os.path.join(folder, 'sth/radio.pkl')
         with open(data_path, 'rb') as f:
             VhnCAlKWjRxhqgHSeKbjhhDxQnALkRNcRpCIywQFGNTzpsrVGNrymKUFcXlPqivs = 'VUXzkbNrwzqDgeOhLFyhQepSYmTXJgjteuLmmcsMirziAfbJwmvGZAMIxvBEStzP'
             ycnqEcLAKXRkyfYMDFBAGJZXVGjaDWItpwUPusILTHKqEZiRspxulXJRznKGYvLm = 'VqTRfjMJtOVEgprRLzxOaBoGIszJkXLyYTAKoZuGetRKxpScDoyiTROEsAQrkzUl'
             MLsIuCjQmTmYjYPQonluLCMOPtILeLoqJBlDmLOrACutkuPMsUyVFTNslxOrxLSB = 'qfTcURkKMurWgwxbluRHisPvObIwgwhjCbVRgHblWTVtWPyXwYvWBjgvlJjMnWaw'
@@ -144,20 +144,18 @@
         folder = os.path.dirname(basepath)
         data_path = os.path.join(folder, 'sth/minus_p.pkl')
         with open(data_path, 'rb') as f:
             ehMYTZEYCdVUeXNYxqlSJwzBafFaEMUMARlMLOVmevzdwrnVcohNUVwXiFXVMJkU = 'mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             JKEpciSvuproDpifMfVOhufoHStTLXBQMWbgsxzQuGbRNfniwLDmephkRLaEUxoS = 'nTqtCZvJCWzfwrwOOsvaVGPPyoHvofDJSGgzSkjBcwUTBWveExbZjaCZyIiuyVAW mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             self.minus_p = pickle.load(f)
     def RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo(self):
-        GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_sql(sql='select * from perovskites_processed', con=self.conn)
+        # GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_sql(sql='select * from perovskites_processed', con=self.conn)
+        GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_csv('./data/perovskites_processed')
         TmbqfbqnVquxMXmLHSnEjOWmgBSkoVjlVGDqAQUorFHyqCjhUgJlFOcbXYCdGcKR = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC['transition_energy_level']
-        TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC.drop(
-            columns=['VE_B', 'B_d-electron', 'B_p-electron', 'B_s-electron', 'B_f-electron', 'X_p-electron',
-                     'X_s-electron',
-                     'EA_X', 'transition_energy_level'])
+        TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC
         TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD['radio'] = self.radio
         zXZGFYqCfHxqTIqpBjfYXnelAAZhtnaScbdyZbebblmKAiwKOLSQSaMlslWhSOYd = 'vBOxUHzKfiSaXGzRdjbtPzMNptqJoLqrEreivQERQYlwLEaILjfaacEsuhpMRydL'
         porBadVHgNNjRnmZvnmzKVFRSjDCUtJEKCrfhxWuZtIYdqqcCewTJwkyuZJjasai = 'wmRFVbcILaJYqkEPfiYTCOjWPHvRxGBTnIqFgMKQnzViBZuySYYjHRzxYRbWmaHT'
         bnYPmRVoglyxwPDULsWtcMZWvjJeSiSqfbecTLMZOgJHJmRRNrWNFKJiTZAZkQjU = 'yUROAUmPmttVrLcRPIPGQKfAZOsbbkNhMsQxliEdlZFplwOqVOxBmkgfubJNtqMV'
         zxhuQkbPMHRKATiGRIAFiGFFaAyCwTaMfRCAXYYdVedxLMPuhJNAfGySCHLxLeqM = 'kFBHSwhSLLNPwOCgRqSUlCfWFTdBzDsBkfAPmOZJZDFviNfgsiIehGTBWjCsNawT'
         sbtSkhJkcxzXfJsTECxExaLQOJPCxsnwSEVwiNMSqIAWZLxAvqFvPPEyXMzJHECK = 'WpiqkjZRtiAkolAvkylPeCtkELVpMBrvSrlTlCbjbKwvNHiTAlQCiJbQkkUwUDnq'
         if zXZGFYqCfHxqTIqpBjfYXnelAAZhtnaScbdyZbebblmKAiwKOLSQSaMlslWhSOYd in porBadVHgNNjRnmZvnmzKVFRSjDCUtJEKCrfhxWuZtIYdqqcCewTJwkyuZJjasai:
```

### Comparing `dsspkg-0.3/dsspkg/dss.py` & `dsspkg-0.3.1/dsspkg/dss.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/dss_p.py` & `dsspkg-0.3.1/dsspkg/dss_p.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/sth/minus.pkl` & `dsspkg-0.3.1/dsspkg/sth/minus.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/sth/minus_p.pkl` & `dsspkg-0.3.1/dsspkg/sth/minus_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/sth/radio.pkl` & `dsspkg-0.3.1/dsspkg/sth/radio.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/dsspkg/sth/radio_p.pkl` & `dsspkg-0.3.1/dsspkg/sth/radio_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3/setup.py` & `dsspkg-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dsspkg",   # 包名字
-    version="0.3",
+    version="0.3.1",
     description="A data splitting and scaling package",
     long_description=long_description,  # 将说明文件设置为README.md
     long_description_content_type="text/markdown",
     packages=find_packages(),   # 默认从当前目录下搜索包
     author="DW",
     author_email="prwe98@gmail.com",
     python_requires='>=3.10',
```

