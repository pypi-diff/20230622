# Comparing `tmp/torch_grammar-0.1.1.tar.gz` & `tmp/torch_grammar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.1.1.tar", max compression
+gzip compressed data, was "torch_grammar-0.2.0.tar", max compression
```

## Comparing `torch_grammar-0.1.1.tar` & `torch_grammar-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.1.1/README.md
--rw-r--r--   0        0        0      643 2023-06-20 18:58:38.653428 torch_grammar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.1.1/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.1.1/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6435 2023-06-20 18:49:37.212473 torch_grammar-0.1.1/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.1.1/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 torch_grammar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.2.0/README.md
+-rw-r--r--   0        0        0      642 2023-06-22 19:34:23.149928 torch_grammar-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.2.0/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.2.0/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6363 2023-06-22 19:33:29.135187 torch_grammar-0.2.0/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.2.0/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 torch_grammar-0.2.0/PKG-INFO
```

### Comparing `torch_grammar-0.1.1/README.md` & `torch_grammar-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.1/pyproject.toml` & `torch_grammar-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "torch-grammar"
-version = "0.1.1"
+version = "0.2.0"
 description = "Restrict LLM generations to a context-free grammar"
 authors = ["Burke Libbey <burke.libbey@shopify.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_grammar"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 torch = "^2.0.1"
 transformers = "^4.30.2"
 sentencepiece = "^0.1.99"
 black = {extras = ["jupyter"], version = "^23.3.0"}
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.272"
```

### Comparing `torch_grammar-0.1.1/torch_grammar/grammar_parser.py` & `torch_grammar-0.2.0/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.1/torch_grammar/grammar_sampler.py` & `torch_grammar-0.2.0/torch_grammar/grammar_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
         self.grammar = grammar
         self.stacks = grammar.init_stacks()
         self.last_size = None
 
     def accept_token(self, token):
         self.stacks = self.grammar.accept_token(token, self.stacks)
 
+    # TODO: batching
     def __call__(self, input_ids, scores):
         if self.last_size is None:
-            self.query_width = len(input_ids[0])
             pass
         elif len(input_ids[0]) == self.last_size + 1:
             self.stacks = self.grammar.accept_token(input_ids[0][-1], self.stacks)
         else:
             raise "Input size changed"
 
         # TODO: the <s> token should be accounted for directly rather than just
         # dropped here...
-        self.grammar.filter_logits(input_ids[0][self.query_width:], scores, self.stacks)
+        self.grammar.filter_logits(scores[0], self.stacks)
 
         self.last_size = len(input_ids[0])
         return scores
 
 
 class GrammarSampler:
     def __init__(self, input_text, start_rule_name, tokenizer):
@@ -187,17 +187,17 @@
 
         et = time.time() - st
         x = torch.tensor(accepts, dtype=torch.bool)
         self.tt += et
         self.nt += 1
         return x
 
-    def filter_logits(self, input_ids, logits, stacks):
+    def filter_logits(self, logits, stacks):
         # resolve each stack to a tensor of True/False for each token
         # indicating acceptance
         acceptance = torch.cat(
             [self.token_acceptance_for_stack(tuple(stack)) for stack in stacks]
         )
         # Merge stacks: any True => True
         acceptance = acceptance.reshape(len(stacks), -1).any(dim=0)
         # Logits to -inf where False
-        logits[0, ~acceptance] = -inf
+        logits[~acceptance] = -inf
```

### Comparing `torch_grammar-0.1.1/torch_grammar/token_trie.py` & `torch_grammar-0.2.0/torch_grammar/token_trie.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.1/PKG-INFO` & `torch_grammar-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.1.1
+Version: 0.2.0
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
```

