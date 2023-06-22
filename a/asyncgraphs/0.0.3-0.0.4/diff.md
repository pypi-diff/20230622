# Comparing `tmp/asyncgraphs-0.0.3.tar.gz` & `tmp/asyncgraphs-0.0.4.tar.gz`

## Comparing `asyncgraphs-0.0.3.tar` & `asyncgraphs-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/asyncgraphs/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/asyncgraphs/construction.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/asyncgraphs/execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/asyncgraphs/py.typed
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/mkdocs.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/changelog.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/install.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/usage/graph.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/usage/source.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/docs/docs/usage/transform.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/tests/execution/__init__.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/tests/execution/test_basic_execution.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/tests/execution/test_source_types.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/tests/execution/test_transformation_types.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/LICENSE
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/README.md
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 asyncgraphs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/asyncgraphs/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/asyncgraphs/construction.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/asyncgraphs/execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/asyncgraphs/py.typed
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/changelog.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/index.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/components/graph.md
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/components/source.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/components/transform.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/usage/construction.md
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/docs/usage/execution.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/tests/execution/__init__.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/tests/execution/test_basic_execution.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/tests/execution/test_source_types.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/tests/execution/test_transformation_types.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/README.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 asyncgraphs-0.0.4/PKG-INFO
```

### Comparing `asyncgraphs-0.0.3/.github/workflows/release.yml` & `asyncgraphs-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `asyncgraphs-0.0.3/.github/workflows/test.yml` & `asyncgraphs-0.0.4/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Tests
 on:
   push:
     branches:
-      - master
+      - main
   pull_request:
     branches:
-      - master
+      - main
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [ "3.10", "3.11" ]
     steps:
```

### Comparing `asyncgraphs-0.0.3/asyncgraphs/construction.py` & `asyncgraphs-0.0.4/asyncgraphs/construction.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,31 @@
     AsyncGenerator,
     AsyncIterable,
     Awaitable,
     Callable,
     Generator,
     Generic,
     Iterable,
-    Optional,
     Set,
     TypeAlias,
     TypeVar,
 )
 
 IN_T = TypeVar("IN_T")
 OUT_T = TypeVar("OUT_T")
 TransformOperation: TypeAlias = Callable[
     [IN_T],
     Generator[OUT_T, Any, Any] | AsyncGenerator[OUT_T, Any] | Awaitable[OUT_T] | OUT_T,
 ]
 
 
 class _NodeBase(Generic[OUT_T]):
-    def __init__(self, name: Optional[str]) -> None:
+    def __init__(self, name: str | None, out_queue_size: int = 0) -> None:
         self.name = name or f"Node<{id(self)}>"
+        self.out_queue_size = out_queue_size
         self.next_nodes: Set[Transform[OUT_T, Any]] = set()
 
     def link_to(
         self, other: Transform[OUT_T, Any] | TransformOperation[OUT_T, Any]
     ) -> Transform[OUT_T, Any]:
         if callable(other):
             other_node = Transform(None, other)
@@ -47,25 +47,31 @@
         self, other: Transform[OUT_T, Any] | TransformOperation[OUT_T, Any]
     ) -> Transform[OUT_T, Any]:
         return self.link_to(other)
 
 
 class Source(_NodeBase[OUT_T]):
     def __init__(
-        self, name: Optional[str], operation: Iterable[OUT_T] | AsyncIterable[OUT_T]
+        self,
+        name: str | None,
+        operation: Iterable[OUT_T] | AsyncIterable[OUT_T],
+        out_queue_size: int = 0,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, out_queue_size)
         self.operation = operation
 
 
 class Transform(_NodeBase[OUT_T], Generic[IN_T, OUT_T]):
     def __init__(
-        self, name: Optional[str], operation: TransformOperation[IN_T, OUT_T]
+        self,
+        name: str | None,
+        operation: TransformOperation[IN_T, OUT_T],
+        out_queue_size: int = 0,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, out_queue_size)
         self.operation = operation
 
 
 class Graph:
     def __init__(self) -> None:
         self.entry_nodes: Set[Source[Any]] = set()
