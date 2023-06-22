# Comparing `tmp/torch_grammar-0.2.0.tar.gz` & `tmp/torch_grammar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.2.0.tar", max compression
+gzip compressed data, was "torch_grammar-0.2.1.tar", max compression
```

## Comparing `torch_grammar-0.2.0.tar` & `torch_grammar-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.2.0/README.md
--rw-r--r--   0        0        0      642 2023-06-22 19:34:23.149928 torch_grammar-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.2.0/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.2.0/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6363 2023-06-22 19:33:29.135187 torch_grammar-0.2.0/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.2.0/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 torch_grammar-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.2.1/README.md
+-rw-r--r--   0        0        0      588 2023-06-22 19:36:26.594443 torch_grammar-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.2.1/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.2.1/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6363 2023-06-22 19:33:29.135187 torch_grammar-0.2.1/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.2.1/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 torch_grammar-0.2.1/PKG-INFO
```

### Comparing `torch_grammar-0.2.0/README.md` & `torch_grammar-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.2.0/pyproject.toml` & `torch_grammar-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "torch-grammar"
-version = "0.2.0"
+version = "0.2.1"
 description = "Restrict LLM generations to a context-free grammar"
 authors = ["Burke Libbey <burke.libbey@shopify.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_grammar"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-torch = "^2.0.1"
-transformers = "^4.30.2"
+torch = "^2.0.0"
+transformers = "^4.29"
 sentencepiece = "^0.1.99"
-black = {extras = ["jupyter"], version = "^23.3.0"}
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.272"
 black = "^23.3.0"
 pytest = "^7.3.2"
 fire = "^0.5.0"
```

### Comparing `torch_grammar-0.2.0/torch_grammar/grammar_parser.py` & `torch_grammar-0.2.1/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.2.0/torch_grammar/grammar_sampler.py` & `torch_grammar-0.2.1/torch_grammar/grammar_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.2.0/torch_grammar/token_trie.py` & `torch_grammar-0.2.1/torch_grammar/token_trie.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.2.0/PKG-INFO` & `torch_grammar-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.2.0
+Version: 0.2.1
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: transformers (>=4.30.2,<5.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: transformers (>=4.29,<5.0)
 Description-Content-Type: text/markdown
 
 # torch-grammar
 
 **Alpha Quality: This might do what you want. It's likely to not do what you
 want. Please open issues!**
```

