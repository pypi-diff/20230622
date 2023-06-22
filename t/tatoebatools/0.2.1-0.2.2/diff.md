# Comparing `tmp/tatoebatools-0.2.1.tar.gz` & `tmp/tatoebatools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tatoebatools-0.2.1.tar", last modified: Sat Jun 25 13:37:55 2022, max compression
+gzip compressed data, was "tatoebatools-0.2.2.tar", last modified: Thu Jun 22 13:14:40 2023, max compression
```

## Comparing `tatoebatools-0.2.1.tar` & `tatoebatools-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:37:55.877112 tatoebatools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-06-25 13:37:55.877112 tatoebatools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5952 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-25 13:37:55.877112 tatoebatools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:37:55.873112 tatoebatools-0.2.1/tatoebatools/
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    17181 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/datafile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/difference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/download_page.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/jpn_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/sentences_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/sentences_cc0.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/sentences_detailed.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/sentences_in_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/sentences_with_audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/table.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)    18862 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/tatoebatools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/transcriptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/update.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/user_languages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/user_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     6409 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tatoebatools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:37:55.877112 tatoebatools-0.2.1/tatoebatools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-06-25 13:37:55.000000 tatoebatools-0.2.1/tatoebatools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-06-25 13:37:55.000000 tatoebatools-0.2.1/tatoebatools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 13:37:55.000000 tatoebatools-0.2.1/tatoebatools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-25 13:37:55.000000 tatoebatools-0.2.1/tatoebatools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-25 13:37:55.000000 tatoebatools-0.2.1/tatoebatools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:37:55.877112 tatoebatools-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6868 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_datafile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_download_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     3365 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     5476 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-06-25 13:37:44.000000 tatoebatools-0.2.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:14:40.222458 tatoebatools-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-22 13:14:40.222458 tatoebatools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:14:40.222458 tatoebatools-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:14:40.218458 tatoebatools-0.2.2/tatoebatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/download_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/jpn_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/sentences_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/sentences_cc0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/sentences_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/sentences_in_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/sentences_with_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/tatoebatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/transcriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/user_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/user_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tatoebatools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:14:40.218458 tatoebatools-0.2.2/tatoebatools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-22 13:14:40.000000 tatoebatools-0.2.2/tatoebatools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 13:14:40.000000 tatoebatools-0.2.2/tatoebatools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:14:40.000000 tatoebatools-0.2.2/tatoebatools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 13:14:40.000000 tatoebatools-0.2.2/tatoebatools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 13:14:40.000000 tatoebatools-0.2.2/tatoebatools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:14:40.222458 tatoebatools-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_download_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-22 13:14:25.000000 tatoebatools-0.2.2/tests/test_version.py
```

### Comparing `tatoebatools-0.2.1/PKG-INFO` & `tatoebatools-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: tatoebatools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library for downloading and reading data from Tatoeba
 Home-page: https://github.com/LBeaudoux/tatoebatools
 Author: L.Beaudoux
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # tatoebatools
 
 [![Actions Status](https://github.com/LBeaudoux/tatoebatools/workflows/CI/badge.svg)](https://github.com/LBeaudoux/tatoebatools/actions?query=workflow%3ACI)
 
 
 **tatoebatools** helps you to integrate [Tatoeba](https://tatoeba.org) into your app more quickly by allowing you to easily download and parse [Tatoeba weekly exports](https://downloads.tatoeba.org/exports/).
 
 ## Installation
 
-This library supports Python 3.7.1+.
+This library supports Python 3.8+.
 
 ```sh
 pip install tatoebatools
 ```
 
 ## Basic Usage
 
@@ -106,14 +105,19 @@
 new_german_texts = [s.text for s in tatoeba.sentences_detailed("deu", scope="added")]
 
 # list all links between French and Italian sentences
 french_italian_links = [(lk.sentence_id, lk.translation_id) for lk in tatoeba.links("fra", "ita")]
 
 # list all French native speakers
 native_french = [x.username for x in tatoeba.user_languages("fra") if x.skill_level == 5]
+
+# map German sentences to their audios
+german_audios = {}
+for audio in tatoeba.sentences_with_audio("deu"):
+    german_audios.setdefault(audio.sentence_id, []).append(audio.audio_id)
 ```
 
 ### Extracting Tatoeba data as dataframe
 
 Since **tatoebatools** relies heavily on the [pandas](https://github.com/pandas-dev/pandas) library, it is possible to load any supported table into memory as a dataframe.
 
 ```python
@@ -153,9 +157,7 @@
         for chunk in reader:
             chunk.to_sql(table_name, con=engine, index=False, if_exists="append")
 
 # add an index on the 'username' column of the 'sentences_detailed' table
 ix = Index('ix_sentences_detailed_username', SentenceDetailed.username)
 ix.create(engine)
 ```
-
-
```

### Comparing `tatoebatools-0.2.1/README.md` & `tatoebatools-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Actions Status](https://github.com/LBeaudoux/tatoebatools/workflows/CI/badge.svg)](https://github.com/LBeaudoux/tatoebatools/actions?query=workflow%3ACI)
 
 
 **tatoebatools** helps you to integrate [Tatoeba](https://tatoeba.org) into your app more quickly by allowing you to easily download and parse [Tatoeba weekly exports](https://downloads.tatoeba.org/exports/).
 
 ## Installation
 
-This library supports Python 3.7.1+.
+This library supports Python 3.8+.
 
 ```sh
 pip install tatoebatools
 ```
 
 ## Basic Usage
 
@@ -88,14 +88,19 @@
 new_german_texts = [s.text for s in tatoeba.sentences_detailed("deu", scope="added")]
 
 # list all links between French and Italian sentences
 french_italian_links = [(lk.sentence_id, lk.translation_id) for lk in tatoeba.links("fra", "ita")]
 
 # list all French native speakers
 native_french = [x.username for x in tatoeba.user_languages("fra") if x.skill_level == 5]
+
+# map German sentences to their audios
+german_audios = {}
+for audio in tatoeba.sentences_with_audio("deu"):
+    german_audios.setdefault(audio.sentence_id, []).append(audio.audio_id)
 ```
 
 ### Extracting Tatoeba data as dataframe
 
 Since **tatoebatools** relies heavily on the [pandas](https://github.com/pandas-dev/pandas) library, it is possible to load any supported table into memory as a dataframe.
 
 ```python
```

### Comparing `tatoebatools-0.2.1/setup.py` & `tatoebatools-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tatoebatools",
-    version="0.2.1",
+    version="0.2.2",
     author="L.Beaudoux",
     description="A library for downloading and reading data from Tatoeba",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LBeaudoux/tatoebatools",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
     ],
-    python_requires=">=3.7.1",
+    python_requires=">=3.8.0",
     install_requires=[
         "beautifulsoup4>=4.9.0",
-        "pandas>=1.3.3",
+        "pandas>=1.5.0",
         "requests>=2.23.0",
         "SQLAlchemy==1.4.23",
         "tqdm>=4.46.0",
     ],
 )
```

### Comparing `tatoebatools-0.2.1/tatoebatools/__init__.py` & `tatoebatools-0.2.2/tatoebatools/__init__.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/config.py` & `tatoebatools-0.2.2/tatoebatools/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,149 +62,173 @@
     "user_languages": UserLanguage,
     "queries": Query,
 }
 
 TABLE_CSV_PARAMS = {
     "sentences_base": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(SentenceBase)),
     },
     "sentences_detailed": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(SentenceDetailed)),
     },
     "sentences_CC0": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(SentenceCC0)),
     },
     "transcriptions": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(Transcription)),
     },
     "links": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(Link)),
     },
     "tags": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(Tag)),
     },
     "user_lists": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "text_col": 4,
         "nb_cols": len(list_attributes(UserList)),
     },
     "sentences_in_lists": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(SentenceInList)),
     },
     "jpn_indices": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(JpnIndex)),
     },
     "sentences_with_audio": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "nb_cols": len(list_attributes(SentenceWithAudio)),
     },
     "user_languages": {
         "delimiter": "\t",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "text_col": 3,
         "nb_cols": len(list_attributes(UserLanguage)),
     },
     "queries": {
         "delimiter": ",",
+        "doublequote": True,
+        "escapechar": "\\",
         "quoting": csv.QUOTE_NONE,
-        "quotechar": "",
+        "quotechar": '"',
         "lineterminator": "\n",
         "text_col": 2,
         "nb_cols": len(list_attributes(Query)),
         "encoding_errors": "ignore",
     },
 }
 
 TABLE_DATAFRAME_PARAMS = {
     "sentences_base": {
         "names": list_attributes(SentenceBase),
-        "na_values": ["\\N"],
+        "na_values": ["N"],
     },
     "sentences_detailed": {
         "names": list_attributes(SentenceDetailed),
         "parse_dates": ["date_added", "date_last_modified"],
         "date_parser": parse_export_date,
-        "na_values": ["\\N", "0000-00-00 00:00:00"],
+        "na_values": ["N", "0000-00-00 00:00:00"],
     },
     "sentences_CC0": {
         "names": list_attributes(SentenceCC0),
         "parse_dates": ["date_last_modified"],
         "date_parser": parse_export_date,
-        "na_values": ["\\N", "0000-00-00 00:00:00"],
+        "na_values": ["N", "0000-00-00 00:00:00"],
     },
     "transcriptions": {
         "names": list_attributes(Transcription),
     },
     "links": {
         "names": list_attributes(Link),
     },
     "tags": {
         "names": list_attributes(Tag),
     },
     "user_lists": {
         "names": list_attributes(UserList),
         "parse_dates": ["date_created", "date_last_modified"],
         "date_parser": parse_export_date,
-        "na_values": ["\\N", "0000-00-00 00:00:00"],
+        "na_values": ["N", "0000-00-00 00:00:00"],
     },
     "sentences_in_lists": {
         "names": list_attributes(SentenceInList),
     },
     "jpn_indices": {
         "names": list_attributes(JpnIndex),
     },
     "sentences_with_audio": {
         "names": list_attributes(SentenceWithAudio),
-        "na_values": ["\\N"],
+        "na_values": ["N"],
     },
     "user_languages": {
         "names": list_attributes(UserLanguage),
-        "na_values": ["\\N"],
+        "na_values": ["N"],
     },
     "queries": {
         "names": list_attributes(Query),
-        "na_values": ["\\N"],
+        "na_values": ["N"],
         "parse_dates": ["date"],
         "date_parser": parse_search_log_date,
         "encoding_errors": "ignore",
     },
 }
