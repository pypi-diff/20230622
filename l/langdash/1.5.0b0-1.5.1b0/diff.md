# Comparing `tmp/langdash-1.5.0b0.tar.gz` & `tmp/langdash-1.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.5.0b0.tar", last modified: Thu Jun 22 00:31:24 2023, max compression
+gzip compressed data, was "langdash-1.5.1b0.tar", last modified: Thu Jun 22 20:28:12 2023, max compression
```

## Comparing `langdash-1.5.0b0.tar` & `langdash-1.5.1b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.989141 langdash-1.5.0b0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.5.0b0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.5.0b0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-22 00:31:24.985141 langdash-1.5.0b0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.5.0b0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.981141 langdash-1.5.0b0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-22 00:31:04.000000 langdash-1.5.0b0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.985141 langdash-1.5.0b0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.5.0b0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.5.0b0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9520 2023-06-19 07:37:15.000000 langdash-1.5.0b0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.5.0b0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.981141 langdash-1.5.0b0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.5.0b0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.5.0b0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6625 2023-06-19 07:37:15.000000 langdash-1.5.0b0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1321 2023-06-19 07:37:15.000000 langdash-1.5.0b0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.5.0b0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7473 2023-06-22 00:31:04.000000 langdash-1.5.0b0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.985141 langdash-1.5.0b0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.5.0b0/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.985141 langdash-1.5.0b0/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.5.0b0/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.5.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.985141 langdash-1.5.0b0/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.5.0b0/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.5.0b0/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.5.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.5.0b0/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.5.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.5.0b0/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5084 2023-06-21 10:26:00.000000 langdash-1.5.0b0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4744 2023-06-13 05:07:37.000000 langdash-1.5.0b0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.5.0b0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     9027 2023-06-22 00:31:04.000000 langdash-1.5.0b0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.5.0b0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-06-13 05:07:37.000000 langdash-1.5.0b0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.5.0b0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.5.0b0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.981141 langdash-1.5.0b0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.5.0b0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.5.0b0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.5.0b0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.5.0b0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 00:31:24.985141 langdash-1.5.0b0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-22 00:31:24.000000 langdash-1.5.0b0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-06-22 00:31:24.000000 langdash-1.5.0b0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-22 00:31:24.000000 langdash-1.5.0b0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-22 00:31:24.000000 langdash-1.5.0b0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-22 00:31:24.000000 langdash-1.5.0b0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-22 00:31:24.989141 langdash-1.5.0b0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.5.0b0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/
+-rw-r--r--   0 user      (1000) user      (1000)    10786 2023-06-06 08:29:05.000000 langdash-1.5.1b0/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-06-06 08:29:05.000000 langdash-1.5.1b0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3727 2023-06-22 20:28:12.160025 langdash-1.5.1b0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2788 2023-06-22 20:23:51.000000 langdash-1.5.1b0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/
+-rw-r--r--   0 user      (1000) user      (1000)       78 2023-06-22 20:26:24.000000 langdash-1.5.1b0/langdash/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/chains/
+-rw-r--r--   0 user      (1000) user      (1000)      178 2023-06-11 00:29:26.000000 langdash-1.5.1b0/langdash/chains/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    14686 2023-06-12 17:23:06.000000 langdash-1.5.1b0/langdash/chains/chains.py
+-rw-r--r--   0 user      (1000) user      (1000)     9520 2023-06-15 22:53:06.000000 langdash-1.5.1b0/langdash/chains/nodes.py
+-rw-r--r--   0 user      (1000) user      (1000)      253 2023-06-11 01:18:11.000000 langdash-1.5.1b0/langdash/chains/typing.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/classify/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.5.1b0/langdash/classify/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2032 2023-06-12 17:25:45.000000 langdash-1.5.1b0/langdash/classify/token_qa.py
+-rw-r--r--   0 user      (1000) user      (1000)     6625 2023-06-15 18:51:05.000000 langdash-1.5.1b0/langdash/core.py
+-rw-r--r--   0 user      (1000) user      (1000)     1321 2023-06-15 23:04:37.000000 langdash-1.5.1b0/langdash/infer.py
+-rw-r--r--   0 user      (1000) user      (1000)     1555 2023-06-07 00:55:46.000000 langdash-1.5.1b0/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)     7473 2023-06-22 00:05:04.000000 langdash-1.5.1b0/langdash/llm_session.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/models/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:46:41.000000 langdash-1.5.1b0/langdash/models/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/models/_mixins/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:30.000000 langdash-1.5.1b0/langdash/models/_mixins/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3412 2023-06-20 01:17:39.000000 langdash-1.5.1b0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/models/_tokenizer/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:39.000000 langdash-1.5.1b0/langdash/models/_tokenizer/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1886 2023-06-13 06:51:21.000000 langdash-1.5.1b0/langdash/models/_tokenizer/_bpe.py
+-rw-r--r--   0 user      (1000) user      (1000)     1532 2023-06-13 06:51:21.000000 langdash-1.5.1b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     2269 2023-06-20 00:04:11.000000 langdash-1.5.1b0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     1546 2023-06-21 19:49:14.000000 langdash-1.5.1b0/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)      664 2023-06-13 06:51:21.000000 langdash-1.5.1b0/langdash/models/_tokenizer/tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     5084 2023-06-20 01:34:02.000000 langdash-1.5.1b0/langdash/models/ctransformers.py
+-rw-r--r--   0 user      (1000) user      (1000)     4744 2023-06-13 06:51:21.000000 langdash-1.5.1b0/langdash/models/llama_cpp.py
+-rw-r--r--   0 user      (1000) user      (1000)      689 2023-06-13 06:46:41.000000 langdash-1.5.1b0/langdash/models/mock.py
+-rw-r--r--   0 user      (1000) user      (1000)     9027 2023-06-22 00:08:52.000000 langdash-1.5.1b0/langdash/models/rwkv_cpp.py
+-rw-r--r--   0 user      (1000) user      (1000)     1005 2023-06-13 06:46:41.000000 langdash-1.5.1b0/langdash/models/sentence_transformers.py
+-rw-r--r--   0 user      (1000) user      (1000)     5472 2023-06-13 06:51:21.000000 langdash-1.5.1b0/langdash/models/transformers.py
+-rw-r--r--   0 user      (1000) user      (1000)      837 2023-06-07 00:55:46.000000 langdash-1.5.1b0/langdash/response.py
+-rw-r--r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:38:13.000000 langdash-1.5.1b0/langdash/sampling.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash/search/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.5.1b0/langdash/search/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1135 2023-06-12 17:46:13.000000 langdash-1.5.1b0/langdash/search/embedding_search.py
+-rw-r--r--   0 user      (1000) user      (1000)     1118 2023-06-09 17:53:33.000000 langdash-1.5.1b0/langdash/search/engine.py
+-rw-r--r--   0 user      (1000) user      (1000)     2861 2023-06-15 19:40:11.000000 langdash-1.5.1b0/langdash/search/multichoice_search.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:28:12.160025 langdash-1.5.1b0/langdash.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3727 2023-06-22 20:28:12.000000 langdash-1.5.1b0/langdash.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1188 2023-06-22 20:28:12.000000 langdash-1.5.1b0/langdash.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-22 20:28:12.000000 langdash-1.5.1b0/langdash.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      199 2023-06-22 20:28:12.000000 langdash-1.5.1b0/langdash.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2023-06-22 20:28:12.000000 langdash-1.5.1b0/langdash.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-22 20:28:12.160025 langdash-1.5.1b0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1605 2023-06-22 20:17:04.000000 langdash-1.5.1b0/setup.py
```

### Comparing `langdash-1.5.0b0/LICENSE.txt` & `langdash-1.5.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/PKG-INFO` & `langdash-1.5.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.5.0b0
+Version: 1.5.1b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -80,15 +80,15 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: WizardLM (shortened Alpaca format without the first prompt line and `# Instruction:`), and Alpaca (the full format). You'll need to specify it for most of the other examples:
+Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
 
 ## License
