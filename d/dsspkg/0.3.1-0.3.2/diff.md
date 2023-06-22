# Comparing `tmp/dsspkg-0.3.1.tar.gz` & `tmp/dsspkg-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsspkg-0.3.1.tar", last modified: Thu Jun 22 08:26:31 2023, max compression
+gzip compressed data, was "dsspkg-0.3.2.tar", last modified: Thu Jun 22 08:55:16 2023, max compression
```

## Comparing `dsspkg-0.3.1.tar` & `dsspkg-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.753914 dsspkg-0.3.1/
--rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.3.1/LICENSE
--rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.3.1/MANIFEST.in
--rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:26:31.753774 dsspkg-0.3.1/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      340 2023-06-22 08:26:23.000000 dsspkg-0.3.1/README.md
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.752022 dsspkg-0.3.1/dsspkg/
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.3.1/dsspkg/__init__.py
--rw-r--r--   0 danielwu   (501) staff       (20)    21574 2023-06-22 08:19:50.000000 dsspkg-0.3.1/dsspkg/data_scaling_split.py
--rw-r--r--   0 danielwu   (501) staff       (20)      583 2023-06-22 07:29:20.000000 dsspkg-0.3.1/dsspkg/dss.py
--rw-r--r--   0 danielwu   (501) staff       (20)    16942 2023-06-22 07:54:03.000000 dsspkg-0.3.1/dsspkg/dss_p.py
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.753573 dsspkg-0.3.1/dsspkg/sth/
--rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.3.1/dsspkg/sth/minus.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.1/dsspkg/sth/minus_p.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.3.1/dsspkg/sth/radio.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.1/dsspkg/sth/radio_p.pkl
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:26:31.752692 dsspkg-0.3.1/dsspkg.egg-info/
--rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/SOURCES.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/dependency_links.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 08:26:31.000000 dsspkg-0.3.1/dsspkg.egg-info/top_level.txt
--rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 08:26:31.753950 dsspkg-0.3.1/setup.cfg
--rw-r--r--   0 danielwu   (501) staff       (20)      560 2023-06-22 08:26:23.000000 dsspkg-0.3.1/setup.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:55:16.450171 dsspkg-0.3.2/
+-rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.3.2/LICENSE
+-rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.3.2/MANIFEST.in
+-rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:55:16.450021 dsspkg-0.3.2/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      340 2023-06-22 08:55:12.000000 dsspkg-0.3.2/README.md
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:55:16.448285 dsspkg-0.3.2/dsspkg/
+-rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.3.2/dsspkg/__init__.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    21564 2023-06-22 08:55:12.000000 dsspkg-0.3.2/dsspkg/data_scaling_split.py
+-rw-r--r--   0 danielwu   (501) staff       (20)      741 2023-06-22 08:55:12.000000 dsspkg-0.3.2/dsspkg/dss.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    16942 2023-06-22 08:55:12.000000 dsspkg-0.3.2/dsspkg/dss_p.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:55:16.449813 dsspkg-0.3.2/dsspkg/sth/
+-rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.3.2/dsspkg/sth/minus.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.2/dsspkg/sth/minus_p.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.3.2/dsspkg/sth/radio.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.3.2/dsspkg/sth/radio_p.pkl
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-22 08:55:16.448794 dsspkg-0.3.2/dsspkg.egg-info/
+-rw-r--r--   0 danielwu   (501) staff       (20)      566 2023-06-22 08:55:16.000000 dsspkg-0.3.2/dsspkg.egg-info/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-22 08:55:16.000000 dsspkg-0.3.2/dsspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-22 08:55:16.000000 dsspkg-0.3.2/dsspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-22 08:55:16.000000 dsspkg-0.3.2/dsspkg.egg-info/top_level.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-22 08:55:16.450209 dsspkg-0.3.2/setup.cfg
+-rw-r--r--   0 danielwu   (501) staff       (20)      560 2023-06-22 08:55:12.000000 dsspkg-0.3.2/setup.py
```

### Comparing `dsspkg-0.3.1/LICENSE` & `dsspkg-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3.1/PKG-INFO` & `dsspkg-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dsspkg
-Version: 0.3.1
+Version: 0.3.2
 Summary: A data splitting and scaling package
 Author: DW
 Author-email: prwe98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A python package for data processing.The data is sliced and normalized based on sklearn
 
 Please put the data into a folder called "data" (if it does not exist, create a new one), the program automatically completes the normalization and slicing.
 
 You can adjust the program file parameters yourself based on your input data
 
