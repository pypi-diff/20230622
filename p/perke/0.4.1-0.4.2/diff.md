# Comparing `tmp/perke-0.4.1.tar.gz` & `tmp/perke-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perke-0.4.1.tar", last modified: Wed Mar 15 07:41:19 2023, max compression
+gzip compressed data, was "perke-0.4.2.tar", last modified: Thu Jun 22 14:45:11 2023, max compression
```

## Comparing `perke-0.4.1.tar` & `perke-0.4.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.767503 perke-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-15 07:40:41.000000 perke-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-15 07:40:41.000000 perke-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-03-15 07:41:19.767503 perke-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-15 07:40:41.000000 perke-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.763502 perke-0.4.1/perke/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-15 07:40:41.000000 perke-0.4.1/perke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-15 07:40:41.000000 perke-0.4.1/perke/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.763502 perke-0.4.1/perke/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:40:41.000000 perke-0.4.1/perke/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-15 07:40:41.000000 perke-0.4.1/perke/base/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-03-15 07:40:41.000000 perke-0.4.1/perke/base/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-15 07:40:41.000000 perke-0.4.1/perke/base/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-15 07:40:41.000000 perke-0.4.1/perke/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.763502 perke-0.4.1/perke/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-15 07:40:41.000000 perke-0.4.1/perke/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-15 07:40:41.000000 perke-0.4.1/perke/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-15 07:40:41.000000 perke-0.4.1/perke/cli/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-15 07:40:41.000000 perke-0.4.1/perke/cli/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.763502 perke-0.4.1/perke/unsupervised/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.767503 perke-0.4.1/perke/unsupervised/graph_based/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/multipartite_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/position_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/single_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/text_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-15 07:40:41.000000 perke-0.4.1/perke/unsupervised/graph_based/topic_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.767503 perke-0.4.1/perke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:40:41.000000 perke-0.4.1/perke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-15 07:40:41.000000 perke-0.4.1/perke/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-15 07:40:41.000000 perke-0.4.1/perke/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 07:41:10.000000 perke-0.4.1/perke/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.763502 perke-0.4.1/perke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 07:41:19.000000 perke-0.4.1/perke.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:41:19.767503 perke-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 07:40:41.000000 perke-0.4.1/requirements/develop.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-15 07:40:41.000000 perke-0.4.1/requirements/documentation.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-15 07:40:41.000000 perke-0.4.1/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 07:40:41.000000 perke-0.4.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 07:41:19.767503 perke-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-15 07:40:41.000000 perke-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.700363 perke-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 14:44:31.000000 perke-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 14:44:31.000000 perke-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-22 14:45:11.700363 perke-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-22 14:44:31.000000 perke-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.696362 perke-0.4.2/perke/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 14:44:31.000000 perke-0.4.2/perke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 14:44:31.000000 perke-0.4.2/perke/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.696362 perke-0.4.2/perke/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:44:31.000000 perke-0.4.2/perke/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-22 14:44:31.000000 perke-0.4.2/perke/base/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-06-22 14:44:31.000000 perke-0.4.2/perke/base/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-22 14:44:31.000000 perke-0.4.2/perke/base/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 14:44:31.000000 perke-0.4.2/perke/base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.696362 perke-0.4.2/perke/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 14:44:31.000000 perke-0.4.2/perke/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 14:44:31.000000 perke-0.4.2/perke/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 14:44:31.000000 perke-0.4.2/perke/cli/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 14:44:31.000000 perke-0.4.2/perke/cli/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.696362 perke-0.4.2/perke/unsupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.700363 perke-0.4.2/perke/unsupervised/graph_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/multipartite_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/position_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/single_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/text_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-22 14:44:31.000000 perke-0.4.2/perke/unsupervised/graph_based/topic_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.700363 perke-0.4.2/perke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:44:31.000000 perke-0.4.2/perke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 14:44:31.000000 perke-0.4.2/perke/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 14:44:31.000000 perke-0.4.2/perke/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 14:45:01.000000 perke-0.4.2/perke/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.696362 perke-0.4.2/perke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 14:45:11.000000 perke-0.4.2/perke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:45:11.700363 perke-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 14:44:31.000000 perke-0.4.2/requirements/develop.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-22 14:44:31.000000 perke-0.4.2/requirements/documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 14:44:31.000000 perke-0.4.2/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 14:44:31.000000 perke-0.4.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:45:11.700363 perke-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-22 14:44:31.000000 perke-0.4.2/setup.py
```

### Comparing `perke-0.4.1/LICENSE` & `perke-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/PKG-INFO` & `perke-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perke
-Version: 0.4.1
+Version: 0.4.2
 Summary: A keyphrase extractor for Persian
 Home-page: https://github.com/alirezatheh/perke
 Author: Alireza Hosseini
 Author-email: alirezatheh@gmail.com
 Project-URL: Bug Tracker, https://github.com/alirezatheh/perke/issues
 Project-URL: Documentation, https://perke.readthedocs.io
 Project-URL: Source Code, https://github.com/alirezatheh/perke
