# Comparing `tmp/wordview-0.2.4.tar.gz` & `tmp/wordview-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.2.4.tar", max compression
+gzip compressed data, was "wordview-0.3.0.tar", max compression
```

## Comparing `wordview-0.2.4.tar` & `wordview-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      867 2023-05-28 14:55:33.259579 wordview-0.2.4/CHANGES.rst
--rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.4/LICENSE
--rw-r--r--   0        0        0     4638 2023-05-28 14:58:06.375929 wordview-0.2.4/README.rst
--rw-r--r--   0        0        0      877 2023-05-28 14:51:21.658364 wordview-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-28 13:04:33.316548 wordview-0.2.4/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.4/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.4/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.4/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.4/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.4/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-05-28 13:04:33.317278 wordview-0.2.4/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-28 10:30:16.290129 wordview-0.2.4/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-05-28 10:30:16.291853 wordview-0.2.4/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-05-28 10:30:16.292732 wordview-0.2.4/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.4/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.4/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-05-28 13:04:33.317988 wordview-0.2.4/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-05-28 10:30:16.293548 wordview-0.2.4/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-05-19 15:06:13.517119 wordview-0.2.4/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 wordview-0.2.4/setup.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-06-22 10:25:56.687295 wordview-0.3.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-22 10:25:56.687295 wordview-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-22 10:25:56.687295 wordview-0.3.0/README.rst
+-rw-r--r--   0        0        0      873 2023-06-22 10:26:22.163890 wordview-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.0/PKG-INFO
```

### Comparing `wordview-0.2.4/CHANGES.rst` & `wordview-0.3.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/LICENSE` & `wordview-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/README.rst` & `wordview-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/pyproject.toml` & `wordview-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.2.4"
+version = "0.3.0"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
@@ -26,12 +26,12 @@
 pytest = ">=7.1"
 pytest-cov = ">=3.0.0"
 ipython = ">=8.4.0"
 sphinx = ">=v6.1.3"
 sphinx-rtd-theme= "1.2.1"
 
 [tool.poetry.scripts]
