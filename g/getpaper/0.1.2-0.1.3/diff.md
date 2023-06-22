# Comparing `tmp/getpaper-0.1.2.tar.gz` & `tmp/getpaper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.2.tar", last modified: Wed Jun 21 22:08:49 2023, max compression
+gzip compressed data, was "getpaper-0.1.3.tar", last modified: Thu Jun 22 20:58:07 2023, max compression
```

## Comparing `getpaper-0.1.2.tar` & `getpaper-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.2/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 22:08:49.405064 getpaper-0.1.2/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.1.2/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.2/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3997 2023-06-21 14:18:41.000000 getpaper-0.1.2/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.2/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5455 2023-06-21 21:39:55.000000 getpaper-0.1.2/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.2/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 22:08:49.405064 getpaper-0.1.2/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 22:08:35.000000 getpaper-0.1.2/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.3/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4019 2023-06-22 20:58:07.287085 getpaper-0.1.3/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3404 2023-06-22 20:56:44.000000 getpaper-0.1.3/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.3/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6944 2023-06-22 20:56:44.000000 getpaper-0.1.3/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.3/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5455 2023-06-21 21:39:55.000000 getpaper-0.1.3/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.3/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4019 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-22 20:58:07.287085 getpaper-0.1.3/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-22 20:56:44.000000 getpaper-0.1.3/setup.py
```

### Comparing `getpaper-0.1.2/LICENSE` & `getpaper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.2/PKG-INFO` & `getpaper-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.2
+Version: 0.1.3
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -25,24 +25,52 @@
 ```bash
 pip install getpaper
 ```
 
 # Usage
 ## Downloading papers
 
-After the installation you can either import the library into your python code or you can use the console scripts, for example:
+After the installation you can either import the library into your python code or you can use the console scripts.
+
+If you install from pip calling download will mean calling getpaper/download.py , for parse - getpaper/parse.py , for index - getpaper/index.py
+
 ```bash
 download download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
 download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
+It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
+```python
+from pathlib import Path
+from typing import List
+from getpaper.download import download_papers
+dois: List[str] = ["10.3390/ijms22031073", "10.1038/s41597-020-00710-z", "wrong"]
+destination: Path = Path("./data/output/test/papers").absolute().resolve()
+threads: int = 5
+results = download_papers(dois, destination, threads)
+successful = results[0]
+failed = results[1]
+```
+Here results will be OrderedDict[str, Path] with successfully downloaded doi->paper_path and List[str] with failed dois, in current example:
+```
+(OrderedDict([('10.3390/ijms22031073',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
+              ('10.1038/s41597-020-00710-z',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
+ ['wrong'])
+```
+Same function can be called from the command line:
+```bash
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+```
+
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
```

### Comparing `getpaper-0.1.2/README.md` & `getpaper-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,24 +7,52 @@
 ```bash
 pip install getpaper
 ```
 
 # Usage
 ## Downloading papers
 
-After the installation you can either import the library into your python code or you can use the console scripts, for example:
+After the installation you can either import the library into your python code or you can use the console scripts.
+
+If you install from pip calling download will mean calling getpaper/download.py , for parse - getpaper/parse.py , for index - getpaper/index.py
+
 ```bash
 download download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
 download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
+It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
+```python
+from pathlib import Path
+from typing import List
+from getpaper.download import download_papers
+dois: List[str] = ["10.3390/ijms22031073", "10.1038/s41597-020-00710-z", "wrong"]
+destination: Path = Path("./data/output/test/papers").absolute().resolve()
+threads: int = 5
+results = download_papers(dois, destination, threads)
+successful = results[0]
+failed = results[1]
+```
+Here results will be OrderedDict[str, Path] with successfully downloaded doi->paper_path and List[str] with failed dois, in current example:
+```
+(OrderedDict([('10.3390/ijms22031073',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
+              ('10.1038/s41597-020-00710-z',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
+ ['wrong'])
+```
+Same function can be called from the command line:
+```bash
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+```
+
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
```

### Comparing `getpaper-0.1.2/getpaper/index.py` & `getpaper-0.1.3/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.2/getpaper/parse.py` & `getpaper-0.1.3/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.2/getpaper/splitter.py` & `getpaper-0.1.3/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.2/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.3/getpaper.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.2
+Version: 0.1.3
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -25,24 +25,52 @@
 ```bash
 pip install getpaper
 ```
 
 # Usage
 ## Downloading papers
 
-After the installation you can either import the library into your python code or you can use the console scripts, for example:
+After the installation you can either import the library into your python code or you can use the console scripts.
+
+If you install from pip calling download will mean calling getpaper/download.py , for parse - getpaper/parse.py , for index - getpaper/index.py
+
 ```bash
 download download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
 download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
+It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
+```python
+from pathlib import Path
+from typing import List
+from getpaper.download import download_papers
+dois: List[str] = ["10.3390/ijms22031073", "10.1038/s41597-020-00710-z", "wrong"]
+destination: Path = Path("./data/output/test/papers").absolute().resolve()
+threads: int = 5
+results = download_papers(dois, destination, threads)
+successful = results[0]
+failed = results[1]
+```
+Here results will be OrderedDict[str, Path] with successfully downloaded doi->paper_path and List[str] with failed dois, in current example:
+```
+(OrderedDict([('10.3390/ijms22031073',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
+              ('10.1038/s41597-020-00710-z',
+               PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
+ ['wrong'])
+```
+Same function can be called from the command line:
+```bash
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+```
+
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
 getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
 ```
 You can also parse papers on a per file basis, for example:
```

### Comparing `getpaper-0.1.2/setup.py` & `getpaper-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

