# Comparing `tmp/MarkLib-1.1.3.tar.gz` & `tmp/MarkLib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkLib-1.1.3.tar", last modified: Thu Aug 25 07:41:40 2022, max compression
+gzip compressed data, was "MarkLib-1.1.4.tar", last modified: Thu Jun 22 20:00:43 2023, max compression
```

## Comparing `MarkLib-1.1.3.tar` & `MarkLib-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 07:41:40.575521 MarkLib-1.1.3/
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 07:41:40.573508 MarkLib-1.1.3/MarkLib/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-24 16:19:34.000000 MarkLib-1.1.3/MarkLib/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      258 2022-08-24 16:29:25.000000 MarkLib-1.1.3/MarkLib/builder.py
--rw-r--r--   0 me         (501) staff       (20)     1851 2022-08-24 16:29:24.000000 MarkLib-1.1.3/MarkLib/grader.py
--rw-r--r--   0 me         (501) staff       (20)      604 2022-08-24 16:19:34.000000 MarkLib-1.1.3/MarkLib/markdata.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 07:41:40.574992 MarkLib-1.1.3/MarkLib/models/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-24 16:19:34.000000 MarkLib-1.1.3/MarkLib/models/__init__.py
--rw-r--r--   0 me         (501) staff       (20)     1199 2022-08-24 16:19:34.000000 MarkLib-1.1.3/MarkLib/models/base.py
--rw-r--r--   0 me         (501) staff       (20)      343 2022-08-24 16:29:27.000000 MarkLib-1.1.3/MarkLib/models/condition.py
--rw-r--r--   0 me         (501) staff       (20)     1485 2022-08-25 07:40:46.000000 MarkLib-1.1.3/MarkLib/task.py
--rw-r--r--   0 me         (501) staff       (20)      125 2022-08-24 16:19:34.000000 MarkLib-1.1.3/MarkLib/taskitem.py
--rw-r--r--   0 me         (501) staff       (20)      308 2022-08-24 16:29:35.000000 MarkLib-1.1.3/MarkLib/taskstage.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 07:41:40.574480 MarkLib-1.1.3/MarkLib.egg-info/
--rw-r--r--   0 me         (501) staff       (20)      168 2022-08-25 07:41:40.000000 MarkLib-1.1.3/MarkLib.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      404 2022-08-25 07:41:40.000000 MarkLib-1.1.3/MarkLib.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2022-08-25 07:41:40.000000 MarkLib-1.1.3/MarkLib.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2022-08-24 16:32:06.000000 MarkLib-1.1.3/MarkLib.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)        9 2022-08-25 07:41:40.000000 MarkLib-1.1.3/MarkLib.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        8 2022-08-25 07:41:40.000000 MarkLib-1.1.3/MarkLib.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)      168 2022-08-25 07:41:40.575332 MarkLib-1.1.3/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)       38 2022-08-25 07:41:40.575567 MarkLib-1.1.3/setup.cfg
--rw-r--r--   0 me         (501) staff       (20)      394 2022-08-25 07:41:31.000000 MarkLib-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:00:43.751212 MarkLib-1.1.4/
+-rw-rw-rw-   0        0        0     1330 2023-06-21 11:21:49.000000 MarkLib-1.1.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-22 20:00:43.607268 MarkLib-1.1.4/MarkLib/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/builder.py
+-rw-rw-rw-   0        0        0     1916 2023-06-22 16:37:47.000000 MarkLib-1.1.4/MarkLib/grader.py
+-rw-rw-rw-   0        0        0      631 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/markdata.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:00:43.735222 MarkLib-1.1.4/MarkLib/models/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/models/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/models/base.py
+-rw-rw-rw-   0        0        0      362 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/models/condition.py
+-rw-rw-rw-   0        0        0     1535 2023-06-22 13:04:35.000000 MarkLib-1.1.4/MarkLib/task.py
+-rw-rw-rw-   0        0        0      132 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/taskitem.py
+-rw-rw-rw-   0        0        0      316 2023-06-21 11:21:49.000000 MarkLib-1.1.4/MarkLib/taskstage.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:00:43.719233 MarkLib-1.1.4/MarkLib.egg-info/
+-rw-rw-rw-   0        0        0      194 2023-06-22 20:00:43.000000 MarkLib-1.1.4/MarkLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-06-22 20:00:43.000000 MarkLib-1.1.4/MarkLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:00:43.000000 MarkLib-1.1.4/MarkLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 20:00:42.000000 MarkLib-1.1.4/MarkLib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-22 20:00:43.000000 MarkLib-1.1.4/MarkLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 20:00:43.000000 MarkLib-1.1.4/MarkLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      194 2023-06-22 20:00:43.743218 MarkLib-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:00:43.751212 MarkLib-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-06-22 19:59:37.000000 MarkLib-1.1.4/setup.py
```

### Comparing `MarkLib-1.1.3/MarkLib/grader.py` & `MarkLib-1.1.4/MarkLib/grader.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import Callable, Iterable
-from collections import Counter
-from itertools import cycle
-from MarkLib.markdata import MarkData, Mistake
-
-
-def default_grading(correct, answer, sub=0.0):
-    return [] if correct == answer else [Mistake(sub=sub)]
-
-
-def iterable_grading(correct: Iterable, answer: Iterable, sub=0.0, big_sub=0.0, item_grading=default_grading):
-    diff = len(correct) - len(answer)
-    extra = [
-        Mistake(sub=sub, big_sub=big_sub, data="Too many items")
-        for _ in range(-diff)
-    ] if diff < 0 else [
-        Mistake(sub=sub, big_sub=big_sub, data="Too few items")
-        for _ in range(diff)
-    ]
-
-    return [
-        Mistake(sub=sub, big_sub=big_sub)
-        for c, a in zip(correct, answer)
-        if item_grading(c, a) != []
-    ] + extra
-
-
-def mistakes_sub_pairs(mistakes):
-    counter = Counter(mistakes)
-    return {
-        mistake: mistake.big_sub if mistake.systematic and count > 1 else mistake.sub
-        for mistake, count
-        in counter.items()
-    }
-
-
-class Grader:
-    markdata: MarkData
-    item_grading_methods: Iterable[Callable] = cycle([default_grading])
-
-    @classmethod
-    def grade(cls, correct, answer):
-        mistakes = [
-            method(correct_stage, answer_stage)
-            for method, correct_stage, answer_stage 
-            in zip(cls.item_grading_methods, correct, answer)
-        ]
-
-        by_items = list(zip(cls.markdata.items, mistakes))
-
-        by_items_counter = [
-            (stage, mistakes_sub_pairs(mistakes))
-            for stage, mistakes
-            in by_items
-        ]
-
-        marks_per_item = [
-            (item, max(item.min_mark, item.max_mark - sum(counter.values())))
-            for item, counter
-            in by_items_counter
-        ]
-
-        mark = sum(mark for item, mark in marks_per_item)
-
-        return mark, marks_per_item
+from typing import Callable, Iterable
+from collections import Counter
+from itertools import cycle
+from MarkLib.markdata import MarkData, Mistake
+
+
+def default_grading(correct, answer, sub=0.0):
+    return [] if correct == answer else [Mistake(sub=sub)]
+
+
+def iterable_grading(correct: Iterable, answer: Iterable, sub=0.0, big_sub=0.0, item_grading=default_grading):
+    diff = len(correct) - len(answer)
+    extra = [
+        Mistake(sub=sub, big_sub=big_sub, data="Too many items")
+        for _ in range(-diff)
+    ] if diff < 0 else [
+        Mistake(sub=sub, big_sub=big_sub, data="Too few items")
+        for _ in range(diff)
+    ]
+
+    return [
+        Mistake(sub=sub, big_sub=big_sub)
+        for c, a in zip(correct, answer)
+        if item_grading(c, a) != []
+    ] + extra
+
+
+def mistakes_sub_pairs(mistakes):
+    counter = Counter(mistakes)
+    return {
+        mistake: mistake.big_sub if mistake.systematic and count > 1 else mistake.sub
+        for mistake, count
+        in counter.items()
+    }
+
+
+class Grader:
+    markdata: MarkData
+    item_grading_methods: Iterable[Callable] = cycle([default_grading])
+
+    @classmethod
+    def grade(cls, correct, answer):
+        mistakes = [
+            method(correct_stage, answer_stage)
+            for method, correct_stage, answer_stage 
+            in zip(cls.item_grading_methods, correct, answer)
+        ]
+
+        by_items = list(zip(cls.markdata.items, mistakes))
+
+        by_items_counter = [
+            (stage, mistakes_sub_pairs(mistakes))
+            for stage, mistakes
+            in by_items
+        ]
+
+        marks_per_item = [
+            (item, max(item.min_mark, item.max_mark - sum(counter.values())))
+            for item, counter
+            in by_items_counter
+        ]
+
+        mark = sum(mark for item, mark in marks_per_item)
+
+        return mark, marks_per_item
```

### Comparing `MarkLib-1.1.3/MarkLib/models/base.py` & `MarkLib-1.1.4/MarkLib/models/base.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from math import isclose
-from pydantic import BaseModel
-from typing import Any, Optional
-
-
-class Point(BaseModel):
-    x: float = 0
-    y: float = 0
-
-    def __eq__(self, other: Any) -> bool:
-        return (
-            isinstance(other, Point) and
-            isclose(self.x, other.x, abs_tol=1e-3) and
-            isclose(self.y, other.y, abs_tol=1e-3)
-        )
-
-
-class PointList(BaseModel):
-    points: list[Point] = []
-
-
-class Vertex(BaseModel):
-    point: Point = None
-
-
-class Edge(BaseModel):
-    v1: Vertex = None
-    v2: Vertex = None
-    weight: int = 0
-
-
-class Graph(BaseModel):
-    vertices: set = set()
-    edges: set = set()
-
-
-class BinTreeNode(BaseModel):
-    data: Any
-    left: Optional[Any]
-    right: Optional[Any]
-
-
-class BinTree(BaseModel):
-    """Binary tree model represented as left-to-right list of nodes."""
-    nodes: list[BinTreeNode]
-
-
-class Region(BaseModel):
-    x_range: tuple[float, float] = (0, 0)
-    y_range: tuple[float, float] = (0, 0)
-
-
-class TableCell(BaseModel):
-    content: Any
-
-
-class TableRow(BaseModel):
-    cells: list[TableCell] = []
-
-
-class Table(BaseModel):
-    rows: list[TableRow] = []
-    
-
-class HeaderTable(Table):
-    headers: list[str] = []
+from math import isclose
+from pydantic import BaseModel
+from typing import Any, Optional
+
+
+class Point(BaseModel):
+    x: float = 0
+    y: float = 0
+
+    def __eq__(self, other: Any) -> bool:
+        return (
+            isinstance(other, Point) and
+            isclose(self.x, other.x, abs_tol=1e-3) and
+            isclose(self.y, other.y, abs_tol=1e-3)
+        )
+
+
+class PointList(BaseModel):
+    points: list[Point] = []
+
+
+class Vertex(BaseModel):
+    point: Point = None
+
+
+class Edge(BaseModel):
+    v1: Vertex = None
+    v2: Vertex = None
+    weight: int = 0
+
+
+class Graph(BaseModel):
+    vertices: set = set()
+    edges: set = set()
+
+
+class BinTreeNode(BaseModel):
+    data: Any
+    left: Optional[Any]
+    right: Optional[Any]
+
+
+class BinTree(BaseModel):
+    """Binary tree model represented as left-to-right list of nodes."""
+    nodes: list[BinTreeNode]
+
+
+class Region(BaseModel):
+    x_range: tuple[float, float] = (0, 0)
+    y_range: tuple[float, float] = (0, 0)
+
+
+class TableCell(BaseModel):
+    content: Any
+
+
+class TableRow(BaseModel):
+    cells: list[TableCell] = []
+
+
+class Table(BaseModel):
+    rows: list[TableRow] = []
+    
+
+class HeaderTable(Table):
+    headers: list[str] = []
```