```

### Comparing `langdash-1.5.0b0/README.md` & `langdash-1.5.1b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: WizardLM (shortened Alpaca format without the first prompt line and `# Instruction:`), and Alpaca (the full format). You'll need to specify it for most of the other examples:
+Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
 
 ## License
```

### Comparing `langdash-1.5.0b0/langdash/chains/chains.py` & `langdash-1.5.1b0/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/chains/nodes.py` & `langdash-1.5.1b0/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/classify/token_qa.py` & `langdash-1.5.1b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/core.py` & `langdash-1.5.1b0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/infer.py` & `langdash-1.5.1b0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/llm.py` & `langdash-1.5.1b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/llm_session.py` & `langdash-1.5.1b0/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.5.1b0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_tokenizer/_bpe.py` & `langdash-1.5.1b0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.5.1b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.5.1b0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.5.1b0/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.5.1b0/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/ctransformers.py` & `langdash-1.5.1b0/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/llama_cpp.py` & `langdash-1.5.1b0/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/mock.py` & `langdash-1.5.1b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/rwkv_cpp.py` & `langdash-1.5.1b0/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/sentence_transformers.py` & `langdash-1.5.1b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/models/transformers.py` & `langdash-1.5.1b0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/response.py` & `langdash-1.5.1b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/sampling.py` & `langdash-1.5.1b0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/search/embedding_search.py` & `langdash-1.5.1b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/search/engine.py` & `langdash-1.5.1b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash/search/multichoice_search.py` & `langdash-1.5.1b0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.0b0/langdash.egg-info/PKG-INFO` & `langdash-1.5.1b0/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.5.0b0
+Version: 1.5.1b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -80,15 +80,15 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: WizardLM (shortened Alpaca format without the first prompt line and `# Instruction:`), and Alpaca (the full format). You'll need to specify it for most of the other examples:
+Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
 
 ## License
```

### Comparing `langdash-1.5.0b0/setup.py` & `langdash-1.5.1b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         # Modules
         "embeddings": ["faiss-cpu"],
 
         # Backend
         "rwkv_cpp": ["tokenizers"],
         "llama_cpp": ["llama-cpp-python"],
         "transformers": ["transformers"],
-        "ctransformers": ["ctransformers @ git+https://git.mysymphony.jp.net/nana/ctransformers.git@efe0b31b65311f2ce4555bbd41616eddfb90d04d"],
+        "ctransformers": ["ctransformers-langdash"],
         "sentence_transformers": ["sentence_transformers"],
     },
 )
```

