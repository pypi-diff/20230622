# Comparing `tmp/CGTasks-1.1.5.tar.gz` & `tmp/CGTasks-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CGTasks-1.1.5.tar", last modified: Thu Aug 25 11:34:25 2022, max compression
+gzip compressed data, was "CGTasks-1.1.6.tar", last modified: Thu Jun 22 20:04:19 2023, max compression
```

## Comparing `CGTasks-1.1.5.tar` & `CGTasks-1.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.769873 CGTasks-1.1.5/
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.766269 CGTasks-1.1.5/CGTasks/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-25 11:18:52.000000 CGTasks-1.1.5/CGTasks/__init__.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.767883 CGTasks-1.1.5/CGTasks/graham/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-25 11:18:46.000000 CGTasks-1.1.5/CGTasks/graham/__init__.py
--rw-r--r--   0 me         (501) staff       (20)     1483 2022-08-25 09:36:20.000000 CGTasks-1.1.5/CGTasks/graham/builder.py
--rw-r--r--   0 me         (501) staff       (20)     2761 2022-08-25 09:36:20.000000 CGTasks-1.1.5/CGTasks/graham/grader.py
--rw-r--r--   0 me         (501) staff       (20)      846 2022-08-25 09:36:20.000000 CGTasks-1.1.5/CGTasks/graham/model.py
--rw-r--r--   0 me         (501) staff       (20)     2431 2022-08-25 11:28:35.000000 CGTasks-1.1.5/CGTasks/graham/task.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.768563 CGTasks-1.1.5/CGTasks/kd_tree/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-25 11:33:41.000000 CGTasks-1.1.5/CGTasks/kd_tree/__init__.py
--rw-r--r--   0 me         (501) staff       (20)     2378 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/kd_tree/builder.py
--rw-r--r--   0 me         (501) staff       (20)     1372 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/kd_tree/grader.py
--rw-r--r--   0 me         (501) staff       (20)     1275 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/kd_tree/model.py
--rw-r--r--   0 me         (501) staff       (20)     1829 2022-08-25 11:29:10.000000 CGTasks-1.1.5/CGTasks/kd_tree/task.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.769462 CGTasks-1.1.5/CGTasks/quickhull/
--rw-r--r--   0 me         (501) staff       (20)        0 2022-08-25 11:33:48.000000 CGTasks-1.1.5/CGTasks/quickhull/__init__.py
--rw-r--r--   0 me         (501) staff       (20)     2095 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/quickhull/builder.py
--rw-r--r--   0 me         (501) staff       (20)     1824 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/quickhull/grader.py
--rw-r--r--   0 me         (501) staff       (20)      911 2022-08-25 11:28:43.000000 CGTasks-1.1.5/CGTasks/quickhull/model.py
--rw-r--r--   0 me         (501) staff       (20)     1771 2022-08-25 11:29:08.000000 CGTasks-1.1.5/CGTasks/quickhull/task.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2022-08-25 11:34:25.767129 CGTasks-1.1.5/CGTasks.egg-info/
--rw-r--r--   0 me         (501) staff       (20)       51 2022-08-25 11:34:25.000000 CGTasks-1.1.5/CGTasks.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      607 2022-08-25 11:34:25.000000 CGTasks-1.1.5/CGTasks.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2022-08-25 11:34:25.000000 CGTasks-1.1.5/CGTasks.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2022-08-25 09:41:34.000000 CGTasks-1.1.5/CGTasks.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)       14 2022-08-25 11:34:25.000000 CGTasks-1.1.5/CGTasks.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        8 2022-08-25 11:34:25.000000 CGTasks-1.1.5/CGTasks.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)       51 2022-08-25 11:34:25.769729 CGTasks-1.1.5/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)       38 2022-08-25 11:34:25.769915 CGTasks-1.1.5/setup.cfg
--rw-r--r--   0 me         (501) staff       (20)      239 2022-08-25 11:34:13.000000 CGTasks-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.412290 CGTasks-1.1.6/
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.164388 CGTasks-1.1.6/CGTasks/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.308334 CGTasks-1.1.6/CGTasks/graham/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/graham/__init__.py
+-rw-rw-rw-   0        0        0     1525 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/graham/builder.py
+-rw-rw-rw-   0        0        0     2831 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/graham/grader.py
+-rw-rw-rw-   0        0        0     1205 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/graham/model.py
+-rw-rw-rw-   0        0        0     2494 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/graham/task.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.348313 CGTasks-1.1.6/CGTasks/kd_tree/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/kd_tree/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/kd_tree/builder.py
+-rw-rw-rw-   0        0        0     1415 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/kd_tree/grader.py
+-rw-rw-rw-   0        0        0     1340 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/kd_tree/model.py
+-rw-rw-rw-   0        0        0     1890 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/kd_tree/task.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.396298 CGTasks-1.1.6/CGTasks/quickhull/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/quickhull/__init__.py
+-rw-rw-rw-   0        0        0     2143 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/quickhull/builder.py
+-rw-rw-rw-   0        0        0     1878 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/quickhull/grader.py
+-rw-rw-rw-   0        0        0      950 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/quickhull/model.py
+-rw-rw-rw-   0        0        0     1809 2023-06-21 11:23:44.000000 CGTasks-1.1.6/CGTasks/quickhull/task.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:04:19.260347 CGTasks-1.1.6/CGTasks.egg-info/
+-rw-rw-rw-   0        0        0      155 2023-06-22 20:04:19.000000 CGTasks-1.1.6/CGTasks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-06-22 20:04:19.000000 CGTasks-1.1.6/CGTasks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:04:19.000000 CGTasks-1.1.6/CGTasks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 20:04:18.000000 CGTasks-1.1.6/CGTasks.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-06-22 20:04:19.000000 CGTasks-1.1.6/CGTasks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 20:04:19.000000 CGTasks-1.1.6/CGTasks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2023-06-22 20:04:19.404296 CGTasks-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:04:19.412290 CGTasks-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      359 2023-06-22 20:03:58.000000 CGTasks-1.1.6/setup.py
```

### Comparing `CGTasks-1.1.5/CGTasks/graham/builder.py` & `CGTasks-1.1.6/CGTasks/graham/builder.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from MarkLib.builder import ModelBuilder
-from .model import GrahamCenterPointCell, GrahamPiCompareCell, GrahamPoint, GrahamPointList, GrahamTable, GrahamTableRow, GrahamToAddCell, GrahamTrinityCell, PiCompare, ToAddGraham
-
-
-class GrahamModelBuilder(ModelBuilder):
-    
-    @classmethod
-    def _build_methods(cls):
-        return [
-            cls._build_internal_point,
-            cls._build_ordered,
-            cls._build_origin,
-            cls._build_steps_table
-        ]
-
-    @staticmethod
-    def _build_internal_point(answer):
-        return GrahamPoint(x=answer.x, y=answer.y)
-    
-    @staticmethod
-    def _build_ordered(answer):
-        return GrahamPointList(points=[GrahamPoint(x=p.x, y=p.y) for p in answer])
-    
-    @staticmethod
-    def _build_origin(answer):
-        return GrahamPoint(x=answer.x, y=answer.y)
-
-    @staticmethod
-    def _build_steps_table(answer):
-        pi_compare = lambda x: PiCompare.less if x else PiCompare.more
-        to_add = lambda x: ToAddGraham.yes if x else ToAddGraham.no
-        rows = [
-            GrahamTableRow(cells=(
-                GrahamTrinityCell(content=tuple(GrahamPoint(x=p.x, y=p.y) for p in row[0])),
-                GrahamPiCompareCell(content=pi_compare(row[1])),
-                GrahamCenterPointCell(content=GrahamPoint(x=row[0][1].x, y=row[0][1].y)),
-                GrahamToAddCell(content=to_add(row[1]))
-            ))
-            for row in answer
-        ]
-        
-        return GrahamTable(rows=rows)
+from MarkLib.builder import ModelBuilder
+from .model import GrahamCenterPointCell, GrahamPiCompareCell, GrahamPoint, GrahamPointList, GrahamTable, GrahamTableRow, GrahamToAddCell, GrahamTrinityCell, PiCompare, ToAddGraham
+
+
+class GrahamModelBuilder(ModelBuilder):
+    
+    @classmethod
+    def _build_methods(cls):
+        return [
+            cls._build_internal_point,
+            cls._build_ordered,
+            cls._build_origin,
+            cls._build_steps_table
+        ]
+
+    @staticmethod
+    def _build_internal_point(answer):
+        return GrahamPoint(x=answer.x, y=answer.y)
+    
+    @staticmethod
+    def _build_ordered(answer):
+        return GrahamPointList(points=[GrahamPoint(x=p.x, y=p.y) for p in answer])
+    
+    @staticmethod
+    def _build_origin(answer):
+        return GrahamPoint(x=answer.x, y=answer.y)
+
+    @staticmethod
+    def _build_steps_table(answer):
+        pi_compare = lambda x: PiCompare.less if x else PiCompare.more
+        to_add = lambda x: ToAddGraham.yes if x else ToAddGraham.no
+        rows = [
+            GrahamTableRow(cells=(
+                GrahamTrinityCell(content=tuple(GrahamPoint(x=p.x, y=p.y) for p in row[0])),
+                GrahamPiCompareCell(content=pi_compare(row[1])),
+                GrahamCenterPointCell(content=GrahamPoint(x=row[0][1].x, y=row[0][1].y)),
+                GrahamToAddCell(content=to_add(row[1]))
+            ))
+            for row in answer
+        ]
+        
+        return GrahamTable(rows=rows)
```

### Comparing `CGTasks-1.1.5/CGTasks/graham/grader.py` & `CGTasks-1.1.6/CGTasks/graham/grader.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from functools import partial
-from MarkLib.grader import Grader, default_grading, iterable_grading
-from MarkLib.markdata import MarkData, ItemMarkData, Mistake
-from .model import GrahamPointList, GrahamTable, PiCompare
-
-
-default025 = partial(default_grading, sub=0.25)
-iterable025 = partial(iterable_grading, sub=0.25)
-
-
-def ordered_grading(correct: GrahamPointList, answer: GrahamPointList):
-    return iterable025(correct.points, answer.points)
-
-
-def steps_table_grading(correct: GrahamTable, answer: GrahamTable):
-    """"
-    row.cells[0] - points' triple
-    row.cells[1] - less/more than pi (True/False)
-    row.cells[2] - center point
-    row.cells[3] - add/delete the point (True/False)
-    """
-    mistakes = []
-    correct_triples = [row.cells[0] for row in correct.rows]
-    answer_triples = [row.cells[0] for row in answer.rows]
-    correct_angles = [row.cells[1] for row in correct.rows]
-    answer_angles = [row.cells[1] for row in answer.rows]
-    correct_less_than_pi = [
-        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
-        for i, row in enumerate(correct.rows[:-1])
-        if row.cells[1].content == PiCompare.less
-    ]
-    answer_less_than_pi = [
-        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
-        for i, row in enumerate(answer.rows[:-1])
-        if row.cells[1].content == PiCompare.less
-    ]
-    correct_more_than_pi = [
-        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
-        for i, row in enumerate(correct.rows[:-1])
-        if row.cells[1].content == PiCompare.more
-    ]
-    answer_more_than_pi = [
-        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
-        for i, row in enumerate(answer.rows[:-1])
-        if row.cells[1].content == PiCompare.more
-    ]
-    mistakes_last = [
-        Mistake(sub=0.25)
-        for row in answer.rows
-        if row.cells[0].content[1] == answer.rows[0].cells[0].content[0]
-    ] + ([Mistake(sub=0.25)] if answer.rows[-1] != correct.rows[-1] else [])
-
-    mistakes.extend(iterable_grading(correct_triples, answer_triples, sub=0.15))
-    mistakes.extend(iterable_grading(correct_angles, answer_angles, sub=0.15))
-    mistakes.extend(iterable_grading(correct_less_than_pi, answer_less_than_pi, sub=0.25))
-    mistakes.extend(iterable_grading(correct_more_than_pi, answer_more_than_pi, sub=0.3, big_sub=0.6))
-    mistakes.extend(mistakes_last)
-
-    return mistakes
-
-
-internal_point = ItemMarkData(max_mark=0.25)
-ordered = ItemMarkData(max_mark=0.25)
-origin = ItemMarkData(max_mark=0.25)
-steps_table = ItemMarkData(max_mark=1.25)
-
-
-class GrahamGrader(Grader):
-    markdata = MarkData(items=[internal_point, ordered, origin, steps_table])
-    item_grading_methods = [default025, ordered_grading, default025, steps_table_grading]
+from functools import partial
+from MarkLib.grader import Grader, default_grading, iterable_grading
+from MarkLib.markdata import MarkData, ItemMarkData, Mistake
+from .model import GrahamPointList, GrahamTable, PiCompare
+
+
+default025 = partial(default_grading, sub=0.25)
+iterable025 = partial(iterable_grading, sub=0.25)
+
+
+def ordered_grading(correct: GrahamPointList, answer: GrahamPointList):
+    return iterable025(correct.points, answer.points)
+
+
+def steps_table_grading(correct: GrahamTable, answer: GrahamTable):
+    """"
+    row.cells[0] - points' triple
+    row.cells[1] - less/more than pi (True/False)
+    row.cells[2] - center point
+    row.cells[3] - add/delete the point (True/False)
+    """
+    mistakes = []
+    correct_triples = [row.cells[0] for row in correct.rows]
+    answer_triples = [row.cells[0] for row in answer.rows]
+    correct_angles = [row.cells[1] for row in correct.rows]
+    answer_angles = [row.cells[1] for row in answer.rows]
+    correct_less_than_pi = [
+        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
+        for i, row in enumerate(correct.rows[:-1])
+        if row.cells[1].content == PiCompare.less
+    ]
+    answer_less_than_pi = [
+        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
+        for i, row in enumerate(answer.rows[:-1])
+        if row.cells[1].content == PiCompare.less
+    ]
+    correct_more_than_pi = [
+        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
+        for i, row in enumerate(correct.rows[:-1])
+        if row.cells[1].content == PiCompare.more
+    ]
+    answer_more_than_pi = [
+        (row.cells[1], row.cells[3], correct.rows[i+1].cells[0])
+        for i, row in enumerate(answer.rows[:-1])
+        if row.cells[1].content == PiCompare.more
+    ]
+    mistakes_last = [
+        Mistake(sub=0.25)
+        for row in answer.rows
+        if row.cells[0].content[1] == answer.rows[0].cells[0].content[0]
+    ] + ([Mistake(sub=0.25)] if answer.rows[-1] != correct.rows[-1] else [])
+
+    mistakes.extend(iterable_grading(correct_triples, answer_triples, sub=0.15))
+    mistakes.extend(iterable_grading(correct_angles, answer_angles, sub=0.15))
+    mistakes.extend(iterable_grading(correct_less_than_pi, answer_less_than_pi, sub=0.25))
+    mistakes.extend(iterable_grading(correct_more_than_pi, answer_more_than_pi, sub=0.3, big_sub=0.6))
+    mistakes.extend(mistakes_last)
+
+    return mistakes
+
+
+internal_point = ItemMarkData(max_mark=0.25)
+ordered = ItemMarkData(max_mark=0.25)
+origin = ItemMarkData(max_mark=0.25)
+steps_table = ItemMarkData(max_mark=1.25)
+
+
+class GrahamGrader(Grader):
+    markdata = MarkData(items=[internal_point, ordered, origin, steps_table])
+    item_grading_methods = [default025, ordered_grading, default025, steps_table_grading]
```

### Comparing `CGTasks-1.1.5/CGTasks/graham/task.py` & `CGTasks-1.1.6/CGTasks/graham/task.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from CGLib.algo.graham import graham
-from CGLib.models.point import Point
-from MarkLib.task import Task
-from MarkLib.taskstage import TaskStage
-from MarkLib.taskitem import TaskItem
-from CGTasks.graham.model import GrahamPoint, GrahamPointList, GrahamTable
-from .builder import GrahamModelBuilder
-
-
-class GrahamItemInternalPoint(TaskItem):
-    description = "Задана множина S із N точок на площині. Знайти внутрішню точку q."
-    answer: GrahamPoint
-
-
-class GrahamStageInternalPoint(TaskStage):
-    description = "Задана множина S із N точок на площині. Знайти внутрішню точку q."
-    items = [GrahamItemInternalPoint]
-
-
-class GrahamItemOrderedList(TaskItem):
-    description = "Використовуючи q як початок координат, побудувати упорядкований за полярним кутом список точок множини S, починаючи із точки \"початок\" проти годинникової стрілки."
-    answer: GrahamPointList
-
-
-class GrahamStageOrderedList(TaskStage):
-    description = "Використовуючи q як початок координат, побудувати упорядкований за полярним кутом список точок множини S, починаючи із точки \"початок\" проти годинникової стрілки."
-    items = [GrahamItemOrderedList]
-
-
-class GrahamItemOriginPoint(TaskItem):
-    description = "Знайти точку \"початок\"."
-    answer: GrahamPoint
-
-
-class GrahamStageOriginPoint(TaskStage):
-    description = "Знайти точку \"початок\"."
-    items = [GrahamItemOriginPoint]
-
-
-class GrahamItemLookup(TaskItem):
-    description = "Організувати обхід."
-    answer: GrahamTable
-
-
-class GrahamStageLookup(TaskStage):
-    description = "Організувати обхід."
-    items = [GrahamItemLookup]
-
-
-class GrahamTask(Task):
-    item_answer_builder = GrahamModelBuilder
-    description = "Метод Грехема"
-    stages = [
-        GrahamStageInternalPoint,
-        GrahamStageOrderedList,
-        GrahamStageOriginPoint,
-        GrahamStageLookup
-    ]
-    solution_method = graham
-
-    @property
-    def unwrapped_condition(self):
-        return [[Point(p.x, p.y) for p in self.condition.point_list]]
+from CGLib.algo.graham import graham
+from CGLib.models.point import Point
+from MarkLib.task import Task
+from MarkLib.taskstage import TaskStage
+from MarkLib.taskitem import TaskItem
+from CGTasks.graham.model import GrahamPoint, GrahamPointList, GrahamTable
+from .builder import GrahamModelBuilder
+
+
+class GrahamItemInternalPoint(TaskItem):
+    description = "Задана множина S із N точок на площині. Знайти внутрішню точку q."
+    answer: GrahamPoint
+
+
+class GrahamStageInternalPoint(TaskStage):
+    description = "Задана множина S із N точок на площині. Знайти внутрішню точку q."
+    items = [GrahamItemInternalPoint]
+
+
+class GrahamItemOrderedList(TaskItem):
+    description = "Використовуючи q як початок координат, побудувати упорядкований за полярним кутом список точок множини S, починаючи із точки \"початок\" проти годинникової стрілки."
+    answer: GrahamPointList
+
+
+class GrahamStageOrderedList(TaskStage):
+    description = "Використовуючи q як початок координат, побудувати упорядкований за полярним кутом список точок множини S, починаючи із точки \"початок\" проти годинникової стрілки."
+    items = [GrahamItemOrderedList]
+
+
+class GrahamItemOriginPoint(TaskItem):
+    description = "Знайти точку \"початок\"."
+    answer: GrahamPoint
+
+
+class GrahamStageOriginPoint(TaskStage):
+    description = "Знайти точку \"початок\"."
+    items = [GrahamItemOriginPoint]
+
+
+class GrahamItemLookup(TaskItem):
+    description = "Організувати обхід."
+    answer: GrahamTable
+
+
+class GrahamStageLookup(TaskStage):
+    description = "Організувати обхід."
+    items = [GrahamItemLookup]
+
+
+class GrahamTask(Task):
+    item_answer_builder = GrahamModelBuilder
+    description = "Метод Грехема"
+    stages = [
+        GrahamStageInternalPoint,
+        GrahamStageOrderedList,
+        GrahamStageOriginPoint,
+        GrahamStageLookup
+    ]
+    solution_method = graham
+
+    @property
+    def unwrapped_condition(self):
+        return [[Point(p.x, p.y) for p in self.condition.point_list]]
```

### Comparing `CGTasks-1.1.5/CGTasks/kd_tree/builder.py` & `CGTasks-1.1.6/CGTasks/kd_tree/builder.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from MarkLib.builder import ModelBuilder
-from MarkLib.models.base import BinTreeNode, Point, Region
-from .model import Intersection, KdTree, KdTreeInterscetionCell, KdTreeOrderedLists, KdTreePartitionCell, KdTreePartitionTableRow, KdTreePoint, KdTreePartitionTable, KdTreePointCell, KdTreeSearchTable, KdTreeSearchTableRow, KdTreeToAddCell, Partition, ToAddKdTree
-
-
-class KdTreeModelBuilder(ModelBuilder):
-
-    @classmethod
-    def _build_methods(cls):
-        return [
-            cls._build_ordered_list,
-            cls._build_partition_table,
-            cls._build_tree,
-            cls._build_search_table
-        ]
-    
-    @staticmethod
-    def _build_ordered_list(answer):
-        return KdTreeOrderedLists(
-            ordered_x=[KdTreePoint(x=p.x, y=p.y) for p in answer[0]],
-            ordered_y=[KdTreePoint(x=p.x, y=p.y) for p in answer[1]]
-        )
-    
-    @staticmethod
-    def _build_partition_table(answer):
-        partition = lambda x: Partition.vertical if x else Partition.horizontal
-        rows = [
-            KdTreePartitionTableRow(cells=(
-                KdTreePointCell(content=KdTreePoint(x=row[0].x, y=row[0].y)),
-                KdTreePartitionCell(content=partition(row[1]))
-            ))
-            for row in answer
-        ]
-
-        return KdTreePartitionTable(rows=rows)
-    
-    @staticmethod
-    def _build_tree(answer):
-        return KdTree(
-            nodes=[
-                BinTreeNode(
-                    data=Point(x=node[0].x, y=node[0].y),
-                    left=Point(x=node[1].x, y=node[1].y) if node[1] else None,
-                    right=Point(x=node[2].x, y=node[2].y) if node[2] else None
-                )
-                for node in answer.nodes
-            ],
-            region=Region(x_range=answer.x_range, y_range=answer.y_range)
-        )
-    
-    @staticmethod
-    def _build_search_table(answer):
-        to_add = lambda x: ToAddKdTree.yes if x else ToAddKdTree.no
-        intersection = lambda x: Intersection.yes if x else Intersection.no
-        rows = [
-            KdTreeSearchTableRow(cells=(
-                KdTreePointCell(content=KdTreePoint(x=row[0].x, y=row[0].y)),
-                KdTreeToAddCell(content=to_add(row[1])),
-                KdTreeInterscetionCell(content=intersection(row[2]))
-            ))
-            for row in answer
-        ]
-
-        return KdTreeSearchTable(rows=rows)
+from MarkLib.builder import ModelBuilder
+from MarkLib.models.base import BinTreeNode, Point, Region
+from .model import Intersection, KdTree, KdTreeInterscetionCell, KdTreeOrderedLists, KdTreePartitionCell, KdTreePartitionTableRow, KdTreePoint, KdTreePartitionTable, KdTreePointCell, KdTreeSearchTable, KdTreeSearchTableRow, KdTreeToAddCell, Partition, ToAddKdTree
+
+
+class KdTreeModelBuilder(ModelBuilder):
+
+    @classmethod
+    def _build_methods(cls):
+        return [
+            cls._build_ordered_list,
+            cls._build_partition_table,
+            cls._build_tree,
+            cls._build_search_table
+        ]
+    
+    @staticmethod
+    def _build_ordered_list(answer):
+        return KdTreeOrderedLists(
+            ordered_x=[KdTreePoint(x=p.x, y=p.y) for p in answer[0]],
+            ordered_y=[KdTreePoint(x=p.x, y=p.y) for p in answer[1]]
+        )
+    
+    @staticmethod
+    def _build_partition_table(answer):
+        partition = lambda x: Partition.vertical if x else Partition.horizontal
+        rows = [
+            KdTreePartitionTableRow(cells=(
+                KdTreePointCell(content=KdTreePoint(x=row[0].x, y=row[0].y)),
+                KdTreePartitionCell(content=partition(row[1]))
+            ))
+            for row in answer
+        ]
+
+        return KdTreePartitionTable(rows=rows)
+    
+    @staticmethod
+    def _build_tree(answer):
+        return KdTree(
+            nodes=[
+                BinTreeNode(
+                    data=Point(x=node[0].x, y=node[0].y),
+                    left=Point(x=node[1].x, y=node[1].y) if node[1] else None,
+                    right=Point(x=node[2].x, y=node[2].y) if node[2] else None
+                )
+                for node in answer.nodes
+            ],
+            region=Region(x_range=answer.x_range, y_range=answer.y_range)
+        )
+    
+    @staticmethod
+    def _build_search_table(answer):
+        to_add = lambda x: ToAddKdTree.yes if x else ToAddKdTree.no
+        intersection = lambda x: Intersection.yes if x else Intersection.no
+        rows = [
+            KdTreeSearchTableRow(cells=(
+                KdTreePointCell(content=KdTreePoint(x=row[0].x, y=row[0].y)),
+                KdTreeToAddCell(content=to_add(row[1])),
+                KdTreeInterscetionCell(content=intersection(row[2]))
+            ))
+            for row in answer
+        ]
+
+        return KdTreeSearchTable(rows=rows)
```

### Comparing `CGTasks-1.1.5/CGTasks/kd_tree/grader.py` & `CGTasks-1.1.6/CGTasks/kd_tree/grader.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from functools import partial
-from MarkLib.grader import Grader, iterable_grading
-from MarkLib.markdata import MarkData, ItemMarkData
-from .model import KdTree, KdTreeOrderedLists, KdTreePartitionTable, KdTreeSearchTable
-
-
-iterable025 = partial(iterable_grading, sub=0.25)
-iterable1 = partial(iterable_grading, sub=1.0)
-
-
-def grade_ordered_lists(correct: KdTreeOrderedLists, answer: KdTreeOrderedLists):
-    return (
-        iterable025(correct.ordered_x, answer.ordered_x) +
-        iterable025(correct.ordered_y, answer.ordered_y)
-    )
-
-
-def grade_partition_table(correct: KdTreePartitionTable, answer: KdTreePartitionTable):
-    return iterable_grading(correct.rows, answer.rows, sub=0.75)
-
-
-def grade_search_tree(correct: KdTree, answer: KdTree):
-    return iterable1(correct.nodes, answer.nodes)
-
-
-def grade_search_table(correct: KdTreeSearchTable, answer: KdTreeSearchTable):
-    return iterable1(correct.rows, answer.rows)
-
-
-ordered_lists = ItemMarkData(max_mark=0.25)
-partition_table = ItemMarkData(max_mark=0.75)
-search_tree = ItemMarkData(max_mark=1)
-search_table = ItemMarkData(max_mark=1)
-
-
-class KdTreeGrader(Grader):
-    markdata = MarkData(items=[ordered_lists, partition_table, search_tree, search_table])
-    item_grading_methods = [
-        grade_ordered_lists,
-        grade_partition_table,
-        grade_search_tree,
-        grade_search_table
-    ]
+from functools import partial
+from MarkLib.grader import Grader, iterable_grading
+from MarkLib.markdata import MarkData, ItemMarkData
+from .model import KdTree, KdTreeOrderedLists, KdTreePartitionTable, KdTreeSearchTable
+
+
+iterable025 = partial(iterable_grading, sub=0.25)
+iterable1 = partial(iterable_grading, sub=1.0)
+
+
+def grade_ordered_lists(correct: KdTreeOrderedLists, answer: KdTreeOrderedLists):
+    return (
+        iterable025(correct.ordered_x, answer.ordered_x) +
+        iterable025(correct.ordered_y, answer.ordered_y)
+    )
+
+
+def grade_partition_table(correct: KdTreePartitionTable, answer: KdTreePartitionTable):
+    return iterable_grading(correct.rows, answer.rows, sub=0.75)
+
+
+def grade_search_tree(correct: KdTree, answer: KdTree):
+    return iterable1(correct.nodes, answer.nodes)
+
+
+def grade_search_table(correct: KdTreeSearchTable, answer: KdTreeSearchTable):
+    return iterable1(correct.rows, answer.rows)
+
+
+ordered_lists = ItemMarkData(max_mark=0.25)
+partition_table = ItemMarkData(max_mark=0.75)
+search_tree = ItemMarkData(max_mark=1)
+search_table = ItemMarkData(max_mark=1)
+
+
+class KdTreeGrader(Grader):
+    markdata = MarkData(items=[ordered_lists, partition_table, search_tree, search_table])
+    item_grading_methods = [
+        grade_ordered_lists,
+        grade_partition_table,
+        grade_search_tree,
+        grade_search_table
+    ]
```

### Comparing `CGTasks-1.1.5/CGTasks/kd_tree/model.py` & `CGTasks-1.1.6/CGTasks/kd_tree/model.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from enum import Enum
-from pydantic import BaseModel
-from MarkLib.models.base import BinTree, HeaderTable, Point, Region, TableCell, TableRow
-
-
-class KdTreePoint(Point):
-    pass
-
-
-class KdTreeOrderedLists(BaseModel):
-    ordered_x: "list[KdTreePoint]"
-    ordered_y: "list[KdTreePoint]"
-
-
-class KdTree(BinTree):
-    region: Region
-
-
-class Partition(str, Enum):
-    vertical = "vertical"
-    horizontal = "horizontal"
-
-
-class ToAddKdTree(str, Enum):
-    yes = "yes"
-    no = "no"
-
-
-class Intersection(str, Enum):
-    yes = "yes"
-    no = "no"
-
-
-class KdTreePointCell(TableCell):
-    content: KdTreePoint
-
-
-class KdTreePartitionCell(TableCell):
-    content: Partition
-
-
-class KdTreeToAddCell(TableCell):
-    content: ToAddKdTree
-
-
-class KdTreeInterscetionCell(TableCell):
-    content: Intersection
-
-
-class KdTreePartitionTableRow(TableRow):
-    cells: "tuple[KdTreePointCell, KdTreePartitionCell]"
-
-
-class KdTreeSearchTableRow(TableRow):
-    cells: "tuple[KdTreePointCell, KdTreeToAddCell, KdTreeInterscetionCell]"
-
-
-class KdTreePartitionTable(HeaderTable):
-    rows: "list[KdTreePartitionTableRow]"
-    headers: "tuple[str, str]" = ('', '')    
-
-
-class KdTreeSearchTable(HeaderTable):
-    rows: "list[KdTreeSearchTableRow]"
-    headers: "tuple[str, str, str]" = ('', '', '')
+from enum import Enum
+from pydantic import BaseModel
+from MarkLib.models.base import BinTree, HeaderTable, Point, Region, TableCell, TableRow
+
+
+class KdTreePoint(Point):
+    pass
+
+
+class KdTreeOrderedLists(BaseModel):
+    ordered_x: "list[KdTreePoint]"
+    ordered_y: "list[KdTreePoint]"
+
+
+class KdTree(BinTree):
+    region: Region
+
+
+class Partition(str, Enum):
+    vertical = "vertical"
+    horizontal = "horizontal"
+
+
+class ToAddKdTree(str, Enum):
+    yes = "yes"
+    no = "no"
+
+
+class Intersection(str, Enum):
+    yes = "yes"
+    no = "no"
+
+
+class KdTreePointCell(TableCell):
+    content: KdTreePoint
+
+
+class KdTreePartitionCell(TableCell):
+    content: Partition
+
+
+class KdTreeToAddCell(TableCell):
+    content: ToAddKdTree
+
+
+class KdTreeInterscetionCell(TableCell):
+    content: Intersection
+
+
+class KdTreePartitionTableRow(TableRow):
+    cells: "tuple[KdTreePointCell, KdTreePartitionCell]"
+
+
+class KdTreeSearchTableRow(TableRow):
+    cells: "tuple[KdTreePointCell, KdTreeToAddCell, KdTreeInterscetionCell]"
+
+
+class KdTreePartitionTable(HeaderTable):
+    rows: "list[KdTreePartitionTableRow]"
+    headers: "tuple[str, str]" = ('', '')    
+
+
+class KdTreeSearchTable(HeaderTable):
+    rows: "list[KdTreeSearchTableRow]"
+    headers: "tuple[str, str, str]" = ('', '', '')
```

### Comparing `CGTasks-1.1.5/CGTasks/kd_tree/task.py` & `CGTasks-1.1.6/CGTasks/kd_tree/task.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from CGLib.algo.kd_tree_method import kd_tree
-from CGLib.models.point import Point
-from MarkLib.task import Task
-from MarkLib.taskstage import TaskStage
-from MarkLib.taskitem import TaskItem
-from CGTasks.kd_tree.model import KdTree, KdTreeOrderedLists, KdTreePartitionTable, KdTreeSearchTable
-from .builder import KdTreeModelBuilder
-
-
-class KdTreeItemOrderedList(TaskItem):
-    description = "Побудувати відсортований по X список."
-    answer: KdTreeOrderedLists
-
-
-class KdTreeItemPartition(TaskItem):
-    description = "Рекурсивно розбити площину на прямокутники."
-    answer: KdTreePartitionTable
-
-
-class KdTreeStagePreprocessing(TaskStage):
-    description = "Попередня обробка"
-    items = [KdTreeItemOrderedList, KdTreeItemPartition]
-
-
-class KdTreeItemTree(TaskItem):
-    description = "Побудувати дерево пошуку."
-    answer: KdTree
-
-
-class KdTreeStageTree(TaskStage):
-    description = "Побудувати дерево пошуку."
-    items = [KdTreeItemTree]
-
-
-class KdTreeItemSearch(TaskItem):
-    description = "Здійснити пошук у дереві."
-    answer: KdTreeSearchTable
-
-
-class KdTreeStageSearch(TaskStage):
-    description = "Здійснити пошук у дереві."
-    items = [KdTreeItemSearch]
-
-
-class KdTreeTask(Task):
-    item_answer_builder = KdTreeModelBuilder
-    description = "Метод kd-дерева"
-    stages = [
-        KdTreeStagePreprocessing,
-        KdTreeStageTree,
-        KdTreeStageSearch
-    ]
-    solution_method = kd_tree
-
-    @property
-    def unwrapped_condition(self):
-        return [
-            [Point(p.x, p.y) for p in self.condition.point_list],
-            self.condition.region.x_range,
-            self.condition.region.y_range
-        ]
+from CGLib.algo.kd_tree_method import kd_tree
+from CGLib.models.point import Point
+from MarkLib.task import Task
+from MarkLib.taskstage import TaskStage
+from MarkLib.taskitem import TaskItem
+from CGTasks.kd_tree.model import KdTree, KdTreeOrderedLists, KdTreePartitionTable, KdTreeSearchTable
+from .builder import KdTreeModelBuilder
+
+
+class KdTreeItemOrderedList(TaskItem):
+    description = "Побудувати відсортований по X список."
+    answer: KdTreeOrderedLists
+
+
+class KdTreeItemPartition(TaskItem):
+    description = "Рекурсивно розбити площину на прямокутники."
+    answer: KdTreePartitionTable
+
+
+class KdTreeStagePreprocessing(TaskStage):
+    description = "Попередня обробка"
+    items = [KdTreeItemOrderedList, KdTreeItemPartition]
+
+
+class KdTreeItemTree(TaskItem):
+    description = "Побудувати дерево пошуку."
+    answer: KdTree
+
+
+class KdTreeStageTree(TaskStage):
+    description = "Побудувати дерево пошуку."
+    items = [KdTreeItemTree]
+
+
+class KdTreeItemSearch(TaskItem):
+    description = "Здійснити пошук у дереві."
+    answer: KdTreeSearchTable
+
+
+class KdTreeStageSearch(TaskStage):
+    description = "Здійснити пошук у дереві."
+    items = [KdTreeItemSearch]
+
+
+class KdTreeTask(Task):
+    item_answer_builder = KdTreeModelBuilder
+    description = "Метод kd-дерева"
+    stages = [
+        KdTreeStagePreprocessing,
+        KdTreeStageTree,
+        KdTreeStageSearch
+    ]
+    solution_method = kd_tree
+
+    @property
+    def unwrapped_condition(self):
+        return [
+            [Point(p.x, p.y) for p in self.condition.point_list],
+            self.condition.region.x_range,
+            self.condition.region.y_range
+        ]
```

### Comparing `CGTasks-1.1.5/CGTasks/quickhull/grader.py` & `CGTasks-1.1.6/CGTasks/quickhull/grader.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from functools import partial
-from MarkLib.grader import Grader, default_grading, iterable_grading
-from MarkLib.markdata import MarkData, ItemMarkData
-from .model import QuickhullPartition, QuickhullTree
-
-
-default025 = partial(default_grading, sub=0.25)
-iterable025 = partial(iterable_grading, sub=0.25)
-iterable1 = partial(iterable_grading, sub=1.0)
-
-
-def grade_partition(correct: QuickhullPartition, answer: QuickhullPartition):
-    mistakes = []
-    
-    correct_h_points = [node.data.h for node in correct.tree.nodes if node.data.h is not None]
-    answer_h_points = [node.data.h for node in answer.tree.nodes if node.data.h is not None]
-    
-    correct_points = [
-        (
-            node.data.points,
-            node.left.points if node.left else None,
-            node.right.points if node.right else None
-        )
-        for node in correct.tree.nodes
-    ]
-    answer_points = [
-        (
-            node.data.points,
-            node.left.points if node.left else None,
-            node.right.points if node.left else None
-        )
-        for node in answer.tree.nodes
-    ]
-
-    mistakes.extend(default025(correct.initial_partition, answer.initial_partition))
-    mistakes.extend(iterable025(correct_h_points, answer_h_points, big_sub=0.5))
-    mistakes.extend(iterable025(correct_points, answer_points))
-    mistakes.extend(iterable025(correct.tree.leaves, answer.tree.leaves))
-
-
-def grade_merge(correct: QuickhullTree, answer: QuickhullTree):
-    return iterable1(
-        [node.data.hull_piece for node in correct.nodes],
-        [node.data.hull_piece for node in answer.nodes]
-    )
-
-
-partition = ItemMarkData(max_mark=1.0)
-merge = ItemMarkData(max_mark=1.0)
-
-
-class QuickhullGrader(Grader):
-    markdata = MarkData(items=[partition, merge])
-    item_grading_methods = [grade_partition, grade_merge]
+from functools import partial
+from MarkLib.grader import Grader, default_grading, iterable_grading
+from MarkLib.markdata import MarkData, ItemMarkData
+from .model import QuickhullPartition, QuickhullTree
+
+
+default025 = partial(default_grading, sub=0.25)
+iterable025 = partial(iterable_grading, sub=0.25)
+iterable1 = partial(iterable_grading, sub=1.0)
+
+
+def grade_partition(correct: QuickhullPartition, answer: QuickhullPartition):
+    mistakes = []
+    
+    correct_h_points = [node.data.h for node in correct.tree.nodes if node.data.h is not None]
+    answer_h_points = [node.data.h for node in answer.tree.nodes if node.data.h is not None]
+    
+    correct_points = [
+        (
+            node.data.points,
+            node.left.points if node.left else None,
+            node.right.points if node.right else None
+        )
+        for node in correct.tree.nodes
+    ]
+    answer_points = [
+        (
+            node.data.points,
+            node.left.points if node.left else None,
+            node.right.points if node.left else None
+        )
+        for node in answer.tree.nodes
+    ]
+
+    mistakes.extend(default025(correct.initial_partition, answer.initial_partition))
+    mistakes.extend(iterable025(correct_h_points, answer_h_points, big_sub=0.5))
+    mistakes.extend(iterable025(correct_points, answer_points))
+    mistakes.extend(iterable025(correct.tree.leaves, answer.tree.leaves))
+
+
+def grade_merge(correct: QuickhullTree, answer: QuickhullTree):
+    return iterable1(
+        [node.data.hull_piece for node in correct.nodes],
+        [node.data.hull_piece for node in answer.nodes]
+    )
+
+
+partition = ItemMarkData(max_mark=1.0)
+merge = ItemMarkData(max_mark=1.0)
+
+
+class QuickhullGrader(Grader):
+    markdata = MarkData(items=[partition, merge])
+    item_grading_methods = [grade_partition, grade_merge]
```

### Comparing `CGTasks-1.1.5/CGTasks/quickhull/model.py` & `CGTasks-1.1.6/CGTasks/quickhull/model.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Optional
-from pydantic import BaseModel
-from MarkLib.models.base import BinTree, BinTreeNode, Point
-
-
-class QuickhullPoint(Point):
-    pass
-
-
-class QuickhullInitialPartition(BaseModel):
-    min_point: QuickhullPoint
-    max_point: QuickhullPoint
-    s1: "list[QuickhullPoint]"
-    s2: "list[QuickhullPoint]"
-
-
-class QuickhullNodeData(BaseModel):
-    points: "list[QuickhullPoint]"
-    h: Optional[QuickhullPoint]
-    hull_piece: "list[QuickhullPoint]"
-
-
-class QuickhullTreeNode(BinTreeNode):
-    data: QuickhullNodeData
-    left: Optional[QuickhullNodeData]
-    right: Optional[QuickhullNodeData]
-
-
-class QuickhullTree(BinTree):
-    nodes: "list[QuickhullTreeNode]"
-
-    @property
-    def leaves(self):
-        return [n for n in self.nodes if n.left is None and n.right is None]
-
-
-class QuickhullPartition(BaseModel):
-    initial_partition: QuickhullInitialPartition
-    tree: QuickhullTree
+from typing import Optional
+from pydantic import BaseModel
+from MarkLib.models.base import BinTree, BinTreeNode, Point
+
+
+class QuickhullPoint(Point):
+    pass
+
+
+class QuickhullInitialPartition(BaseModel):
+    min_point: QuickhullPoint
+    max_point: QuickhullPoint
+    s1: "list[QuickhullPoint]"
+    s2: "list[QuickhullPoint]"
+
+
+class QuickhullNodeData(BaseModel):
+    points: "list[QuickhullPoint]"
+    h: Optional[QuickhullPoint]
+    hull_piece: "list[QuickhullPoint]"
+
+
+class QuickhullTreeNode(BinTreeNode):
+    data: QuickhullNodeData
+    left: Optional[QuickhullNodeData]
+    right: Optional[QuickhullNodeData]
+
+
+class QuickhullTree(BinTree):
+    nodes: "list[QuickhullTreeNode]"
+
+    @property
+    def leaves(self):
+        return [n for n in self.nodes if n.left is None and n.right is None]
+
+
+class QuickhullPartition(BaseModel):
+    initial_partition: QuickhullInitialPartition
+    tree: QuickhullTree
```

### Comparing `CGTasks-1.1.5/CGTasks/quickhull/task.py` & `CGTasks-1.1.6/CGTasks/quickhull/task.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from CGLib.algo.quickhull import quickhull
-from CGLib.models.point import Point
-from MarkLib.task import Task
-from MarkLib.taskitem import TaskItem
-from MarkLib.taskstage import TaskStage
-from CGTasks.quickhull.model import QuickhullPartition, QuickhullTree
-from .builder import QuickhullModelBuilder
-
-
-class QuickhullItemPartition(TaskItem):
-    description = "Здійснити розбиття. Подати у вигляді дерева."
-    answer: QuickhullPartition
-
-
-class QuickhullStagePartition(TaskStage):
-    description = "Здійснити розбиття. Подати у вигляді дерева."
-    items = [QuickhullItemPartition]
-
-
-class QuickhullItemMerge(TaskItem):
-    description = "Злиття. Рекурсивний підйом, результат - конкатенація списків. Починаючи із листків дерева, рекурсивно конкатенуємо упорядковані за годинниковою стрілкою списки."
-    answer: QuickhullTree
-
-
-class QuickhullStageMerge(TaskStage):
-    description = "Злиття. Рекурсивний підйом, результат - конкатенація списків. Починаючи із листків дерева, рекурсивно конкатенуємо упорядковані за годинниковою стрілкою списки."
-    items = [QuickhullItemMerge]
-
-
-class QuickhullTask(Task):
-    item_answer_builder = QuickhullModelBuilder
-    description = "Метод Швидкобол"
-    stages = [QuickhullStagePartition, QuickhullStageMerge]
-    solution_method = quickhull
-
-    @property
-    def unwrapped_condition(self):
-        return [[Point(p.x, p.y) for p in self.condition.point_list]]
+from CGLib.algo.quickhull import quickhull
+from CGLib.models.point import Point
+from MarkLib.task import Task
+from MarkLib.taskitem import TaskItem
+from MarkLib.taskstage import TaskStage
+from CGTasks.quickhull.model import QuickhullPartition, QuickhullTree
+from .builder import QuickhullModelBuilder
+
+
+class QuickhullItemPartition(TaskItem):
+    description = "Здійснити розбиття. Подати у вигляді дерева."
+    answer: QuickhullPartition
+
+
+class QuickhullStagePartition(TaskStage):
+    description = "Здійснити розбиття. Подати у вигляді дерева."
+    items = [QuickhullItemPartition]
+
+
+class QuickhullItemMerge(TaskItem):
+    description = "Злиття. Рекурсивний підйом, результат - конкатенація списків. Починаючи із листків дерева, рекурсивно конкатенуємо упорядковані за годинниковою стрілкою списки."
+    answer: QuickhullTree
+
+
+class QuickhullStageMerge(TaskStage):
+    description = "Злиття. Рекурсивний підйом, результат - конкатенація списків. Починаючи із листків дерева, рекурсивно конкатенуємо упорядковані за годинниковою стрілкою списки."
+    items = [QuickhullItemMerge]
+
+
+class QuickhullTask(Task):
+    item_answer_builder = QuickhullModelBuilder
+    description = "Метод Швидкобол"
+    stages = [QuickhullStagePartition, QuickhullStageMerge]
+    solution_method = quickhull
+
+    @property
+    def unwrapped_condition(self):
+        return [[Point(p.x, p.y) for p in self.condition.point_list]]
```

### Comparing `CGTasks-1.1.5/CGTasks.egg-info/SOURCES.txt` & `CGTasks-1.1.6/CGTasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