-script_download = "wordview.bin.downloads:download_nltk_req"
+nltk_download_script = "bin.downloads:download_nltk_req"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wordview-0.2.4/wordview/anomaly/gaussianize.py` & `wordview-0.3.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/anomaly/normaldist.py` & `wordview-0.3.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/clustering/cluster.py` & `wordview-0.3.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/mwes/am.py` & `wordview-0.3.0/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/mwes/mwe.py` & `wordview-0.3.0/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/mwes/mwe_utils.py` & `wordview-0.3.0/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/preprocessing/cleaning.py` & `wordview-0.3.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/text_analysis/core.py` & `wordview-0.3.0/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/wordview/text_analysis/wrapper.py` & `wordview-0.3.0/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.4/setup.py` & `wordview-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wordview
+Version: 0.3.0
+Summary: Wordview is a Python package for text analysis.
+License: MIT
+Keywords: nlp,text analysis,statistics
+Author: meghdadFar
+Author-email: meghdad.farahmand@gmail.com
+Requires-Python: >=3.9,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: langdetect (>=1.0.9)
+Requires-Dist: nltk (==3.6.6)
+Requires-Dist: pandas (==2.0.1)
+Requires-Dist: plotly (==5.5.0)
+Requires-Dist: scikit-learn (==1.2.2)
+Requires-Dist: scipy (==1.10.0)
+Requires-Dist: sentence-transformers (==2.2.2)
+Requires-Dist: tabulate (==0.9.0)
+Requires-Dist: tqdm (==4.62.3)
+Requires-Dist: wordcloud (==1.9.1.1)
+Description-Content-Type: text/x-rst
+
+Wordview (Work In Progress)
+###########################
+
+|PyPI version|
+
+|Python 3.9|
+
+Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
+Wordview's Python API is open-source and available under the `MIT
+license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
+offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
+more information about this framework.
+
+|text_analysis_cover|
+
+
+Usage
+######
+
+Install the package via ``pip``:
+
+``pip install wordview``
+
+To explore various features and functionalities, consult the documentation pages. The following sections
+present a high-level description of Wordview's features and functionalities. For details, tutorials and worked examples, corresponding 
+documentation pages are linked in each section.
+
+
+Exploratory Data Analysis (EDA)
+###############################
+
+Wordview presents many statistics about your data in form of plots and tables allowing you to 
+have both a high-level and detailed overview of your data. For instance, which languages
+are present in your dataset, how many unique words and unique words are there in your dataset, what percentage 
+of them are Adjectives, Nouns or Verbs, what are the most common POS tags, etc. Wordview also provides several statistics for labels in labeled datasets.
+
+
+Text Analysis
+*************
+Using this feature, you can have an overview of your text data in terms of various statistics, plots and distribution.
+See `text analysis documentation pages <./docs/source/textstats.rst>`__  for usage and examples.
+
+
+Label Analysis
+**************
+Wordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.
+See `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.
+
+
+Feature Extraction
+###################
+
+Wordview has various functionalities for feature extraction from text, including Multiword Expressions (MWEs), clusters, anomalies and 
+outliers, and more. See the following sections as well as the linked documentation page in each section for details.
+
+Multiword Expressions
+*********************
+
+Multiword Expressions (MWEs) are phrases that can be treated as a single
+semantic unit. E.g. *swimming pool* and *climate change*. MWEs have
+application in different areas including: parsing, language models,
+language generation, terminology extraction, and topic models. Wordview can extract different types of MWEs from text.
+See `MWEs documentation page <./docs/source/mwes.rst>`__ for usage and examples.
+
+Anomalies and Outliers
+**********************
+
+Anomalies and outliers have wide applications in Machine Learning. While in
+some cases, you can capture them and remove them from the data to improve the
+performance of a downstream ML model, in other cases, they become the data points
+of interest where we endeavor to find them in order to shed light into our data.
+
+Wordview offers several anomaly and outlier detection functions.
+See `anomalies documentation page <./docs/source/anomalies.rst>`__ for usage and examples.
+
+
+Clusters
+*********
+Clustering can be used to identify different groups of documents with similar information, in an unsupervised fashion.
+Despite it's ability to provide valuable insights into your data, you do not need labeled data for clustering. See
+`wordview`'s `clustering documentation page <./docs/source/clustering.rst>`__ for usage and examples.
+
+
+Utilities
+#########
+
+Wordview offers a number of utility functions that you can use for common pre and post processing tasks in NLP. 
+See `utilities documentation page <./docs/source/utilities.rst>`__ for usage and examples.
+
+Contributing
+############
+
+Thank you for contributing to wordview! We and the users of this repo
+appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
+
+
+.. |PyPI version| image:: https://badge.fury.io/py/wordview.svg
+    :target: https://badge.fury.io/py/wordview
+
+.. |Python 3.9| image:: https://img.shields.io/badge/python-3.9-blue.svg
+   :target: https://www.python.org/downloads/release/python-390/
+.. |verbs| image:: docs/figs/verbs.png
+.. |nouns| image:: docs/figs/nouns.png
+.. |adjs| image:: docs/figs/adjectives.png
+.. |doclen| image:: docs/figs/doclen.png
+.. |wordszipf| image:: docs/figs/wordszipf.png
+.. |labels| image:: docs/figs/labels.png
+.. |cover| image:: docs/figs/abstract_cover_2.png
+.. |clustering_cover| image:: docs/figs/clustering_cover.png
+.. |text_analysis_cover| image:: docs/figs/text_analysis.png
 
-packages = \
-['wordview',
- 'wordview.anomaly',
- 'wordview.clustering',
- 'wordview.mwes',
- 'wordview.preprocessing',
- 'wordview.text_analysis']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['langdetect>=1.0.9',
- 'nltk==3.6.6',
- 'pandas==2.0.1',
- 'plotly==5.5.0',
- 'scikit-learn==1.2.2',
- 'scipy==1.10.0',
- 'sentence-transformers==2.2.2',
- 'tabulate==0.9.0',
- 'tqdm==4.62.3',
- 'wordcloud==1.9.1.1']
-
-entry_points = \
-{'console_scripts': ['script_download = '
-                     'wordview.bin.downloads:download_nltk_req']}
-
-setup_kwargs = {
-    'name': 'wordview',
-    'version': '0.2.4',
-    'description': 'Wordview is a Python package for text analysis.',
-    'long_description': "Wordview (Work In Progress)\n###########################\n\n|PyPI version|\n\n|Python 3.9|\n\nWordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.\nWordview's Python API is open-source and available under the `MIT\nlicense <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,\noffer a framework on top of Wordview for enterprise use under a commercial license. See this page for\nmore information about this framework.\n\n|text_analysis_cover|\n\n\nUsage\n######\n\nInstall the package via ``pip``:\n\n``pip install wordview``\n\nTo explore various features and functionalities, consult the documentation pages. The following sections\npresent a high-level description of Wordview's features and functionalities. For details, tutorials and worked examples, corresponding \ndocumentation pages are linked in each section.\n\n\nExploratory Data Analysis (EDA)\n###############################\n\nWordview presents many statistics about your data in form of plots and tables allowing you to \nhave both a high-level and detailed overview of your data. For instance, which languages\nare present in your dataset, how many unique words and unique words are there in your dataset, what percentage \nof them are Adjectives, Nouns or Verbs, what are the most common POS tags, etc. Wordview also provides several statistics for labels in labeled datasets.\n\n\nText Analysis\n*************\nUsing this feature, you can have an overview of your text data in terms of various statistics, plots and distribution.\nSee `text analysis documentation pages <./docs/source/textstats.rst>`__  for usage and examples.\n\n\nLabel Analysis\n**************\nWordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.\nSee `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.\n\n\nFeature Extraction\n###################\n\nWordview has various functionalities for feature extraction from text, including Multiword Expressions (MWEs), clusters, anomalies and \noutliers, and more. See the following sections as well as the linked documentation page in each section for details.\n\nMultiword Expressions\n*********************\n\nMultiword Expressions (MWEs) are phrases that can be treated as a single\nsemantic unit. E.g. *swimming pool* and *climate change*. MWEs have\napplication in different areas including: parsing, language models,\nlanguage generation, terminology extraction, and topic models. Wordview can extract different types of MWEs from text.\nSee `MWEs documentation page <./docs/source/mwes.rst>`__ for usage and examples.\n\nAnomalies and Outliers\n**********************\n\nAnomalies and outliers have wide applications in Machine Learning. While in\nsome cases, you can capture them and remove them from the data to improve the\nperformance of a downstream ML model, in other cases, they become the data points\nof interest where we endeavor to find them in order to shed light into our data.\n\nWordview offers several anomaly and outlier detection functions.\nSee `anomalies documentation page <./docs/source/anomalies.rst>`__ for usage and examples.\n\n\nClusters\n*********\nClustering can be used to identify different groups of documents with similar information, in an unsupervised fashion.\nDespite it's ability to provide valuable insights into your data, you do not need labeled data for clustering. See\n`wordview`'s `clustering documentation page <./docs/source/clustering.rst>`__ for usage and examples.\n\n\nUtilities\n#########\n\nWordview offers a number of utility functions that you can use for common pre and post processing tasks in NLP. \nSee `utilities documentation page <./docs/source/utilities.rst>`__ for usage and examples.\n\nContributing\n############\n\nThank you for contributing to wordview! We and the users of this repo\nappreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.\n\n\n.. |PyPI version| image:: https://badge.fury.io/py/wordview.svg\n    :target: https://badge.fury.io/py/wordview\n\n.. |Python 3.9| image:: https://img.shields.io/badge/python-3.9-blue.svg\n   :target: https://www.python.org/downloads/release/python-390/\n.. |verbs| image:: docs/figs/verbs.png\n.. |nouns| image:: docs/figs/nouns.png\n.. |adjs| image:: docs/figs/adjectives.png\n.. |doclen| image:: docs/figs/doclen.png\n.. |wordszipf| image:: docs/figs/wordszipf.png\n.. |labels| image:: docs/figs/labels.png\n.. |cover| image:: docs/figs/abstract_cover_2.png\n.. |clustering_cover| image:: docs/figs/clustering_cover.png\n.. |text_analysis_cover| image:: docs/figs/text_analysis.png\n\n\n",
-    'author': 'meghdadFar',
-    'author_email': 'meghdad.farahmand@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.11',
-}
 
 
-setup(**setup_kwargs)
```

