# Comparing `tmp/comex-0.1.2.tar.gz` & `tmp/comex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.1.2.tar", last modified: Fri Jun  2 11:56:52 2023, max compression
+gzip compressed data, was "comex-0.1.3.tar", last modified: Thu Jun 22 04:19:09 2023, max compression
```

## Comparing `comex-0.1.2.tar` & `comex-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-27 09:03:42.000000 comex-0.1.2/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)    11440 2023-06-02 11:56:52.920000 comex-0.1.2/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)    10823 2023-06-02 07:57:13.000000 comex-0.1.2/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-06-02 11:56:52.920000 comex-0.1.2/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-27 09:03:43.000000 comex-0.1.2/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      104 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3664 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/AST/
--rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/codeviews/AST/AST.py
--rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/AST/AST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/AST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/CFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    51528 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)    78323 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/CST/
--rwxrwxrwx   0 noble      (501) staff       (20)     2540 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CST/CST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/DFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-31 12:50:30.000000 comex-0.1.2/src/comex/codeviews/DFG/DFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/DFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/SDFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     4535 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    32117 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)    61608 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/SDFG/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/combined_graph/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/combined_graph/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/combined_graph/combined_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/tree_parser/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     8617 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/cs_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     6152 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/tree_parser/custom_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)    10057 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/java_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1818 2023-05-29 09:20:48.000000 comex-0.1.2/src/comex/tree_parser/parser_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/utils/
--rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/DFG_utils.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/utils/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)    19424 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/cs_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)    25191 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/java_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1083 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/postprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/preprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/src_parser.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)    11440 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-27 09:03:42.000000 comex-0.1.3/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)    13520 2023-06-22 04:19:09.860000 comex-0.1.3/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)    12903 2023-06-22 04:08:47.000000 comex-0.1.3/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-06-22 04:19:09.860000 comex-0.1.3/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-27 09:03:43.000000 comex-0.1.3/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      104 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3664 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/AST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/codeviews/AST/AST.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/AST/AST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/AST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/CFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    97324 2023-06-22 04:17:23.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    78345 2023-06-22 04:17:23.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/CST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     2542 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/codeviews/CST/CST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/DFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-31 12:50:30.000000 comex-0.1.3/src/comex/codeviews/DFG/DFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/DFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/SDFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4581 2023-06-09 05:17:59.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    57510 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    61649 2023-06-18 03:38:41.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/SDFG/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/combined_graph/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/combined_graph/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/combined_graph/combined_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/tree_parser/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/tree_parser/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    11275 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/tree_parser/cs_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     6210 2023-06-08 11:12:38.000000 comex-0.1.3/src/comex/tree_parser/custom_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    10039 2023-06-08 11:12:38.000000 comex-0.1.3/src/comex/tree_parser/java_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1818 2023-05-29 09:20:48.000000 comex-0.1.3/src/comex/tree_parser/parser_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/utils/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/DFG_utils.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/utils/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    26499 2023-06-14 16:12:07.000000 comex-0.1.3/src/comex/utils/cs_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    25220 2023-06-07 04:40:53.000000 comex-0.1.3/src/comex/utils/java_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1134 2023-06-07 04:40:53.000000 comex-0.1.3/src/comex/utils/postprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/preprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/src_parser.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)    13520 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.1.2/LICENSE` & `comex-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/PKG-INFO` & `comex-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,15 @@
-Metadata-Version: 2.1
-Name: comex
-Version: 0.1.2
-Summary: Generate combined multi-code view graphs
-Home-page: https://github.com/IBM/tree-sitter-codeviews
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
-
+---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
@@ -41,29 +23,29 @@
 ```console
 pip install -r requirements-dev.txt
 ```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
-### Usage as a CLI
+## Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
 
 The attributes and options supported by the CLI are well documented and can be viewed by running:
 ```console
 comex --help
 ```
 
 For example, to generate a combined CFG and DFG graph for a java file, you can run:
 ```console
 comex --lang "java" --code-file ./test.java --graphs "cfg,dfg"
 ```
 
-### Usage as a Python Package
+## Usage as a Python Package
 
 The comex package can be used by importing required drivers as follows:
 
 ```python
 from comex.codeviews.combined_graph.combined_driver import CombinedDriver
 
 CombinedDriver(
@@ -83,16 +65,43 @@
 
 output_file: denotes the output file to which the generated graph is written
 
 graph_format: denotes the format of the output graph. Currently supported formats are "dot" and "json". To generate both pass "all"
 
 codeviews: refers to the configuration passed for each codeview
 ````
+---
+## Limitations
+
+While `comex` provides _method-level_ and _file-level_ support for both Java and C\#, it's important to note the following limitations and known issues:
+
+### Java
+- **No Inter-file Analysis Support**: The tool currently does not support codeviews that involve interactions between multiple Java files. It is designed to generate codeviews for individual Java files only.
+
+- **Syntax Errors in Code**: Despite supporting non-compileable code, to ensure accurate codeviews, the input Java code must be free of syntax errors. Code with syntax errors may not be correctly parsed and displayed in the generated codeviews.
+
+- **Limited Support for Function Call Arguments**: The tool does not provide proper support for when a function call is passed as an argument to another function call in Java code. The resulting codeview might not accurately represent the intended behavior in such cases.
+
+### C\#
+In addition to the limitations mentioned for Java, the tool has the following limitations specific to C#:
+
+- **No Support for Lambda Functions and Arrow Expressions**: The tool does not support codeviews involving lambda functions and arrow expressions in C#. The generated codeviews may not accurately represent these language features.
+
+- **No Support for Compiler Directives**: Compiler directives, such as pragma directives, are not supported by the tool. Code involving such directives may not be properly displayed in the generated codeviews.
+
+- **Incomplete Operator Declaration Support**: The tool may have limited support for operator declarations in C#. Certain constraints and edge cases related to operator overloading might not be fully captured in the generated codeviews.
+
+- **Limited Support for Inheritance and Abstraction**: The tool's support for inheritance and abstraction in C# is not fully comprehensive. Codeviews involving complex inheritance hierarchies or advanced abstraction patterns may not be accurately represented.
+
+Please note that while we continuously work to improve the tool and address these limitations, the current implementation may not be perfect. We appreciate your understanding and encourage you to provide feedback and report any issues you encounter, as this helps us enhance the tool's capabilities.
+
+---
+
 
-### Output Examples:
+## Output Examples:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 ![Sample AST CFG DFG](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/sample.png)
 
 Below we present more examples of input code snippets and generated codeviews for both Java and C#.
```

### Comparing `comex-0.1.2/README.md` & `comex-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+Metadata-Version: 2.1
+Name: comex
+Version: 0.1.3
+Summary: Generate combined multi-code view graphs
+Home-page: https://github.com/IBM/tree-sitter-codeviews
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
-
+---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
@@ -24,29 +40,29 @@
 ```console
 pip install -r requirements-dev.txt
 ```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
-### Usage as a CLI
+## Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
 
 The attributes and options supported by the CLI are well documented and can be viewed by running:
 ```console
 comex --help
 ```
 
 For example, to generate a combined CFG and DFG graph for a java file, you can run:
 ```console
 comex --lang "java" --code-file ./test.java --graphs "cfg,dfg"
 ```
 
-### Usage as a Python Package
+## Usage as a Python Package
 
 The comex package can be used by importing required drivers as follows:
 
 ```python
 from comex.codeviews.combined_graph.combined_driver import CombinedDriver
 
 CombinedDriver(
@@ -66,16 +82,43 @@
 
 output_file: denotes the output file to which the generated graph is written
 
 graph_format: denotes the format of the output graph. Currently supported formats are "dot" and "json". To generate both pass "all"
 
 codeviews: refers to the configuration passed for each codeview
 ````
+---
+## Limitations
+
+While `comex` provides _method-level_ and _file-level_ support for both Java and C\#, it's important to note the following limitations and known issues:
+
+### Java
+- **No Inter-file Analysis Support**: The tool currently does not support codeviews that involve interactions between multiple Java files. It is designed to generate codeviews for individual Java files only.
+
+- **Syntax Errors in Code**: Despite supporting non-compileable code, to ensure accurate codeviews, the input Java code must be free of syntax errors. Code with syntax errors may not be correctly parsed and displayed in the generated codeviews.
+
+- **Limited Support for Function Call Arguments**: The tool does not provide proper support for when a function call is passed as an argument to another function call in Java code. The resulting codeview might not accurately represent the intended behavior in such cases.
+
+### C\#
+In addition to the limitations mentioned for Java, the tool has the following limitations specific to C#:
+
+- **No Support for Lambda Functions and Arrow Expressions**: The tool does not support codeviews involving lambda functions and arrow expressions in C#. The generated codeviews may not accurately represent these language features.
+
+- **No Support for Compiler Directives**: Compiler directives, such as pragma directives, are not supported by the tool. Code involving such directives may not be properly displayed in the generated codeviews.
+
+- **Incomplete Operator Declaration Support**: The tool may have limited support for operator declarations in C#. Certain constraints and edge cases related to operator overloading might not be fully captured in the generated codeviews.
+
+- **Limited Support for Inheritance and Abstraction**: The tool's support for inheritance and abstraction in C# is not fully comprehensive. Codeviews involving complex inheritance hierarchies or advanced abstraction patterns may not be accurately represented.
+
+Please note that while we continuously work to improve the tool and address these limitations, the current implementation may not be perfect. We appreciate your understanding and encourage you to provide feedback and report any issues you encounter, as this helps us enhance the tool's capabilities.
+
+---
+
 
-### Output Examples:
+## Output Examples:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 ![Sample AST CFG DFG](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/sample.png)
 
 Below we present more examples of input code snippets and generated codeviews for both Java and C#.
```

### Comparing `comex-0.1.2/setup.cfg` & `comex-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.1.2
+version = 0.1.3
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.1.2/src/comex/cli.py` & `comex-0.1.3/src/comex/cli.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/AST/AST.py` & `comex-0.1.3/src/comex/codeviews/AST/AST.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/AST/AST_driver.py` & `comex-0.1.3/src/comex/codeviews/AST/AST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/CFG/CFG.py` & `comex-0.1.3/src/comex/codeviews/CFG/CFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/CFG/CFG_csharp.py` & `comex-0.1.3/src/comex/codeviews/CFG/CFG_csharp.py`

 * *Files 27% similar despite different names*

```diff
@@ -55,20 +55,37 @@
             "constructor_calls": {},
             "object_instantiate": {},
             "label_statement_map": {},
             "return_statement_map": {},
             "label_switch_map": {},
             "switch_child_map": {},
             "switch_equivalent_map": {},
+            "lambda_map": {},
         }
+        # TODO: Check this against C# grammar.json
+        self.types = ["scoped_type_identifier", "type_identifier", "generic_type"]
 
         self.index_counter = max(self.index.values())
+        self.CFG_node_indices = []
+        self.symbol_table = self.parser.symbol_table
+        self.declaration = self.parser.declaration
+        self.declaration_map = self.parser.declaration_map
         self.CFG_node_list, self.CFG_edge_list = self.CFG_cs()
         self.graph = self.to_networkx(self.CFG_node_list, self.CFG_edge_list)
 
+    def get_index(self, node):
+        return self.index[(node.start_point, node.end_point, node.type)]
+
+    def check_inner_class(self, node):
+        while node.parent is not None:
+            if node.parent.type == "class_declaration":
+                return True
+            node = node.parent
+        return False
+
     def get_basic_blocks(self, CFG_node_list, CFG_edge_list):
         G = self.to_networkx(CFG_node_list, CFG_edge_list)
         components = nx.weakly_connected_components(G)
         # NOTE: May need to sort these components according to line number (this one is more foolproof but harder to implement) or the first element in the set (less foolproof, but I think it can be proved, easier to implement).
         # As of now coincidentally the AST node numbering and the list of nodes in networkx are according ot the line numbers
         block_index = 1
         for block in components:
@@ -77,48 +94,103 @@
             block_index += 1
 
     def get_key(self, val, dictionary):
         for key, value in dictionary.items():
             if val in value:
                 return key
 
+    # TODO: Check the correctness of this function
+    def get_containing_method(self, node):
+        operator_declaration = ["operator_declaration", "conversion_operator_declaration"]
+        method_declaration = ["method_declaration", "constructor_declaration", "local_function_statement"]
+        while node is not None:
+            if node.type == 'lambda_expression':
+                return node
+            if node.type in method_declaration:
+                return node
+            if node.type == "accessor_list" or node.type in operator_declaration:
+                return node
+            node = node.parent
+        while node is not None:
+            if node.type in self.statement_types["node_list_type"]:
+                return node
+            node = node.parent
+
     def append_block_index(self, CFG_node_list):
         new_list = []
         for node in CFG_node_list:
             block_index = self.get_key(node[0], self.records["basic_blocks"])
             new_list.append((node[0], node[1], node[2], node[3], block_index))
         return new_list
 
-    def add_edge(self, src_node, dest_node, edge_type):
+    def add_edge(self, src_node, dest_node, edge_type, additional_data=None):
         if src_node == None or dest_node == None:
             logger.error(
                 "Node where adding edge is attempted is none {}->{}",
                 src_node,
                 dest_node,
             )
             logger.warning(traceback.format_stack()[-2])
+            # print(src_node, dest_node, edge_type)
             raise NotImplementedError
+        elif dest_node == 2:
+            # print("Attempt to add exit node")
+            return
         else:
-            self.CFG_edge_list.append((src_node, dest_node, edge_type))
+            for src, dest, ty, *_ in self.CFG_edge_list:
+                if src == src_node and dest == dest_node and "method_call" not in edge_type:
+                    return
+            # print(src_node, dest_node, edge_type)
+            self.CFG_edge_list.append((src_node, dest_node, edge_type, additional_data))
+
+    def handle_next(self, src_node, dest_node, edge_type):
+        if dest_node == None:
+            try:
+                current_containing_method = self.get_index(self.get_containing_method(src_node))
+            except:
+                return
+            try:
+                self.records["return_statement_map"][current_containing_method].append(self.get_index(src_node))
+            except:
+                self.records["return_statement_map"][current_containing_method] = [self.get_index(src_node)]
 
-    def get_next_index(self, node_key, node_value):
+        else:
+            self.add_edge(self.get_index(src_node), self.get_index(dest_node), edge_type)
 
+    # TODO: Change all calls of get_next_index to match
+    def get_next_index(self, node_value):
+        # If exiting a method, don't return
         next_node = node_value.next_named_sibling
+        # TODO: Check if "block" works or not
+        while next_node is not None and next_node.type == "block" and len(
+                list(filter(lambda child: child.is_named, next_node.children))) == 0:
+            next_node = next_node.next_named_sibling
+        # TODO: Check if check_inner_class works properly or not)
+        if next_node is not None and next_node.type == "class_declaration":
+            # Check if its a local class
+            if self.check_inner_class(node_value):
+                next_node = next_node.next_named_sibling
+        next_node_index = -1  # Just using a dummy initial value
         if next_node == None:
             # Sibling not found
-
             current_node = node_value
             while current_node.parent is not None:
                 if (
                         current_node.parent.type
                         in self.statement_types["loop_control_statement"]
                 ):
                     next_node = current_node.parent
                     break
+                if current_node.parent.type == "if_statement":
+                    next_node_index, next_node = self.get_next_index(current_node.parent)
+                    break
                 next_node = current_node.next_named_sibling
