# Comparing `tmp/rdfhash-0.4.5.tar.gz` & `tmp/rdfhash-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfhash-0.4.5.tar", last modified: Tue Jun  6 16:52:37 2023, max compression
+gzip compressed data, was "rdfhash-0.4.6.tar", last modified: Thu Jun 22 21:37:50 2023, max compression
```

## Comparing `rdfhash-0.4.5.tar` & `rdfhash-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.990050 rdfhash-0.4.5/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 16:52:37.989918 rdfhash-0.4.5/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.5/README.md
--rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.5/pyproject.toml
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.988065 rdfhash-0.4.5/rdfhash/
--rw-r--r--   0 grahamneil   (501) staff       (20)      147 2023-06-06 14:58:14.000000 rdfhash-0.4.5/rdfhash/__init__.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     4136 2023-06-06 14:58:10.000000 rdfhash-0.4.5/rdfhash/cli.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.5/rdfhash/logger.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     9839 2023-06-06 16:30:35.000000 rdfhash-0.4.5/rdfhash/main.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.989433 rdfhash-0.4.5/rdfhash/utils/
--rw-r--r--   0 grahamneil   (501) staff       (20)      592 2023-06-06 08:26:03.000000 rdfhash-0.4.5/rdfhash/utils/__init__.py
--rw-r--r--   0 grahamneil   (501) staff       (20)    10765 2023-06-06 16:50:17.000000 rdfhash-0.4.5/rdfhash/utils/graph.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     2944 2023-06-06 08:26:03.000000 rdfhash-0.4.5/rdfhash/utils/hash.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.988866 rdfhash-0.4.5/rdfhash.egg-info/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)      383 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/SOURCES.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/dependency_links.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/entry_points.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       63 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/requires.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/top_level.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 16:52:37.990085 rdfhash-0.4.5/setup.cfg
--rw-r--r--   0 grahamneil   (501) staff       (20)     1006 2023-06-06 16:51:53.000000 rdfhash-0.4.5/setup.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.989646 rdfhash-0.4.5/test/
--rw-r--r--   0 grahamneil   (501) staff       (20)     3924 2023-06-06 16:44:42.000000 rdfhash-0.4.5/test/test_examples.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-22 21:37:50.230293 rdfhash-0.4.6/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5602 2023-06-22 21:37:50.230167 rdfhash-0.4.6/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5184 2023-06-22 21:34:48.000000 rdfhash-0.4.6/README.md
+-rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.6/pyproject.toml
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-22 21:37:50.228620 rdfhash-0.4.6/rdfhash/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      147 2023-06-22 01:10:49.000000 rdfhash-0.4.6/rdfhash/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     4160 2023-06-22 21:34:48.000000 rdfhash-0.4.6/rdfhash/cli.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2023-06-22 01:10:49.000000 rdfhash-0.4.6/rdfhash/logger.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     9839 2023-06-22 01:10:49.000000 rdfhash-0.4.6/rdfhash/main.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-22 21:37:50.229874 rdfhash-0.4.6/rdfhash/utils/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      592 2023-06-22 01:10:49.000000 rdfhash-0.4.6/rdfhash/utils/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)    10925 2023-06-22 21:34:48.000000 rdfhash-0.4.6/rdfhash/utils/graph.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     2944 2023-06-22 01:10:49.000000 rdfhash-0.4.6/rdfhash/utils/hash.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-22 21:37:50.229498 rdfhash-0.4.6/rdfhash.egg-info/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5602 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)      383 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/SOURCES.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/dependency_links.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/entry_points.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       63 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/requires.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-22 21:37:50.000000 rdfhash-0.4.6/rdfhash.egg-info/top_level.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-22 21:37:50.230409 rdfhash-0.4.6/setup.cfg
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1013 2023-06-22 21:34:48.000000 rdfhash-0.4.6/setup.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-22 21:37:50.230003 rdfhash-0.4.6/test/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     3910 2023-06-22 21:34:48.000000 rdfhash-0.4.6/test/test_examples.py
```

### Comparing `rdfhash-0.4.5/rdfhash/cli.py` & `rdfhash-0.4.6/rdfhash/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import sys
 import logging
 
 from rdfhash.main import hash_subjects, reverse_hash_subjects
 from rdfhash.logger import logger
-from rdfhash.utils.hash import hashlib_methods
-from rdfhash.utils.graph import mime, file_ext
+from rdfhash.utils.hash import hash_types
+from rdfhash.utils.graph import mime, file_ext, graph_types
 
 
 def get_parser():
     """Return argument parser for command 'hash_subjects'.
     Returns: argparse.ArgumentParser: _description_
     """
     parser = argparse.ArgumentParser(
@@ -19,67 +19,71 @@
         ),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
         "data",
         nargs="+",
