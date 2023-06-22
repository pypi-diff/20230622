# Comparing `tmp/hmmer_tables-0.2.0.tar.gz` & `tmp/hmmer_tables-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.2.0.tar", max compression
+gzip compressed data, was "hmmer_tables-0.3.0.tar", max compression
```

## Comparing `hmmer_tables-0.2.0.tar` & `hmmer_tables-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-21 14:58:44.943275 hmmer_tables-0.2.0/LICENSE
--rw-r--r--   0        0        0       15 2023-06-21 14:58:44.943275 hmmer_tables-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      367 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3152 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1885 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/interval.py
--rw-r--r--   0        0        0       72 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     1880 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      442 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/LICENSE
+-rw-r--r--   0        0        0       15 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3419 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1885 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/interval.py
+-rw-r--r--   0        0        0       72 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     2131 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      441 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 hmmer_tables-0.3.0/PKG-INFO
```

### Comparing `hmmer_tables-0.2.0/LICENSE` & `hmmer_tables-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.2.0/hmmer_tables/domtbl.py` & `hmmer_tables-0.3.0/hmmer_tables/domtbl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import dataclasses
 from typing import List, Iterable
 
-from pydantic import BaseModel
+from pydantic import BaseModel, RootModel
 
 from hmmer_tables.csv_iter import csv_iter
 from hmmer_tables.interval import PyInterval, RInterval
 from hmmer_tables.path_like import PathLike
 
 __all__ = [
     "DomTBLCoord",
     "DomTBLDomScore",
     "DomTBLIndex",
     "DomTBLRow",
     "DomTBLSeqScore",
+    "DomTBL",
     "read_domtbl",
 ]
 
 
 class DomTBLIndex(BaseModel):
     name: str
     accession: str
@@ -85,14 +86,27 @@
     def __iter__(self):
         return iter(self._asdict().values())
 
     def _field_types(self):
         return {f.name: f.type for f in dataclasses.fields(self)}
 
 
+class DomTBL(RootModel):
+    root: List[DomTBLRow]
+
+    def __iter__(self):
+        return iter(self.root)
+
+    def __getitem__(self, item):
+        return self.root[item]
+
+    def __len__(self):
+        return len(self.root)
+
+
 def _read_domtbl_stream(stream: Iterable[str]):
     rows = []
     for x in csv_iter(stream):
         seq_score = DomTBLSeqScore(
             e_value=float(x[6]), score=float(x[7]), bias=float(x[8])
         )
         domain = DomTBLDomScore(
@@ -111,20 +125,20 @@
             hmm_coord=DomTBLCoord(start=int(x[15]), stop=int(x[16])),
             ali_coord=DomTBLCoord(start=int(x[17]), stop=int(x[18])),
             env_coord=DomTBLCoord(start=int(x[19]), stop=int(x[20])),
             acc=float(x[21]),
             description=" ".join(x[22:]),
         )
         rows.append(row)
-    return rows
+    return DomTBL.model_validate(rows)
 
 
 def read_domtbl(
     filename: PathLike | None = None, stream: Iterable[str] | None = None
-) -> List[DomTBLRow]:
+) -> DomTBL:
     """
     Read domtbl file type.
     """
     if filename is not None:
         assert stream is None
         with open(filename, "r") as stream:
             return _read_domtbl_stream(stream)
```

### Comparing `hmmer_tables-0.2.0/hmmer_tables/interval.py` & `hmmer_tables-0.3.0/hmmer_tables/interval.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.2.0/hmmer_tables/tbl.py` & `hmmer_tables-0.3.0/hmmer_tables/tbl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Iterable
 
-from pydantic import BaseModel
+from pydantic import BaseModel, RootModel
 
 from hmmer_tables.csv_iter import csv_iter
 from hmmer_tables.path_like import PathLike
 
-__all__ = ["TBLScore", "TBLRow", "TBLIndex", "TBLDom", "read_tbl"]
+__all__ = ["TBLScore", "TBLRow", "TBLIndex", "TBLDom", "read_tbl", "TBL"]
 
 
 class TBLIndex(BaseModel):
     name: str
     accession: str
 
 
@@ -35,14 +35,27 @@
     query: TBLIndex
     full_sequence: TBLScore
     best_1_domain: TBLScore
     domain_numbers: TBLDom
     description: str
 
 
+class TBL(RootModel):
+    root: List[TBLRow]
+
+    def __iter__(self):
+        return iter(self.root)
+
+    def __getitem__(self, item):
+        return self.root[item]
+
+    def __len__(self):
+        return len(self.root)
+
+
 def _read_tbl_stream(stream: Iterable[str]) -> List[TBLRow]:
     rows = []
     for x in csv_iter(stream):
         seq = TBLScore(e_value=float(x[4]), score=float(x[5]), bias=float(x[6]))
         dom = TBLScore(e_value=float(x[7]), score=float(x[8]), bias=float(x[9]))
         row = TBLRow(
             target=TBLIndex(name=x[0], accession=x[1]),
@@ -58,20 +71,20 @@
                 dom=int(x[15]),
                 rep=int(x[16]),
                 inc=int(x[17]),
             ),
             description=" ".join(x[18:]),
         )
         rows.append(row)
-    return rows
+    return TBL.model_validate(rows)
 
 
 def read_tbl(
     filename: PathLike | None = None, stream: Iterable[str] | None = None
-) -> List[TBLRow]:
+) -> TBL:
     """
     Read tbl file type.
     """
     if filename is not None:
         assert stream is None
         with open(filename, "r") as stream:
             return _read_tbl_stream(stream)
```

### Comparing `hmmer_tables-0.2.0/PKG-INFO` & `hmmer_tables-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.2.0
+Version: 0.3.0
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.9)
+Requires-Dist: pydantic (>=2.0b3)
 Description-Content-Type: text/markdown
 
 # hmmer-tables
```