```

### Comparing `asyncgraphs-0.0.3/asyncgraphs/execution.py` & `asyncgraphs-0.0.4/asyncgraphs/execution.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,35 +7,39 @@
 import sentinel
 
 from asyncgraphs.construction import Graph, Source, Transform, TransformOperation
 
 CompletedSignal = sentinel.create("CompletedSignal")
 
 
-async def run(graph: Graph) -> None:
+async def run(graph: Graph, default_queue_size: int = 0) -> None:
     tasks = []
     for s_node in graph.entry_nodes:
         s_out_queues = set()
         for t_node in s_node.next_nodes:
-            t_in_queue: Queue[Any] = Queue()
-            branch_run_info = _get_transform_run_info(t_in_queue, t_node)
+            t_in_queue: Queue[Any] = Queue(
+                maxsize=s_node.out_queue_size or default_queue_size
+            )
+            branch_run_info = _get_transform_run_info(
+                t_in_queue, t_node, default_queue_size
+            )
             s_out_queues.add(t_in_queue)
             tasks += [run_transform(i, n, o) for i, n, o in branch_run_info]
         tasks.append(run_source(s_node, s_out_queues))
     await asyncio.gather(*tasks)
 
 
 def _get_transform_run_info(
-    in_queue: Queue[Any], node: Transform[Any, Any]
+    in_queue: Queue[Any], node: Transform[Any, Any], default_queue_size: int
 ) -> List[Tuple[Queue[Any], Transform[Any, Any], Set[Queue[Any]]]]:
     to_return = []
     node_out_queues = set()
     for n in node.next_nodes:
-        q: Queue[Any] = Queue()
-        to_return += _get_transform_run_info(q, n)
+        q: Queue[Any] = Queue(maxsize=node.out_queue_size or default_queue_size)
+        to_return += _get_transform_run_info(q, n, default_queue_size)
         node_out_queues.add(q)
     return to_return + [(in_queue, node, node_out_queues)]
 
 
 async def run_source(node: Source[Any], out_queues: Set[Queue[Any]]) -> None:
     if isinstance(node.operation, AsyncIterable):
         async for data_out in node.operation:
```

### Comparing `asyncgraphs-0.0.3/docs/docs/usage/source.md` & `asyncgraphs-0.0.4/docs/components/source.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Source
 
 A source in AsyncGraphs is a Node that simply generates data.
 
-Sources are attached directly to [Graph](./graph.md) objects and take no input.
+Sources are attached directly to [Graph](graph.md) objects and take no input.
 
 Any python Iterable or AsyncIterable can be used.
 
 ```python
 from asyncgraphs import Graph
 
 g = Graph()
```

### Comparing `asyncgraphs-0.0.3/tests/execution/test_basic_execution.py` & `asyncgraphs-0.0.4/tests/execution/test_basic_execution.py`

 * *Files identical despite different names*

### Comparing `asyncgraphs-0.0.3/tests/execution/test_source_types.py` & `asyncgraphs-0.0.4/tests/execution/test_source_types.py`

 * *Files identical despite different names*

### Comparing `asyncgraphs-0.0.3/tests/execution/test_transformation_types.py` & `asyncgraphs-0.0.4/tests/execution/test_transformation_types.py`

 * *Files identical despite different names*

### Comparing `asyncgraphs-0.0.3/.gitignore` & `asyncgraphs-0.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-docs/_build/
+docs_/_build/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `asyncgraphs-0.0.3/LICENSE` & `asyncgraphs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgraphs-0.0.3/pyproject.toml` & `asyncgraphs-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 dependencies = [
     "sentinel >=1.0.0,<1.1.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/SamVermeulen42/asyncgraphs"
+Documentation = "https://samvermeulen42.github.io/asyncgraphs/"
 
 [project.optional-dependencies]
 dev = [
     "pytest >=7.2.1,<8.0.0",
     "pytest-asyncio >=0.20.0,<0.21.0",
     "coverage >=7.1.0,<8.0",
     "mypy ==1.0.1",
```