@@ -22,14 +22,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: Persian
 Requires-Python: >=3.8
@@ -37,15 +38,15 @@
 License-File: LICENSE
 
 # Perke
 [![tests](https://github.com/alirezatheh/perke/workflows/tests/badge.svg)](https://github.com/alirezatheh/perke/actions/workflows/tests.yaml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/AlirezaTheH/perke/main.svg)](https://results.pre-commit.ci/latest/github/alirezatheh/perke/main)
 [![PyPI Version](https://img.shields.io/pypi/v/perke)](https://pypi.python.org/pypi/perke)
 [![Python Versions](https://img.shields.io/pypi/pyversions/perke)](https://pypi.org/project/perke)
-[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/latest/?badge=stable)
+[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/stable/?badge=stable)
 
 Perke is a Python keyphrase extraction package for Persian language. It
 provides an end-to-end keyphrase extraction pipeline in which each component
 can be easily modified or extended to develop new models.
 
 ## Installation
 - The easiest way to install is from PyPI:
```

### Comparing `perke-0.4.1/README.md` & `perke-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Perke
 [![tests](https://github.com/alirezatheh/perke/workflows/tests/badge.svg)](https://github.com/alirezatheh/perke/actions/workflows/tests.yaml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/AlirezaTheH/perke/main.svg)](https://results.pre-commit.ci/latest/github/alirezatheh/perke/main)
 [![PyPI Version](https://img.shields.io/pypi/v/perke)](https://pypi.python.org/pypi/perke)
 [![Python Versions](https://img.shields.io/pypi/pyversions/perke)](https://pypi.org/project/perke)
-[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/latest/?badge=stable)
+[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/stable/?badge=stable)
 
 Perke is a Python keyphrase extraction package for Persian language. It
 provides an end-to-end keyphrase extraction pipeline in which each component
 can be easily modified or extended to develop new models.
 
 ## Installation
 - The easiest way to install is from PyPI:
```

### Comparing `perke-0.4.1/perke/base/data_structures.py` & `perke-0.4.2/perke/base/data_structures.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/perke/base/extractor.py` & `perke-0.4.2/perke/base/extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,46 +41,53 @@
         """
         Initializes the extractor.
 
         Parameters
         ----------
         valid_pos_tags:
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'ADJ'}`.
         """
         self.word_normalization_method: Optional[str] = None
         self.sentences: List[Sentence] = []
         self.candidates: DefaultDict[str, Candidate] = defaultdict(Candidate)
         self.stopwords: Set[str] = set(hazm.stopwords_list()) | set(
             punctuation_marks
         )
         if valid_pos_tags is None:
-            valid_pos_tags = {'N', 'Ne', 'AJ', 'AJe'}
+            valid_pos_tags = {'NOUN', 'ADJ'}
         self.valid_pos_tags: Set[str] = valid_pos_tags
 
     def load_text(
         self,
         input: Union[str, Path],
         word_normalization_method: WordNormalizationMethod = 'stemming',
+        universal_pos_tags: bool = True,
     ) -> None:
         """
         Loads the text of a document or string.
 
         Parameters
         ----------
         input:
             Input, this can be either raw text or filepath.
 
         word_normalization_method:
             Word normalization method, defaults to `'stemming'`. See
             `perke.base.types.WordNormalizationMethod` for available
             methods.
+
+        universal_pos_tags:
+            Whether to use universal part of speech tags or not,
+            defaults to `True`.
         """
         # Initialize reader
-        reader = RawTextReader(input, word_normalization_method)
+        reader = RawTextReader(
+            input, word_normalization_method, universal_pos_tags
+        )
 
         # Load sentences
         self.sentences = reader.read()
 
         self.word_normalization_method = word_normalization_method
 
     def _is_redundant(
@@ -221,15 +228,15 @@
             List of part of speech tags assigned to words of the
             occurrence
 
         offset:
             The offset of the occurrence
 
         normalized_words:
-            List of normalized of words of the occurrence
+            List of normalized words of the occurrence
         """
         # Build the canonical form of the candidate
         canonical_form = ' '.join(normalized_words)
 
         # Create candidate if not exist and add occurrence
         self.candidates[canonical_form].add_occurrence(
             words, offset, pos_tags, normalized_words
@@ -302,15 +309,15 @@
                         continue
 
                 # Add sequence as candidate if it is not empty
                 if len(sequence_offsets) > 0:
                     first = sequence_offsets[0]
                     last = sequence_offsets[-1]
 
-                    # Add the ngram as a new candidate occurrence
+                    # Add the n-gram as a new candidate occurrence
                     self._add_candidate_occurrence(
                         words=sentence.words[first : last + 1],
                         offset=offset_shift + first,
                         pos_tags=sentence.pos_tags[first : last + 1],
                         normalized_words=sentence.normalized_words[
                             first : last + 1
                         ],
@@ -332,28 +339,28 @@
         Parameters
         ----------
         grammar:
             grammar defining part of speech patterns of noun phrases,
             defaults to::
                 r\"""
                 NP:
-                    <P>{<N>}<V>
+                    {<NOUN>}<VERB>
                 NP:
-                    {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                    <N>}{<.*e?>'
+                    {<DET(,EZ)?|NOUN(,EZ)?|NUM(,EZ)?|ADJ(,EZ)|PRON><DET(,EZ)|NOUN(,EZ)|NUM(,EZ)|ADJ(,EZ)|PRON>*}
+                    <NOUN>}{<.*(,EZ)?>
                 \"""
         """
         # Initialize default grammar if none provided
         if grammar is None:
             grammar = r"""
                 NP:
-                    <P>{<N>}<V>
+                    {<NOUN>}<VERB>
                 NP:
-                    {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                    <N>}{<.*e?>
+                    {<DET(,EZ)?|NOUN(,EZ)?|NUM(,EZ)?|ADJ(,EZ)|PRON><DET(,EZ)|NOUN(,EZ)|NUM(,EZ)|ADJ(,EZ)|PRON>*}
+                    <NOUN>}{<.*(,EZ)?>
             """
 
         # Initialize parser
         parser = nltk.RegexpParser(grammar)
 
         # Loop through the sentences
         offset_shift = 0
```

### Comparing `perke-0.4.1/perke/base/readers.py` & `perke-0.4.2/perke/base/readers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from os.path import dirname, join
 from pathlib import Path
 from typing import List
 
 import hazm
 
 from perke.base.data_structures import Sentence
 from perke.base.types import WordNormalizationMethod
@@ -27,36 +26,43 @@
         The hazm lemmatizer instance
 
     pos_tagger:
         The hazm pos tagger instance
     """
 
     def __init__(
-        self, word_normalization_method: WordNormalizationMethod
+        self,
+        word_normalization_method: WordNormalizationMethod,
+        universal_pos_tags: bool,
     ) -> None:
         """
         Initializes the reader.
 
         Parameters
         ----------
         word_normalization_method:
             Word normalization method, see
             `perke.base.types.WordNormalizationMethod` for available
             methods.
+
+        universal_pos_tags:
+            Whether to use universal part of speech tags or not
         """
         self.word_normalization_method: WordNormalizationMethod = (
             word_normalization_method
         )
         self.normalizer: hazm.Normalizer = hazm.Normalizer()
         self.stemmer: hazm.Stemmer = hazm.Stemmer()
         self.lemmatizer: hazm.Lemmatizer = hazm.Lemmatizer()
-        model_filepath = join(
-            dirname(dirname(__file__)), 'resources', 'postagger.model'
+        self.pos_tagger: hazm.POSTagger = hazm.POSTagger(
+            model=str(
+                Path(__file__).parent.parent / 'resources' / 'pos_tagger.model'
+            ),
+            universal_tag=universal_pos_tags,
         )
-        self.pos_tagger: hazm.POSTagger = hazm.POSTagger(model=model_filepath)
 
 
 class RawTextReader(Reader):
     """
     Reader for raw text
 
     Attributes
@@ -65,29 +71,33 @@
         Raw text to read sentences from
     """
 
     def __init__(
         self,
         input: str,
         word_normalization_method: WordNormalizationMethod,
+        universal_pos_tags,
     ) -> None:
         """
         Initializes the reader.
 
         Parameters
         ----------
         input:
             Input, this can be either raw text or filepath.
 
         word_normalization_method:
             Word normalization method, see
             `perke.base.types.WordNormalizationMethod` for available
             methods.
+
+        universal_pos_tags:
+            Whether to use universal part of speech tags or not
         """
-        super().__init__(word_normalization_method)
+        super().__init__(word_normalization_method, universal_pos_tags)
 
         # If input is a filepath
         if isinstance(input, Path):
             assert input.exists()
             with open(input, encoding='utf-8') as file:
                 self.text: str = file.read()
```

### Comparing `perke-0.4.1/perke/cli/base.py` & `perke-0.4.2/perke/cli/base.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/perke/cli/clear.py` & `perke-0.4.2/perke/cli/clear.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/__init__.py` & `perke-0.4.2/perke/unsupervised/graph_based/__init__.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/multipartite_rank.py` & `perke-0.4.2/perke/unsupervised/graph_based/multipartite_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         Initializes  MultipartiteRank.
 
         Parameters
         ----------
         valid_pos_tags:
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'ADJ'}`.
         """
         super().__init__(valid_pos_tags)
         self.topic_ids: Dict[str, int] = {}
         self.graph: nx.DiGraph = nx.DiGraph()
 
     def _cluster_topics(
         self,
```

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/position_rank.py` & `perke-0.4.2/perke/unsupervised/graph_based/position_rank.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,16 +38,18 @@
         """
         Initializes PositionRank.
 
         Parameters
         ----------
         valid_pos_tags:
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'NOUN,EZ', 'ADJ', 'ADJ,EZ'}`.
         """
+        if valid_pos_tags is None:
+            valid_pos_tags = {'NOUN', 'NOUN,EZ', 'ADJ', 'ADJ,EZ'}
         super().__init__(valid_pos_tags)
         self.positions: DefaultDict[str, float] = defaultdict(float)
 
     def select_candidates(
         self,
         grammar: Optional[str] = None,
         maximum_length: int = 3,
@@ -62,30 +64,29 @@
         Parameters
         ----------
         grammar:
             Grammar defining part of speech patterns of noun phrases,
             defaults to::
                 r\"""
                 NP:
-                    <P>{<N>}<V>
+                    {<NOUN>}<VERB>
                 NP:
-                    {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                    <N>}{<.*e?>.
+                    {<DET(,EZ)?|NOUN(,EZ)?|NUM(,EZ)?|ADJ(,EZ)|PRON><DET(,EZ)|NOUN(,EZ)|NUM(,EZ)|ADJ(,EZ)|PRON>*}
+                    <NOUN>}{<.*(,EZ)?>
                 \"""
-
         maximum_length: `int`
             Maximum length in words of the candidate, defaults to `3`.
         """
         if grammar is None:
             grammar = r"""
                 NP:
-                    <P>{<N>}<V>
+                    {<NOUN>}<VERB>
                 NP:
-                    {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                    <N>}{<.*e?>
+                    {<DET(,EZ)?|NOUN(,EZ)?|NUM(,EZ)?|ADJ(,EZ)|PRON><DET(,EZ)|NOUN(,EZ)|NUM(,EZ)|ADJ(,EZ)|PRON>*}
+                    <NOUN>}{<.*(,EZ)?>
             """
 
         # Select sequence of noun phrases with given pattern
         self._select_candidates_with_grammar(grammar=grammar)
 
         self._filter_candidates(maximum_length)
```

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/single_rank.py` & `perke-0.4.2/perke/unsupervised/graph_based/single_rank.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """
         Initializes SingleRank.
 
         Parameters
         ----------
         valid_pos_tags:
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'ADJ'}`.
         """
         super().__init__(valid_pos_tags)
         self.graph_edges_are_weighted: bool = True
 
     def _build_word_graph(self, window_size: int = 10) -> None:
         """
         Builds a graph representation of the text just like TextRank
```

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/text_rank.py` & `perke-0.4.2/perke/unsupervised/graph_based/text_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         """
         Initializes TextRank.
 
         Parameters
         ----------
         valid_pos_tags:
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'ADJ'}`.
         """
         super().__init__(valid_pos_tags)
         self.graph: nx.Graph = nx.Graph()
         self.graph_edges_are_weighted: bool = False
 
     def select_candidates(self) -> None:
         """
```

### Comparing `perke-0.4.1/perke/unsupervised/graph_based/topic_rank.py` & `perke-0.4.2/perke/unsupervised/graph_based/topic_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         """
         Initializes TopicRank.
 
         Parameters
         ----------
         valid_pos_tags: `set[str]`, optional
             Set of valid part of speech tags, defaults to nouns and
-            adjectives. I.e. `{'N', 'Ne', 'AJ', 'AJe'}`.
+            adjectives. I.e. `{'NOUN', 'ADJ'}`.
         """
         super().__init__(valid_pos_tags)
         self.graph: nx.Graph = nx.Graph()
         self.topics: List[List[str]] = []
 
     def select_candidates(self) -> None:
         """
```

### Comparing `perke-0.4.1/perke/utils/functions.py` & `perke-0.4.2/perke/utils/functions.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/perke.egg-info/PKG-INFO` & `perke-0.4.2/perke.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perke
-Version: 0.4.1
+Version: 0.4.2
 Summary: A keyphrase extractor for Persian
 Home-page: https://github.com/alirezatheh/perke
 Author: Alireza Hosseini
 Author-email: alirezatheh@gmail.com
 Project-URL: Bug Tracker, https://github.com/alirezatheh/perke/issues
 Project-URL: Documentation, https://perke.readthedocs.io
 Project-URL: Source Code, https://github.com/alirezatheh/perke
@@ -22,14 +22,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: Persian
 Requires-Python: >=3.8
@@ -37,15 +38,15 @@
 License-File: LICENSE
 
 # Perke
 [![tests](https://github.com/alirezatheh/perke/workflows/tests/badge.svg)](https://github.com/alirezatheh/perke/actions/workflows/tests.yaml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/AlirezaTheH/perke/main.svg)](https://results.pre-commit.ci/latest/github/alirezatheh/perke/main)
 [![PyPI Version](https://img.shields.io/pypi/v/perke)](https://pypi.python.org/pypi/perke)
 [![Python Versions](https://img.shields.io/pypi/pyversions/perke)](https://pypi.org/project/perke)
-[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/latest/?badge=stable)
+[![Documentation Status](https://readthedocs.org/projects/perke/badge/?version=stable)](https://perke.readthedocs.io/en/stable/?badge=stable)
 
 Perke is a Python keyphrase extraction package for Persian language. It
 provides an end-to-end keyphrase extraction pipeline in which each component
 can be easily modified or extended to develop new models.
 
 ## Installation
 - The easiest way to install is from PyPI:
```

### Comparing `perke-0.4.1/perke.egg-info/SOURCES.txt` & `perke-0.4.2/perke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perke-0.4.1/setup.py` & `perke-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
         'Natural Language :: Persian',
     ],
```