-        help="Input RDF string or file path. Supported file formats are '.nt', '.nq', '.ttl', '.trig', '.n3', '.xml', '.rdf'.",
+        help="Input RDF string or file path.\nSupported file formats: ['."
+        + "', '.".join(file_ext.keys())
+        + "']",
     )
 
     parser.add_argument(
         "-f",
         "--format",
-        help="Input format. Supports 'turtle', 'ntriples', 'nquads', 'xml', 'n3'.",
+        help="Input format.\nSupports: ['" + "', '".join(mime.keys()) + "']",
         default="text/turtle",
     )
 
     parser.add_argument(
         "-g",
         "--graph",
         default="oxrdflib",
-        help="Graph library to use. Supports 'oxrdflib', 'rdflib', 'oxigraph'.",
+        help="Graph library to use.\nSupports: ['"
+        + "', '".join(graph_types.keys())
+        + "']",
     )
 
     parser.add_argument(
         "-a",
         "--accept",
         default="text/turtle",
-        help="Output accept format. Supports 'turtle', 'ntriples', 'nquads', 'xml', 'n3'.",
+        help=f"Output accept format.\nSupports: ['" + "', '".join(mime.keys()) + "']",
     )
 
     parser.add_argument(
         "-t",
         "--template",
         default="{method}:{value}",
         help="Hash URI template. '{method}' corresponds to the hashing method (eg. 'sha256'). '{value}' corresponds to the calculated hash value.",
     )
 
     parser.add_argument(
         "-m",
         "--method",
         "--hash-method",
         default="sha256",
-        help="Hash method. Supports '" + "', '".join(hashlib_methods.keys()) + "'.",
+        help="Hash method.\nSupports: ['" + "', '".join(hash_types.keys()) + "']",
     )
 
     parser.add_argument(
         "-s",
         "--sparql",
         "--sparql-select-subjects",
-        default="SELECT DISTINCT ?s WHERE { ?s ?p ?o . FILTER (isBlank(?s)) }",
+        default="SELECT ?s WHERE { ?s ?p ?o . FILTER (isBlank(?s)) }",
         help="SPARQL SELECT query returning subject URIs to replace with hash of"
         " their triples. Defaults to all blank node subjects.",
     )
 
     parser.add_argument(
         "-r",
         "--reverse",
         action="store_true",
-        help="Reverse hashed URIs to Blank Nodes. --template is used to identify hashed URI te",
+        help="Reverse hashed URIs to Blank Nodes. --template is used to identify hashed URI template.",
     )
 
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Show 'info' level logs.",
```

### Comparing `rdfhash-0.4.5/rdfhash/logger.py` & `rdfhash-0.4.6/rdfhash/logger.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.5/rdfhash/main.py` & `rdfhash-0.4.6/rdfhash/main.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.5/rdfhash/utils/__init__.py` & `rdfhash-0.4.6/rdfhash/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.5/rdfhash/utils/graph.py` & `rdfhash-0.4.6/rdfhash/utils/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,20 +301,22 @@
         return self
 
     def _parse_file(self, path, format):
         self.graph.load(path, format)
         return self
 
     def serialize(self, path=None, format=None):
+        if format == None:
+            format = self.default_format
         if path:
-            self.graph.dump(path, format)
+            self.graph.dump(path, mime_type=format)
             return True
         else:
             with io.BytesIO() as buffer:
-                self.graph.dump(buffer, format)
+                self.graph.dump(buffer, mime_type=format)
                 buffer.seek(0)
                 res = buffer.read()
             return res.decode("utf-8")
 
     def subjects(self, predicate=None, object=None, graph=None):
         return self.graph.quads_for_pattern(None, predicate, object, graph)
 
@@ -323,15 +325,17 @@
 
     def objects(self, subject=None, predicate=None, graph=None):
         return self.graph.quads_for_pattern(subject, predicate, None, graph)
 
     def quads(self, quad):
         return self.graph.quads_for_pattern(*quad)
 
-    def triples(self, triple):
+    def triples(self, triple=None):
+        if triple == None:
+            triple = (None, None, None)
         return self.quads(triple)
 
     def term_to_string(self, term, expand_literals=False):
         if expand_literals and type(term) == self.Literal:
             value, datatype, language = term.value, term.datatype, term.language
             if datatype == self.xsd_boolean:
                 value = str(value.capitalize())
```

### Comparing `rdfhash-0.4.5/rdfhash/utils/hash.py` & `rdfhash-0.4.6/rdfhash/utils/hash.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.5/setup.py` & `rdfhash-0.4.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 from os import path, getcwd
 
 setup(
     name="rdfhash",
-    version="0.4.5",
+    version="0.4.6",
     author="Neil Graham",
     author_email="grahamneiln@gmail.com",
     url="https://github.com/NeilGraham/rdfhash",
     license_files="LICENSE.txt",
     description="De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.\n' pairs sorted.",
     long_description=open(path.join(getcwd(), "README.md")).read()
-    # Replace local links to 'docs/' to Github page 'docs/'.
+    # Replace relative links with absolute links to GitHub for PyPi
     .replace(
         "](docs/",
         "](https://github.com/NeilGraham/rdfhash/blob/master/docs/",
     ),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     entry_points={"console_scripts": ["rdfhash = rdfhash.cli:cli"]},
```

### Comparing `rdfhash-0.4.5/test/test_examples.py` & `rdfhash-0.4.6/test/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from rdfhash.logger import logger
 from rdfhash.utils.hash import (
     hash_types,
     hash_types_requiring_length,
     hash_types_resolvable,
 )
 from rdfhash.utils.graph import graph_types
-from utils import compare_graphs, graph_differences
+from utils import compare_graphs, graph_diff
 
 repo_dir = path.dirname(Path(__file__).parent.absolute())
 ttl_files = (
     path.relpath(file) for file in glob(path.join(repo_dir, "examples", "*.ttl"))
 )
 
 resolvable_hash_methods = list(hash_types_resolvable.copy())
@@ -87,15 +87,15 @@
 
     # Write output of function to file path if 'force_write' is True.
     if force_write:
         logger.warning(f"Forcing write to file path: {hash_file_path}")
         graph.serialize(hash_file_path, format="text/turtle")
 
     if not success:
-        differences = graph_differences(graph_generated, graph_actual)
+        differences = graph_diff(graph_generated, graph_actual)
         diff_s = ""
 
         if len(differences["in_g1_not_g2"]) > 0:
             diff_s += "Test File Only:\n"
             for triple in differences["in_g1_not_g2"]:
                 diff_s += differences["in_g1_not_g2"].serialize(format="turtle")
             diff_s += "\n\n"
```