+                if current_node.type in self.statement_types["definition_types"]:
+                    next_node = None
+                    break
                 if next_node is not None:
                     for i, child in enumerate(next_node.parent.children):
                         # if child.type == "while" and child.parent.type == "do_statement":
                         #     return None
                         if (
                                 child.type == "while"
                                 and child.parent.type == "do_statement"
@@ -140,22 +212,49 @@
                                 next_node = None
                                 break
                 if next_node is not None:
                     break
                 current_node = current_node.parent
 
         if next_node == None:
-            return 2
-        if next_node.type == "block":
-            for child in next_node.children:
-                if child.is_named:
-                    next_node = child
-                    break
+            return 2, None
+        if next_node.type in self.statement_types["definition_types"]:
+            return 2, None
+
+        # if next_node.type == "block":
+        #     for child in next_node.children:
+        #         if child.is_named:
+        #             next_node = child
+        #             break
 
-        return self.index[(next_node.start_point, next_node.end_point, next_node.type)]
+        # return self.index[(next_node.start_point, next_node.end_point, next_node.type)]
+        try:
+            # WARNING: Might need to replace if with while
+            if next_node.type == "block":
+                for child in next_node.children:
+                    if child.is_named:
+                        next_node = child
+                        break
+            # Returns the index of the next node and the node object of the next node
+            try:
+                current_containing_method = self.get_index(self.get_containing_method(node_value))
+                next_containing_method = self.get_index(self.get_containing_method(next_node))
+            except:
+                return 2, None
+            if current_containing_method != next_containing_method:
+                return 2, None
+            else:
+                return (self.get_index(next_node), next_node)
+
+        except Exception as e:
+            # return 2, None
+            # print("DO NOT IGNORE", e)
+            logger.warning(traceback.format_stack()[-2])
+            raise NotImplementedError
+            return next_node_index, next_node
 
     def edge_first_line(self, current_node_key, current_node_value):
         # We need to add an edge to the first statement in the next basic block
         node_index = self.index[current_node_key]
         try:
             current_block_index = self.get_key(node_index, self.records["basic_blocks"])
             next_block_index = current_block_index + 1
@@ -164,31 +263,37 @@
             dest_node = first_line_index
             self.add_edge(
                 src_node, dest_node, "first_next_line"
             )  # We could maybe differentiate this
         except:
             # Most probably the block is empty
             # add a direct edge to the next statement
-            # print("HIT AN EMPTY BLOCK")
-            next_index = self.get_next_index(current_node_key, current_node_value)
-            self.add_edge(node_index, next_index, "next_line")
+            if current_node_value.type == "method_declaration":
+                return
+            next_index, next_node = self.get_next_index(current_node_value)
+            self.handle_next(current_node_value, next_node, "next_line")
 
     def edge_to_body(self, current_node_key, current_node_value, body_type, edge_type):
         # We need to add an edge to the first statement in the body block
         src_node = self.index[current_node_key]
         # [current_node_value.field_name_for_child(i) for i,child in enumerate(current_node_value.children)]
         body_node = current_node_value.child_by_field_name(body_type)
         if body_node is None:
             body_nodes = [
                 child for child in current_node_value.children if child.type == "block"
             ]
             if body_nodes:
                 body_node = body_nodes[0]
-            else:
+            elif current_node_value.type == "while_statement":
                 body_node = current_node_value.named_children[-1]
+            else:
+                try:
+                    body_node = current_node_value.named_children[0]
+                except:
+                    body_node = current_node_value.named_children[-1]
         flag = False
         while body_node.type == "block":
             for child in body_node.children:
                 if child.is_named:
                     flag = True
                     body_node = child
                     break
@@ -217,135 +322,690 @@
                     if child.is_named:
                         block_node = child
                         break
             else:
                 block_node = block_node[0]
 
         if block_node.is_named is False:
-            return (
-                self.index[
-                    (
-                        current_node_value.start_point,
-                        current_node_value.end_point,
-                        current_node_value.type,
-                    )
-                ],
-                current_node_value.type,
-            )
+            return (current_node_value, current_node_value.type)
+        # if block_node.is_named is False:
+        #     return (
+        #         self.index[
+        #             (
+        #                 current_node_value.start_point,
+        #                 current_node_value.end_point,
+        #                 current_node_value.type,
+        #             )
+        #         ],
+        #         current_node_value.type,
+        #     )
 
         while block_node.type == "block":
             named_children = list(
                 filter(
                     lambda child: child.is_named == True, reversed(block_node.children)
                 )
             )
             if len(named_children) == 0:
                 # It means there is an empty block - thats why no named nodes inside
-                return (
-                    self.index[
-                        (
-                            current_node_value.start_point,
-                            current_node_value.end_point,
-                            current_node_value.type,
-                        )
-                    ],
-                    current_node_value.type,
-                )
+                return (current_node_value, current_node_value.type)
+                # return (
+                #     self.index[
+                #         (
+                #             current_node_value.start_point,
+                #             current_node_value.end_point,
+                #             current_node_value.type,
+                #         )
+                #     ],
+                #     current_node_value.type,
+                # )
             block_node = named_children[0]
             if block_node.type in self.statement_types["node_list_type"]:
-                return (
-                    self.index[
-                        (block_node.start_point, block_node.end_point, block_node.type)
-                    ],
-                    block_node.type,
-                )
-        return (
-            self.index[(block_node.start_point, block_node.end_point, block_node.type)],
-            block_node.type,
-        )
+                return (block_node, block_node.type)
+                # return (
+                #     self.index[
+                #         (block_node.start_point, block_node.end_point, block_node.type)
+                #     ],
+                #     block_node.type,
+                # )
+        return (block_node, block_node.type)
+        # return (
+        #     self.index[(block_node.start_point, block_node.end_point, block_node.type)],
+        #     block_node.type,
+        # )
+
+    # TODO: Check correctness of the next 3 functions
+    def get_class_name(self, node):
+        reference_node = node.child_by_field_name("function")
+        if reference_node is not None:
+            try:
+                reference_node = list(filter(lambda child: child.type == "member_access_expression", reference_node.children))[0]
+        #     # reference_node = list(filter(lambda child: child.type == "member_access_expression", node.children))[0]
+        #     reference_node = list(filter(lambda child: child.type == "member_access_expression", reference_node.children))[0]
+            except:
+                try:
+                    reference_node = list(filter(lambda child: child.type == "identifier", reference_node.children))[0]
+                except:
+                    reference_node = None
+            #     print(reference_node)
+            #     pass
+                
+        types = ["scoped_type_identifier", "type_identifier", "generic_type"]
+        if reference_node is None or reference_node.type == "this":
+            while node is not None:
+                if node.type == "class_declaration":
+                    # class_index = self.get_index(node)
+                    class_name = list(filter(lambda child: child.type == "identifier", node.children))[0]
+                    class_name = [class_name.text.decode("UTF-8")]
+                    break
+                if node.type == "struct_declaration":
+                    class_name = list(filter(lambda child: child.type == "identifier", node.children))[0]
+                    class_name = [class_name.text.decode("UTF-8")]
+                if node.type == "local_function_statement":
+                    class_name = list(filter(lambda child: child.type == "identifier", node.children))[0]
+                    class_name = [class_name.text.decode("UTF-8")]
+                node = node.parent
+
+            if class_name is None:
+                class_name = ["Unknown"]
+            # try:
+            #     class_name += self.records['extends'][class_name[0]]
+            # except:
+            #     class_name = ["Unknown"]
+            #     pass
+            return class_name
+        try:
+            reference_index = self.get_index(reference_node)
+            # reference_node = reference_node.text.decode("UTF-8").split(".")[0:-1]
+            declaration_index = self.declaration_map[reference_index]
+            class_name = [self.symbol_table["data_type"][declaration_index]]
+            try:
+                class_name += self.records['extends'][class_name[0]]
 
-    def function_list(self, current_node):
-        if current_node.type == "method_invocation":
-            # maintain a list of all method invocations
-            method_name = current_node.child_by_field_name("name").text.decode("UTF-8")
+            except:
+                pass
+            return class_name
+
+        except:
+            # If a static method has been explicitly called on a class name
+            if reference_node is not None:
+                if reference_node.type == "object_creation_expression":
+                    class_name = list(filter(lambda child: child.type in types, reference_node.children))[0]
+                    class_name = [class_name.text.decode("UTF-8")]
+                else:
+                    class_name = [reference_node.text.decode("UTF-8")]
+                try:
+                    class_name += self.records['extends'][class_name[0]]
+                except:
+                    pass
+                return class_name
+
+            return None
+
+    def get_return_type(self, current_node):
+        method_name = current_node.child_by_field_name("name").text.decode("UTF-8")
+        class_name = self.get_class_name(current_node)
+        if class_name is not None:
+            class_name = class_name[0]
+            method_name = (class_name, method_name)
+        else:
+            method_name = (None, method_name)
+        signature = ()
+        argument_list = current_node.child_by_field_name("arguments")
+        argument_list = list(filter(lambda child: child.is_named, argument_list.children))
+        signature = self.get_signature(argument_list)
+        function_key = (method_name, signature)
+        try:
+            data_type = self.records["return_type"][function_key]
+        except:
+            data_type = "void"
+        # records["return_type"][((class_name,method_name), signature)] = return_type
+        return data_type
+
+    def get_signature(self, argument_list):
+        literal_type_map = {
+            "character_literal": "char",
+            "string_literal": "String",
+            "decimal_integer_literal": "int",
+            "integer_literal": "int",
+            "boolean": "boolean",
+            "decimal_floating_point_literal": "double",  # If float, won't work
+        }
+        signature = []
+        for argument in argument_list:
+            argument = argument.named_children[-1]
+            if argument.type == "identifier":
+                identifier_index = self.get_index(argument)
+                try:
+                    declaration_index = self.declaration_map[identifier_index]
+                    data_type = self.symbol_table["data_type"][declaration_index]
+                except Exception as e:
+                    data_type = "Unknown"
+                signature.append(data_type)
+            elif argument.type == "method_invocation":
+                try:
+                    data_type = self.get_return_type(argument)
+                except:
+                    data_type = "Unknown"
+                signature.append(data_type)
+            elif argument.type == "field_access":
+                field_variable = argument.children[-1]
+                identifier_index = self.get_index(field_variable)
+                try:
+                    declaration_index = self.declaration_map[identifier_index]
+                    data_type = self.symbol_table["data_type"][declaration_index]
+                except Exception as e:
+                    data_type = "Unknown"
+                signature.append(data_type)
+            elif argument.type == "this":
+                signature.append(self.get_class_name(argument)[0])
+            else:
+                try:
+                    signature.append(literal_type_map[argument.type])
+                except:
+                    signature.append("Unknown")
+        return tuple(signature)
 
+    # def function_list(self, current_node):
+    #     if current_node.type == "method_invocation":
+    #         # maintain a list of all method invocations
+    #         method_name = current_node.child_by_field_name("name").text.decode("UTF-8")
+
+    #         parent_node = None
+    #         pointer_node = current_node
+    #         while pointer_node is not None:
+    #             if (
+    #                     pointer_node.parent is not None
+    #                     and pointer_node.parent.type
+    #                     in self.statement_types["node_list_type"]
+    #             ):
+    #                 parent_node = pointer_node.parent
+    #                 break
+    #             pointer_node = pointer_node.parent
+
+    #         # Removing this if condition will treat all print sttements as function calls as well
+    #         if method_name != "println" and method_name != "print":
+    #             # index : (AST_id, method_name) (AST_id is of the parent node)
+    #             if method_name in self.records["function_calls"].keys():
+    #                 self.records["function_calls"][method_name].append(
+    #                     (
+    #                         self.index_counter,
+    #                         self.index[
+    #                             (
+    #                                 parent_node.start_point,
+    #                                 parent_node.end_point,
+    #                                 parent_node.type,
+    #                             )
+    #                         ],
+    #                     )
+    #                 )
+    #             else:
+    #                 self.index_counter += 1
+    #                 self.records["function_calls"][method_name] = [
+    #                     (
+    #                         self.index_counter,
+    #                         self.index[
+    #                             (
+    #                                 parent_node.start_point,
+    #                                 parent_node.end_point,
+    #                                 parent_node.type,
+    #                             )
+    #                         ],
+    #                     )
+    #                 ]
+    #                 # Patent node of function call AST id maps to AST id or index of dummy external funciton call node
+    #                 # self.records['function_calls'][index] = (self.index_counter, method_name)
+    #                 if method_name not in self.records["method_list"].keys():
+    #                     self.CFG_node_list.append(
+    #                         (
+    #                             self.index_counter,
+    #                             0,
+    #                             "function_call: " + method_name,
+    #                             "external_function",
+    #                         )
+    #                     )
+
+    #     for child in current_node.children:
+    #         if child.is_named:
+    #             self.function_list(child)
+    # TODO: Check correctness nd function calls to this
+    def function_list(self, current_node, node_list):
+        current_index = self.get_index(current_node)
+        if current_node.type == "method_invocation" or current_node.type == "invocation_expression" :
             parent_node = None
             pointer_node = current_node
             while pointer_node is not None:
-                if (
-                        pointer_node.parent is not None
-                        and pointer_node.parent.type
-                        in self.statement_types["node_list_type"]
-                ):
-                    parent_node = pointer_node.parent
-                    break
+                if (pointer_node.parent is not None and pointer_node.parent.type in self.statement_types[
+                    "node_list_type"]):
+                    try:
+                        p = pointer_node.parent
+                        parent_node = node_list[(p.start_point, p.end_point, p.type)]
+                        break
+                    except Exception as e:
+                        pass
                 pointer_node = pointer_node.parent
+            parent_index = self.get_index(parent_node)
+            # maintain a list of all method invocations
+            # IDENTIFY THE CLASS THAT THE ALIAS BELONGS TO AND USE THAT IN THE MAP MAYBE? 
+            base_method_name = current_node.child_by_field_name("function").text.decode("UTF-8")
+            base_method_name = base_method_name.split(".")[-1]
+            # print(base_method_name)
+            signature = ()
+            argument_list = current_node.child_by_field_name("arguments")
+            argument_list = list(filter(lambda child: child.is_named, argument_list.children))
+            # print(argument_list)
+            signature = self.get_signature(argument_list)
+            class_name_list = self.get_class_name(current_node)
+            # print(class_name_list)
+            if class_name_list is None:
+                method_name = (None, base_method_name)
+                function_key = (method_name, signature)
+                if method_name[1] != "println" and method_name[1] != "print":
+                    if function_key in self.records["function_calls"].keys():
+                        self.records["function_calls"][function_key].append((current_index, parent_index))
+                    else:
+                        self.records["function_calls"][function_key] = [(current_index, parent_index)]
+            else:
+                for class_name in class_name_list:
+                    method_name = (class_name, base_method_name)
+                    function_key = (method_name, signature)
+                    if method_name[1] != "println" and method_name[1] != "print":
+                        if function_key in self.records["function_calls"].keys():
+                            self.records["function_calls"][function_key].append((current_index, parent_index))
+                        else:
+                            self.records["function_calls"][function_key] = [(current_index, parent_index)]
+        elif current_node.type == "object_creation_expression":
+            parent_node = None
+            pointer_node = current_node
+            while pointer_node is not None:
+                if (pointer_node.parent is not None and pointer_node.parent.type in self.statement_types[
+                    "node_list_type"]):
+                    try:
+                        p = pointer_node.parent
+                        parent_node = node_list[(p.start_point, p.end_point, p.type)]
+                        # parent_node = pointer_node.parent
+                        break
+                    except Exception as e:
+                        pass
+                pointer_node = pointer_node.parent
+            parent_index = self.get_index(parent_node)
+            # type_name = list(filter(lambda child : child.type in self.types, current_node.children))
+            # type_name = type_name[0].text.decode("utf-8")
+            type_name = current_node.child_by_field_name("type").text.decode("utf-8")
+            try:
+                self.records["object_instantiate"][type_name].append((current_index, parent_index))
+            except:
+                self.records["object_instantiate"][type_name] = [(current_index, parent_index)]
+                # break
+            signature = ()
+            argument_list = current_node.child_by_field_name("arguments")
+            try:
+                argument_list = list(filter(lambda child: child.is_named, argument_list.children))
+            except:
+                argument_list = []
+            signature = self.get_signature(argument_list)
+            method_name = (type_name, type_name)
+            function_key = (method_name, signature)
+            if function_key in self.records["constructor_calls"].keys():
+                self.records["constructor_calls"][function_key].append((current_index, parent_index))
+            else:
+                self.records["constructor_calls"][function_key] = [(current_index, parent_index)]
 
-            # Removing this if condition will treat all print sttements as function calls as well
-            if method_name != "println" and method_name != "print":
-                # index : (AST_id, method_name) (AST_id is of the parent node)
-                if method_name in self.records["function_calls"].keys():
-                    self.records["function_calls"][method_name].append(
-                        (
-                            self.index_counter,
-                            self.index[
-                                (
-                                    parent_node.start_point,
-                                    parent_node.end_point,
-                                    parent_node.type,
-                                )
-                            ],
-                        )
-                    )
-                else:
-                    self.index_counter += 1
-                    self.records["function_calls"][method_name] = [
-                        (
-                            self.index_counter,
-                            self.index[
-                                (
-                                    parent_node.start_point,
-                                    parent_node.end_point,
-                                    parent_node.type,
-                                )
-                            ],
-                        )
-                    ]
-                    # Patent node of function call AST id maps to AST id or index of dummy external funciton call node
-                    # self.records['function_calls'][index] = (self.index_counter, method_name)
-                    if method_name not in self.records["method_list"].keys():
-                        self.CFG_node_list.append(
-                            (
-                                self.index_counter,
-                                0,
-                                "function_call: " + method_name,
-                                "external_function",
-                            )
-                        )
+        elif current_node.type == "explicit_constructor_invocation":
+            parent_node = current_node
+            parent_index = self.get_index(parent_node)
+            type_name = current_node.child_by_field_name("constructor").text.decode("utf-8")
+            if type_name == 'this':  # TODO: Add super also here for now
+                type_name_list = self.get_class_name(current_node)
+                for type_name in type_name_list:
+                    # TODO: Replace this condition with a method level check flag
+                    if type_name != "test":
+                        try:
+                            self.records["object_instantiate"][type_name].append((current_index, current_index))
+                        except:
+                            self.records["object_instantiate"][type_name] = [(current_index, current_index)]
+
+                        signature = ()
+                        argument_list = current_node.child_by_field_name("arguments")
+                        argument_list = list(filter(lambda child: child.is_named, argument_list.children))
+                        signature = self.get_signature(argument_list)
+                        method_name = (type_name, type_name)
+                        function_key = (method_name, signature)
+                        if function_key in self.records["constructor_calls"].keys():
+                            self.records["constructor_calls"][function_key].append((current_index, parent_index))
+                        else:
+                            self.records["constructor_calls"][function_key] = [(current_index, parent_index)]
+
+            elif type_name == 'super':
+                pass
+            else:
+                raise Exception("Explicit constructor invocation not handled")
+
+        elif current_node.type == "method_declaration" or current_node.type == "constructor_declaration":
+            last_line, _ = self.get_block_last_line(current_node, "body")
+            try:
+                self.records["return_statement_map"][current_index].append(self.get_index(last_line))
+            except:
+                self.records["return_statement_map"][current_index] = [self.get_index(last_line)]
+
+        elif current_node.type == "class_declaration":
+            # If constructor exits, find the last line of the constructor
+            # If no constructor, find the last line before a method starts
+            # If empty of if only methods, then just return from the class
+            constructor_node = None
+            constructor_count = 0
+            empty_flag = True
+            last_statement = None
+            class_node = current_node.child_by_field_name("body")
+            class_children = list(filter(lambda
+                                             child: child.is_named and child.type != "method_declaration" and child.type != "class_declaration",
+                                         class_node.children))
+            for child in reversed(class_children):
+                if child.type in self.statement_types["node_list_type"]:
+                    empty_flag = False
+                    if last_statement is None and child.type != "constructor_declaration":
+                        last_statement = child
+                if child.type == "constructor_declaration":
+                    constructor_node = child
+                    constructor_count += 1
+                    break
+            if empty_flag == True:
+                try:
+                    self.records["return_statement_map"][current_index].append(current_index)
+                except:
+                    self.records["return_statement_map"][current_index] = [current_index]
+            elif constructor_count == 1:
+                last_line, _ = self.get_block_last_line(constructor_node, "body")
+                try:
+                    self.records["return_statement_map"][current_index].append(self.get_index(last_line))
+                except:
+                    self.records["return_statement_map"][current_index] = [self.get_index(last_line)]
+            elif last_statement is not None:
+                last_index = self.get_index(last_statement)
+                try:
+                    self.records["return_statement_map"][current_index].append(last_index)
+                except:
+                    self.records["return_statement_map"][current_index] = [last_index]
+            elif constructor_node is not None:
+                last_line, _ = self.get_block_last_line(constructor_node, "body")
+                try:
+                    self.records["return_statement_map"][current_index].append(self.get_index(last_line))
+                except:
+                    self.records["return_statement_map"][current_index] = [self.get_index(last_line)]
 
         for child in current_node.children:
             if child.is_named:
-                self.function_list(child)
+                self.function_list(child, node_list)
+
+    # TODO: Check correctness
+    def get_all_statements(self, current_node, node_list, statements):
+        for child in current_node.children:
+            if child.is_named and child.type in self.statement_types["node_list_type"]:
+                child_key = (child.start_point, child.end_point, child.type)
+                if child_key in node_list.keys():
+                    statements.append(child)
+            self.get_all_statements(child, node_list, statements)
+        return statements
 
     def add_dummy_nodes(self):
         self.CFG_node_list.append((1, 0, "start_node", "start"))
-        self.CFG_node_list.append((2, 0, "exit_node", "exit"))
+        # self.CFG_node_list.append((2, 0, "exit_node", "exit"))
 
-    def add_dummy_edges(self):
-        for node_name, node_index in self.records["function_calls"].items():
+    # def add_dummy_edges(self):
+    #     for node_name, node_index in self.records["function_calls"].items():
+    #         for node in node_index:
+    #             if node_name not in self.records["method_list"].keys():
+    #                 self.add_edge(node[1], node[0], "function_call")
+    #                 self.add_edge(node[0], node[1], "function_return")
+    #             else:
+    #                 self.add_edge(
+    #                     node[1],
+    #                     self.records["method_list"][node_name],
+    #                     "recursive_method_call",
+    #                 )
+
+    def get_signature_nodes(self, node):
+        signature = []
+        formal_parameters = node.child_by_field_name('parameters')
+        formal_parameters = list(filter(lambda x: x.type == 'formal_parameter', formal_parameters.children))
+
+        for formal_parameter in formal_parameters:
+            for child in formal_parameter.children:
+                if child.type != "identifier":
+                    signature.append(child.text.decode('utf-8'))
+        return tuple(signature)
+
+    def get_class_name_nodes(self, node):
+        type_identifiers = ["type_identifier", "generic_type", "scoped_type_identifier"]
+        "Returns the class name when a method declaration or constructor declaration is passed to it"
+
+        while node is not None:
+            if node.type == "class_body" and node.parent.type == "class_declaration":
+                node = node.parent
+                class_index = self.index[(node.start_point, node.end_point, node.type)]
+                class_name = list(filter(lambda child: child.type == "identifier", node.children))[0]
+                return class_index, class_name.text.decode("UTF-8")
+            elif node.type == "class_body" and node.parent.type == "object_creation_expression":
+                node = node.parent
+                class_index = self.index[(node.start_point, node.end_point, node.type)]
+                class_name = list(filter(lambda child: child.type in type_identifiers, node.children))[0]
+                return class_index, class_name.text.decode("UTF-8")
+            node = node.parent
+
+    def inner_function(self, current_node):
+        """Returns true if the current node is inside an inner function"""
+        method_counter = 0
+        while current_node is not None:
+            if current_node.type == "method_declaration":
+                method_counter += 1
+            current_node = current_node.parent
+        if method_counter > 1:
+            return True
+        else:
+            return False
+
+    def returns_inner_definition(self, node, inner_node):
+
+        """Returns the inner definition index if exists"""
+        for c in node.children:
+            if c.is_named and c.type == "method_declaration":
+                method_name = list(filter(lambda child: child.type == "identifier", c.children))[0].text.decode("utf-8")
+                _, class_name = self.get_class_name_nodes(c)
+                signature = self.get_signature_nodes(c)
+                # TODO: Take out the common unitility functions like get class name and signture
+                inner_node.append(self.records["method_list"][((class_name, method_name), signature)])
+                return
+            else:
+                self.returns_inner_definition(c, inner_node)
+        return
+
+    def get_matched_constructor(self, node):
+        for node_signature, node_ind in self.records["constructor_calls"].items():
+            for node_search in node_ind:
+                if node == node_search:
+                    if node_signature in self.records["constructor_list"].keys():
+                        method_index = self.records["constructor_list"][node_signature]
+                        return method_index
+
+        for node_signature, node_ind in self.records["constructor_calls"].items():
+            for node_search in node_ind:
+                flag = False
+                if node == node_search:
+                    for list_signature, list_index in self.records["constructor_list"].items():
+                        flag = True
+                        list_signature_list = list(list_signature[1])
+                        node_signature_list = list(node_signature[1])
+                        if len(list_signature_list) != len(node_signature_list):
+                            flag = False
+                        else:
+                            for i in range(len(list_signature_list)):
+                                if list_signature_list[i] != "Unknown" and node_signature_list[i] != "Unknown" and \
+                                        list_signature_list[i] != node_signature_list[i]:
+                                    flag = False
+                                    break
+                        if flag == True:
+                            return list_index
+
+    def add_method_call_edges(self):
+        # print("Method List")
+        # print(*self.records["method_list"].items(), sep="\n")
+        # print("Constructor List")
+        # print(*self.records["constructor_list"].items(), sep="\n")
+        # print("Function Calls")
+        # print(*self.records["function_calls"].items(), sep="\n")
+        # print("Object instantiations")
+        # print(*self.records["object_instantiate"].items(), sep="\n")
+        # print("Constuctor Calls")
+        # print(*self.records["constructor_calls"].items(), sep="\n")
+        # print("extends")
+        # print(self.records["extends"])
+        # print("Declaration Map")
+        # print(self.declaration_map)
+        # print("SymboL_TABLE.DATATYPES")
+        # print(self.symbol_table["data_type"])
+        # print("declaration")
+        # print(self.declaration)
+        # print("____________________________________________________________________________")
+        # print("return_statement_map")
+        # print(self.records["return_statement_map"])
+
+        for node_signature, node_index in self.records["function_calls"].items():
+            # node_index[1] is suppposed to be the statement node number of the function call
+            # node_index[0] is the dummy index value assigned to the dummy node created for the external function call
+            # Update: node_index[0] is no longer dummy index but the ast id of the function invocation node
             for node in node_index:
-                if node_name not in self.records["method_list"].keys():
-                    self.add_edge(node[1], node[0], "function_call")
-                    self.add_edge(node[0], node[1], "function_return")
-                else:
-                    self.add_edge(
-                        node[1],
-                        self.records["method_list"][node_name],
-                        "recursive_method_call",
-                    )
+                if node_signature in self.records["method_list"].keys():
+                    method_index = self.records["method_list"][node_signature]
+                    # Find the class name before indexing records["method_list"]
+                    edge_type = "method_call|" + str(node[0])
+                    self.add_edge(node[1], self.records["method_list"][node_signature], edge_type)
+                    # Add the returning edge
+                    # Use the return statement index available in records. And add an edge from all the return statements to the calling line here
+                    try:
+                        for return_node in self.records["return_statement_map"][method_index]:
+                            self.add_edge(return_node, node[1], "method_return")
+                    except:
+                        # If you can't find return statements, then add an edge from the last line 
+                        # Handled by adding the last line to the return statement map in self.function_calls
+                        pass
+        for node_name, node_index in self.records["object_instantiate"].items():
+            for node in node_index:
+                if node_name in self.records["class_list"].keys():
+                    class_index = self.records["class_list"][node_name]
+                    edge_type = "constructor_call|" + str(node[0])
+                    additional_data_index = self.get_matched_constructor(node)
+                    additional_data = {}
+                    if additional_data_index is not None:
+                        additional_data = {"target_constructor": additional_data_index}
+                    # for node_signature, node_ind in self.records["constructor_calls"].items():
+                    #     for node_search in node_ind:
+                    #         if node == node_search:
+                    #             if node_signature in self.records["constructor_list"].keys():
+                    #                 method_index = self.records["constructor_list"][node_signature]
+                    #                 additional_data = {"target_constructor": method_index}
+                    #                 print(node_signature, method_index)
+                    #                 break
+                    #     if additional_data:
+                    #         break
+                    # assert additional_data
+                    # print("ADDING EDGE", node[1], class_index, edge_type, additional_data)
+                    self.add_edge(node[1], class_index, edge_type, additional_data=additional_data)
+                    try:
+                        for return_node in self.records["return_statement_map"][class_index]:
+                            self.add_edge(return_node, node[1], "class_return")
+                    except Exception as e:
+                        # If you can't find return statements, then add an edge from the last line 
+                        # Handled by adding the last line to the return statement map in self.function_calls
+                        pass
+
+        for node_signature, node_index in self.records["constructor_calls"].items():
+            for node in node_index:
+                if node_signature in self.records["constructor_list"].keys():
+                    method_index = self.records["constructor_list"][node_signature]
+                    try:
+                        for return_node in self.records["return_statement_map"][method_index]:
+                            self.add_edge(return_node, node[1], "class_return")
+                    except:
+                        # If you can't find return statements, then add an edge from the last line 
+                        # Handled by adding the last line to the return statement map in self.function_calls
+                        pass
+
+        # for lambda expressions
+        # for node_key, lambda_expression in self.records["lambda_map"].items():
+        for lambda_key, statement_node in self.records["lambda_map"].items():
+            # lambda_index = self.index[node_key]
+            lambda_index = self.index[lambda_key]
+            # self.edge_to_body(node_key, lambda_expression, "body", "lambda_invocation")
+            self.add_edge(self.get_index(statement_node), lambda_index, "lambda_invocation")
+            # TODO: maintain a return map for all points of return
+            try:
+                for return_node in self.records["return_statement_map"][lambda_index]:
+                    self.add_edge(return_node, self.get_index(statement_node), "lambda_return 1")
+            except:
+                pass
+                for lambda_expression in self.get_all_lambda_body(statement_node):
+                    # Note: Might need to move this to before the try
+                    last_line, line_type = self.get_block_last_line(lambda_expression, "body")
+                    if line_type not in self.statement_types['node_list_type']:
+                        self.add_edge(self.get_index(lambda_expression), self.get_index(statement_node),
+                                      "lambda_return 2")
+                    else:
+                        last_line_index = self.get_index(last_line)
+                        self.add_edge(last_line_index, self.get_index(statement_node), "lambda_return 3")
+
+    def return_next_node(self, node_value):
+        # node_value = node_value.parent  
+        next_node = node_value.next_named_sibling
+        while next_node is None and node_value.parent.type in self.statement_types['statement_holders']:
+            if node_value.parent.parent.type == 'method_declaration':
+                next_node = node_value.parent.next_named_sibling
+                return next_node
+            else:
+                node_value = node_value.parent
+                next_node = node_value.next_named_sibling
+        if node_value.parent.type in self.statement_types['statement_holders']:
+            return next_node
+        return None
+
+    def add_class_edge(self, node_value):
+        class_attributes = ["field_declaration", "accessor_list"]
+        # Not included: ["record_declaration", "method_declaration","compact_constructor_declaration","class_declaration","interface_declaration","annotation_type_declaration","enum_declaration","block","static_initializer","constructor_declaration"]
+        current_index = self.get_index(node_value)
+        current_node = node_value.child_by_field_name("body")
+        flag = False
+        # Chain all class level attributes together and append to class declaration.
+        current_fields = list(filter(lambda x: x.type in class_attributes, current_node.children))
+        for field in current_fields:
+            if field.type == "accessor_list":
+                # Find the first line insdie the block
+                block = list(filter(lambda x: x.type == "block", field.children))[0]
+                try:
+                    field = list(filter(lambda x: x.is_named, block.children))[-1]
+                except:
+                    continue
+                field_index = self.get_index(field)
+            else:
+                field_index = self.get_index(field)
+                self.add_edge(current_index, field_index, "class_next")
+            current_index = field_index
+
+        # If constructor exists, chain it to the last field
+        constructors = list(filter(lambda x: x.type == "constructor_declaration", current_node.children))
+        for constructor in constructors:
+            constructor_index = self.get_index(constructor)
+            self.add_edge(current_index, constructor_index, "constructor_next")
+
+        # In case main method exists, chain main method at the end
+        try:
+            methods = list(filter(lambda x: x.type == "method_declaration", current_node.children))
+            for method in methods:
+                if self.records["main_method"] == self.get_index(method):
+                    self.add_edge(current_index, self.records["main_method"], "main_method_next")
+        except:
+            pass
 
     def read_index(self, index):
         return list(self.index.keys())[list(self.index.values()).index(index)]
 
     def CFG_cs(self):
         warning_counter = 0
         node_list = {}
@@ -365,203 +1025,314 @@
         #             for case in equivalent:
         #                 if case not in self.records["label_statement_map"]:
         #                     self.records["label_statement_map"]
 
         # Initial for loop required for basic block creation and simple control flow within a block ----------------------------
         for node_key, node_value in node_list.items():
             current_node_type = node_key[2]
-            if current_node_type in self.statement_types["non_control_statement"]:
+            if current_node_type in self.statement_types["non_control_statement"] and current_node_type not in \
+                    self.statement_types["scope_only_blocks"]:
                 # if current_node_type not in self.statement_types['terminal_inner']:
-                if cs_nodes.return_switch_child(node_value) is None:
+                if (
+                        cs_nodes.return_switch_child(node_value) is None
+                        and node_value.parent is not None
+                        and node_value.parent.type
+                        in self.statement_types["statement_holders"]
+                ):
+                    # if cs_nodes.return_switch_child(node_value) is None:
                     try:
+                        # print("_________________-")
+                        # print(node_value.text.decode("utf-8"), node_value.type)
+                        check = False
                         src_node = self.index[node_key]
                         if node_value.type == "labeled_statement":
                             if "statement" in node_value.named_children[-1].type:
                                 src_node = get_index(
                                     node_value.named_children[-1], self.index
                                 )
                         next_node = node_value.next_named_sibling
-                        if next_node and next_node.type == "block":
+                        if next_node is not None and next_node.type == "accessor_list":
+                            try:
+                                child = list(filter(lambda x: x.type == "block", next_node.children))[0]
+                                next_node = child
+                            except:
+                                pass
+                        while next_node is not None and next_node.type == "block" and len(
+                                list(filter(lambda child: child.is_named, next_node.children))) == 0:
+                            next_node = next_node.next_named_sibling
+                        # If it is a local class, skip it and go for the next node
+                        if next_node is not None and next_node.type == "class_declaration":
+                            # Check if its a local class
+                            if self.check_inner_class(node_value):
+                                next_node = next_node.next_named_sibling
+                        # TODO: This might break next line, check all test cases
+                        # if next_node is None and self.get_containing_method(node_value).type == "constructor_declaration": 
+                        #     self.handle_next(node_value, None, "constructor_return")
+                        if next_node is None and node_value.parent.type == 'block':
+                            next_node = self.return_next_node(node_value)
+                            if next_node is None:
+                                continue
+                            dest_node = self.get_index(next_node)
+                            check = True
+                            if next_node.type in self.statement_types["node_list_type"] and next_node.type not in \
+                                    self.statement_types["definition_types"]:
+                                self.add_edge(src_node, dest_node, "next_line $")
+
+                        flag = False
+                        while next_node.type == "block" and len(next_node.named_children):
                             for child in next_node.children:
-                                if child.type in self.statement_types["node_list_type"]:
-                                    self.add_edge(
-                                        src_node,
-                                        self.index[
-                                            (
-                                                child.start_point,
-                                                child.end_point,
-                                                child.type,
-                                            )
-                                        ],
-                                        "into_block",
-                                    )
-                                    break
-                        else:
-                            dest_node = self.index[
-                                (
-                                    next_node.start_point,
-                                    next_node.end_point,
-                                    next_node.type,
-                                )
-                            ]
-                            if dest_node in self.records["switch_child_map"].keys():
-                                dest_node = self.records["switch_child_map"][dest_node]
-                            for i, child in enumerate(next_node.parent.children):
-                                if child == next_node:
-                                    field_name = next_node.parent.field_name_for_child(
-                                        i
-                                    )
-                                    if field_name is None:
-                                        self.add_edge(src_node, dest_node, "next_line")
+                                if child.is_named:
+                                    if child.type in self.statement_types["node_list_type"]:
+                                        flag = True
+                                        next_node = child
+                                        break
                                     else:
-                                        # TODO Triage
-                                        next_node = None
-                    except:
+                                        next_node = child
+                                        break
+
+                            if flag == True:
+                                break
+
+                        dest_node = self.get_index(next_node)
+                        if dest_node in self.records["switch_child_map"].keys():
+                            dest_node = self.records["switch_child_map"][dest_node]
+                        if check is False and next_node.type in self.statement_types[
+                            'node_list_type'] and next_node.type not in self.statement_types["definition_types"]:
+                            self.add_edge(src_node, dest_node, "next_line 1")
+                        # if next_node and next_node.type == "block":
+                        #     for child in next_node.children:
+                        #         if child.type in self.statement_types["node_list_type"]:
+                        #             self.add_edge(
+                        #                 src_node,
+                        #                 self.index[
+                        #                     (
+                        #                         child.start_point,
+                        #                         child.end_point,
+                        #                         child.type,
+                        #                     )
+                        #                 ],
+                        #                 "into_block",
+                        #             )
+                        #             break
+                        # else:
+                        #     dest_node = self.index[
+                        #         (
+                        #             next_node.start_point,
+                        #             next_node.end_point,
+                        #             next_node.type,
+                        #         )
+                        #     ]
+                        #     if dest_node in self.records["switch_child_map"].keys():
+                        #         dest_node = self.records["switch_child_map"][dest_node]
+                        #     for i, child in enumerate(next_node.parent.children):
+                        #         if child == next_node:
+                        #             field_name = next_node.parent.field_name_for_child(
+                        #                 i
+                        #             )
+                        #             if field_name is None:
+                        #                 self.add_edge(src_node, dest_node, "next_line")
+                        #             else:
+                        #                 # TODO Triage
+                        #                 next_node = None
+                    except Exception as e:
+                        # print("EXCEPTION: ", e)
+                        # print(traceback.format_exc())
                         pass
 
             elif current_node_type in self.statement_types["not_implemented"]:
-                print("WARNING: Not implemented ", current_node_type)
+                logger.warning("WARNING: Not implemented ", current_node_type)
                 warning_counter += 1
 
         self.get_basic_blocks(self.CFG_node_list, self.CFG_edge_list)
         self.CFG_node_list = self.append_block_index(self.CFG_node_list)
-
-        self.function_list(self.root_node)
-
+        self.CFG_node_indices = list(map(lambda x: x[0], self.CFG_node_list))
+        self.function_list(self.root_node, node_list)
         self.add_dummy_nodes()
-        self.add_dummy_edges()
+        # self.add_dummy_edges()
         # ------------------------------------------------------------------------------
         # At this point, the self.CFG_node_list has basic block index appended to it
         # ------------------------------------------------------------------------------
         first_guy_hit = False
         for node_key, node_value in node_list.items():
             current_node_type = node_key[2]
             current_index = self.index[node_key]
             if current_node_type in [
                 "method_declaration",
                 "interface_declaration",
                 "constructor_declaration",
                 "property_declaration",
             ]:
                 # We need to add an edge to the first statement in the next basic block
-                if not first_guy_hit:
-                    first_guy_hit = True
-                    self.add_edge(1, current_index, "next")
+                # if not first_guy_hit:
+                #     first_guy_hit = True
+                #     self.add_edge(1, current_index, "next")
+                try:
+                    # If main method exists, this will work
+                    # print(self.records["main_method"], "main method", self.records["main_class"], "main class")
+
+                    if current_index == self.records["main_method"]:
+                        self.add_edge(1, self.records["main_class"], "next")
+                        # self.add_edge(self.records["main_class"], current_index, "next")
+                except Exception as e:
+                    # print("Exxxxxxx", e)
+                    declarations = ["class_declaration", "interface_declaration"]
+                    if node_value.type != "interface_declaration" and node_value.parent.parent.type in declarations:
+                        # We need to add an edge to the first statement in the next basic block
+                        self.add_edge(1, current_index, "next")
+
                 self.edge_first_line(node_key, node_value)
-                last_line_index, line_type = self.get_block_last_line(
+                # TODO: Change all occurences of get_block_last_line
+                last_line, line_type = self.get_block_last_line(
                     node_value, "body"
                 )
+                last_line_index = self.get_index(last_line)
+                try:
+                    if current_case_index == self.records["main_method"]:
+                        if line_type in self.statement_types["non_control_statement"]:
+                            if last_line_index in self.records["switch_child_map"].keys():
+                                last_line_index = self.records["switch_child_map"][last_line_index]
+                            # self.add_edge(last_line_index, 2, "exit_next")
+                except:
+                    # No main method in this snippet
+                    pass
+                # TODO: Not sure if this part makes sense
                 if line_type in self.statement_types["non_control_statement"]:
                     if last_line_index in self.records["switch_child_map"].keys():
                         last_line_index = self.records["switch_child_map"][
                             last_line_index
                         ]
                     if line_type == "labeled_statement":
                         statement_node = node_list[self.read_index(last_line_index)]
                         if "statement" in statement_node.named_children[-1].type:
                             last_line_index = get_index(
                                 statement_node.named_children[-1], self.index
                             )
-                    self.add_edge(last_line_index, 2, "exit_next")
+                    # self.add_edge(last_line_index, 2, "exit_next")
 
             # ------------------------------------------------------------------------------------------------
+            elif current_node_type == "interface_declaration":
+                self.edge_first_line(node_key, node_value)
+            # ------------------------------------------------------------------------------
+            if current_node_type == "class_declaration":
+                self.add_class_edge(node_value)
+            elif current_node_type == "import_declaration":
+                next_node = node_value.next_named_sibling
+                if next_node is not None and next_node.type != "import_declaration":
+                    try:
+                        self.add_edge(current_index, self.records["main_class"], "next")
+                    except:
+                        pass
+            # ------------------------------------------------------------------------------------------------
             elif current_node_type == "lock_statement":
                 self.edge_first_line(node_key, node_value)
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "body"
                 )
-                next_dest_index = self.get_next_index(node_key, node_value)
+                last_line_index = self.get_index(last_line)
+                next_dest_index, next_node = self.get_next_index(node_value)
                 if line_type in self.statement_types["non_control_statement"]:
                     self.add_edge(last_line_index, next_dest_index, "lock_released")
                 #     self.add_edge(last_line_index, 2, 'exit_next')
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "labeled_statement":
                 self.edge_first_line(node_key, node_value)
-
+            # ------------------------------------------------------------------------------------------------
             elif current_node_type in [
                 "checked_statement",
                 "fixed_statement",
                 "unsafe_statement",
                 "using_statement",
                 "local_function_statement",
             ]:
                 self.edge_first_line(node_key, node_value)
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "body"
                 )
