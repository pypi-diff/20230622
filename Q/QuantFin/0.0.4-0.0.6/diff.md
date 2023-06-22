# Comparing `tmp/QuantFin-0.0.4.tar.gz` & `tmp/QuantFin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantFin-0.0.4.tar", last modified: Thu Jun 22 12:26:32 2023, max compression
+gzip compressed data, was "QuantFin-0.0.6.tar", last modified: Thu Jun 22 12:31:05 2023, max compression
```

## Comparing `QuantFin-0.0.4.tar` & `QuantFin-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:26:32.200181 QuantFin-0.0.4/
--rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.4/LICENSE
--rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:26:32.200665 QuantFin-0.0.4/PKG-INFO
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:26:32.194839 QuantFin-0.0.4/QuantFin/
--rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.4/QuantFin/HandleError.py
--rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.4/QuantFin/MarketRisk.py
--rw-r--r--   0 stephencheung   (501) staff       (20)    13350 2023-06-19 15:09:08.000000 QuantFin-0.0.4/QuantFin/PanelRegs.py
--rwx------   0 stephencheung   (501) staff       (20)     8087 2023-06-19 15:11:23.000000 QuantFin-0.0.4/QuantFin/Portfolio.py
--rwx------   0 stephencheung   (501) staff       (20)     2835 2023-06-19 15:11:28.000000 QuantFin-0.0.4/QuantFin/Proxy.py
--rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.4/QuantFin/ReqData.py
--rwx------   0 stephencheung   (501) staff       (20)      256 2023-06-19 17:28:02.000000 QuantFin-0.0.4/QuantFin/__init__.py
--rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.4/QuantFin/_deciles.py
--rwx------   0 stephencheung   (501) staff       (20)     2303 2023-06-19 15:02:45.000000 QuantFin-0.0.4/QuantFin/_regression.py
--rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-22 11:51:05.000000 QuantFin-0.0.4/QuantFin/tool.py
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:26:32.199418 QuantFin-0.0.4/QuantFin.egg-info/
--rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:26:31.000000 QuantFin-0.0.4/QuantFin.egg-info/PKG-INFO
--rw-r--r--   0 stephencheung   (501) staff       (20)      416 2023-06-22 12:26:32.000000 QuantFin-0.0.4/QuantFin.egg-info/SOURCES.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-22 12:26:31.000000 QuantFin-0.0.4/QuantFin.egg-info/dependency_links.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-22 12:26:31.000000 QuantFin-0.0.4/QuantFin.egg-info/requires.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-22 12:26:31.000000 QuantFin-0.0.4/QuantFin.egg-info/top_level.txt
--rwx------   0 stephencheung   (501) staff       (20)     3394 2023-06-22 12:18:10.000000 QuantFin-0.0.4/README.md
--rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-22 12:26:04.000000 QuantFin-0.0.4/SETUP.py
--rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-22 12:26:32.201373 QuantFin-0.0.4/setup.cfg
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:31:05.808019 QuantFin-0.0.6/
+-rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.6/LICENSE
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:31:05.808238 QuantFin-0.0.6/PKG-INFO
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:31:05.803028 QuantFin-0.0.6/QuantFin/
+-rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.6/QuantFin/HandleError.py
+-rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.6/QuantFin/MarketRisk.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)    13350 2023-06-19 15:09:08.000000 QuantFin-0.0.6/QuantFin/PanelRegs.py
+-rwx------   0 stephencheung   (501) staff       (20)     8087 2023-06-19 15:11:23.000000 QuantFin-0.0.6/QuantFin/Portfolio.py
+-rwx------   0 stephencheung   (501) staff       (20)     2835 2023-06-19 15:11:28.000000 QuantFin-0.0.6/QuantFin/Proxy.py
+-rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.6/QuantFin/ReqData.py
+-rwx------   0 stephencheung   (501) staff       (20)      256 2023-06-19 17:28:02.000000 QuantFin-0.0.6/QuantFin/__init__.py
+-rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.6/QuantFin/_deciles.py
+-rwx------   0 stephencheung   (501) staff       (20)     2303 2023-06-19 15:02:45.000000 QuantFin-0.0.6/QuantFin/_regression.py
+-rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-22 11:51:05.000000 QuantFin-0.0.6/QuantFin/tool.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:31:05.807640 QuantFin-0.0.6/QuantFin.egg-info/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:31:05.000000 QuantFin-0.0.6/QuantFin.egg-info/PKG-INFO
+-rw-r--r--   0 stephencheung   (501) staff       (20)      416 2023-06-22 12:31:05.000000 QuantFin-0.0.6/QuantFin.egg-info/SOURCES.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-22 12:31:05.000000 QuantFin-0.0.6/QuantFin.egg-info/dependency_links.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-22 12:31:05.000000 QuantFin-0.0.6/QuantFin.egg-info/requires.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-22 12:31:05.000000 QuantFin-0.0.6/QuantFin.egg-info/top_level.txt
+-rwx------   0 stephencheung   (501) staff       (20)     3394 2023-06-22 12:18:10.000000 QuantFin-0.0.6/README.md
+-rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-22 12:29:23.000000 QuantFin-0.0.6/SETUP.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-22 12:31:05.809185 QuantFin-0.0.6/setup.cfg
```

### Comparing `QuantFin-0.0.4/LICENSE` & `QuantFin-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/PKG-INFO` & `QuantFin-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.4
+Version: 0.0.6
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
-Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
+Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/TEST.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `QuantFin-0.0.4/QuantFin/MarketRisk.py` & `QuantFin-0.0.6/QuantFin/MarketRisk.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/PanelRegs.py` & `QuantFin-0.0.6/QuantFin/PanelRegs.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/Portfolio.py` & `QuantFin-0.0.6/QuantFin/Portfolio.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/Proxy.py` & `QuantFin-0.0.6/QuantFin/Proxy.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/ReqData.py` & `QuantFin-0.0.6/QuantFin/ReqData.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/_deciles.py` & `QuantFin-0.0.6/QuantFin/_deciles.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/_regression.py` & `QuantFin-0.0.6/QuantFin/_regression.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin/tool.py` & `QuantFin-0.0.6/QuantFin/tool.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/QuantFin.egg-info/PKG-INFO` & `QuantFin-0.0.6/QuantFin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.4
+Version: 0.0.6
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
-Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
+Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/TEST.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `QuantFin-0.0.4/README.md` & `QuantFin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.4/SETUP.py` & `QuantFin-0.0.6/SETUP.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="QuantFin",
     packages=["QuantFin"],
-    version="0.0.4",
+    version="0.0.6",
     license="MIT",
     description="Library for Academic Research on Asset Pricing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stephen Zhang",
     author_email="stephen_se@outlook.com",
     url="https://github.com/yuz0101/QuantFin",
-    download_url='https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz',
+    download_url='https://github.com/yuz0101/QuantFin/archive/refs/tags/TEST.tar.gz',
     keywords=['ACADEMIC', 'EMPIRICAL', 'FIANCE', 'RESEARCH', 'QUANT', 'PORTFOLIO'],
     install_requires=["numpy", "pandas", "linearmodels", "statsmodels", "requests"],
     
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

