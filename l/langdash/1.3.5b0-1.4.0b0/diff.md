# Comparing `tmp/langdash-1.3.5b0.tar.gz` & `tmp/langdash-1.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.3.5b0.tar", last modified: Wed Jun 14 22:44:35 2023, max compression
+gzip compressed data, was "langdash-1.4.0b0.tar", last modified: Mon Jun 19 07:37:26 2023, max compression
```

## Comparing `langdash-1.3.5b0.tar` & `langdash-1.4.0b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.744075 langdash-1.3.5b0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.5b0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.5b0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-14 22:44:35.744075 langdash-1.3.5b0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.5b0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.5b0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     8176 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.5b0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.5b0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.5b0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1150 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.5b0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.5b0/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.5b0/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3355 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.744075 langdash-1.3.5b0/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.5b0/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1810 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1564 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5135 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4744 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7586 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.5b0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.5b0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.5b0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1658 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-14 22:44:35.744075 langdash-1.3.5b0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.3.5b0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.376474 langdash-1.4.0b0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.4.0b0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.4.0b0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-19 07:37:26.376474 langdash-1.4.0b0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.4.0b0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.372474 langdash-1.4.0b0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.372474 langdash-1.4.0b0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.4.0b0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.4.0b0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9520 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.4.0b0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.368474 langdash-1.4.0b0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.4.0b0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.4.0b0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6625 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1321 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.4.0b0/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7361 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.376474 langdash-1.4.0b0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.4.0b0/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.376474 langdash-1.4.0b0/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.4.0b0/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3411 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.376474 langdash-1.4.0b0/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.4.0b0/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.4.0b0/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.4.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2029 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1564 2023-06-14 22:44:24.000000 langdash-1.4.0b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.4.0b0/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5080 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4744 2023-06-13 05:07:37.000000 langdash-1.4.0b0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.4.0b0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7586 2023-06-14 22:44:24.000000 langdash-1.4.0b0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.4.0b0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-06-13 05:07:37.000000 langdash-1.4.0b0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.4.0b0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.4.0b0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.372474 langdash-1.4.0b0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.4.0b0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.4.0b0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.4.0b0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.4.0b0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-19 07:37:26.372474 langdash-1.4.0b0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-19 07:37:26.000000 langdash-1.4.0b0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1658 2023-06-19 07:37:26.000000 langdash-1.4.0b0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-19 07:37:26.000000 langdash-1.4.0b0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-19 07:37:26.000000 langdash-1.4.0b0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-19 07:37:26.000000 langdash-1.4.0b0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-19 07:37:26.376474 langdash-1.4.0b0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.4.0b0/setup.py
```

### Comparing `langdash-1.3.5b0/LICENSE.txt` & `langdash-1.4.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/PKG-INFO` & `langdash-1.4.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.5b0
+Version: 1.4.0b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.5b0/README.md` & `langdash-1.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/chains/chains.py` & `langdash-1.4.0b0/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/chains/nodes.py` & `langdash-1.4.0b0/langdash/chains/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -99,30 +99,34 @@
 
   def __init__(
     self,
     ld: "Langdash",
     returns: str,
     end: Optional[Union[str, int]],
     padleft: str = "",
-    infer_args: Optional[InferArgs] = None
+    infer_args: Optional[InferArgs] = None,
+    end_is_token: bool = False,
   ):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
     self._infer_args = infer_args