-version：0.3.1
+version：0.3.2
```

### Comparing `dsspkg-0.3.1/dsspkg/data_scaling_split.py` & `dsspkg-0.3.2/dsspkg/data_scaling_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,17 @@
         basepath = os.path.abspath(__file__)
         folder = os.path.dirname(basepath)
         data_path = os.path.join(folder, 'sth/minus_p.pkl')
         with open(data_path, 'rb') as f:
             ehMYTZEYCdVUeXNYxqlSJwzBafFaEMUMARlMLOVmevzdwrnVcohNUVwXiFXVMJkU = 'mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             JKEpciSvuproDpifMfVOhufoHStTLXBQMWbgsxzQuGbRNfniwLDmephkRLaEUxoS = 'nTqtCZvJCWzfwrwOOsvaVGPPyoHvofDJSGgzSkjBcwUTBWveExbZjaCZyIiuyVAW mURUjcEhfgzdhnwVNWWzSEyvDDBJbemjEanmuIneiazyMOlSWmrfISCSrYSeyCdw'
             self.minus_p = pickle.load(f)
-    def RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo(self):
+    def RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo(self, file_path):
         # GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_sql(sql='select * from perovskites_processed', con=self.conn)
-        GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_csv('./data/perovskites_processed')
+        GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC = pd.read_csv(file_path)
         TmbqfbqnVquxMXmLHSnEjOWmgBSkoVjlVGDqAQUorFHyqCjhUgJlFOcbXYCdGcKR = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC['transition_energy_level']
         TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD = GlhSfuvOjyzUoGZuOCqunESiMBcMgwcTquRPMEzDYnzxXWldNASKLTMQPclwODFC
         TzUJGnxUiSGPIQkRTbnRpnUoexJLmKhpAeVZMrWQouPOuNXCNKczPyQtJtjUfrhD['radio'] = self.radio
         zXZGFYqCfHxqTIqpBjfYXnelAAZhtnaScbdyZbebblmKAiwKOLSQSaMlslWhSOYd = 'vBOxUHzKfiSaXGzRdjbtPzMNptqJoLqrEreivQERQYlwLEaILjfaacEsuhpMRydL'
         porBadVHgNNjRnmZvnmzKVFRSjDCUtJEKCrfhxWuZtIYdqqcCewTJwkyuZJjasai = 'wmRFVbcILaJYqkEPfiYTCOjWPHvRxGBTnIqFgMKQnzViBZuySYYjHRzxYRbWmaHT'
         bnYPmRVoglyxwPDULsWtcMZWvjJeSiSqfbecTLMZOgJHJmRRNrWNFKJiTZAZkQjU = 'yUROAUmPmttVrLcRPIPGQKfAZOsbbkNhMsQxliEdlZFplwOqVOxBmkgfubJNtqMV'
         zxhuQkbPMHRKATiGRIAFiGFFaAyCwTaMfRCAXYYdVedxLMPuhJNAfGySCHLxLeqM = 'kFBHSwhSLLNPwOCgRqSUlCfWFTdBzDsBkfAPmOZJZDFviNfgsiIehGTBWjCsNawT'
```

### Comparing `dsspkg-0.3.1/dsspkg/dss.py` & `dsspkg-0.3.2/dsspkg/dss.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import dsspkg.data_scaling_split
 from dsspkg.data_scaling_split import wLmuqTrVgslfeyjrOtaYviJoRWXfNoatYjtNICttwpMWvVKifNtgQTjUygntDsoQ
 from dsspkg.dss_p import nxvcNfbRPmURCsTmliTcPqUQXJgtouLhtBZqKYcxKXARgeQlLgfgoOWiOQQbvEpE
 
 dss = dsspkg.data_scaling_split.wLmuqTrVgslfeyjrOtaYviJoRWXfNoatYjtNICttwpMWvVKifNtgQTjUygntDsoQ()
-
-X_train, X_test, y_train, y_test = dss.RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo()
+def data_split(file_path):
+    X_train, X_test, y_train, y_test = dss.RBTPVqAIIclqYjsDJGvHTIuOYkDQIChIXTICtWRKZQgoLrJRCXsmluOKJksnAGZo(file_path=file_path)
+    return X_train, X_test, y_train, y_test
 
 dssp = nxvcNfbRPmURCsTmliTcPqUQXJgtouLhtBZqKYcxKXARgeQlLgfgoOWiOQQbvEpE()