```

### Comparing `tatoebatools-0.2.1/tatoebatools/datafile.py` & `tatoebatools-0.2.2/tatoebatools/datafile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import logging
+import re
 from io import StringIO, TextIOBase
 from pathlib import Path
 
 import pandas as pd
 from tqdm import tqdm
 
 from .utils import get_byte_size, get_extended_name
@@ -29,16 +30,18 @@
 class DataFile:
     """A data file handler"""
 
     def __init__(
         self,
         file_path_or_data=StringIO(),
         delimiter="\t",
+        doublequote=True,
+        escapechar="\\",
         quoting=csv.QUOTE_NONE,
-        quotechar="",
+        quotechar='"',
         lineterminator="\n",
         na_values=None,
         text_col=None,
         nb_cols=None,
         encoding_errors=None,
     ):
         """
@@ -46,21 +49,33 @@
         ----------
         file_path_or_data : pathlib.Path, str, StringIO, pd.DataFrame
             The local path of a datafile, or a file-like object, or
             a pandas dataframe, or a data string
         delimiter : str, optional
             the field delimiter used by this data file,
             by default "\t"
+        doublequote : str, optional
+            Controls how instances of quotechar appearing inside a
+            field should themselves be quoted. When True, the character
+            is doubled. When False, the escapechar is used as a prefix
+            to the quotechar. It defaults to True.
+            On output, if doublequote is False and no escapechar is set,
+            Error is raised if a quotechar is found in a field.
+        escapechar: str, optional
+            A one-character string used by the writer to escape
+            the delimiter if quoting is set to QUOTE_NONE and the
+            quotechar if doublequote is False. On reading, the escapechar
+            removes any special meaning from the following character.
         quoting : csv module constant, optional
             the field quoting rule used by this data file,
             by default csv.QUOTE_NONE
         quotechar : str, optional
             A one-character string used to quote fields containing
             special characters, such as the delimiter or quotechar,
-            or which contain new-line characters, by default ""
+            or which contain new-line characters, by default '"'
         lineterminator : str, optional
             The string used to terminate lines produced by the csv
             writers, by default "\n"
         na_values : list, optional
             Additional strings to recognize as NA/NaN in dataframes.
             By default the following values are interpreted as NaN:
             ‘’, ‘#N/A’, ‘#N/A N/A’, ‘#NA’, ‘-1.#IND’, ‘-1.#QNAN’,
@@ -73,14 +88,16 @@
             The expected number of columns per row, by default None
         encoding_errors: str, optional
             set 'ignore' to ignore the malformed data and continue
             without further notice. Note that ignoring encoding
             errors can lead to data loss.
         """
         self._dm = delimiter