-                if line_type in self.statement_types["non_control_statement"]:
-                    self.add_edge(
-                        last_line_index,
-                        self.index[
-                            (
-                                node_value.start_point,
-                                node_value.end_point,
-                                node_value.type,
-                            )
-                        ],
-                        "return_control",
-                    )
-                # next_dest_index = self.get_next_index(node_key, node_value)
+                last_line_index = self.get_index(last_line)
+                next_dest_index, next_node = self.get_next_index(node_value)
+                if line_type in self.statement_types["non_control_statement"] and line_type not in self.statement_types[
+                    "scope_only_blocks"]:
+                    self.handle_next(last_line, next_node, "next_line *")
+                    # self.add_edge(
+                    #     last_line_index,
+                    #     self.index[
+                    #         (
+                    #             node_value.start_point,
+                    #             node_value.end_point,
+                    #             node_value.type,
+                    #         )
+                    #     ],
+                    #     "return_control",
+                    # )
+                # next_dest_index, next_node = self.get_next_index(node_value)
                 # self.add_edge(self.index[node_key], next_dest_index, 'next_line')
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "if_statement":
                 # Find the if block body and the else block body if exists (first statement inside them, add an edge)
                 # Find the line just after the entire if_statement
-                next_dest_index = self.get_next_index(node_key, node_value)
+                next_dest_index, next_node = self.get_next_index(node_value)
                 # consequence
                 self.edge_to_body(node_key, node_value, "consequence", "pos_next")
                 # Find the last line in the consequence block and add an edge to the next statement
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "consequence"
                 )