-X = dssp.aFcbVogSJsJSyduTNWMqDpEwRWTEoNYvNPgaAWPSfjMHmLHgiVWHPRVucToSMtGH()
+def data_split_p(file_path):
+    X = dssp.aFcbVogSJsJSyduTNWMqDpEwRWTEoNYvNPgaAWPSfjMHmLHgiVWHPRVucToSMtGH(data_path=file_path)
+    return X
```

### Comparing `dsspkg-0.3.1/dsspkg/dss_p.py` & `dsspkg-0.3.2/dsspkg/dss_p.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
                 continue
             else:
                 hCBSKBbDFfAmfFacRtvibsxTcqEgCxxhaqfOOSTMIWwPvdDYHBdUyAgfVSyGDJRu = False
 class nxvcNfbRPmURCsTmliTcPqUQXJgtouLhtBZqKYcxKXARgeQlLgfgoOWiOQQbvEpE:
     def __init__(self):
         pass
         ekYLZiouqidpdcOSqPeReRjrvuSexINgFuySZOBBrCLJBTZfyoSmmeOiUrMEFcko = 'elUILWNnbpZesTMuecejgoLpnMkzEoPlnfdHfzFFjJzoYvJxmLCIgDsrGzASXbLc'
-    def aFcbVogSJsJSyduTNWMqDpEwRWTEoNYvNPgaAWPSfjMHmLHgiVWHPRVucToSMtGH(self):
-        ljIVReQvmCyXxoElAjTByjrQIoavehXPfuIsIlMpjzvQBLjJiNLkEzGsUZIJUkiP = pd.read_csv('./data/unkonwn.csv')
+    def aFcbVogSJsJSyduTNWMqDpEwRWTEoNYvNPgaAWPSfjMHmLHgiVWHPRVucToSMtGH(self, data_path):
+        ljIVReQvmCyXxoElAjTByjrQIoavehXPfuIsIlMpjzvQBLjJiNLkEzGsUZIJUkiP = pd.read_csv(data_path)
         FmewbOVncCxYmBtIzPkOoIoSzOGEULXveuqSrJgsaTvrwwWLCXbsmYbZkFftaWjg = ljIVReQvmCyXxoElAjTByjrQIoavehXPfuIsIlMpjzvQBLjJiNLkEzGsUZIJUkiP.drop(columns=['A-site', 'B-site', 'X-site', 'defect', 'element_first', 'element_second'])
 
         basepath = os.path.abspath(__file__)
         folder = os.path.dirname(basepath)
         data_path = os.path.join(folder, 'sth/radio_p.pkl')
         with open(data_path, 'rb') as f:
             FCxXHnRgBJtoumpDAyHzdJdjzpxCmORSkhDWFRzbsfvleOEiECKgjdeishxApIku = 'FxVAzwfSYJgUhUHpqsVQqAqIVigkkoimyNzeCilbuTORuVZIQJPlniThczYfHLxZ'
```

### Comparing `dsspkg-0.3.1/dsspkg/sth/minus.pkl` & `dsspkg-0.3.2/dsspkg/sth/minus.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3.1/dsspkg/sth/minus_p.pkl` & `dsspkg-0.3.2/dsspkg/sth/minus_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3.1/dsspkg/sth/radio.pkl` & `dsspkg-0.3.2/dsspkg/sth/radio.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3.1/dsspkg/sth/radio_p.pkl` & `dsspkg-0.3.2/dsspkg/sth/radio_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.3.1/dsspkg.egg-info/PKG-INFO` & `dsspkg-0.3.2/dsspkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dsspkg
-Version: 0.3.1
+Version: 0.3.2
 Summary: A data splitting and scaling package
 Author: DW
 Author-email: prwe98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A python package for data processing.The data is sliced and normalized based on sklearn
 
 Please put the data into a folder called "data" (if it does not exist, create a new one), the program automatically completes the normalization and slicing.
 
 You can adjust the program file parameters yourself based on your input data
 
-version：0.3.1
+version：0.3.2
```

### Comparing `dsspkg-0.3.1/setup.py` & `dsspkg-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dsspkg",   # 包名字
-    version="0.3.1",
+    version="0.3.2",
     description="A data splitting and scaling package",
     long_description=long_description,  # 将说明文件设置为README.md
     long_description_content_type="text/markdown",
     packages=find_packages(),   # 默认从当前目录下搜索包
     author="DW",
     author_email="prwe98@gmail.com",
     python_requires='>=3.10',
```