+        self._dq = doublequote
+        self._ec = escapechar
         self._qt = quoting
         self._qc = quotechar
         self._lt = lineterminator
         self._na = na_values
         self._tc = text_col
         self._nc = nb_cols
 
@@ -103,55 +120,60 @@
             else:
                 self._fp = Path(file_path_or_data)
         elif isinstance(file_path_or_data, pd.DataFrame):
             self._f = StringIO()
             file_path_or_data.to_csv(
                 self._f,
                 sep=self._dm,
+                doublequote=self._dq,
+                escapechar=self._ec,
                 quoting=self._qt,
                 quotechar=self._qc,
-                line_terminator=self._lt,
+                lineterminator=self._lt,
                 na_rep=self._na[0] if self._na else "",
                 header=None,
                 index=False,
             )
             self._f.seek(0)
             self._fp = None
         elif isinstance(file_path_or_data, TextIOBase):  # file-like scenario
             self._f = file_path_or_data
             self._f.seek(0)
             self._fp = None
         else:
             data_type = type(file_path_or_data)
             raise TypeError(f"{data_type} is not a valid 'file_path_or_data'")
 
+        # clean file buffer from known problematic characters
+        if self._tc:
+            self._f = self._get_cleaned_file_buffer()
+
         # init 'raw row' iterator
         self._rd = csv.reader(
             self._f,
             delimiter=self._dm,
+            doublequote=self._dq,
+            escapechar=self._ec,
             quoting=self._qt,
             quotechar=self._qc,
             lineterminator=self._lt,
         )
         # init 'working row' value buffer
         self._wr = []
 
     def __del__(self):
