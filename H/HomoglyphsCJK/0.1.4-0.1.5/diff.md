# Comparing `tmp/HomoglyphsCJK-0.1.4.tar.gz` & `tmp/HomoglyphsCJK-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.1.4.tar", last modified: Tue Jun  6 05:44:35 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.1.5.tar", last modified: Thu Jun 22 05:35:00 2023, max compression
```

## Comparing `HomoglyphsCJK-0.1.4.tar` & `HomoglyphsCJK-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.984540 HomoglyphsCJK-0.1.4/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.982028 HomoglyphsCJK-0.1.4/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)      122 2023-05-27 07:13:42.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)    10932 2023-05-27 06:58:42.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.983818 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-06-06 05:44:35.984227 HomoglyphsCJK-0.1.4/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3545 2023-05-27 07:08:05.000000 HomoglyphsCJK-0.1.4/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-06-06 05:44:35.984635 HomoglyphsCJK-0.1.4/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      967 2023-06-06 05:43:27.000000 HomoglyphsCJK-0.1.4/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-22 05:35:00.236416 HomoglyphsCJK-0.1.5/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-22 05:35:00.235236 HomoglyphsCJK-0.1.5/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      122 2023-05-27 07:13:42.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)    10932 2023-05-27 06:58:42.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-22 05:35:00.236110 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4443 2023-06-22 05:35:00.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-06-22 05:35:00.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-06-22 05:35:00.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-06-22 05:35:00.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-06-22 05:35:00.000000 HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4443 2023-06-22 05:35:00.236283 HomoglyphsCJK-0.1.5/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3899 2023-06-22 05:34:27.000000 HomoglyphsCJK-0.1.5/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-06-22 05:35:00.236458 HomoglyphsCJK-0.1.5/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      967 2023-06-22 05:30:46.000000 HomoglyphsCJK-0.1.5/setup.py
```

### Comparing `HomoglyphsCJK-0.1.4/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.1.5/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.4/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.1.5/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.1.5/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.4
+Version: 0.1.5
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,15 @@
 pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: use **homoglyph_pairwise_distance** to calculate homoglyph distance between two strings, or use **homoglyph_merge** to merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use **homoglyph_merge** or **homoglyph_pairwise_distance** on specific language, the dict will be downloaded automatically if not already exist, otherwise load from your current directory. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + **homoglyph_merge** merges two dataframes. When you merge two dataframes, you can specify the parallel argument to use multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores.
++ Note that homoglyph_merge de-duplicates your passed in key columns and will in the end only return one unique value of the key specified. if you need to merge panel dataset to cross-sectional dataset for instance, you can de-duplicate the panel dataset key before you pass it in, then you will need to merge back your panel data using the matched key.
 
 ```python
 from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
```

### Comparing `HomoglyphsCJK-0.1.4/PKG-INFO` & `HomoglyphsCJK-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.4
+Version: 0.1.5
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,15 @@
 pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: use **homoglyph_pairwise_distance** to calculate homoglyph distance between two strings, or use **homoglyph_merge** to merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use **homoglyph_merge** or **homoglyph_pairwise_distance** on specific language, the dict will be downloaded automatically if not already exist, otherwise load from your current directory. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + **homoglyph_merge** merges two dataframes. When you merge two dataframes, you can specify the parallel argument to use multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores.
++ Note that homoglyph_merge de-duplicates your passed in key columns and will in the end only return one unique value of the key specified. if you need to merge panel dataset to cross-sectional dataset for instance, you can de-duplicate the panel dataset key before you pass it in, then you will need to merge back your panel data using the matched key.
 
 ```python
 from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
```

### Comparing `HomoglyphsCJK-0.1.4/README.md` & `HomoglyphsCJK-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: use **homoglyph_pairwise_distance** to calculate homoglyph distance between two strings, or use **homoglyph_merge** to merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use **homoglyph_merge** or **homoglyph_pairwise_distance** on specific language, the dict will be downloaded automatically if not already exist, otherwise load from your current directory. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + **homoglyph_merge** merges two dataframes. When you merge two dataframes, you can specify the parallel argument to use multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores.
++ Note that homoglyph_merge de-duplicates your passed in key columns and will in the end only return one unique value of the key specified. if you need to merge panel dataset to cross-sectional dataset for instance, you can de-duplicate the panel dataset key before you pass it in, then you will need to merge back your panel data using the matched key.
 
 ```python
 from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
```

### Comparing `HomoglyphsCJK-0.1.4/setup.py` & `HomoglyphsCJK-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r",encoding='utf-8') as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.1.4",
+    version="0.1.5",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

