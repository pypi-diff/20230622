# Comparing `tmp/finvader-1.0.0.tar.gz` & `tmp/finvader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finvader-1.0.0.tar", last modified: Sun May 28 13:21:37 2023, max compression
+gzip compressed data, was "finvader-1.0.1.tar", last modified: Wed Jun 21 23:05:50 2023, max compression
```

## Comparing `finvader-1.0.0.tar` & `finvader-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:37.225856 finvader-1.0.0/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 finvader-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3032 2023-05-28 13:21:37.225856 finvader-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2326 2023-05-28 13:11:28.000000 finvader-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:37.215918 finvader-1.0.0/finvader/
--rw-rw-rw-   0        0        0     6705 2023-05-27 17:29:37.000000 finvader-1.0.0/finvader/Henry.py
--rw-rw-rw-   0        0        0   302545 2023-05-26 21:35:39.000000 finvader-1.0.0/finvader/SentiBignomics.py
--rw-rw-rw-   0        0        0       48 2023-05-28 11:35:13.000000 finvader-1.0.0/finvader/__init__.py
--rw-rw-rw-   0        0        0     3182 2023-05-28 10:51:52.000000 finvader-1.0.0/finvader/finvader.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:37.224470 finvader-1.0.0/finvader.egg-info/
--rw-rw-rw-   0        0        0     3032 2023-05-28 13:21:37.000000 finvader-1.0.0/finvader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-28 13:21:37.000000 finvader-1.0.0/finvader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 13:21:37.000000 finvader-1.0.0/finvader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-28 13:21:37.000000 finvader-1.0.0/finvader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 13:21:37.000000 finvader-1.0.0/finvader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      551 2023-05-28 13:20:50.000000 finvader-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 13:21:37.232022 finvader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-05-28 13:20:50.000000 finvader-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.305246 finvader-1.0.1/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 finvader-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3033 2023-06-21 23:05:50.305246 finvader-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2023-05-29 19:00:12.000000 finvader-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.289502 finvader-1.0.1/finvader/
+-rw-rw-rw-   0        0        0     6705 2023-05-27 17:29:37.000000 finvader-1.0.1/finvader/Henry.py
+-rw-rw-rw-   0        0        0   302545 2023-05-26 21:35:39.000000 finvader-1.0.1/finvader/SentiBignomics.py
+-rw-rw-rw-   0        0        0       48 2023-05-28 11:35:13.000000 finvader-1.0.1/finvader/__init__.py
+-rw-rw-rw-   0        0        0     3182 2023-05-28 10:51:52.000000 finvader-1.0.1/finvader/finvader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.305246 finvader-1.0.1/finvader.egg-info/
+-rw-rw-rw-   0        0        0     3033 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      551 2023-06-21 23:04:28.000000 finvader-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 23:05:50.305246 finvader-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      619 2023-06-21 23:04:28.000000 finvader-1.0.1/setup.py
```

### Comparing `finvader-1.0.0/PKG-INFO` & `finvader-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finvader
-Version: 1.0.0
+Version: 1.0.1
 Summary: VADER sentiment classifier updated with financial lexicons
 Home-page: https://github.com/PetrKorab/FinVADER
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/FinVADER
 Project-URL: Bug Tracker, https://github.com/PetrKorab/FinVADER/issues
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # FinVADER
-**VADER sentiment classifier updated with financial lexicon**
+**VADER sentiment classifier updated with financial lexicons**
 
 
 **VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
 general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
 worse on texts that use domain-specific language, such as finance or economics.
 
 **FinVADER** improves VADER's classification accuracy, including two finance lexicons: [SentiBignomics](https://github.com/consose/SentiBigNomics),
```

### Comparing `finvader-1.0.0/README.md` & `finvader-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # FinVADER
-**VADER sentiment classifier updated with financial lexicon**
+**VADER sentiment classifier updated with financial lexicons**
 
 
 **VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
 general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
 worse on texts that use domain-specific language, such as finance or economics.
 
 **FinVADER** improves VADER's classification accuracy, including two finance lexicons: [SentiBignomics](https://github.com/consose/SentiBigNomics),
```

### Comparing `finvader-1.0.0/finvader/Henry.py` & `finvader-1.0.1/finvader/Henry.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.0/finvader/SentiBignomics.py` & `finvader-1.0.1/finvader/SentiBignomics.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.0/finvader/finvader.py` & `finvader-1.0.1/finvader/finvader.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.0/finvader.egg-info/PKG-INFO` & `finvader-1.0.1/finvader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finvader
-Version: 1.0.0
+Version: 1.0.1
 Summary: VADER sentiment classifier updated with financial lexicons
 Home-page: https://github.com/PetrKorab/FinVADER
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/FinVADER
 Project-URL: Bug Tracker, https://github.com/PetrKorab/FinVADER/issues
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # FinVADER
-**VADER sentiment classifier updated with financial lexicon**
+**VADER sentiment classifier updated with financial lexicons**
 
 
 **VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
 general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
 worse on texts that use domain-specific language, such as finance or economics.
 
 **FinVADER** improves VADER's classification accuracy, including two finance lexicons: [SentiBignomics](https://github.com/consose/SentiBigNomics),
```

### Comparing `finvader-1.0.0/pyproject.toml` & `finvader-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "finvader"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "VADER sentiment classifier updated with financial lexicons"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `finvader-1.0.0/setup.py` & `finvader-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="finvader",
-        version="1.0.0",
+        version="1.0.1",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["finvader"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/FinVADER",
         python_requires='>=3.8',
-        install_requires = ['nltk==3.8.1'],
+        install_requires = ['nltk == 3.6.2'],
         license='MIT License'
     )
```