-
         if self._f:
             self._f.close()
 
     def __iter__(self):
-
         self.pos = 0
 
         return self
 
     def __next__(self):
-
         next_row = self._wr
         try:
             if not next_row:  # first line
                 next_row = next(self._rd)
             row_cnt = 1
             while True:
                 self._wr = next(self._rd)
@@ -189,15 +211,14 @@
                         return next_row
                     else:
                         msg = f"bad row in {self.path.name}: {next_row}"
                         logger.debug(msg)
 
     @reset_pos
     def __str__(self):
-
         return self._f.read()
 
     @property
     def pos(self):
         """Get the current position in this datafile"""
         return self._f.tell()
 
@@ -209,14 +230,16 @@
     @reset_pos
     def as_dataframe(self, **parameters):
         """Get the pandas dataframe of this datafile
         Parameters are any argument supported by 'pandas.read_csv'
         """
         params = {
             "sep": self._dm,
+            "doublequote": self._dq,
+            "escapechar": self._ec,
             "quoting": self._qt,
             "quotechar": self._qc,
             "lineterminator": self._lt,
             "na_values": self._na,
             "header": None,
             "index_col": None,
             "names": None,
@@ -256,14 +279,16 @@
             text_col = usecols.index(self._tc)
         except ValueError:
             text_col = None
 
         return DataFile(
             dframe,
             delimiter=self._dm,
+            doublequote=self._dq,
+            escapechar=self._ec,
             quoting=self._qt,
             quotechar=self._qc,
             lineterminator=self._lt,
             text_col=text_col,
             nb_cols=len(usecols),
         )
 
@@ -276,14 +301,16 @@
         'converter' (optional): a converter applied to the filter column
         """
         if row_filters:
             fb = StringIO()
             wt = csv.writer(
                 fb,
                 delimiter=self._dm,
+                doublequote=self._dq,
+                escapechar=self._ec,
                 quoting=self._qt,
                 quotechar=self._qc,
                 lineterminator=self._lt,
             )
             for row in self:
                 try:
                     for flt in row_filters:
@@ -296,14 +323,16 @@
                 else:
                     wt.writerow(row)
             fb.seek(0)
 
             return DataFile(
                 fb,
                 delimiter=self._dm,
+                doublequote=self._dq,
+                escapechar=self._ec,
                 quoting=self._qt,
                 quotechar=self._qc,
                 lineterminator=self._lt,
                 text_col=self._tc,
                 nb_cols=self._nc,
             )
 
@@ -324,14 +353,16 @@
             lsuffix="left",
             rsuffix="right",
         )
 
         return DataFile(
             join_dframe,
             delimiter=self._dm,
+            doublequote=self._dq,
+            escapechar=self._ec,
             quoting=self._qt,
             quotechar=self._qc,
             lineterminator=self._lt,
             text_col=self._tc,
             nb_cols=self._nc,
         )
 
@@ -339,14 +370,16 @@
         """Find 'added' and 'removed' rows to this data file
         compared to its former local version (if any)
         """
         fname_old = get_extended_name(self.path, "old")
         dfile_old = DataFile(
             self.path.parent.joinpath(fname_old),
             delimiter=self._dm,
+            doublequote=self._dq,
+            escapechar=self._ec,
             quoting=self._qt,
             quotechar=self._qc,
             lineterminator=self._lt,
             text_col=self._tc,
             nb_cols=self._nc,
         )
         diffs = {}
@@ -368,14 +401,16 @@
                 tags = {"added": "right_only", "removed": "left_only"}
                 for k, v in tags.items():
                     mask = merger["_merge"] == v
                     diff_df = merger.loc[mask].drop(columns="_merge")
                     diffs[k] = DataFile(
                         diff_df,
                         delimiter=self._dm,
+                        doublequote=self._dq,
+                        escapechar=self._ec,
                         quoting=self._qt,
                         quotechar=self._qc,
                         lineterminator=self._lt,
                         text_col=self._tc,
                         nb_cols=self._nc,
                     )
                 if save:  # save difference files in the same directory
@@ -405,28 +440,32 @@
                 if all(fields):
                     # classify the rows
                     fname = self._get_out_filename(fields)
                     fb = buffer.setdefault(fname, StringIO())
                     wt = csv.writer(
                         fb,
                         delimiter=self._dm,
+                        doublequote=self._dq,
+                        escapechar=self._ec,
                         quoting=self._qt,
                         quotechar=self._qc,
                         lineterminator=self._lt,
                     )
                     wt.writerow(row)
 
             if pbar:  # imcrement progress bar by the byte size of the row
                 pbar.update(get_byte_size(row, self._dm, self._lt))
 
         splits = []
         for fname, fb in buffer.items():
             split = DataFile(
                 fb,
                 delimiter=self._dm,
+                doublequote=self._dq,
+                escapechar=self._ec,
                 quoting=self._qt,
                 quotechar=self._qc,
                 lineterminator=self._lt,
                 text_col=self._tc,
                 nb_cols=self._nc,
             )
             if save:  # save split files in the same parent directory
@@ -441,20 +480,36 @@
             splits.append(split)
 
         if pbar:
             pbar.close()
 
         return splits
 
+    def _get_cleaned_file_buffer(self):
+        """Clean known problematic characters from the file objext"""
+        file_content = self._f.read()
+        # multiline 'details' fields in 'user_languages' table have escaped
+        # new lines that can be removed
+        file_content = re.sub(r"\n\\\n", "  ", file_content)
+        # the 'list_name' field of the 'user_lists' table may have escaped
+        # tab delimiter that can be removed
+        file_content = re.sub(r"\\" + self._dm + r"+", " ", file_content)
+        fb = StringIO()
+        fb.write(file_content)
+        fb.seek(0)
+        return fb
+
     def _get_fixed_file_buffer(self):
         """Try to fix multiline rows found into the file objext"""
         fb = StringIO()
         wt = csv.writer(
             fb,
             delimiter=self._dm,
+            doublequote=self._dq,
+            escapechar=self._ec,
             quoting=self._qt,
             quotechar=self._qc,
             lineterminator=self._lt,
         )
         wt.writerows(iter(self))
         fb.seek(0)
```

### Comparing `tatoebatools-0.2.1/tatoebatools/difference.py` & `tatoebatools-0.2.2/tatoebatools/difference.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/download.py` & `tatoebatools-0.2.2/tatoebatools/download.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/download_page.py` & `tatoebatools-0.2.2/tatoebatools/download_page.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/exceptions.py` & `tatoebatools-0.2.2/tatoebatools/exceptions.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/jpn_indices.py` & `tatoebatools-0.2.2/tatoebatools/jpn_indices.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/models.py` & `tatoebatools-0.2.2/tatoebatools/models.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/queries.py` & `tatoebatools-0.2.2/tatoebatools/queries.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/sentences_base.py` & `tatoebatools-0.2.2/tatoebatools/sentences_base.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/sentences_cc0.py` & `tatoebatools-0.2.2/tatoebatools/sentences_cc0.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/sentences_detailed.py` & `tatoebatools-0.2.2/tatoebatools/sentences_detailed.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/sentences_with_audio.py` & `tatoebatools-0.2.2/tatoebatools/sentences_with_audio.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/table.py` & `tatoebatools-0.2.2/tatoebatools/table.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/tatoebatools.py` & `tatoebatools-0.2.2/tatoebatools/tatoebatools.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/transcriptions.py` & `tatoebatools-0.2.2/tatoebatools/transcriptions.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/update.py` & `tatoebatools-0.2.2/tatoebatools/update.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/user_languages.py` & `tatoebatools-0.2.2/tatoebatools/user_languages.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/user_lists.py` & `tatoebatools-0.2.2/tatoebatools/user_lists.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools/utils.py` & `tatoebatools-0.2.2/tatoebatools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import bz2
 import csv
 import logging
 import math
+import os
 import tarfile
 from pathlib import Path
 
 import pandas as pd
 import requests
 from tqdm import tqdm
 
@@ -85,15 +86,33 @@
         with tarfile.open(arx_path) as tar:
             out_filenames = tar.getnames()
             out_paths = [arx_path.parent.joinpath(fn) for fn in out_filenames]
             # rename latest extracted files at this path for file comparison
             for fp in out_paths:
                 indicate_as_old(fp)
 
-            tar.extractall(arx_path.parent)
+            def is_within_directory(directory, target):
+                abs_directory = os.path.abspath(directory)
+                abs_target = os.path.abspath(target)
+
+                prefix = os.path.commonprefix([abs_directory, abs_target])
+
+                return prefix == abs_directory
+
+            def safe_extract(
+                tar, path=".", members=None, *, numeric_owner=False
+            ):
+                for member in tar.getmembers():
+                    member_path = os.path.join(path, member.name)
+                    if not is_within_directory(path, member_path):
+                        raise Exception("Attempted Path Traversal in Tar File")
+
+                tar.extractall(path, members, numeric_owner=numeric_owner)
+
+            safe_extract(tar, arx_path.parent)
 
         arx_path.unlink()
     except FileNotFoundError:
         logger.error(f"{arx_path} not found by file extractor")
         return []
     except tarfile.ReadError:
         logger.error(f"{arx_path} is not an extractable archive")
@@ -196,15 +215,15 @@
     """
     return [x for x in any_class.__dict__.keys() if not x.startswith("_")]
 
 
 def is_na(element):
     """Check if an element is 'not available'"""
     if isinstance(element, str):
-        return element == "\\N"
+        return element == "N"
     elif isinstance(element, float):
         return math.isnan(element)
     return False
 
 
 def parse_export_date(datetime_string):
     """Parse a datetime string from a weekly export file"""
```

### Comparing `tatoebatools-0.2.1/tatoebatools/version.py` & `tatoebatools-0.2.2/tatoebatools/version.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tatoebatools.egg-info/PKG-INFO` & `tatoebatools-0.2.2/tatoebatools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: tatoebatools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library for downloading and reading data from Tatoeba
 Home-page: https://github.com/LBeaudoux/tatoebatools
 Author: L.Beaudoux
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # tatoebatools
 
 [![Actions Status](https://github.com/LBeaudoux/tatoebatools/workflows/CI/badge.svg)](https://github.com/LBeaudoux/tatoebatools/actions?query=workflow%3ACI)
 
 
 **tatoebatools** helps you to integrate [Tatoeba](https://tatoeba.org) into your app more quickly by allowing you to easily download and parse [Tatoeba weekly exports](https://downloads.tatoeba.org/exports/).
 
 ## Installation
 
-This library supports Python 3.7.1+.
+This library supports Python 3.8+.
 
 ```sh
 pip install tatoebatools
 ```
 
 ## Basic Usage
 
@@ -106,14 +105,19 @@
 new_german_texts = [s.text for s in tatoeba.sentences_detailed("deu", scope="added")]
 
 # list all links between French and Italian sentences
 french_italian_links = [(lk.sentence_id, lk.translation_id) for lk in tatoeba.links("fra", "ita")]
 
 # list all French native speakers
 native_french = [x.username for x in tatoeba.user_languages("fra") if x.skill_level == 5]
+
+# map German sentences to their audios
+german_audios = {}
+for audio in tatoeba.sentences_with_audio("deu"):
+    german_audios.setdefault(audio.sentence_id, []).append(audio.audio_id)
 ```
 
 ### Extracting Tatoeba data as dataframe
 
 Since **tatoebatools** relies heavily on the [pandas](https://github.com/pandas-dev/pandas) library, it is possible to load any supported table into memory as a dataframe.
 
 ```python
@@ -153,9 +157,7 @@
         for chunk in reader:
             chunk.to_sql(table_name, con=engine, index=False, if_exists="append")
 
 # add an index on the 'username' column of the 'sentences_detailed' table
 ix = Index('ix_sentences_detailed_username', SentenceDetailed.username)
 ix.create(engine)
 ```
-
-
```

### Comparing `tatoebatools-0.2.1/tatoebatools.egg-info/SOURCES.txt` & `tatoebatools-0.2.2/tatoebatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tests/test_datafile.py` & `tatoebatools-0.2.2/tests/test_datafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from unittest.mock import patch
 
 import pandas as pd
 from tatoebatools.datafile import DataFile
 
 
 class TestDataFileInit:
-
     data = "a,b,c\nd,e,f\n"
     params = {"delimiter": ","}
 
     def test_string_arg(self):
         dfile = DataFile(self.data)
         assert str(dfile) == self.data
 
@@ -36,15 +35,14 @@
 
     def test_file_lik_object_arg(self):
         dfile = DataFile(StringIO(self.data), **self.params)
         assert str(dfile) == self.data
 
 
 class TestDataFileIterator:
-
     delimiters = ("\t", ",")
 
     def test_empty(self):
         for dm in self.delimiters:
             dfile = DataFile("", delimiter=dm)
             assert [row for row in dfile] == []
 
@@ -66,15 +64,15 @@
 
     def test_with_null_field(self):
         in_rows = [["a", "\\N", "c"]]
         for dm in self.delimiters:
             s = "\n".join([dm.join(r) for r in in_rows])
             dfile = DataFile(s, delimiter=dm)
             out_rows = [row for row in dfile]
-            assert out_rows == in_rows
+            assert out_rows == [["a", "N", "c"]]
 
     def test_delimiter_split_end_column(self):
         for dm in self.delimiters:
             in_rows = [["a", "b", "c", "c"]]
             s = "\n".join([dm.join(r) for r in in_rows])
             dfile = DataFile(s, delimiter=dm, nb_cols=3, text_col=2)
             out_rows = [row for row in dfile]
@@ -105,22 +103,21 @@
             assert out_rows == [["a", "b", "c"], ["d", "e e", "f"]]
 
     def test_quoted_text(self):
         for dm in self.delimiters:
             in_rows = [["foo", 'foo "bar" baz', "bar"]]
             s = "\n".join([dm.join(r) for r in in_rows])
             dfile = DataFile(
-                s, delimiter=dm, quotechar="", quoting=csv.QUOTE_NONE
+                s, delimiter=dm, quotechar="'", quoting=csv.QUOTE_NONE
             )
             out_rows = [row for row in dfile]
             assert out_rows == in_rows
 
 
 class TestDataFileAsDataFrame:
-
     delimiters = ("\t", ",")
 
     def test_empty(self):
         for dm in self.delimiters:
             dfile = DataFile("", delimiter=dm)
             dframe = dfile.as_dataframe()
             assert dframe.equals(pd.DataFrame())
@@ -149,15 +146,14 @@
             dfile = DataFile(s, delimiter=dm)
             dframe1 = dfile.as_dataframe(index_col=[0])
             dframe2 = pd.DataFrame(in_rows).set_index([0])
             assert dframe1.equals(dframe2)
 
 
 class TestDataFileExtract:
-
     delimiters = ("\t", ",")
     data = "a,b,c\nd,e,f\n"
     params = {"delimiter": ","}
 
     def test_extract_columns(self):
         dfile = DataFile(self.data, **self.params)
         dfile_cols = dfile.extract_columns(usecols=[0, 1])
@@ -167,15 +163,14 @@
         dfile = DataFile(self.data, **self.params)
         row_filters = [{"col_index": 0, "ok_values": {"d"}}]
         dfile_rows = dfile.extract_rows(row_filters=row_filters)
         assert str(dfile_rows) == str(DataFile("d,e,f\n", **self.params))
 
 
 class TestDataFileJoin:
-
     delimiters = ("\t", ",")
     data = "a,b,c\nd,e,f\n"
     params = {"delimiter": ","}
 
     def test_join_dataframe(self):
         dfile = DataFile(self.data, **self.params)
         other_dframe = pd.DataFrame([["a", "b"], ["c", "d"], ["e", "f"]])
```

### Comparing `tatoebatools-0.2.1/tests/test_download_page.py` & `tatoebatools-0.2.2/tests/test_download_page.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tests/test_table.py` & `tatoebatools-0.2.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tests/test_update.py` & `tatoebatools-0.2.2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `tatoebatools-0.2.1/tests/test_utils.py` & `tatoebatools-0.2.2/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,28 +88,32 @@
     def test_with_archive(self, m_tar_open, m_unlink):
         m_tar = m_tar_open.return_value.__enter__.return_value
         m_tar.getnames.return_value = self.out_filenames
 
         out_filepaths = extract(self.archive_path)
 
         m_tar_open.assert_called_once_with(Path(self.archive_path))
-        m_tar.extractall.assert_called_once_with(Path(self.out_dir))
+        m_tar.extractall.assert_called_once_with(
+            Path(self.out_dir), None, numeric_owner=False
+        )
         assert m_tar.getnames.call_count == 1
         assert m_unlink.call_count == 1
         assert out_filepaths == [Path(fp) for fp in self.out_filepaths]
 
     @patch("tatoebatools.utils.tarfile.open")
     def test_without_archive(self, m_tar_open):
         m_tar = m_tar_open.return_value.__enter__.return_value
         m_tar.extractall.side_effect = ReadError
 
         out_filepaths = extract(self.archive_path)
 
         m_tar_open.assert_called_once_with(Path(self.archive_path))
-        m_tar.extractall.assert_called_once_with(Path(self.out_dir))
+        m_tar.extractall.assert_called_once_with(
+            Path(self.out_dir), None, numeric_owner=False
+        )
         assert out_filepaths == []
 
     @patch("tatoebatools.utils.tarfile.open", side_effect=FileNotFoundError)
     def test_without_file(self, m_tar_open):
         out_filepaths = extract(self.archive_path)
 
         assert out_filepaths == []
```

### Comparing `tatoebatools-0.2.1/tests/test_version.py` & `tatoebatools-0.2.2/tests/test_version.py`

 * *Files identical despite different names*