+                last_line_index = self.get_index(last_line)
                 # Also add an edge from the last guy to the next statement after the if
                 # print(last_line_index, line_type)
                 if line_type in self.statement_types["non_control_statement"]:
-                    self.add_edge(last_line_index, next_dest_index, "next_line")
+                    self.handle_next(last_line, next_node, "next_line")
 
                 # alternative = node_value.child_by_field_name('alternative')
                 # print("alternative", alternative)
+                empty_if = False
+                if last_line_index == current_index:
+                    empty_if = True
+                    self.handle_next(node_value, next_node, "next_line")
                 if node_value.child_by_field_name("alternative") is not None:
 
                     # alternative
                     self.edge_to_body(node_key, node_value, "alternative", "neg_next")
                     # Find the last line in the alternative block
-                    last_line_index, line_type = self.get_block_last_line(
+                    last_line, line_type = self.get_block_last_line(
                         node_value, "alternative"
                     )
                     # print(last_line_index, line_type)
                     if line_type in self.statement_types["non_control_statement"]:
-                        self.add_edge(last_line_index, next_dest_index, "next_line")
+                        self.handle_next(last_line, next_node, "next_line")
+                    if empty_if and last_line_index == current_index:
+                        self.handle_next(node_value, next_node, "next_line")
                 else:
                     # When else is not there add a direct edge from if node to the next statement
                     # if node_value.parent.type == "block" and node_value.parent.parent.type == "do_statement":
                     #     pass
                     # TODO FIX LOGIC IMP
                     # elif cs_nodes.return_index_of_first_parent_of_type(node_value, 'switch_section') is not None:
                     #     pass
                     # else:
-                    self.add_edge(current_index, next_dest_index, "next_line")
+                    self.handle_next(node_value, next_node, "next_line")
+                    # self.add_edge(current_index, next_dest_index, "next_line")
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type in self.statement_types["loop_control_statement"]:
                 # Get the node immediately after the while statement
-                next_dest_index = self.get_next_index(node_key, node_value)
+                next_dest_index, next_node = self.get_next_index(node_value)
 
                 # Add an edge from this node to the first line in the body
                 self.edge_to_body(node_key, node_value, "body", "pos_next")
 
                 # Find the last line in the body block
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "body"
                 )
-
+                last_line_index = self.get_index(last_line)
                 # Add an edge from this node to the next line after the loop statement
-                self.add_edge(current_index, next_dest_index, "neg_next")
+                self.handle_next(node_value, next_node, "neg_next")
                 # Add an edge from the last statement in the body to this node
                 if line_type in self.statement_types["non_control_statement"]:
                     self.add_edge(last_line_index, current_index, "loop_control")
 
                 # Add a self loop in case of for loops
                 if current_node_type != "while_statement":
                     self.add_edge(current_index, current_index, "loop_update")
@@ -571,24 +1342,24 @@
                 # Find the corresponding while statement
                 # Add an edge from this node to the first line in the body
                 # Find the last statement in the body and an edge frpom last line to the while node
                 # Add an edge from the while node to the first line in the block or to the current do node
                 # Add an edge from the while node to the next statement after the do_statement
 
                 # Get the node immediately after the while statement
-                next_dest_index = self.get_next_index(node_key, node_value)
+                next_dest_index, next_node = self.get_next_index(node_value)
 
                 # Add an edge from this node to the first line in the body
                 self.edge_to_body(node_key, node_value, "body", "pos_next")
 
                 # Find the last line in the body block
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "block"
                 )
-
+                last_line_index = self.get_index(last_line)
                 # Search the CFG_node_list for parameterized_expression with parent do_statement with AST_id = src_node
                 # for k, v in node_list.items():
                 #     # print(k,v)
                 #     if self.index[
                 #         (v.parent.start_point, v.parent.end_point, v.parent.type)] == current_index:
                 #         if 'expression' in k[2]:
                 #             while_index = self.index[k]
@@ -636,47 +1407,64 @@
 
                 # add edge from this node to the loop_control statement or do statement
 
                 src_node = self.index[node_key]
                 dest_node = self.index[
                     (loop_node.start_point, loop_node.end_point, loop_node.type)
                 ]
+                label_name = list(filter(lambda child: child.type == "identifier", node_value.children))
                 # label_name = list(filter(lambda child: child.type == 'identifier', node_value.children))
                 # if len(label_name) > 0:
                 #     target_name = label_name[0].text.decode('UTF-8').strip()
                 #     dest_node = self.records['label_statement_map'][target_name]
+                if len(label_name) > 0:
+                    target_name = label_name[0].text.decode("UTF-8") + ":"
+                    dest_node = self.index[self.records["label_statement_map"][target_name]]  # Check on this later
                 self.CFG_edge_list.append((src_node, dest_node, "jump_next"))
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "break_statement":
                 # if it is inside a switch, it is handled here and also refer to switch_expression,
                 # if it is inside a loop, handle it here