+    self._end_is_token = end_is_token
 
   def __repr__(self):
     return f"<Returns arg={self._returns}>"
 
   def __call__(
     self, session: "LLMGenerationSession", args: "LDNodeArgs"
   ) -> "LDNodeGenerator":
     for i, respinfer in enumerate(
-      session.infer(end=self._end, args=self._infer_args)
+      session.infer(
+        end=self._end, args=self._infer_args, end_is_token=self._end_is_token
+      )
     ):
       if i == 0:
         if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       elif respinfer.tokid == -1:  # end
         if self._padleft and respinfer.running_infer.startswith(self._padleft):
           respinfer.running_infer = respinfer.running_infer[len(self
@@ -134,55 +138,72 @@
 class _LDChoiceTokensCache:
   choices_tokens: List[List[int]]
   heal_prefix: str
 
 
 class LDChoice(LDNode):
   """ Choice node """
+  _token_cache: Optional[WeakKeyDictionary["LLMGenerationSession",
+                                           _LDChoiceTokensCache]]
 
   def __init__(
     self,
     ld: "Langdash",
     returns: str,
-    choices: List[str],
+    choices: Union[str, List[str]],
     padleft: str = "",
     padright: str = "",
     argmax: bool = False
   ):
     super().__init__(ld)
     self._returns = returns
     self._choices = choices
     self._padleft = padleft
     self._padright = padright
     self._argmax = argmax
 
-    self._choices_preprocessed = [
-      f"{self._padleft}{choice}{self._padright}" for choice in self._choices
-    ]
-    self._token_cache: WeakKeyDictionary[
-      "LLMGenerationSession", _LDChoiceTokensCache] = WeakKeyDictionary()
+    if isinstance(self._choices, str):
+      self._choices_preprocessed = []
+      self._token_cache = None
+    else:
+      self._choices_preprocessed = self._preprocess_choices(self._choices)
+      self._token_cache = WeakKeyDictionary()
 
   def __repr__(self):
     return f"<Choices {self._returns}>"
 
+  def _preprocess_choices(self, choices: List[str]) -> List[str]:
+    if self._padleft or self._padright:
+      return [f"{self._padleft}{choice}{self._padright}" for choice in choices]
+    else:
+      return choices
+
+  def _get_token_cache_once(
+    self, session: "LLMGenerationSession", heal_prefix: str,
+    choices_preprocessed: List[str]
+  ) -> _LDChoiceTokensCache:
+    return _LDChoiceTokensCache(
+      choices_tokens=[
+        session.tokenize(heal_prefix + text) for text in choices_preprocessed
+      ],
+      heal_prefix=heal_prefix
+    )
+
   def _get_token_cache(
     self, session: "LLMGenerationSession", heal_prefix: str
   ) -> _LDChoiceTokensCache:
+    assert self._token_cache is not None
     try:
       cache = self._token_cache[session]
       if cache.heal_prefix == heal_prefix:
         return cache
     except KeyError:
       pass
-    cache = _LDChoiceTokensCache(
-      choices_tokens=[
-        session.tokenize(heal_prefix + text)
-        for text in self._choices_preprocessed
-      ],
-      heal_prefix=heal_prefix
+    cache = self._get_token_cache_once(
+      session, heal_prefix, self._choices_preprocessed
     )
     self._token_cache[session] = cache
     return cache
 
   def __call__(
     self, session: "LLMGenerationSession", args: "LDNodeArgs"
   ) -> "LDNodeGenerator":
@@ -191,15 +212,33 @@
     heal_prefix: str = ""
     if session.token_healing and \
       isinstance(session, LLMGenerationSessionForRawText) and \
       session._next_token is not None:
       heal_prefix = session._next_token[1]
       session._next_token = None
 
-    cache = self._get_token_cache(session, heal_prefix)
+    if isinstance(self._choices, str):
+      try:
+        choices = args[self._choices]
+      except KeyError:
+        raise KeyError(
+          f"Expected \"{self._choices}\" argument to be passed into chain."
+        )
+
+      if not isinstance(choices, list) or not all(
+        isinstance(choice, str) for choice in choices
+      ):
+        raise TypeError(f"Expected \"{self._choices}\" to be List[str]")
+
+      cache = self._get_token_cache_once(
+        session, heal_prefix, self._preprocess_choices(choices)
+      )
+    else:  # List[str]
+      choices = self._choices
+      cache = self._get_token_cache(session, heal_prefix)
     choices_tokens: List[Tuple[int, List[int]]] = [
       (i, list(reversed(tokens)))
       for i, tokens in enumerate(cache.choices_tokens)
     ]
 
     while len(choices_tokens) > 1:
       probs = session.next_token_probs()
@@ -231,15 +270,15 @@
         if tokens[-1] == tokid:
           tokens.pop()
           choices_tokens.append((i, tokens))
 
     choice, remaining = choices_tokens.pop()
     for tokid in reversed(remaining):
       session.inject(tokid)
-    yield RespInfer(-1, "", self._choices[choice])
+    yield RespInfer(-1, "", choices[choice])
     yield RespInject(tokens_counter=len(cache.choices_tokens[choice]))
 
 
 class LDRepeat(LDNode):
   """ Repeat node """
 
   def __init__(
```

### Comparing `langdash-1.3.5b0/langdash/classify/token_qa.py` & `langdash-1.4.0b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/core.py` & `langdash-1.4.0b0/langdash/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 
   def text(self, *args, **kwargs):
     """
     Creates a raw text node.
     
     Args:
       text (str): The raw text.
+      add_special_tokens (bool):
+        Whether to treat text as containing special tokens or not.
+        Optional. Defaults to False.
       
     Returns:
       The text node.
     """
     return chains.LDText(self, *args, **kwargs)
 
   def format_args(self, *args, **kwargs):
@@ -167,15 +170,17 @@
 
   def choice(self, *args, **kwargs):
     """
     Creates a new choice node with the specified choices.
     
     Args:
       returns (str): The name of the return value.
-      choices (List[str]): List of choice strings
+      choices (Union[str, List[str]]):
+        Either the list of choice strings or the name of the argument
+        containing the list.
       padleft (str):
         Left padding for every choice string.
       padright (str):
         Right padding for every choice string.
     
     Returns:
       The choice node.
```

### Comparing `langdash-1.3.5b0/langdash/infer.py` & `langdash-1.4.0b0/langdash/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 @dataclass
 class InferArgs:
   """
   Data class for inference arguments.
   
   Attributes:
-    min_new_tokens: Minimum number of new tokens to generate
+    min_new_tokens:
+      Minimum number of new tokens to generate.
+      If this is set, the `end` argument passed to the session's infer method
+       will be interpreted as *a single token*. Special tokens count as an end token.
     max_new_tokens: Maximum number of new tokens to generate
     temperature: Temperature
     top_k: Top-K parameter. If set, generation defaults to top-K. Works with top_p
     top_p: Top-P parameter
     typical_mass: Mass parameter. If set, generation will use typical sampling
     max_rep_ctx: Maximum number of tokens to look back for repetition penalty
     rep_penalty: Repetition penalty, applied to logits for every repeated token
```

### Comparing `langdash-1.3.5b0/langdash/llm.py` & `langdash-1.4.0b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/llm_session.py` & `langdash-1.4.0b0/langdash/llm_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,39 +125,44 @@
     Returns the probabilities for next token.
     """
     raise NotImplementedError("next_token_probs")
 
   def flush_token(self):
     raise NotImplementedError("flush_token")
 
-  def _infer(self, end: Optional[Union[str, int]],
-             args: InferArgs) -> Generator[RespInfer, None, None]:
+  def _infer(
+    self, end: Optional[Union[str, int]], args: InferArgs, end_is_token: bool
+  ) -> Generator[RespInfer, None, None]:
     raise NotImplementedError("_infer")
 
   def infer(
     self,
     end: Optional[Union[str, int]],
-    args: Optional[InferArgs] = None
+    args: Optional[InferArgs] = None,
+    end_is_token: bool = False,
   ) -> Generator[RespInfer, None, None]:
     """
     Infer the next tokens from the input sequence.
 
     Args:
       end (Optional[Union[str, int]]):
         The end of the output sequence.
         If set to None, the output sequence will be generated until the maximum number of tokens is reached.
       args (Optional[InferArgs]):
         Optional inference parameters.
+      end_is_token (bool):
+        If set, the end string will be interpreted as a token.
+        Defaults to False.
         
     Returns:
       Inference response
     """
     if not args:
       args = self.default_infer_args
-    yield from self._infer(end, args)
+    yield from self._infer(end=end, args=args, end_is_token=end_is_token)
 
   def inject(
     self, text: Union[str, int], add_special_tokens: bool = False
   ) -> int:
     raise NotImplementedError("inject")
```

### Comparing `langdash-1.3.5b0/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.4.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     raise NotImplementedError("tokenize")
 
   def decode(self, tokids: List[int]) -> str:
     raise NotImplementedError("decode")
 
-  def _infer(self, end: Optional[Union[str, int]],
-             args: InferArgs) -> Generator[RespInfer, None, None]:
+  def _infer(
+    self, end: Optional[Union[str, int]], args: InferArgs, end_is_token: bool
+  ) -> Generator[RespInfer, None, None]:
     generated = ""
     buffered_tokens: Optional[BufferedToken] = None
     ctx: List[int] = []
 
     if isinstance(end, str):
       if len(end) == 0:
         end = self._model.eos_token
-      elif args.min_new_tokens > 0:
-        endtoks = self.tokenize(end)
+      elif end_is_token or args.min_new_tokens > 0:
+        endtoks = self.tokenize(end, add_special_tokens=True)
         assert len(endtoks) == 1
         end = endtoks[0]
 
     if self._logits is None:
       raise ValueError("no prompt provided")
 
     for i in range(args.max_new_tokens):
```

### Comparing `langdash-1.3.5b0/langdash/models/_tokenizer/_bpe.py` & `langdash-1.4.0b0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.4.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.4.0b0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from typing import List, Union, Optional, Generator
+import warnings
 from .tokenizer import Tokenizer, BufferedToken
 from ._bpe import decode as bpe_decode
 
 
 class HFTokenizer(Tokenizer):
   vocab: List[str]
 
   def __init__(self, tokenizer):
     self.tokenizer = tokenizer
-    assert not self.tokenizer.is_fast
-    assert self.tokenizer.errors == "strict"
-    if hasattr(self.tokenizer, "bpe"):
-      self.vocab = [
-        bpe_decode(token) for token in
-        self.tokenizer.convert_ids_to_tokens(range(self.tokenizer.vocab_size))
-      ]
-    else:
-      self.vocab = self.tokenizer.convert_ids_to_tokens(
-        range(self.tokenizer.vocab_size)
+    if self.tokenizer.is_fast:
+      warnings.warn(
+        "The `use_fast=False` parameter should be passed to the tokenizer to handle UTF-8 characters spanning multiple tokens."
       )
+      self.vocab = []
+    else:
+      assert self.tokenizer.errors == "strict"
+      if hasattr(self.tokenizer, "bpe"):
+        self.vocab = [
+          bpe_decode(token) for token in self.tokenizer
+          .convert_ids_to_tokens(range(self.tokenizer.vocab_size))
+        ]
+      else:
+        self.vocab = self.tokenizer.convert_ids_to_tokens(
+          range(self.tokenizer.vocab_size)
+        )
 
   def encode(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self.tokenizer.encode(text, add_special_tokens=add_special_tokens)
 
   def decode(self, tokens: List[int]) -> str:
     return self.tokenizer.decode(tokens)
```

### Comparing `langdash-1.3.5b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py` & `langdash-1.4.0b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.4.0b0/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/ctransformers.py` & `langdash-1.4.0b0/langdash/models/ctransformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,21 @@
   model: CTransformersLLM
   tokenizer: Tokenizer
   vocab: List[bytes]
   last_called_session: Optional[weakref.ref]
   eos_token: int
 
   def __init__(
-    self,
-    model_path: str,
-    transformers_tokenizer: Optional[Any] = None,
-    *args,
-    **kwargs
+    self, model_path: str, tokenizer: Optional[Any] = None, *args, **kwargs
   ):
     self.model = ctransformers.AutoModelForCausalLM.from_pretrained(
       model_path, **kwargs
     )
-    if transformers_tokenizer is not None:
-      self.tokenizer = HFTokenizer(transformers_tokenizer)
+    if tokenizer is not None:
+      self.tokenizer = HFTokenizer(tokenizer)
     else:
       mapping = [
         self.model.token_id_to_str(tokid)
         for tokid in range(self.model.vocab_size)
       ]
       self.tokenizer = BytesDictTokenizer(
         lambda text, **_k: self.model.tokenize(text),
```

### Comparing `langdash-1.3.5b0/langdash/models/llama_cpp.py` & `langdash-1.4.0b0/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/mock.py` & `langdash-1.4.0b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/rwkv_cpp.py` & `langdash-1.4.0b0/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/sentence_transformers.py` & `langdash-1.4.0b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/models/transformers.py` & `langdash-1.4.0b0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/response.py` & `langdash-1.4.0b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/sampling.py` & `langdash-1.4.0b0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/search/embedding_search.py` & `langdash-1.4.0b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/search/engine.py` & `langdash-1.4.0b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/langdash/search/multichoice_search.py` & `langdash-1.4.0b0/langdash/search/multichoice_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Generator, Callable, Tuple, List, Union
+from itertools import islice
 from langdash.chains import LDChainCached
 from langdash.search.engine import Engine
 
 
 def number_based_prompt(search: "MultichoiceSearch", key: int,
                         document: str) -> Tuple[str, str]:
   return str(key), f"{key}. {document}\n"
@@ -92,8 +93,8 @@
     doc_probs_with_text = list(
       zip(range(len(self._documents)), self._documents, doc_probs)
     )
     doc_probs_with_text.sort(key=lambda x: x[2], reverse=True)
     if max_documents == -1:
       yield from iter(doc_probs_with_text)
     else:
-      yield from iter(doc_probs_with_text[0:max_documents])
+      yield from islice(doc_probs_with_text, max_documents)
```

### Comparing `langdash-1.3.5b0/langdash.egg-info/PKG-INFO` & `langdash-1.4.0b0/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.5b0
+Version: 1.4.0b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.5b0/langdash.egg-info/SOURCES.txt` & `langdash-1.4.0b0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.5b0/setup.py` & `langdash-1.4.0b0/setup.py`

 * *Files identical despite different names*

