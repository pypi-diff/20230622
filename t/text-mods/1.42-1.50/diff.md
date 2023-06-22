# Comparing `tmp/text_mods-1.42.tar.gz` & `tmp/text_mods-1.50.tar.gz`

## Comparing `text_mods-1.42.tar` & `text_mods-1.50.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 text_mods-1.42/src/Example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.42/src/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.42/src/setup.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 text_mods-1.42/src/text_mods.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.42/LICENSE.txt
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 text_mods-1.42/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.42/pyproject.toml
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 text_mods-1.42/PKG-INFO
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 text_mods-1.50/src/Example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.50/src/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.50/src/setup.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 text_mods-1.50/src/text_mods.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.50/LICENSE.txt
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 text_mods-1.50/README.md
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.50/pyproject.toml
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 text_mods-1.50/PKG-INFO
```

### Comparing `text_mods-1.42/src/text_mods.py` & `text_mods-1.50/src/text_mods.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import string
 import random
 from typing import List
 from collections import Counter
 
 import nltk
 from nltk.corpus import stopwords, wordnet
-from nltk.tokenize import word_tokenize
+from nltk.tokenize import word_tokenize, sent_tokenize
 from nltk.stem import PorterStemmer, WordNetLemmatizer
 from nltk import pos_tag, ne_chunk
 from nltk.tree import Tree
 from functools import lru_cache
 
 from transformers import pipeline
 from googletrans import Translator
-from functools import lru_cache
 
 stemmer = PorterStemmer()
 lemmatizer = WordNetLemmatizer()
 
 STOPWORDS_LANGUAGE = 'english'
 stopwords = set(stopwords.words(STOPWORDS_LANGUAGE))
 
@@ -54,30 +53,30 @@
     return re.sub(html_pattern, '', text)
 
 def remove_punctuation(text: str) -> str:
     translator = str.maketrans('', '', string.punctuation)
     return text.translate(translator)
 
 def replace_with_first_synonym(text: str) -> str:
-    tokens = nltk.word_tokenize(text)
+    tokens = word_tokenize(text)
     new_text = [get_synonyms(token)[0] if get_synonyms(token) else token for token in tokens]
     return ' '.join(new_text)
 
 def replace_with_random_synonym(text: str, method: str) -> str:
-    tokens = nltk.word_tokenize(text)
+    tokens = word_tokenize(text)
     new_text = [random.choice(get_synonyms(token, method)) if get_synonyms(token, method) else token for token in tokens]
     return ' '.join(new_text)
 
 def count_word_frequencies(text: str) -> Counter:
-    tokens = nltk.word_tokenize(text)
+    tokens = word_tokenize(text)
     return Counter(tokens)
 
 def remove_stopwords(text: str) -> str:
     stop_words = set(stopwords.words(STOPWORDS_LANGUAGE))
-    tokens = nltk.word_tokenize(text)
+    tokens = word_tokenize(text)
     filtered_text = [token for token in tokens if token.lower() not in stop_words]
     return ' '.join(filtered_text)
 
 def summarize_text(text: str) -> str:
     summarizer = pipeline("summarization")
     summary = summarizer(text, max_length=100, min_length=30, do_sample=False)
     return summary[0]['summary']
@@ -112,7 +111,29 @@
     return text.lower()
 
 def make_capitalized(text: str) -> str:
     return text.title()
 
 def make_reversed(text: str) -> str:
     return text[::-1]
+
+translator = Translator()
+
+def translate_text(text: str, src_lang: str, dest_lang: str) -> str:
+    translation = translator.translate(text, src=src_lang, dest=dest_lang)
+    return translation.text
+
+def detect_language(text: str) -> str:
+    detection = translator.detect(text)
+    return detection.lang
+
+def tokenize_sentences(text: str) -> List[str]:
+    sentences = sent_tokenize(text)
+    return sentences
+
+def tokenize_words(text: str) -> List[str]:
+    words = word_tokenize(text)
+    return words
+
+def remove_numbers(text: str) -> str:
+    text_without_numbers = re.sub(r'\d+', '', text)
+    return text_without_numbers
```

### Comparing `text_mods-1.42/LICENSE.txt` & `text_mods-1.50/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text_mods-1.42/README.md` & `text_mods-1.50/README.md`

 * *Files identical despite different names*

### Comparing `text_mods-1.42/PKG-INFO` & `text_mods-1.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_mods
-Version: 1.42
+Version: 1.50
 Summary: This code defines a collection of functions for formatting and modifying text
 Project-URL: Homepage, https://github.com/Ilija-nik1/text_mods
 Author: I_N-01
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