-                parent_node = node_value.parent
-                loop_node = None
-                while parent_node is not None:
-                    if (
-                            parent_node.type
-                            in self.statement_types["loop_control_statement"]
-                            + ["do_statement"]
-                            or parent_node.type == "switch_expression"
-                            or parent_node.type == "switch_statement"
-                    ):
-                        loop_node = parent_node
-                        break
-                    parent_node = parent_node.parent
-                if loop_node is not None:
-                    next_dest_index = self.get_next_index(
-                        (loop_node.start_point, loop_node.end_point, loop_node.type),
-                        loop_node,
-                    )
-                    # label_name = list(filter(lambda child: child.type == 'identifier', node_value.children))
-                    # if len(label_name) > 0:
-                    #     target_name = label_name[0].text.decode('UTF-8') + ":"
-                    #     next_dest_index = self.records['label_statement_map'][target_name]
-                    self.add_edge(current_index, next_dest_index, "jump_next")
+                label_name = list(filter(lambda child: child.type == "identifier", node_value.children))
+                if len(label_name) > 0:
+                    target_name = label_name[0].text.decode("UTF-8") + ":"
+                    # next_dest_index = self.records['label_statement_map'][target_name]
+                    label_key = self.records["label_statement_map"][target_name]
+                    label_node = node_list[label_key]
+                    next_dest_index, next_node = self.get_next_index(label_node)
+                    # need to get the node corresponding to this index, and then get the next node
+                    self.handle_next(node_value, next_node, "jump_next")
+                else:
+                    parent_node = node_value.parent
+                    loop_node = None
+                    while parent_node is not None:
+                        if (
+                                parent_node.type
+                                in self.statement_types["loop_control_statement"]
+                                + ["do_statement"]
+                                or parent_node.type == "switch_expression"
+                                or parent_node.type == "switch_statement"
+                        ):
+                            loop_node = parent_node
+                            break
+                        parent_node = parent_node.parent
+
+                    # if loop_node is not None:
+                    #     next_dest_index, next_node = self.get_next_index(
+                    #         (loop_node.start_point, loop_node.end_point, loop_node.type),
+                    #         loop_node,
+                    #     )
+                    #     # label_name = list(filter(lambda child: child.type == 'identifier', node_value.children))
+                    #     # if len(label_name) > 0:
+                    #     #     target_name = label_name[0].text.decode('UTF-8') + ":"
+                    #     #     next_dest_index = self.records['label_statement_map'][target_name]
+                    #     self.add_edge(current_index, next_dest_index, "jump_next")
+                    next_dest_index, next_node = self.get_next_index(loop_node)
+                    self.handle_next(node_value, next_node, "jump_next")
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "goto_statement":
                 target_name = node_value.text.decode("UTF-8").replace(";", "").replace("goto", "").strip()
                 if target_name in self.records["label_statement_map"]:
                     next_dest_index = self.records["label_statement_map"][target_name]
                 else:
                     switch_node = cs_nodes.return_index_of_first_parent_of_type(
@@ -711,18 +1499,15 @@
 
                 try:
                     next_dest_index = self.index[
                         (loop_node.start_point, loop_node.end_point, loop_node.type)
                     ]
                 except:
                     # Handle yield when no loop parent or switch parent
-                    next_dest_index = self.get_next_index(
-                        (node_value.start_point, node_value.end_point, node_value.type),
-                        node_value,
-                    )
+                    next_dest_index, next_node = self.get_next_index(node_value)
 
                 self.add_edge(current_index, next_dest_index, "yield_exit")
             # ------------------------------------------------------------------------------------------------
             elif (
                     current_node_type == "switch_expression"
                     or current_node_type == "switch_statement"
             ):
@@ -750,15 +1535,15 @@
                 # in case of a break statement, add an edge to the next statement outside the switch
                 # in case of default, add an edge to the next statement outside the switch
                 # in case of no default, add an edge from last block to the next statement outside the switch
                 case_node_list = {}
                 # default_exists = False
 
                 # Find the next statement outside the switch
-                next_dest_index = self.get_next_index(node_key, node_value)
+                next_dest_index, next_node = self.get_next_index(node_value)
 
                 if current_index in self.records["label_switch_map"]:
                     if "default" not in self.records["label_switch_map"][current_index]:
                         self.add_edge(
                             current_index, next_dest_index, "switch_no_default"
                         )
 
@@ -886,23 +1671,48 @@
                 for k, v in case_node_list.items():
                     current_case_index = self.index[k]
                     parent = v.parent
                     while parent.parent is not None:
                         parent = parent.parent
                         if parent.type == "local_declaration_statement":
                             break
-                    next_dest_index = self.get_next_index(None, parent)
+                    next_dest_index, next_node = self.get_next_index(parent)
                     self.add_edge(current_case_index, next_dest_index, "switch_out")
 
                 # in case of a break statement, add an edge to the next statement outside the switch
                 # -> Handled in break statement
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "return_statement":
-                self.add_edge(current_index, 2, "return_exit")
+                # self.add_edge(current_index, 2, "return_exit")
+                # Check if it returns a function with an inner definition
+                # method_list will give us the index of the inner function
+                inner_definition = []
+                self.returns_inner_definition(node_value, inner_definition)
+
+                if len(inner_definition) > 0:
+                    inner_definition = inner_definition[0]
+                    # inner_index = self.index[(inner_definition.start_point, inner_definition.end_point, inner_definition.type)]
+                    # TODOD: Perhaps remove this because inconsistent wih newly decided logic
+                    self.add_edge(current_index, inner_definition, "return_next")
+
+                if not self.inner_function(node_value):
+                    # pass
+                    # Instead of an edge to exit node, we update the return map
+                    # self.add_edge(current_index, 2, "return_exit")
+                    containing_method = self.get_index(self.get_containing_method(node_value))
+
+                    try:
+                        self.records["return_statement_map"][containing_method].append(current_index)
+                    except:
+                        self.records["return_statement_map"][containing_method] = [current_index]
+                # else: TODO: When inner functions are properly implemented
+                #       save it in the return map?
+                #     next_dest_index, next_node = self.get_next_index(node_value)
+                #     self.add_edge(current_index, next_dest_index, "return_exit")
 
             # ------------------------------------------------------------------------------------------------
             elif current_node_type == "try_statement":
                 # Add edge from try block to first statement inside the block
                 self.edge_to_body(node_key, node_value, "body", "next")
                 catch_node_list = {}
                 finally_node = None
@@ -953,55 +1763,57 @@
                                 catch_index = self.index[catch_node]
                                 # if statement.type != 'return_statement': The Exception can occur on the RHS so the catch_exception edge should be there
                                 self.add_edge(
                                     statement_index, catch_index, "catch_exception"
                                 )
 
                 # Find the next statement outside the try block
-                next_dest_index = self.get_next_index(node_key, node_value)
+                next_dest_index, next_node = self.get_next_index(node_value)
                 exit_next = None
 
                 # finally block is optional
                 if finally_node is not None:
                     # From last line of finally to next statement outside the try block
-                    last_line_index, line_type = self.get_block_last_line(
+                    last_line, line_type = self.get_block_last_line(
                         finally_node, "body"
                     )
                     if line_type in self.statement_types["non_control_statement"]:
-                        self.add_edge(last_line_index, next_dest_index, "finally_exit")
+                        self.handle_next(last_line, next_node, "finally_exit")
                     # For the remaining portion, set finally block as next node if exists
-                    exit_next = self.index[
-                        (
-                            finally_node.start_point,
-                            finally_node.end_point,
-                            finally_node.type,
-                        )
-                    ]
+                    # exit_next = self.index[
+                    #     (
+                    #         finally_node.start_point,
+                    #         finally_node.end_point,
+                    #         finally_node.type,
+                    #     )
+                    # ]
+                    exit_next = finally_node
                 else:
-                    exit_next = next_dest_index
+                    exit_next = next_node
 
                 # From last line of try block to finally or to next statement outside the try block
-                last_line_index, line_type = self.get_block_last_line(
+                last_line, line_type = self.get_block_last_line(
                     node_value, "body"
                 )
                 if (
                         line_type in self.statement_types["non_control_statement"]
                         or finally_node is not None
                 ):
-                    self.add_edge(last_line_index, exit_next, "try_exit")
+                    self.handle_next(last_line, exit_next, "try_exit")
                 # From last line of every catch block to finally or to next statement outside the try block
                 for catch_node, catch_value in catch_node_list.items():
-                    last_line_index, line_type = self.get_block_last_line(
+                    last_line, line_type = self.get_block_last_line(
                         catch_value, "body"
                     )
+                    last_line_index = self.get_index(last_line)
                     if line_type in self.statement_types["non_control_statement"]:
-                        self.add_edge(last_line_index, exit_next, "catch_exit")
+                        self.handle_next(last_line, exit_next, "catch_exit")
                         # Case of empty catch block
                     elif last_line_index == self.index[catch_node]:
-                        self.add_edge(last_line_index, exit_next, "catch_exit")
+                        self.handle_next(last_line, exit_next, "catch_exit")
                         # ------------------------------------------------------------------------------------------------
             elif current_node_type == "throw_statement":
                 # Control goes to the first catch in the call stack (dynamic call stack) Nothing to do statically
                 # Essentially exits the function
 
                 parent = node_value.parent
                 try_flag = False
@@ -1023,14 +1835,14 @@
                             self.add_edge(
                                 current_index,
                                 get_index(child, self.index),
                                 "throw_catch",
                             )
             else:
                 pass
-
+        self.add_method_call_edges()
         if warning_counter > 0:
-            print(
+            logger.warning(
                 "Total number of warnings from unimplemented statement types: ",
                 warning_counter,
             )
         return self.CFG_node_list, self.CFG_edge_list
```

### Comparing `comex-0.1.2/src/comex/codeviews/CFG/CFG_driver.py` & `comex-0.1.3/src/comex/codeviews/CFG/CFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/CFG/CFG_java.py` & `comex-0.1.3/src/comex/codeviews/CFG/CFG_java.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if src_node == None or dest_node == None:
             logger.error(
                 "Node where adding edge is attempted is none {}->{}",
                 src_node,
                 dest_node,
             )
             logger.warning(traceback.format_stack()[-2])
-            print(src_node, dest_node, edge_type)
+            # print(src_node, dest_node, edge_type)
             raise NotImplementedError
         else:
             for src, dest, ty, *_ in self.CFG_edge_list:
                 if src == src_node and dest == dest_node:
                     return
             self.CFG_edge_list.append((src_node, dest_node, edge_type, additional_data))
 
@@ -189,15 +189,15 @@
             if current_containing_method != next_containing_method:
                 return 2, None
             else:
                 return (self.get_index(next_node), next_node)
         
         except Exception as e:
             # return 2, None
-            print("DO NOT IGNORE", e)
+            # print("DO NOT IGNORE", e)
             logger.warning(traceback.format_stack()[-2])
             raise NotImplementedError
             return next_node_index, next_node
 
     def edge_first_line(self, current_node_key, current_node_value):
         # We need to add an edge to the first statement in the next basic block
         node_index = self.index[current_node_key]
@@ -865,15 +865,15 @@
                             self.add_edge(src_node, dest_node, "next_line 1")
 
                         
                     except:
                         pass
 
             elif current_node_type in self.statement_types["not_implemented"]:
-                print("WARNING: Not implemented ", current_node_type)
+                logger.warning("WARNING: Not implemented ", current_node_type)
                 warning_counter += 1
 
         self.get_basic_blocks(self.CFG_node_list, self.CFG_edge_list)
         self.CFG_node_list = self.append_block_index(self.CFG_node_list)
         self.CFG_node_indices = list(map(lambda x: x[0], self.CFG_node_list))
         self.function_list(self.root_node, node_list)
         self.add_dummy_nodes()
@@ -1401,9 +1401,9 @@
                         if ( k[2] == "catch_clause" and self.get_index(v.parent) == current_index):
                             catch_node_list[k] = v
                     # if len(catch_node_list) == 0:
                     #     self.add_edge(current_index, 2, "throw_exit")
         
         self.add_method_call_edges()
         if warning_counter > 0:
-            print("Total number of warnings from unimplemented statement types: ", warning_counter)
+            logger.warning("Total number of warnings from unimplemented statement types: ", warning_counter)
         return self.CFG_node_list, self.CFG_edge_list
```

### Comparing `comex-0.1.2/src/comex/codeviews/CST/CST_driver.py` & `comex-0.1.3/src/comex/codeviews/CST/CST_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         )
         # postprocessor.write_to_dot(self.graph, os.path.join(grandparent_folder,"output_graphs/CST_output.dot"))
 
     def postorder_traversal(self, node):
         if node.children:
             for child in node.children:
                 self.postorder_traversal(child)
-        print(node.type)
+        # print(node.type)
 
     def create_CST_id(self, root_node, CST_index, CST_id):
         current_node_id = CST_id[0]
         CST_id[0] += 1
         CST_index[
             (root_node.start_point, root_node.end_point, root_node.type)
         ] = current_node_id
```

### Comparing `comex-0.1.2/src/comex/codeviews/DFG/DFG_driver.py` & `comex-0.1.3/src/comex/codeviews/DFG/DFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/codeviews/SDFG/SDFG.py` & `comex-0.1.3/src/comex/codeviews/SDFG/SDFG.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os.path
 import time
 
 import networkx as nx
 from loguru import logger
 
-from ...codeviews.CFG.CFG_driver import CFGDriver
-from .SDFG_csharp import dfg_csharp
-from .SDFG_java import dfg_java
-from ...utils import postprocessor, DFG_utils
+from comex.codeviews.CFG.CFG_driver import CFGDriver
+from comex.codeviews.SDFG.SDFG_csharp import dfg_csharp
+from comex.codeviews.SDFG.SDFG_java import dfg_java
+from comex.utils import postprocessor, DFG_utils
 
 debug = False
 
-
 # if any(
 #         # GITHUB_ACTIONS
 #         x in os.environ for x in ("PYCHARM_HOSTED",)
 # ):
 #     debug = True
 
+
 class DfgRda:
     def __init__(
             self,
             src_language="java",
             src_code="",
             output_file=None,
             graph_format="dot",
```

### Comparing `comex-0.1.2/src/comex/codeviews/SDFG/SDFG_csharp.py` & `comex-0.1.3/src/comex/codeviews/SDFG/SDFG_csharp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import time
 from collections import defaultdict
 import copy
 
 import pprint
 
 import networkx as nx
 
@@ -10,33 +12,44 @@
 from deepdiff import DeepDiff
 
 from loguru import logger
 
 pp = pprint.PrettyPrinter(indent=4)
 system_type = ("Console", "System", "String")
 debug = False
+
 # if any(
-#     # GITHUB_ACTIONS
-#     x in os.environ for x in ("PYCHARM_HOSTED",)
+#         # GITHUB_ACTIONS
+#         x in os.environ for x in ("PYCHARM_HOSTED",)
 # ):
 #     debug = True
 
+
 def scope_check(parent_scope, child_scope):
     for p in parent_scope:
         if p not in child_scope:
             return False
     return True
 
 
 class Identifier:
     def __init__(self, parser, node, line=None, declaration=False, full_ref=None, method_call=False):
         self.core = st(node)
+        class_node = return_first_parent_of_types(node, "class_declaration")
         if full_ref is None:
             full_ref = node
+        self.parent_class = class_node
         self.unresolved_name = st(full_ref)
+        if self.unresolved_name.startswith("this."):
+            self.unresolved_name = st(full_ref)[5:]
+        if class_node is not None:
+            class_name = st(class_node.child_by_field_name("name"))
+            self.parent_class = class_name
+            if self.unresolved_name.startswith(class_name + "."):
+                self.unresolved_name = self.unresolved_name[len(class_name) + 1:]
         self.line = line
         self.declaration = declaration
         self.method_call = method_call
         self.satisfied = method_call
         if self.method_call and self.declaration:
             method_resolution = self.unresolved_name.split(".")
             # br.attribute2.attr.method1
@@ -47,15 +60,27 @@
             # Option 2 - method call only affects subattribute
             resolved_name = ".".join(method_resolution[:-1])
             self.name = resolved_name
         else:
             self.name = self.unresolved_name
         if not self.name:
             self.name = self.unresolved_name
-        self.scope = parser.symbol_table["scope_map"][get_index(node, parser.index)]
+        if node.parent.type == "member_access_expression":
+            og_node = node.parent
+            node = recursively_get_children_of_types(og_node, ['identifier'], index=parser.index,
+                                                                 check_list=parser.symbol_table["scope_map"])[0]
+        variable_index = get_index(node, parser.index)
+        self.variable_scope = parser.symbol_table["scope_map"][variable_index]
+        if variable_index in parser.declaration_map:
+            self.scope = parser.symbol_table["scope_map"][parser.declaration_map[variable_index]]
+        else:
+            # self.scope = variable_scope
+            # Declaration does not exist hence it is given
+            # the outermost scope
+            self.scope = [0]
         if line is not None:
             self.real_line_no = read_index(parser.index, line)[0][0]
 
     def __eq__(self, other):
         # if not isinstance(other, Identifier):
         #     return NotImplemented
         # if self.name == other.name:
@@ -118,15 +143,15 @@
     return list(index.keys())[list(index.values()).index(idx)]
 
 
 def parent_remapping_callback(node):
     if node is None:
         return None
     elif node.type == "do_statement":
-        return None
+        return node.named_children[-1]
     elif node.type == "try_statement":
         return None
         # while_node = None
         # for child in node.children:
         #     if child.type == "while":
         #         while_node = child.next_named_sibling
         #         break
@@ -215,21 +240,20 @@
 
 def add_entry(parser, rda_table, statement_id, used=None, defined=None, declaration=False, core=None,
               method_call=False):
     if statement_id not in rda_table:
         rda_table[statement_id] = defaultdict(list)
     if not used and not defined:
         return
+    mapped_node = None
     if core is None:
         current_node = used or defined
         if current_node.type == "member_access_expression":
-            recurse_node = recursively_get_children_of_types(current_node, ['identifier'], index=parser.index,
-                                                             check_list=parser.symbol_table["scope_map"])
-            if recurse_node:
-                current_node = recurse_node[-1]
+            current_node = recursively_get_children_of_types(current_node, ['identifier'], index=parser.index,
+                                                             check_list=parser.symbol_table["scope_map"])[-1]
             if defined is not None:
                 defined = current_node
             else:
                 used = current_node
         if (
                 current_node.parent is not None
                 and current_node.parent.type == "member_access_expression"
@@ -248,32 +272,68 @@
                 current_node = current_node.parent
 
             if (
                     current_node.parent is not None
                     and current_node.parent.type == "invocation_expression"
             ):
                 if not st(current_node).startswith(system_type):
-                    add_entry(parser, rda_table, statement_id, defined=used or defined, core=current_node, declaration=True,
+                    if (used or defined).type == "identifier":
+                        method_cs = (used or defined).parent.named_children[0]
+                        # set_add(rda_table[statement_id]["def"],
+                        #         Identifier(parser, (used or defined).parent.named_children[0], statement_id, full_ref=None,
+                        #                    # declaration=True,
+                        #                    method_call=True))
+                    add_entry(parser, rda_table, statement_id, defined=used or defined, core=method_cs,
+                              # declaration=True,
                               method_call=True)
-                    add_entry(parser, rda_table, statement_id, used=used or defined, core=current_node, declaration=True,
+                    add_entry(parser, rda_table, statement_id, used=used or defined, core=method_cs,
+                              # declaration=True,
                               method_call=True)
+                if mapped_node is not None:
+                    set_add(rda_table[statement_id]["def"],
+                            Identifier(parser, mapped_node, statement_id, full_ref=mapped_node, declaration=declaration,
+                                       method_call=method_call))
                 return
             if defined is not None:
-                add_entry(parser, rda_table, statement_id, defined=defined, core=current_node, declaration=declaration, method_call=method_call)
+                add_entry(parser, rda_table, statement_id, defined=defined, core=current_node, declaration=declaration,
+                          method_call=method_call)
+                if mapped_node is not None:
+                    set_add(rda_table[statement_id]["def"],
+                            Identifier(parser, mapped_node, statement_id, full_ref=mapped_node, declaration=declaration,
+                                       method_call=method_call))
             else:
-                add_entry(parser, rda_table, statement_id, used=used, core=current_node, declaration=declaration, method_call=method_call)
+                add_entry(parser, rda_table, statement_id, used=used, core=current_node, declaration=declaration,
+                          method_call=method_call)
             return
+        elif current_node.next_sibling and current_node.next_sibling.type == "." and current_node.parent is not None and current_node.parent.type == "invocation_expression":
+            if not st(current_node).startswith(system_type):
+                if (used or defined).type == "identifier":
+                    set_add(rda_table[statement_id]["def"],
+                            Identifier(parser, used or defined, statement_id, full_ref=None,
+                                       # declaration=True,
+                                       method_call=True))
+    if st(core).startswith(system_type):
+        return
     if defined is not None:
         if get_index(defined, parser.index) not in parser.symbol_table["scope_map"]:
             return
         set_add(rda_table[statement_id]["def"],
-                Identifier(parser, defined, statement_id, full_ref=core, declaration=declaration, method_call=method_call))
+                Identifier(parser, defined, statement_id, full_ref=core, declaration=declaration,
+                           method_call=method_call))
+        if mapped_node is not None:
+            set_add(rda_table[statement_id]["def"],
+                    Identifier(parser, mapped_node, statement_id, full_ref=mapped_node, declaration=declaration,
+                               method_call=method_call))
     else:
         if get_index(used, parser.index) not in parser.symbol_table["scope_map"]:
             return
+        if mapped_node is not None and method_call:
+            set_add(rda_table[statement_id]["def"],
+                    Identifier(parser, mapped_node, statement_id, full_ref=mapped_node, declaration=declaration,
+                               method_call=method_call))
         set_add(rda_table[statement_id]["use"],
                 Identifier(parser, used, full_ref=core, declaration=declaration, method_call=method_call))
 
 
 def check_field_name(req_child):
     for i, child in enumerate(req_child.parent.children):
         if req_child == child:
@@ -303,15 +363,23 @@
                     #                           'member_access_expression'],
                     node.children,
                 )
             )
         )
     else:
         result.extend(list(filter(lambda child: child.type in st_types, node.children)))
+        additional_cs = []
+        for n in result:
+            if n.type == "parameter" and n == n.parent.named_children[0]:
+                additional_cs.append(n)
+        for n in additional_cs:
+            result.remove(n)
     for child in node.named_children:
+        if node.type == "parameter" and child == node.named_children[0]:
+            continue
         if child in stop_types:
             continue
         if child.type not in st_types:
             result = recursively_get_children_of_types(
                 child, st_types, result=result, stop_types=stop_types, index=index, check_list=check_list
             )
     return result
@@ -335,58 +403,99 @@
     return result
 
 
 def print_table(index, new_result, iteration=0):
     table = [f"\nRDA: iteration {iteration}\n"]
     for key in new_result:
         try:
-            table.append(str(read_index(index, key)[0][0]+1)+"\n")
+            table.append(str(read_index(index, key)[0][0] + 1) + "\n")
         except:
-            table.append(str(key)+"\n")
+            table.append(str(key) + "\n")
         for key2 in new_result[key]:
             table.append(f"\t{key2}:")
             for entry in new_result[key][key2]:
-                table.append(str(entry)+",")
+                table.append(str(entry) + ",")
             table.append("\n")
     logger.debug("".join(table))
 
 
-def start_rda(index, rda_table, CFG_results):
-    if debug:
+def start_rda(index, rda_table, graph, pre_solve=False):
+    if debug and not pre_solve:
         print_table(index, rda_table)
-    cfg = CFG_results.graph
-    nodes = CFG_results.graph.nodes
+    remove_set = []
+    # "method_return", "class_return"
+    if pre_solve:
+        remove_set = ["method_call", "method_return", "class_return", "constructor_call"]
+    graph = copy.deepcopy(graph)
+    remove_edges = []
+    if remove_set:
+        for edge in graph.edges:
+            if "label" in graph.edges[edge] and graph.edges[edge]["label"] in remove_set:
+                remove_edges.append(edge)
+        graph.remove_edges_from(remove_edges)
+
+    cfg = graph
+    nodes = graph.nodes
     old_result = {}
     iteration = 0
     for node in nodes:
         old_result[node] = {
             "IN": set(),
             "OUT": set()
         }
     # for node in nodes:
     #     connected_derivers = [t for (s, t) in cfg.out_edges(node)]
     #     old_result[node]["OUT"] = compute_out(old_result, connected_derivers, rda_table[node]["def"] if node in rda_table else [])
     new_result = copy.deepcopy(old_result)
     while True:
         iteration = iteration + 1
+        iteration_returners = {}
         for node in nodes:
-            connected_feeders = [s for (s, t) in cfg.in_edges(node)]
+            connected_feeders = []
+            returning_feeders = []
+            for (s, t) in cfg.in_edges(node):
+                if "label" in cfg.edges[s, t, 0] and cfg.edges[s, t, 0]["label"] in ["method_return", "class_return"]:
+                    returning_feeders.append(s)
+                else:
+                    connected_feeders.append(s)
             feeder_union = set()
+            returner_union = set()
             for feeder in connected_feeders:
                 feeder_union = feeder_union.union(old_result[feeder]["OUT"])
+            for returner in returning_feeders:
+                returner_union = returner_union.union(old_result[returner]["OUT"])
+            for (s, t) in cfg.out_edges(node):
+                if s != t:
+                    iteration_returners[t] = iteration_returners[t].union(
+                        returner_union) if t in iteration_returners else returner_union
             new_result[node]["IN"] = feeder_union
             def_info = rda_table[node]["def"] if node in rda_table else set()
             names_defined = [defined.name for defined in def_info]
+            # if defined.param_declaration is None
             selective_difference = set()
             for already_defined in feeder_union:
+                # if already_defined.immutable_declaration:
+                #     selective_difference.add(already_defined)
                 if already_defined.name in names_defined:
                     continue
                 else:
                     selective_difference.add(already_defined)
             new_result[node]["OUT"] = selective_difference.union(def_info)
+        for node in iteration_returners:
+            def_info = rda_table[node]["def"] if node in rda_table else set()
+            names_defined = [defined.name for defined in def_info]
+            selective_difference = set()
+            for already_defined in iteration_returners[node]:
+                # if already_defined.immutable_declaration:
+                #     selective_difference.add(already_defined)
+                if already_defined.name in names_defined:
+                    continue
+                else:
+                    selective_difference.add(already_defined)
+            new_result[node]["OUT"] = new_result[node]["OUT"].union(selective_difference)
         ddiff = DeepDiff(
             old_result,
             new_result,
             ignore_order=True,
         )
         if ddiff == {}:
             # for node in nodes:
@@ -399,78 +508,125 @@
             #         if outgoing in all_defs:
             #             continue
             #     connected_derivers = [t for (s, t) in cfg.out_edges(node)]
             #     for deriver in connected_derivers:
             #         for incoming in new_result[deriver]["IN"]:
             #             if incoming in rda_table[node]["def"]:
             #                 continue
-            if debug:
+            if debug and not pre_solve:
                 logger.info("RDA: Completed in iteration {}", iteration)
                 print_table(index, new_result, iteration)
             break
         old_result = copy.deepcopy(new_result)
     return new_result
 
 
 def add_edge(final_graph, a, b, attrib=None, pre_solve=False):
     if (pre_solve and attrib) or not final_graph.has_edge(a, b):
         final_graph.add_edge(a, b)
         if attrib is not None:
             nx.set_edge_attributes(final_graph, {(a, b, 0): attrib})
 
 
-def get_required_edges_from_def_to_use(index, cfg, rda_solution, rda_table, graph_nodes, properties=None):
+def get_required_edges_from_def_to_use(index, cfg, rda_solution, rda_table, graph_nodes, all_classes,
+                                       additional_edges=None, processed_edges=None, pre_solve=False, properties=None):
+    if additional_edges is None:
+        additional_edges = []
+    if processed_edges is None:
+        processed_edges = []
     final_graph = copy.deepcopy(cfg)
+    # twin_edges = [
+    #     "constructor_call", "method_call"
+    # ]
+    # twins = []
+    # retain_edges = [
+    #     "constructor_call", "class_return", "method_call", "method_return"
+    # ]
+    # retains = []
+    # additional_edges = []
+    # for edge in list(final_graph.edges()):
+    #     edge_data = final_graph.get_edge_data(*edge)[0]
+    #     if edge_data["label"] in retain_edges:
+    #         retains.append(edge)
+    #     # if edge_data["label"] in twin_edges:
+    #     #     twins.append(edge)
     final_graph.remove_edges_from(list(final_graph.edges()))
     for node in graph_nodes:
         rda_info = rda_table[node] if node in rda_table else None
         if rda_info is not None:
             use_info = rda_info["use"]
             # def_info = rda_info["def"]
         else:
             use_info = set()
             # def_info = set()
         # names_used = [used.name for used in use_info]
         for used in use_info:
             for available_def in rda_solution[node]["IN"]:
                 if available_def.name == used.name:
+                    # if available_def not in rda_solution[node]["OUT"]:
+                    #     for line_def in rda_table[node]["def"]:
+                    #         if line_def.name == available_def.name:
+                    #             if line_def.declaration:
+                    #                 available_def = line_def
                     # if available_def in rda_table[available_def.line]["def"]:
-                    if available_def.declaration:
-                        if scope_check(available_def.scope, used.scope):
-                            add_edge(final_graph, available_def.line, node)
-                            used.satisfied = True
-                    else:
-                        add_edge(final_graph, available_def.line, node)
+                    if scope_check(available_def.scope, used.scope):
+                        # if available_def.declaration:
+                        # if available_def.immutable_declaration:
+                        #     for other_def in rda_solution[node]["IN"]:
+                        #         if other_def.name == available_def.name and other_def.param_declaration:
+                        #             if not used.core.startswith("this"):
+                        #                 available_def = other_def
+                        #             break
+                        add_edge(final_graph, available_def.line, node, {'used_def': f"'{used.name}'"}, pre_solve)
                         used.satisfied = True
+                    # else:
+                    #         add_edge(final_graph, available_def.line, node, {'used_def': used.name}, pre_solve)
+                    #         used.satisfied = True
                 elif "." in used.name or "." in available_def.name:
                     if len(used.name.split(".")) < len(available_def.name.split(".")):
                         smaller = used
                         bigger = available_def
                     else:
                         smaller = available_def
                         bigger = used
                     if bigger.name.strip().startswith(smaller.name.strip()):
                         if not bigger.name.strip().replace(smaller.name.strip(), "").strip().startswith("."):
                             continue
 
                         # add_edge(final_graph, bigger.line or node, smaller.line or node)
-                        add_edge(final_graph, available_def.line or node, used.line or node)
+                        add_edge(final_graph, available_def.line or node, used.line or node, {'used_def': f"'{used.name}'"},
+                                 pre_solve)
                         used.satisfied = True
             if not used.satisfied:
-                if properties.get("last_use", False):
-                    for i in rda_table:
-                        for entry in rda_table[i]["use"]:
-                            if entry.name == used.name and i != node:
-                                # TODO: THIS IS AN AP - Make sure edges added here are right
-                                if not nx.has_path(cfg, i, node):
-                                    continue
-                                add_edge(final_graph, i, node, {'color': 'green'})
+                if used.core in all_classes:
+                    static_derive_class = all_classes[used.core]
+                    fields = recursively_get_children_of_types(static_derive_class, "field_declaration")
+                    for field in fields:
+                        field_pieces = st(field).replace(";", "").split()
+                        if "static" in field_pieces:
+                            if used.name.replace(used.core + ".", "") in field_pieces:
+                                processed_edges.append((get_index(field, index), node))
+                else:
+                    if not pre_solve and properties.get("last_use", False):
+                        for i in rda_table:
+                            for entry in rda_table[i]["use"]:
+                                if entry.name == used.name and i != node:
+                                    # TODO: THIS IS AN AP - Make sure edges added here are right
+                                    if i in cfg and node in cfg:
+                                        # TODO: check missing i and handle it
+                                        if not nx.has_path(cfg, i, node):
+                                            continue
+                                        add_edge(final_graph, i, node, {'color': 'green'})
+                                    # used.satisfied = True
+                            #         break
+                            # if used.satisfied:
+                            #     break
         if properties.get("last_def", False):
             for available_def in rda_solution[node]["IN"] - rda_solution[node]["OUT"]:
-                ignore_nodes = ['for_statement', 'while_statement', 'if_statement', 'switch_statement']
+                ignore_nodes = ['for_statement', 'while_statement', 'if_statement', 'switch_statement', "for_each_statement"]
                 if read_index(index, node)[-1] in ignore_nodes or read_index(index, available_def.line)[
                     -1] in ignore_nodes:
                     continue
                 add_edge(final_graph, available_def.line, node, {'color': 'orange'})
         # for definition in def_info:
         #     for available_def in rda_solution[node]["IN"]:
         #         if "." in definition.name or "." in available_def.name:
@@ -481,59 +637,213 @@
         #                 smaller = available_def
         #                 bigger = definition
         #             if bigger.name.strip().startswith(smaller.name.strip()):
         #                 if not bigger.name.strip().replace(smaller.name.strip(), "").strip().startswith("."):
         #                     continue
         #                 # add_edge(final_graph, bigger.line or node, smaller.line or node)
         #                 add_edge(final_graph, smaller.line or node, bigger.line or node)
-
+    if not pre_solve:
+        for edge in additional_edges:
+            if debug:
+                add_edge(final_graph, *edge, {'color': 'yellow'})
+            else:
+                add_edge(final_graph, *edge)
+        for edge in processed_edges:
+            add_edge(final_graph, *edge)
+    # for edge in twins:
+    #     continue
+    #     add_edge(final_graph, edge[0], edge[1])
+    #     add_edge(final_graph, edge[1], edge[0])
     return final_graph
 
 
-def rda_cfg_map(rda_solution, CFG_results):
+def rda_cfg_map(rda_solution, CFG_results, remove_unused=True):
     graph = CFG_results.graph
     attrs = {}
     for edge in list(graph.edges):
         out_set = rda_solution[edge[0]]["OUT"]
         in_set = rda_solution[edge[1]]["IN"]
         intersection = set_intersection(out_set, in_set)
         data = graph.get_edge_data(*edge)
         if intersection:
             data['label'] = ",".join([str(intr) for intr in intersection])
         else:
-            graph.remove_edge(*edge)
+            if remove_unused:
+                graph.remove_edge(*edge)
             # logger.warning("Unable to remap edge {}", edge)
         attrs[edge] = data
     nx.set_edge_attributes(graph, attrs)
     return graph
 
 
+def call_variable(call_variable_map, node, edge_for, check_virtual=True):
+    for virtual_var, actual_var in call_variable_map[node]:
+        if check_virtual:
+            if st(virtual_var) == edge_for:
+                return actual_var
+        else:
+            if st(actual_var) == edge_for:
+                return virtual_var
+    return None
+
+
 def dfg_csharp(properties, CFG_results):
     properties = properties
     parser = CFG_results.parser
     index = parser.index
     tree = parser.tree
     assignment = ["assignment_expression"]
     def_statement = ["variable_declarator"]
     increment_statement = ["postfix_unary_expression", "prefix_unary_expression"]
     variable_type = ['identifier', 'this_expression']
     method_calls = ["invocation_expression"]
 
     switch_type = ['switch_expression', 'switch_statement']
     # switch_cases = ['switch_expression_arm', 'switch_section']
-    handled_cases = ["switch_section", "local_declaration_statement"]
 
     method_declaration = ['method_declaration']
     handled_types = assignment + def_statement + increment_statement + method_calls + method_declaration + switch_type
 
+    method_invocation = method_calls + ["object_creation_expression", "explicit_constructor_invocation"]
+
+    call_variable_map = {}
+    handled_cases = ["switch_section", "local_declaration_statement"] + ["class_declaration"]
+
     # if_statement = ["if_statement", "else"]
     # for_statement = ["for_statement"]
     # enhanced_for_statement = ["for_each_statement"]
     # while_statement = ["while_statement"]
 
+    additional_edges = []
+    processed_edges = []
+    cfg_graph = copy.deepcopy(CFG_results.graph)
+
+    node_list = CFG_results.node_list
+
+    all_classes = {
+        st(node_list[read_index(index, x)].child_by_field_name("name")): node_list[read_index(index, x)]
+        for x, y in cfg_graph.nodes(data=True) if 'type_label' in y and y['type_label'] == "class_declaration"
+    }
+    uninitiated_classes = [x for x, y in cfg_graph.nodes(data=True) if 'type_label' in y and
+                           y['type_label'] == "class_declaration" and cfg_graph.in_degree(x) == 0]
+
+    start_rda_init_time = time.time()
+    for edge in list(cfg_graph.edges()):
+        edge_data = cfg_graph.get_edge_data(*edge)[0]
+        # If there is object creation
+        if edge_data["label"] == "class_return":
+            # call_statement = node_list[read_index(index, edge[1])]
+            # call_node = recursively_get_children_of_types(call_statement, method_invocation)[0]
+            if read_index(index, edge[0]) not in node_list:
+                continue
+            last_statement = node_list[read_index(index, edge[0])]
+            class_node = return_first_parent_of_types(last_statement, "class_declaration")
+            class_name = st(class_node.child_by_field_name("name"))
+            class_methods = recursively_get_children_of_types(class_node, method_declaration)
+            class_id = get_index(class_node, index)
+            # find all simple paths between class_id and edge[0]
+            all_paths = nx.all_simple_paths(cfg_graph, source=class_id, target=edge[0])
+            # only_path = nx.shortest_path(cfg_graph, source=class_id, target=edge[0])
+            unique_constructor_children = set()
+            for path in all_paths:
+                for node in path:
+                    unique_constructor_children.add(node)
+            if len(unique_constructor_children) == 0:
+                unique_constructor_children.add(edge[0])
+            # unique_constructor_children = set(only_path)
+            # for nkey, nvalue in node_list.items():
+            #     if node_has_parent(nvalue, class_node):
+            #         unique_constructor_children.add(index[nkey])
+            for class_method in class_methods:
+                class_method_name = st(class_method.child_by_field_name("name"))
+                if class_method_name != class_name:
+                    add_edge(cfg_graph, edge[0], get_index(class_method, index))
+
+            for n_id in unique_constructor_children:
+                additional_edges.append((n_id, edge[1]))
+        # 702 -> 776 check C#
+        # Handle method_call edges and all constructor calls if there are parameters
+        elif edge_data["label"] in ["constructor_call", "method_call"]:
+
+            # class_attributes = ["field_declaration", "static_initializer"]
+            # Not included: ["record_declaration", "method_declaration","compact_constructor_declaration","class_declaration","interface_declaration","annotation_type_declaration","enum_declaration","block","static_initializer","constructor_declaration"]
+
+            call_statement = node_list[read_index(index, edge[0])]
+            if call_statement.type in method_invocation:
+                call_node = call_statement
+            else:
+                marked_index = int(edge_data["controlflow_type"].rsplit("|", 1)[-1])
+                call_nodes = recursively_get_children_of_types(call_statement, method_invocation)
+                for call_node in call_nodes:
+                    if marked_index == get_index(call_node, index):
+                        break
+            method = node_list[read_index(index, edge[1])]
+            if method.type == "class_declaration":
+                class_node = method
+                constructors = recursively_get_children_of_types(class_node, "constructor_declaration")
+                if constructors:
+                    if "target_constructor" in edge_data:
+                        target_constructor = edge_data["target_constructor"]
+                        for constructor in constructors:
+                            if get_index(constructor, index) == target_constructor:
+                                method = constructor
+                                break
+                    else:
+                        continue
+                        # TODO if this else is hit its an AP
+                        # method = constructors[0]
+                else:
+                    continue
+            actual_variables = recursively_get_children_of_types(call_node.child_by_field_name("arguments"), variable_type, index=parser.index,
+                                                                          stop_types=statement_types[
+                                                                              "statement_holders"])
+                # call_node.child_by_field_name("arguments")
+            virtual_variables = []
+            for node in method.named_children:
+                if "parameter_list" in node.type:
+                    virtual_variables = recursively_get_children_of_types(node, variable_type, index=parser.index,
+                                                                          stop_types=statement_types[
+                                                                              "statement_holders"])
+            if actual_variables:
+                # TODO: Handle var_args Type... IterableObject
+                var_args = False
+                if var_args or len(actual_variables) == len(virtual_variables):
+                    for actual_var, virtual_var in zip(actual_variables, virtual_variables):
+                        method_statement_id = edge[1]
+                        if method_statement_id not in call_variable_map:
+                            call_variable_map[method_statement_id] = []
+                        call_variable_map[method_statement_id].append((virtual_var, actual_var))
+                    processed_edges.append(edge)
+                else:
+                    # print(edge[0], edge[1])
+                    logger.error("Number of actual and virtual variables do not match")
+                    if not var_args:
+                        pass
+                        # assert len(actual_variables) == len(virtual_variables)
+        elif edge_data["label"] == "method_return":
+            return_statement = node_list[read_index(index, edge[0])]
+            if return_statement.type == "return_statement" and return_statement.named_children:
+                processed_edges.append(edge)
+        elif edge_data["label"] == "lambda_invocation":
+            processed_edges.append(edge)
+
+    for class_id in uninitiated_classes:
+        class_node = node_list[read_index(index, class_id)]
+        class_name = st(class_node.child_by_field_name("name"))
+        class_methods = recursively_get_children_of_types(class_node, method_declaration)
+
+        descendants = [x for x in nx.descendants(cfg_graph, class_id) if
+                       cfg_graph.out_degree(x) == 0 and cfg_graph.in_degree(x) == 1]
+
+        for class_method in class_methods:
+            class_method_name = st(class_method.child_by_field_name("name"))
+            if class_method_name != class_name:
+                for descendant in descendants:
+                    add_edge(cfg_graph, descendant, get_index(class_method, index))
+
     rda_table = {}
     for root_node in traverse_tree(tree, variable_type):
         if not root_node.is_named:
             if root_node.type == "while" and root_node.parent.type == "do_statement":
                 root_node = root_node.next_named_sibling
                 parent_id = get_index(root_node, index)
                 identifiers_used = recursively_get_children_of_types(root_node, variable_type, index=parser.index,
@@ -550,15 +860,15 @@
                                                                      check_list=parser.symbol_table["scope_map"])
                 if identifiers_used:
                     add_entry(parser, rda_table, parent_id, defined=identifiers_used[-1])
         if root_node.type == "return_statement":
             parent_id = get_index(root_node, index)
             if len(root_node.children) < 2:
                 continue
-            if root_node.children[1].type == "method_invocation":
+            if root_node.children[1].type == "invocation_expression":
                 continue
             identifiers_used = recursively_get_children_of_types(root_node, variable_type, index=parser.index,
                                                                  check_list=parser.symbol_table["scope_map"])
             for identifier in identifiers_used:
                 add_entry(parser, rda_table, parent_id, used=identifier)
         if root_node.type in def_statement:
             parent_statement = return_first_parent_of_types(root_node, statement_types["node_list_type"])
@@ -692,14 +1002,18 @@
             parent_statement = return_first_parent_of_types(
                 root_node,
                 # statement_types["node_list_type"],
                 # [x for x in statement_types["node_list_type"] if x not in block_types],
                 statement_types["non_control_statement"] + statement_types["control_statement"],
                 stop_types=['block'] + handled_types
             )
+            if parent_statement is None:
+                continue
+            if parent_statement.type in handled_cases:
+                continue
             parent_id = get_index(parent_statement, index)
             if parent_id is None:
                 continue
             if parent_id not in CFG_results.graph.nodes:
                 if parent_statement and parent_statement.type in handled_cases:
                     continue
                 raise NotImplementedError
@@ -718,13 +1032,149 @@
             #     add_entry(parser, rda_table, parent_id, used=root_node)
             # else:
             identifiers_used = recursively_get_children_of_types(root_node, variable_type, stop_types=handled_types,
                                                                  index=parser.index,
                                                                  check_list=parser.symbol_table["scope_map"])
             for identifier in identifiers_used:
                 add_entry(parser, rda_table, parent_id, used=identifier)
-    rda_solution = start_rda(index, rda_table, CFG_results)
-    # pp.pprint(rda_solution)
-    final_graph = get_required_edges_from_def_to_use(CFG_results.parser.index, CFG_results.graph, rda_solution, rda_table,
-                                                     CFG_results.graph.nodes, properties=properties)
-    debug_graph = rda_cfg_map(rda_solution, CFG_results)
+    # rda_solution = start_rda(index, rda_table, CFG_results)
+    # # pp.pprint(rda_solution)
+    # final_graph = get_required_edges_from_def_to_use(CFG_results.parser.index, CFG_results.graph, rda_solution, rda_table,
+    #                                                  CFG_results.graph.nodes, properties=properties)
+    # debug_graph = rda_cfg_map(rda_solution, CFG_results)
+    # return final_graph, debug_graph, rda_table, rda_solution
+
+    end_rda_init_time = time.time()
+    end_rda_presolve_time = 0
+    start_rda_presolve_time = 0
+    end_alias_analysis_time = 0
+    start_alias_analysis_time = 0
+    if properties.get("alex_algo", True):
+        start_rda_presolve_time = time.time()
+        rda_solution = start_rda(index, rda_table, cfg_graph, pre_solve=True)
+        # pp.pprint(rda_solution)
+        final_graph = get_required_edges_from_def_to_use(index, cfg_graph, rda_solution, rda_table,
+                                                         cfg_graph.nodes, all_classes, additional_edges,
+                                                         processed_edges,
+                                                         pre_solve=True, properties=properties)
+        used_classes_or_methods = set()
+        for edge in cfg_graph.edges:
+            if "label" in cfg_graph.edges[edge] and cfg_graph.edges[edge]["label"] in ["method_call",
+                                                                                       "constructor_call"]:
+                final_graph.nodes[edge[0]][cfg_graph.edges[edge]["label"]] = edge[1]
+                used_classes_or_methods.add(edge[1])
+        end_rda_presolve_time = time.time()
+        start_alias_analysis_time = time.time()
+        al_analysis = set()
+        proc_analysis = set()
+
+        for node in final_graph.nodes:
+            if node not in used_classes_or_methods:
+                continue
+            if final_graph.nodes[node]["type_label"] == "method_declaration":
+                if "main" in final_graph.nodes[node]["label"]:
+                    continue
+                handled_node_leaf_pair = set()
+                for leaf in nx.algorithms.dag.descendants(final_graph, node):
+                    if len([x for x in final_graph.edges(leaf) if x[0] != x[1]]) == 0:
+                        # print("Leaf: ", leaf)
+                        # final_graph.add_edge(leaf, "exit")
+                        # used_names = [n.name for n in rda_table[leaf]['def']]
+                        # if len(used_names) != 1:
+                        #     logger.error("Multiple used names: %s", used_names)
+                        # get shortest path from node to leaf
+                        paths = nx.all_simple_paths(final_graph, node, leaf)
+                        # print("All_Simple: ", node, leaf)
+                        for path in paths:
+                            # get first edge in path
+                            first_edge = (path[0], path[1], 0)
+                            # get last edge in path
+                            last_edge = (path[-2], path[-1], 0)
+                            # get data for edge
+                            if "used_def" not in final_graph.edges[first_edge]:
+                                continue
+                            edge_for = final_graph.edges[first_edge]["used_def"][1:-1]
+                            # get data for last edge
+                            edge_for_last = final_graph.edges[last_edge]["used_def"][1:-1]
+                            defined_cores = [d.name for d in rda_table[leaf]["def"]]
+                            call_node = None
+                            # print("cs:" + edge_for_last)
+                            if edge_for_last not in defined_cores:
+                                # "method_return", "class_return"
+                                if any([x in final_graph.nodes[leaf] for x in ["method_call", "constructor_call"]]):
+                                    if "method_call" in final_graph.nodes[leaf]:
+                                        call_node = final_graph.nodes[leaf]["method_call"]
+                                    elif "constructor_call" in final_graph.nodes[leaf]:
+                                        call_node = final_graph.nodes[leaf]["constructor_call"]
+                            node_leaf_key = str(leaf) + "_" + str(edge_for)
+                            if node_leaf_key in handled_node_leaf_pair:
+                                continue
+                            handled_node_leaf_pair.add(node_leaf_key)
+                            if node in call_variable_map:
+                                if call_node:
+                                    proc_analysis.add((node, leaf, edge_for, call_node))
+                                # al_analysis.append((node, leaf, edge_for, call_node))
+                                if edge_for_last not in defined_cores:
+                                    n = -1
+                                    while edge_for_last not in defined_cores:
+                                        n = n - 1
+                                        if abs(n - 1) > len(path):
+                                            break
+                                        last_edge = (path[n - 1], path[n], 0)
+                                        if "used_def" not in final_graph.edges[last_edge]:
+                                            continue
+                                        edge_for_last = final_graph.edges[last_edge]["used_def"][1:-1]
+                                        defined_cores = [d.name for d in rda_table[path[n]]["def"]]
+                                        if edge_for_last in defined_cores:
+                                            al_analysis.add((node, path[n], edge_for, None))
+                                else:
+                                    al_analysis.add((node, leaf, edge_for, call_node))
+
+        while proc_analysis:
+            temp_proc_analysis = set()
+            for node, leaf, edge_for, call_node in proc_analysis:
+                completed_analysis = set()
+                for al_entry in al_analysis:
+                    if al_entry[0] == call_node:
+                        mapped_node = call_variable(call_variable_map, call_node, edge_for, check_virtual=False)
+                        if al_entry[2] != st(mapped_node):
+                            continue
+                        leaf = al_entry[1]
+                        completed_analysis.add((node, leaf, edge_for, al_entry[3]))
+                        if al_entry[3] is not None:
+                            temp_proc_analysis.add((node, leaf, edge_for, al_entry[3]))
+                al_analysis.update(completed_analysis)
+            proc_analysis = temp_proc_analysis
+
+        for node, leaf, edge_for, call_node in al_analysis:
+            mapped_node = call_variable(call_variable_map, node, edge_for)
+            # print(st(mapped_node))
+            if mapped_node:
+                if mapped_node.type == "method_invocation":
+                    # if a reference is passed back it is ignored in alias analysis
+                    # to handle turn this into a while loop and trace the return chain
+                    #     track_leaf = leaf
+                    #     leaf_node = node_list[read_index(index, track_leaf)]
+                    #     if leaf_node.type == "return_statement":
+                    # print("skipped")
+                    continue
+                # [(st(a),st(b)) for a,b in call_variable_map[100]]
+                # print(edge_for, final_graph.nodes[leaf]["label"])
+                set_add(rda_table[leaf]["def"],
+                        Identifier(parser, mapped_node, leaf, full_ref=mapped_node,
+                                   declaration=True,
+                                   method_call=True))
+        end_alias_analysis_time = time.time()
+    # print_table(index, rda_table)
+    start_rda_time = time.time()
+    rda_solution = start_rda(index, rda_table, cfg_graph)
+    final_graph = get_required_edges_from_def_to_use(index, cfg_graph, rda_solution, rda_table,
+                                                     cfg_graph.nodes, all_classes, additional_edges, processed_edges,
+                                                     pre_solve=False, properties=properties)
+    end_rda_time = time.time()
+    if debug:
+        logger.warning("RDA init, presolve, alias, rda: {}, {}, {}, {}", end_rda_init_time - start_rda_init_time,
+                       end_rda_presolve_time - start_rda_presolve_time,
+                       end_alias_analysis_time - start_alias_analysis_time,
+                       end_rda_time - start_rda_time)
+    debug_graph = rda_cfg_map(rda_solution, CFG_results, remove_unused=False)
     return final_graph, debug_graph, rda_table, rda_solution
```

### Comparing `comex-0.1.2/src/comex/codeviews/SDFG/SDFG_java.py` & `comex-0.1.3/src/comex/codeviews/SDFG/SDFG_java.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import pprint
 import time
+import os
 from collections import defaultdict
 
 import networkx as nx
 from deepdiff import DeepDiff
 from loguru import logger
 
 from ...utils.java_nodes import statement_types
@@ -33,18 +34,14 @@
 # call_variable_map = {}
 # node_list = {}
 debug = False
 # if any(
 #         # GITHUB_ACTIONS
 #         x in os.environ for x in ("PYCHARM_HOSTED",)
 # ):
-#     debug = any(
-#         # GITHUB_ACTIONS
-#         x in os.environ for x in ("PYCHARM_HOSTED",)
-# ):
 #     debug = True
 # properties = {
 #     "last_use": False,
 #     "last_def": False,
 #     "alex_algo": False
 # }
 
@@ -1176,14 +1173,15 @@
                             last_edge = (path[-2], path[-1], 0)
                             # get data for edge
                             edge_for = final_graph.edges[first_edge]["used_def"]
                             # get data for last edge
                             edge_for_last = final_graph.edges[last_edge]["used_def"]
                             defined_cores = [d.core for d in rda_table[leaf]["def"]]
                             call_node = None
+                            # print("java:" + edge_for_last)
                             if edge_for_last not in defined_cores:
                                 # "method_return", "class_return"
                                 if any([x in final_graph.nodes[leaf] for x in ["method_call", "constructor_call"]]):
                                     if "method_call" in final_graph.nodes[leaf]:
                                         call_node = final_graph.nodes[leaf]["method_call"]
                                     elif "constructor_call" in final_graph.nodes[leaf]:
                                         call_node = final_graph.nodes[leaf]["constructor_call"]
@@ -1223,21 +1221,23 @@
                         if al_entry[3] is not None:
                             temp_proc_analysis.add((node, leaf, edge_for, al_entry[3]))
                 al_analysis.update(completed_analysis)
             proc_analysis = temp_proc_analysis
 
         for node, leaf, edge_for, call_node in al_analysis:
             mapped_node = call_variable(call_variable_map, node, edge_for)
+            # print(st(mapped_node))
             if mapped_node:
                 if mapped_node.type == "method_invocation":
                     # if a reference is passed back it is ignored in alias analysis
                     # to handle turn this into a while loop and trace the return chain
                     #     track_leaf = leaf
                     #     leaf_node = node_list[read_index(index, track_leaf)]
                     #     if leaf_node.type == "return_statement":
+                    # print("skipped")
                     continue
                 # [(st(a),st(b)) for a,b in call_variable_map[100]]
                 # print(edge_for, final_graph.nodes[leaf]["label"])
                 set_add(rda_table[leaf]["def"],
                         Identifier(parser, mapped_node, leaf, full_ref=mapped_node,
                                    declaration=True,
                                    method_call=True))
```

### Comparing `comex-0.1.2/src/comex/codeviews/combined_graph/combined_driver.py` & `comex-0.1.3/src/comex/codeviews/combined_graph/combined_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/tree_parser/cs_parser.py` & `comex-0.1.3/src/comex/tree_parser/cs_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..tree_parser.custom_parser import CustomParser
-
+from loguru import logger
 
 class CSParser(CustomParser):
     def __init__(self, src_language, src_code):
         super().__init__(src_language, src_code)
 
     def check_declaration(self, current_node):
-        parent_types = ["variable_declarator", "catch_declaration"]
+        parent_types = ["variable_declarator", "catch_declaration", "parameter"]
         current_types = ["identifier"]
         if (
                 current_node.parent is not None
                 and current_node.parent.type in parent_types
                 and current_node.type in current_types
         ):
             return True
@@ -26,23 +26,44 @@
         # print(node.type, node.text.decode('utf-8'))
         if node.type == "parameter":
             return node.children[0].text.decode('utf-8')
 
         for child in node.parent.children:
             # print(child.type, child.text.decode('utf-8'))
             if child.type in datatypes:
+                if child.type == "implicit_type":
+                    # print("___________")
+                    try:
+                        object_type = node.named_children[-1].named_children[-1].named_children[0]
+                        return object_type.text.decode('utf-8')
+                    except:
+                        logger.warning("ERROR")
+                
+                # print(child.type, child.text.decode('utf-8'))
                 return child.text.decode('utf-8')
         return None
 
     def scope_check(self, parent_scope, child_scope):
         for p in parent_scope:
             if p not in child_scope:
                 # print("parent", parent_scope, "child", child_scope)
                 return False
         return True
+    
+    # TODO: Check correctness
+    def longest_scope_match(self, name_matches, symbol_table):
+        """Given a list of name matches, return the longest scope match"""
+        # [(ind, var), (ind,var)]
+        scope_array = list(map(lambda x: symbol_table['scope_map'][x[0]], name_matches))
+        # scope_array.sort(key=lambda x: len(x), reverse=True)
+        # index = max(range(len(scope_array)), key=lambda x: len(x))
+        max_val = max(scope_array, key=lambda x: len(x))
+        for i in range(len(scope_array)):
+            if scope_array[i] == max_val:
+                return name_matches[i][0]
 
     def create_all_tokens(
             self,
             src_code,
             root_node,
             all_tokens,
             label,
@@ -154,42 +175,67 @@
                     # ? not sure about this yet Console.writeline - if i say expression it will pick console if i say name it will pick the object but java side it picks the parent?
                     method_map.append(current_index)
 
                 while (
                         current_node.parent is not None
                         and current_node.parent.type == "member_access_expression"
                 ):
-                    current_node = current_node.parent
+                    if current_node.parent.next_named_sibling is not None and current_node.parent.next_named_sibling.type == "argument_list":
+                        break
+                    else:
+                        current_node = current_node.parent
 
                 if (
                         current_node.parent is not None
                         and current_node.parent.type == "invocation_expression"
                 ):
                     method_map.append(index)
                 label[index] = current_node.text.decode("UTF-8")
 
-            # Modify this to take care of scope
             if self.check_declaration(current_node):
                 variable_name = label[index]
                 declaration[index] = variable_name
 
                 variable_type = self.get_type(current_node.parent)
                 if variable_type is not None:
                     symbol_table["data_type"][index] = variable_type
             else:
                 current_scope = symbol_table['scope_map'][index]
-                for (ind, var) in declaration.items():
-                    if var == label[index]:
+                if current_node.type == "member_access_expression":
+                    field_variable = current_node.children[-1]
+                    # entire_variable_name = current_node.text.decode('utf-8')
+                    field_variable_name = field_variable.text.decode('utf-8')
+                    
+                    for (ind,var) in declaration.items():
+                        if var == field_variable_name:
+                            parent_scope = symbol_table['scope_map'][ind]
+                            if self.scope_check(parent_scope, current_scope):
+                                declaration_map[index] = ind
+                                break
+                else:
+                    name_matches = []
+                    for (ind, var) in declaration.items():
+                        if var == label[index]:
+                            parent_scope = symbol_table['scope_map'][ind]
+                            if self.scope_check(parent_scope, current_scope):
+                                name_matches.append((ind,var))
+                    for (ind, var) in name_matches:
                         parent_scope = symbol_table['scope_map'][ind]
-                        # print(ind,var)
-                        if self.scope_check(parent_scope, current_scope):
-                            # print(ind, var)
-                            # print("^^", current_node.parent.type, index, var, "Current:", current_scope, "Parent:", parent_scope)
-                            declaration_map[index] = ind
-                            break
+                        closest_index = self.longest_scope_match(name_matches, symbol_table)
+                        declaration_map[index] = closest_index
+                        break
+                    # for (ind, var) in declaration.items():
+                    #     if var == label[index]:
+                    #         parent_scope = symbol_table['scope_map'][ind]
+                    #         # print(ind,var)
+                    #         if self.scope_check(parent_scope, current_scope):
+                    #             # print(ind, var)
+                    #             # print("^^", current_node.parent.type, index, var, "Current:", current_scope, "Parent:", parent_scope)
+                    #             declaration_map[index] = ind
+                    #             break
 
         else:
             for child in root_node.children:
                 self.create_all_tokens(
                     src_code,
                     child,
                     all_tokens,
```

### Comparing `comex-0.1.2/src/comex/tree_parser/custom_parser.py` & `comex-0.1.3/src/comex/tree_parser/custom_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,32 @@
 
         grammar_repos = [
             ("https://github.com/tree-sitter/tree-sitter-java", "09d650def6cdf7f479f4b78f595e9ef5b58ce31e"),
             ("https://github.com/tree-sitter/tree-sitter-c-sharp", "3ef3f7f99e16e528e6689eae44dff35150993307")
         ]
         vendor_languages = []
 
-        if not os.path.isfile(shared_languages):
-            print("First time running COMEX: Setting up tree-sitter grammars")
-            for url, commit in grammar_repos:
-                vendor_language = os.path.join(clone_directory, url.rstrip("/").split("/")[-1])
-                vendor_languages.append(vendor_language)
-                if os.path.exists(vendor_language):
-                    shutil.rmtree(vendor_language)
-                os.makedirs(vendor_language, exist_ok=True)
-                subprocess.check_call(["git", "init"], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-                subprocess.check_call(["git", "remote", "add", "origin", url], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-                subprocess.check_call(["git", "fetch", "--depth=1", "origin", commit], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-                subprocess.check_call(["git", "checkout", commit], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-        else:
-            for url, commit in grammar_repos:
-                vendor_language = os.path.join(clone_directory, url.rstrip("/").split("/")[-1])
-                vendor_languages.append(vendor_language)
+        for url, commit in grammar_repos:
+            grammar = url.rstrip("/").split("/")[-1]
+            vendor_language = os.path.join(clone_directory, grammar)
+            vendor_languages.append(vendor_language)
+            if os.path.isfile(shared_languages) and not os.path.exists(vendor_language):
+                os.remove(shared_languages)
+            elif not os.path.isfile(shared_languages) and os.path.exists(vendor_language):
+                shutil.rmtree(vendor_language)
+            elif not os.path.isfile(shared_languages) and not os.path.exists(vendor_language):
+                pass
+            else:
+                continue
+            print(f"Intial Setup: First time running COMEX on {grammar}")
+            os.makedirs(vendor_language, exist_ok=True)
+            subprocess.check_call(["git", "init"], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+            subprocess.check_call(["git", "remote", "add", "origin", url], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+            subprocess.check_call(["git", "fetch", "--depth=1", "origin", commit], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+            subprocess.check_call(["git", "checkout", commit], cwd=vendor_language, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
 
         # build_id = ""
         # for vendor_language in vendor_languages:
         #     commit_hash = get_commit_hash(vendor_language)
         #     if commit_hash:
         #         build_id += commit_hash
         #     else:
```

### Comparing `comex-0.1.2/src/comex/tree_parser/java_parser.py` & `comex-0.1.3/src/comex/tree_parser/java_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,15 @@
 
                 variable_type = self.get_type(current_node.parent)
                 if variable_type is not None:
                     symbol_table["data_type"][index] = variable_type
             else:
                 current_scope = symbol_table['scope_map'][index]
 
-                if current_node.type == "field_access":
-                    
+                if current_node.type == "field_access":   
                     field_variable = current_node.children[-1]
                     # entire_variable_name = current_node.text.decode('utf-8')
                     field_variable_name = field_variable.text.decode('utf-8')
 
                     for (ind,var) in declaration.items():
                         if var == field_variable_name:
                             parent_scope = symbol_table['scope_map'][ind]
```

### Comparing `comex-0.1.2/src/comex/tree_parser/parser_driver.py` & `comex-0.1.3/src/comex/tree_parser/parser_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/utils/DFG_utils.py` & `comex-0.1.3/src/comex/utils/DFG_utils.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/utils/cs_nodes.py` & `comex-0.1.3/src/comex/utils/cs_nodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,24 +6,29 @@
     "local_function_statement",
 ]
 class_declaration_statements = [
     "constructor_declaration",
     "interface_declaration",
     "property_declaration",
     "class_declaration",
+    "field_declaration",
+    "struct_declaration",
+    "local_function_statement",
+    
 ]
 
 inner_node_type = [
     "empty_statement",
     "local_declaration_statement",
     # 'local_variable_declaration'
     # ! used in DFG graphcodebert - Swapped with local_declaration_statement
     # '_declaration',
     "labeled_statement",
     "expression_statement",
+    
 ] + scope_only_blocks
 non_control_statements = inner_node_type + class_declaration_statements
 loop_control_statements = ["for_each_statement", "while_statement", "for_statement"]
 control_statements = loop_control_statements + [
     "do_statement",
     "goto_statement",
     "throw_statement",
@@ -36,31 +41,46 @@
     "switch_statement",
     "switch_expression_arm",
     "switch_section",
     "lock_statement",  # 'synchronized_statement',
     "try_statement",
     # 'try_with_resources_statement'
 ]
+statement_holders = [
+        "block",
+        # "switch_block_statement_group",
+        "switch_body",
+        "switch_section",
+        "declaration_list"
+        # "constructor_body",
+        # "declaration_list",
+        # "module_body",
+        # "program"
+    ]
 # based on handling simmilarity
 statement_types = {
     "node_list_type": non_control_statements
     + control_statements
-    + ["method_declaration"],
+    + ["method_declaration", "local_function_statement"],
     "scope_only_blocks": scope_only_blocks,
     "outer_node_type": ["for_statement"],
     "inner_node_type": inner_node_type,
     "non_control_statement": non_control_statements,
     "control_statement": control_statements,
     "loop_control_statement": loop_control_statements,
     # 'terminal_inner': ['switch_expression_arm', 'switch_section'],
     "not_implemented": [
         # 'try_with_resources_statement'
     ],
+    "statement_holders": statement_holders,
+    "definition_types": ["method_declaration", "constructor_declaration", "class_declaration", "field_declaration", "interface_declaration", "operator_declaration", "conversion_operator_declaration"]
 }
 # TODO: add method_return_types
+method_return_types = ['integral_type', 'void_type', 'type_identifier', 'generic_type', 'scoped_type_identifier', 'floating_point_type', 'boolean_type', 'array_type']
+
 
 def cl(child):
     if child is None:
         # logger.error
         return ""
     else:
         return child.text.decode()
@@ -91,15 +111,94 @@
 
 def return_index_of_first_parent_of_type(node, parent_type):
     while node.parent is not None:
         if node.parent.type == parent_type:
             return node.parent
         node = node.parent
     return None
-
+def get_signature(node):
+    signature = []
+    formal_parameters = node.child_by_field_name('parameters')
+    formal_parameters = list(filter(lambda x: x.type == 'parameter', formal_parameters.named_children))
+    # for formal_parameter in formal_parameters:
+    #     for child in formal_parameter.children:
+    #         if child.type != "identifier":
+    #             signature.append(child.text.decode('utf-8'))\
+    for formal_parameter in formal_parameters:
+        param_type = formal_parameter.child_by_field_name('type')
+        if param_type is None:
+            try:
+                param_type = list(filter(lambda x: x.type == 'identifier', formal_parameter.named_children))[0]
+                param_text = param_type.text.decode('utf-8')
+                if '[]' in param_text:
+                    param_text = param_text.split('[',1)
+                    param_text = " [".join(param_text)
+                signature.append(param_text)
+            except:
+                pass
+        else:
+            param_text = param_type.text.decode('utf-8')
+            if '[]' in param_text:
+                param_text = param_text.split('[',1)
+                # print(param_text)
+                param_text = " [".join(param_text)
+                # print(param_text)
+            signature.append(param_text)
+
+    return tuple(signature)
+
+def abstract_method(node):
+    method_body = get_child_of_type(node, ["block"])
+    while node is not None:
+        if node.type == "declaration_list" and node.parent.type == "class_declaration":
+            node = node.parent
+
+            modifiers = get_child_of_type(node, ["modifiers"])
+            if modifiers is not None and "abstract" in modifiers.text.decode("utf-8") and method_body is None:
+                return True
+        node = node.parent
+    return False
+def get_child_of_type(node, type_list):
+    out = list(filter(lambda x : x.type in type_list, node.children))
+    if len(out) > 0:
+        return out[0]
+    else: 
+        return None
+def get_class_name(node, index):
+    "Returns the class name when a method declaration or constructor declaration is passed to it"
+    type_identifiers = ["type_identifier", "generic_type", "scoped_type_identifier"]
+    while node is not None:
+        if node.type == "declaration_list" and node.parent.type == "class_declaration":
+            node = node.parent
+        
+            class_index = index[(node.start_point, node.end_point, node.type)]
+            class_name = [(list(filter(lambda child: child.type == "identifier", node.children))[0]).text.decode("UTF-8")]
+            
+            interface_node = get_child_of_type(node, ["super_interfaces"])
+            if interface_node is not None:
+                class_name.append(get_child_of_type(interface_node, ["type_list"]).text.decode("UTF-8"))
+
+            superclass_node = get_child_of_type(node, ["superclass"])
+            if superclass_node is not None:
+                class_name.append(get_child_of_type(superclass_node, ["type_identifier"]).text.decode("UTF-8"))
+
+            return class_index, class_name
+        
+        elif node.type == "declaration_list" and node.parent.type == "object_creation_expression":
+            node = node.parent
+            class_index = index[(node.start_point, node.end_point, node.type)]
+            class_name = [list(filter(lambda child: child.type in type_identifiers, node.children))[0].text.decode("UTF-8")]
+            return class_index, class_name
+        elif node.type == "interface_body" and node.parent.type == "interface_declaration":
+            return None
+            node = node.parent
+            class_index = index[(node.start_point, node.end_point, node.type)]
+            class_name = list(filter(lambda child: child.type == "identifier", node.children))[0]
+            return class_index, class_name.text.decode("UTF-8")
+        node = node.parent
 
 def get_nodes(root_node=None, node_list={}, graph_node_list=[], index={}, records={}):
     """
     Returns statement level nodes recursively from the concrete syntax tree passed to it. Uses records to maintain required supplementary information.
     noe_list maintains an intermediate representation and graph_node_list returns the final list.
     """
     #  These are within statements so handled separately - logic after assumed statements to be finest granularity
@@ -186,46 +285,84 @@
             node_list[
                 (root_node.start_point, root_node.end_point, root_node.type)
             ] = root_node
             # Set default label values for the node and then modify based on node type if required in the following
             # if-else ladder
             label = root_node.text.decode("UTF-8")
             type_label = "expression_statement"
+            # print(label, root_node.type)
             if root_node.type in [
                 "method_declaration",
                 "interface_declaration",
                 "constructor_declaration",
                 "property_declaration",
             ]:
+                # method_name = list(
+                #     filter(lambda child: child.type == "identifier", root_node.children)
+                # )
+                # parameter_list = list(
+                #     filter(
+                #         lambda child: child.type == "parameter_list", root_node.children
+                #     )
+                # )
+                # label = method_name[-1].text.decode("UTF-8")
+                # if parameter_list:
+                #     label = label + parameter_list[0].text.decode("UTF-8")
+                # type_label = root_node.type
+                # # ? make sure records is being updated for the newer updates if required
+                # records["method_list"][method_name[-1].text.decode("UTF-8")] = index[
+                #     root_node.start_point, root_node.end_point, root_node.type
+                # ]
+                # graph_node_list.append(
+                #     (
+                #         index[
+                #             (root_node.start_point, root_node.end_point, root_node.type)
+                #         ],
+                #         method_name[-1].start_point[0],
+                #         label,
+                #         type_label,
+                #     )
+                # )
+                label = ""
+                for child in root_node.children:
+                    if child.type != "block" and child.type != "constructor_body":
+                        label = label + " " + child.text.decode('utf-8')
                 method_name = list(
                     filter(lambda child: child.type == "identifier", root_node.children)
                 )
-                parameter_list = list(
-                    filter(
-                        lambda child: child.type == "parameter_list", root_node.children
-                    )
-                )
-                label = method_name[-1].text.decode("UTF-8")
-                if parameter_list:
-                    label = label + parameter_list[0].text.decode("UTF-8")
+                method_name = method_name[0].text.decode("UTF-8")
+                method_index = index[(root_node.start_point, root_node.end_point, root_node.type)]
                 type_label = root_node.type
-                # ? make sure records is being updated for the newer updates if required
-                records["method_list"][method_name[-1].text.decode("UTF-8")] = index[
-                    root_node.start_point, root_node.end_point, root_node.type
-                ]
-                graph_node_list.append(
-                    (
-                        index[
-                            (root_node.start_point, root_node.end_point, root_node.type)
-                        ],
-                        method_name[-1].start_point[0],
-                        label,
-                        type_label,
-                    )
-                )
+                try:
+                    signature = get_signature(root_node)
+                    class_index, class_name_list = get_class_name(root_node, index)
+                    if method_name == "Main":
+                        # print("Main method found")
+                        records["main_method"] = method_index
+                        records["main_class"] = class_index
+                    if abstract_method(root_node) == False:
+                        for class_name in class_name_list:
+                            if root_node.type == "constructor_declaration":
+                                if class_name == method_name:
+                                    records["constructor_list"][((class_name,method_name), signature)] = method_index
+                                return_type = None
+                            else:
+                                records["method_list"][((class_name,method_name), signature)] = method_index
+                                try:
+                                    return_type = list(filter(lambda child: child.type in method_return_types, root_node.children))
+                                    return_type = return_type[0].text.decode("UTF-8")
+                                except:
+                                    raise Exception("No return type found for method, update method_return_types", method_name)
+                            
+                            records["return_type"][((class_name,method_name), signature)] = return_type
+
+                except Exception as e:
+                    # print("*******", e)
+                    pass
+                graph_node_list.append((method_index, root_node.start_point[0],label,type_label))
             elif (
                 root_node.type == "class_declaration"
                 # or root_node.type == "constructor_declaration"
             ):
                 modifiers = list(filter(lambda child: child.type != "declaration_list", root_node.children))
                 class_name = list(filter(lambda child: child.type == "identifier", root_node.children))[0].text.decode("UTF-8")
                 label = ""
```

### Comparing `comex-0.1.2/src/comex/utils/java_nodes.py` & `comex-0.1.3/src/comex/utils/java_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,16 @@
             # Set default label values for the node and then modify based on node type if required in the following if-else ladder
             label = root_node.text.decode("UTF-8")
             type_label = "expression_statement"
             if check_anonymous_class(root_node) and root_node.type not in statement_types["definition_types"]:
                 try:
                     label = label.split("{")[0] + label.split("}")[-1]
                 except:
-                    print("INCORRECT anonymous class label", label)
+                    # print("INCORRECT anonymous class label", label)
+                    pass
             # elif check_lambda(root_node) and root_node.type not in statement_types["definition_types"]:
             elif check_lambda(root_node) and root_node.type not in statement_types["definition_types"]:
                 raw_label = root_node.text.decode("utf-8")
 
                 label = ""
                 for lambda_expression in get_all_lambda_body(root_node):
                     split_label = raw_label.split(lambda_expression.text.decode("utf-8"),2)
@@ -354,15 +355,15 @@
                 try:
                     if "{" in label:
                         label = label.split("{")[0] + label.split("}")[-1]
                     else:
                         label = root_node.text.decode('utf-8')
                 except:
                     raise Exception("INCORRECT lambda expression label", label)
-                    print("INCORRECT lambda expression label", label)
+                    # print("INCORRECT lambda expression label", label)
 
             elif (root_node.type == "method_declaration" or root_node.type == "constructor_declaration"):
                 label = ""
                 for child in root_node.children:
                     if child.type != "block" and child.type != "constructor_body":
                         label = label + " " + child.text.decode('utf-8')
                 method_name = list(
```

### Comparing `comex-0.1.2/src/comex/utils/postprocessor.py` & `comex-0.1.3/src/comex/utils/postprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import json
 import os
 import re
 from subprocess import check_call
 
 import networkx as nx
 from networkx.readwrite import json_graph
@@ -22,15 +23,16 @@
     return graph_json
 
 
 def to_dot(graph):
     return nx.nx_pydot.to_pydot(graph)
 
 
-def write_to_dot(graph, filename, output_png=False):
+def write_to_dot(og_graph, filename, output_png=False):
+    graph = copy.deepcopy(og_graph)
     if not os.getenv("GITHUB_ACTIONS"):
         for node in graph.nodes:
             if 'label' in graph.nodes[node]:
                 graph.nodes[node]['label'] = re.escape(graph.nodes[node]['label'])
         nx.nx_pydot.write_dot(graph, filename)
         if output_png:
             check_call(
```

### Comparing `comex-0.1.2/src/comex/utils/preprocessor.py` & `comex-0.1.3/src/comex/utils/preprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex/utils/src_parser.py` & `comex-0.1.3/src/comex/utils/src_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.2/src/comex.egg-info/PKG-INFO` & `comex-0.1.3/src/comex.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -18,16 +18,15 @@
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
-
+---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
@@ -41,29 +40,29 @@
 ```console
 pip install -r requirements-dev.txt
 ```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
-### Usage as a CLI
+## Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
 
 The attributes and options supported by the CLI are well documented and can be viewed by running:
 ```console
 comex --help
 ```
 
 For example, to generate a combined CFG and DFG graph for a java file, you can run:
 ```console
 comex --lang "java" --code-file ./test.java --graphs "cfg,dfg"
 ```
 
-### Usage as a Python Package
+## Usage as a Python Package
 
 The comex package can be used by importing required drivers as follows:
 
 ```python
 from comex.codeviews.combined_graph.combined_driver import CombinedDriver
 
 CombinedDriver(
@@ -83,16 +82,43 @@
 
 output_file: denotes the output file to which the generated graph is written
 
 graph_format: denotes the format of the output graph. Currently supported formats are "dot" and "json". To generate both pass "all"
 
 codeviews: refers to the configuration passed for each codeview
 ````
+---
+## Limitations
+
+While `comex` provides _method-level_ and _file-level_ support for both Java and C\#, it's important to note the following limitations and known issues:
+
+### Java
+- **No Inter-file Analysis Support**: The tool currently does not support codeviews that involve interactions between multiple Java files. It is designed to generate codeviews for individual Java files only.
+
+- **Syntax Errors in Code**: Despite supporting non-compileable code, to ensure accurate codeviews, the input Java code must be free of syntax errors. Code with syntax errors may not be correctly parsed and displayed in the generated codeviews.
+
+- **Limited Support for Function Call Arguments**: The tool does not provide proper support for when a function call is passed as an argument to another function call in Java code. The resulting codeview might not accurately represent the intended behavior in such cases.
+
+### C\#
+In addition to the limitations mentioned for Java, the tool has the following limitations specific to C#:
+
+- **No Support for Lambda Functions and Arrow Expressions**: The tool does not support codeviews involving lambda functions and arrow expressions in C#. The generated codeviews may not accurately represent these language features.
+
+- **No Support for Compiler Directives**: Compiler directives, such as pragma directives, are not supported by the tool. Code involving such directives may not be properly displayed in the generated codeviews.
+
+- **Incomplete Operator Declaration Support**: The tool may have limited support for operator declarations in C#. Certain constraints and edge cases related to operator overloading might not be fully captured in the generated codeviews.
+
+- **Limited Support for Inheritance and Abstraction**: The tool's support for inheritance and abstraction in C# is not fully comprehensive. Codeviews involving complex inheritance hierarchies or advanced abstraction patterns may not be accurately represented.
+
+Please note that while we continuously work to improve the tool and address these limitations, the current implementation may not be perfect. We appreciate your understanding and encourage you to provide feedback and report any issues you encounter, as this helps us enhance the tool's capabilities.
+
+---
+
 
-### Output Examples:
+## Output Examples:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 ![Sample AST CFG DFG](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/sample.png)
 
 Below we present more examples of input code snippets and generated codeviews for both Java and C#.
```

### Comparing `comex-0.1.2/src/comex.egg-info/SOURCES.txt` & `comex-0.1.3/src/comex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

