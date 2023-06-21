# Comparing `tmp/python_adjudicator-0.2.1.tar.gz` & `tmp/python_adjudicator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.2.1.tar", max compression
+gzip compressed data, was "python_adjudicator-0.3.0.tar", max compression
```

## Comparing `python_adjudicator-0.2.1.tar` & `python_adjudicator-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.2.1/LICENSE
--rw-r--r--   0        0        0     2560 2023-06-20 18:55:00.878072 python_adjudicator-0.2.1/README.md
--rw-r--r--   0        0        0     1874 2023-06-20 18:56:25.123563 python_adjudicator-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2019 2023-06-20 18:55:00.880353 python_adjudicator-0.2.1/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3137 2023-06-20 18:55:00.880578 python_adjudicator-0.2.1/src/adjudicator/Executor.py
--rw-r--r--   0        0        0     1530 2023-06-20 18:55:00.880788 python_adjudicator-0.2.1/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     5579 2023-06-20 18:55:00.881002 python_adjudicator-0.2.1/src/adjudicator/Params.py
--rw-r--r--   0        0        0      892 2023-06-20 18:55:00.881198 python_adjudicator-0.2.1/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     4652 2023-06-20 18:55:00.881419 python_adjudicator-0.2.1/src/adjudicator/Rule.py
--rw-r--r--   0        0        0      739 2023-06-20 18:55:00.881611 python_adjudicator-0.2.1/src/adjudicator/Rule_test.py
--rw-r--r--   0        0        0     4475 2023-06-20 18:55:47.321833 python_adjudicator-0.2.1/src/adjudicator/RulesEngine.py
--rw-r--r--   0        0        0     2643 2023-06-20 18:55:00.882143 python_adjudicator-0.2.1/src/adjudicator/RulesEngine_test.py
--rw-r--r--   0        0        0     3121 2023-06-20 18:55:09.531720 python_adjudicator-0.2.1/src/adjudicator/RulesGraph.py
--rw-r--r--   0        0        0     2615 2023-06-20 18:55:00.882556 python_adjudicator-0.2.1/src/adjudicator/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-06-20 18:55:00.882716 python_adjudicator-0.2.1/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      682 2023-06-20 18:56:25.123762 python_adjudicator-0.2.1/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-20 18:55:00.883062 python_adjudicator-0.2.1/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-06-20 18:55:00.883183 python_adjudicator-0.2.1/src/adjudicator/py.typed
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 python_adjudicator-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3862 2023-06-21 23:01:08.385844 python_adjudicator-0.3.0/README.md
+-rw-r--r--   0        0        0     2048 2023-06-21 23:01:41.788080 python_adjudicator-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2119 2023-06-21 22:55:41.840466 python_adjudicator-0.3.0/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3214 2023-06-21 22:55:41.841814 python_adjudicator-0.3.0/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-06-21 22:55:41.842426 python_adjudicator-0.3.0/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     7246 2023-06-21 22:55:41.842936 python_adjudicator-0.3.0/src/adjudicator/Params.py
+-rw-r--r--   0        0        0     1054 2023-06-21 22:55:41.843369 python_adjudicator-0.3.0/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     5978 2023-06-21 22:55:41.844148 python_adjudicator-0.3.0/src/adjudicator/RuleEngine.py
+-rw-r--r--   0        0        0     2741 2023-06-21 22:55:41.844722 python_adjudicator-0.3.0/src/adjudicator/RuleEngine_test.py
+-rw-r--r--   0        0        0     5460 2023-06-21 22:55:41.845250 python_adjudicator-0.3.0/src/adjudicator/RuleGraph.py
+-rw-r--r--   0        0        0     3932 2023-06-21 22:55:41.845569 python_adjudicator-0.3.0/src/adjudicator/RuleGraph_test.py
+-rw-r--r--   0        0        0      426 2023-06-21 22:55:41.847616 python_adjudicator-0.3.0/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      800 2023-06-21 23:01:41.788376 python_adjudicator-0.3.0/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-21 22:55:41.848771 python_adjudicator-0.3.0/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-06-21 22:55:41.849105 python_adjudicator-0.3.0/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     6856 2023-06-21 22:56:10.537884 python_adjudicator-0.3.0/src/adjudicator/rule.py
+-rw-r--r--   0        0        0      824 2023-06-21 22:56:15.991531 python_adjudicator-0.3.0/src/adjudicator/rule_test.py
+-rw-r--r--   0        0        0     4609 1970-01-01 00:00:00.000000 python_adjudicator-0.3.0/PKG-INFO
```

### Comparing `python_adjudicator-0.2.1/LICENSE` & `python_adjudicator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.1/pyproject.toml` & `python_adjudicator-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
@@ -41,24 +41,24 @@
 # ...
 
 [tool.slap]
 typed = true
 
 [tool.slap.test]
 check  = "slap check"
-black  = "black --check examples/ src/ tests/"
-flake8 = "flake8 examples/ src/ tests/"
-isort  = "isort --check-only examples/ src/ tests/"
+black  = "black --check examples/ src/ tests/ --exclude examples/hello.py"
+flake8 = "flake8 examples/ src/ tests/ --exclude examples/hello.py"
+isort  = "isort --check-only examples/ src/ tests/ --extend-skip examples/hello.py"
 mypy   = "dmypy run examples/ src/"
 pycln  = "pycln examples/ src/ tests/ --check"
-pytest = "pytest examples/ src/ tests/ -vv --doctest-modules"
+pytest = "pytest src/ tests/ -vv --doctest-modules"
 
 [tool.slap.run]
 "docs:build" = ">&2 echo 'Not implemented' && exit 1"
-fmt          = "pycln src/ tests/ examples/ && black src/ tests/ examples/ && isort src/ tests/ examples/"
+fmt          = "pycln src/ tests/ examples/ && black src/ tests/ examples/ --exclude examples/hello.py && isort src/ tests/ examples/ --extend-skip examples/hello.py && python examples/update_readme.py"
 
 [tool.mypy]
 python_version = "3.10"
 explicit_package_bases = true
 mypy_path = ["src"]
 namespace_packages = true
 pretty = true
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/Cache.py` & `python_adjudicator-0.3.0/src/adjudicator/Cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from adjudicator.Params import Params
-    from adjudicator.Rule import Rule
+    from adjudicator.rule import ProductionRule
 
 
 class Cache(ABC):
     """
     Base class for all cache implementations.
     """
 
     @abstractmethod
-    def has(self, rule: Rule, params: Params) -> bool:
+    def has(self, rule: ProductionRule, params: Params) -> bool:
         """
         Return True if the specified rule and params have been evaluated.
         """
 
     @abstractmethod
-    def get(self, rule: Rule, params: Params) -> Any:
+    def get(self, rule: ProductionRule, params: Params) -> Any:
         """
         Return the result of evaluating the specified rule and params.
 
         Raise a #KeyError if the specified rule and params have not been evaluated.
         """
 
     @abstractmethod
-    def set(self, rule: Rule, params: Params, value: Any) -> None:
+    def set(self, rule: ProductionRule, params: Params, value: Any) -> None:
         """
         Set the result of evaluating the specified rule and params.
         """
 
     @staticmethod
     def none() -> "Cache":
         """
@@ -51,33 +51,33 @@
 
 
 class NoneCache(Cache):
     """
     Cache implementation that does not cache anything.
     """
 
-    def has(self, rule: Rule, params: Params) -> bool:
+    def has(self, rule: ProductionRule, params: Params) -> bool:
         return False
 
-    def get(self, rule: Rule, params: Params) -> Any:
+    def get(self, rule: ProductionRule, params: Params) -> Any:
         raise KeyError()
 
-    def set(self, rule: Rule, params: Params, value: Any) -> None:
+    def set(self, rule: ProductionRule, params: Params, value: Any) -> None:
         pass
 
 
 class MemoryCache(Cache):
     """
     In-memory cache implementation.
     """
 
     def __init__(self) -> None:
         self._cache: dict[int, Any] = {}
 
-    def has(self, rule: Rule, params: Params) -> bool:
+    def has(self, rule: ProductionRule, params: Params) -> bool:
         return hash((rule.id, params)) in self._cache
 
-    def get(self, rule: Rule, params: Params) -> Any:
+    def get(self, rule: ProductionRule, params: Params) -> Any:
         return self._cache[hash((rule.id, params))]
 
-    def set(self, rule: Rule, params: Params, value: Any) -> None:
+    def set(self, rule: ProductionRule, params: Params, value: Any) -> None:
         self._cache[hash((rule.id, params))] = value
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/Executor.py` & `python_adjudicator-0.3.0/src/adjudicator/Executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from concurrent.futures import Future, ThreadPoolExecutor
 from threading import Lock
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from adjudicator.Cache import Cache
     from adjudicator.Params import Params
-    from adjudicator.Rule import Rule
-    from adjudicator.RulesEngine import RulesEngine
+    from adjudicator.rule import ProductionRule
+    from adjudicator.RuleEngine import RuleEngine
 
 
 class Executor(ABC):
     """
     Executor for rules.
     """
 
     @abstractmethod
-    def execute(self, rule: Rule, params: Params, engine: RulesEngine) -> Any:
+    def execute(self, rule: ProductionRule, params: Params, engine: RuleEngine) -> Any:
         """
         Execute the specified rule with the specified params.
         """
         ...
 
     @staticmethod
     def simple(cache: Cache) -> "Executor":
@@ -45,23 +45,23 @@
     """
     A simple executor that executes rules in the current thread.
     """
 
     def __init__(self, cache: Cache) -> None:
         self._cache = cache
 
-    def execute(self, rule: Rule, params: Params, engine: RulesEngine) -> Any:
+    def execute(self, rule: ProductionRule, params: Params, engine: RuleEngine) -> Any:
         try:
             return self._cache.get(rule, params)
         except KeyError:
-            with engine.as_current():
-                result = rule.execute(params)
+            with engine.activate():
+                result = rule.func(params)
             assert isinstance(
                 result, rule.output_type
-            ), "Rule output (type: %r) does not match Rule output type: %r" % (
+            ), "ProductionRule output (type: %r) does not match ProductionRule output type: %r" % (
                 type(result),
                 rule.output_type,
             )
             self._cache.set(rule, params, result)
             return result
 
 
@@ -72,33 +72,33 @@
 
     def __init__(self, cache: Cache) -> None:
         self._cache = cache
         self._lock = Lock()
         self._pending: dict[int, Future[Any]] = {}
         self._executor = ThreadPoolExecutor()
 
-    def _on_result(self, rule: Rule, params: Params, key: int) -> None:
+    def _on_result(self, rule: ProductionRule, params: Params, key: int) -> None:
         with self._lock:
             future = self._pending.pop(key)
             assert future.done(), "Future is not done"
             result = future.result()
             assert isinstance(
                 result, rule.output_type
-            ), "Rule output (type: %r) does not match Rule output type: %r" % (
+            ), "ProductionRule output (type: %r) does not match ProductionRule output type: %r" % (
                 type(result),
                 rule.output_type,
             )
             self._cache.set(rule, params, result)
 
-    def execute(self, rule: Rule, params: Params, engine: RulesEngine) -> Any:
+    def execute(self, rule: ProductionRule, params: Params, engine: RuleEngine) -> Any:
         try:
             return self._cache.get(rule, params)
         except KeyError:
             key = hash((rule.id, params))
             with self._lock:
                 try:
                     future = self._pending[key]
                 except KeyError:
-                    future = self._executor.submit(rule.execute, params)
+                    future = self._executor.submit(rule.func, params)
                     self._pending[key] = future
                     future.add_done_callback(lambda _: self._on_result(rule, params, key))
             return future.result()
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/HashSupport.py` & `python_adjudicator-0.3.0/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.1/src/adjudicator/Rule_test.py` & `python_adjudicator-0.3.0/src/adjudicator/rule_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from adjudicator import Params
-from adjudicator.Rule import Rule, collect_rules, rule
+from adjudicator.rule import ProductionRule, RuleTypes, collect_rules, rule
 
 
 def test__collect_rules__picks_up_rules_from_nonlocals() -> None:
-    @rule
+    @rule()
     def a() -> int:
         return 42
 
-    def get_rules() -> list[Rule]:
-        @rule
+    def get_rules() -> list[RuleTypes]:
+        @rule()
         def b() -> int:
             return 42
 
         return list(collect_rules())
 
     assert len(get_rules()) == 2
     assert {x.id.rpartition(".")[2] for x in get_rules()} == {"a", "b"}
 
 
 def test__collect_rules__from_instance_methods() -> None:
     class MyClass:
-        @rule
+        @rule()
         def my_rule(self, param: int) -> str:
             return str(param) + "!"
 
     obj = MyClass()
     rules = collect_rules(obj)
     assert len(rules) == 1
-    assert rules[0](Params([42])) == "42!"
+    assert isinstance(rules[0], ProductionRule)
+    assert rules[0].func(Params([42])) == "42!"
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/RulesEngine.py` & `python_adjudicator-0.3.0/src/adjudicator/RuleEngine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,107 @@
 from __future__ import annotations
 
+import importlib
+import types
 from contextlib import contextmanager
 from typing import Any, ClassVar, Iterable, Iterator, TypeVar
 
 from adjudicator.Cache import Cache
 from adjudicator.Executor import Executor
 from adjudicator.HashSupport import HashSupport
 from adjudicator.Params import Params
-from adjudicator.Rule import Rule
-from adjudicator.RulesGraph import RulesGraph
+from adjudicator.rule import RuleTypes, collect_rules
+from adjudicator.RuleGraph import RuleGraph
 from adjudicator.Signature import Signature
 
 T = TypeVar("T")
 
 
-class RulesEngine:
+class RuleEngine:
     """
     A simple rules engine.
+
+    It is composed of rules, built-in facts (i.e. parameters that are available to all rules), an executor for
+    executing rules, a cache for caching rule results. It provides a high-level API for building a rule graph
+    and for evaluating rules.
+
+    A RuleEngine can be made the current engine by using the #activate() context manager. This allows rules to
+    evaluate other rules by calling #get() function, which delegates to the current engine.
     """
 
     def __init__(
         self,
-        rules: Iterable[Rule] | RulesGraph,
+        rules: Iterable[RuleTypes] | RuleGraph = (),
         facts: Params.InitType | None = None,
         executor: Executor | None = None,
     ) -> None:
-        self.graph = RulesGraph(rules)
+        self.graph = RuleGraph(rules)
         self.hashsupport = HashSupport()
-        self.facts = Params(facts or (), self.hashsupport)
+        self.facts = Params(facts or (), hasher=self.hashsupport)
         self.executor = executor or Executor.simple(Cache.memory())
 
-    _current_engine_stack: ClassVar[list[RulesEngine]] = []
+    # Activation
+
+    _current_engine_stack: ClassVar[list[RuleEngine]] = []
 
     @contextmanager
-    def as_current(self) -> Iterator[None]:
+    def activate(self) -> Iterator[None]:
         """
         Set the engine as the current engine for the duration of the context. Calls to #current() will return it
         as long as the context manager is active.
         """
 
         try:
-            RulesEngine._current_engine_stack.append(self)
+            RuleEngine._current_engine_stack.append(self)
             yield
         finally:
-            assert RulesEngine._current_engine_stack.pop() is self
+            assert RuleEngine._current_engine_stack.pop() is self
 
     @staticmethod
-    def current() -> "RulesEngine":
-        if RulesEngine._current_engine_stack:
-            return RulesEngine._current_engine_stack[-1]
-        raise RuntimeError("No current RulesEngine")
-
-    def get(self, output_type: type[T], params: Params) -> T:
-        """
-        Evaluate the rules to derive the specified *output_type* from the given parameters.
-        """
-
-        if not params and output_type in self.facts:
-            return self.facts.get(output_type)
-
-        sig = Signature(set(params.types()) | set(self.facts.types()), output_type)
-        rules = self.graph.find_path(sig)
-        assert len(rules) > 0, "Empty path?"
-
-        output: Any = None
-        for rule in rules:
-            inputs = self.facts.filter(rule.input_types) | params.filter(rule.input_types)
-            output = self.executor.execute(rule, inputs, self)
-            params = params | Params({rule.output_type: output}, self.hashsupport)
-
-        assert isinstance(output, output_type), f"Expected {output_type}, got {type(output)}"
-        return output
+    def current() -> "RuleEngine":
+        if RuleEngine._current_engine_stack:
+            return RuleEngine._current_engine_stack[-1]
+        raise RuntimeError("No current RuleEngine")
+
+    # Rule graph management
+
+    def load_module(self, module: str | types.ModuleType, func_name: str = "rules", autocollect: bool = True) -> None:
+        """
+        This function imports a Python module and invokes it's `rules()` function, passing the RuleEngine as the
+        only argument. The `rules()` function should return an iterable of Rule or UnionRule objects. If the module
+        has no `rules()` function and *autocollect* is True, then all rules that can be found at the module's top
+        level will be collected with the #collect_rules() function.
+        """
+
+        if isinstance(module, str):
+            module = importlib.import_module(module)
+        func = getattr(module, func_name, None)
+        if func is None:
+            if not autocollect:
+                raise ValueError(f"Module {module} has no {func_name}() function")
+            rules: Iterable[RuleTypes] = collect_rules(module)
+        else:
+            rules = func(self)
+        self.graph.add_rules(rules)
 
-    def add_rules(self, rules: Iterable[Rule]) -> None:
-        self.graph.update(rules)
+    # Global facts
 
-    def assert_facts(self, facts: Params.InitType) -> None:
+    def assert_(self, facts: Params.InitType) -> None:
         """
         Assert facts to the rules engine. Note that this will fail if a fact of the given type already exists in
         the rules engine.
         """
 
         facts = Params(facts)
         overlap = self.facts.types() & facts.types()
         if overlap:
             raise ValueError(f"Fact(s) of type {overlap} already exist(s)")
         self.facts = self.facts | facts
 
-    def retract_facts(self, facts: Params.InitType) -> None:
+    def retract(self, facts: Params.InitType) -> None:
         """
         Retract facts from the rules engine. Note that this will fail if a fact of the given type does not exist in
         the rules engine, or if the value specfified for a type does not match the value in the rules engine.
         """
 
         facts = Params(facts)
         missing = facts.types() - self.facts.types()
@@ -104,23 +114,46 @@
                 raise ValueError(
                     f"Cannot retract fact of type {type_} because the fact provided does not match the same type of "
                     "fact in the rules engine."
                 )
 
         self.facts = self.facts - facts.types()
 
+    # Computation
+
+    def get(self, output_type: type[T], params: Params) -> T:
+        """
+        Evaluate the rules to derive the specified *output_type* from the given parameters.
+        """
+
+        if not params and output_type in self.facts:
+            return self.facts.get(output_type)
+
+        sig = Signature(frozenset(params.types()) | frozenset(self.facts.types()), output_type)
+        rules = self.graph.find_path(sig)
+        assert len(rules) > 0, "Empty path?"
+
+        output: Any = None
+        for rule in rules:
+            inputs = self.facts.filter(rule.input_types) | params.filter(rule.input_types)
+            output = self.executor.execute(rule, inputs, self)
+            params = params | Params({rule.output_type: output}, hasher=self.hashsupport)
+
+        assert isinstance(output, output_type), f"Expected {output_type}, got {type(output)}"
+        return output
+
 
 def get(output_type: type[T], *inputs: object) -> T:
     """
     Delegate to the engine to retrieve the specified output type given the input parameters. If the first argument
     is a dictionary, it will be used as the input parameters and no arguments can follow.
     """
 
-    engine = RulesEngine.current()
+    engine = RuleEngine.current()
 
     if inputs and isinstance(inputs[0], dict):
         assert len(inputs) == 1, "No arguments allowed after dictionary"
-        params = Params(inputs[0], engine.hashsupport)
+        params = Params(inputs[0], hasher=engine.hashsupport)
     else:
-        params = Params(inputs, engine.hashsupport)
+        params = Params(inputs, hasher=engine.hashsupport)
 
     return engine.get(output_type, params)
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/RulesEngine_test.py` & `python_adjudicator-0.3.0/src/adjudicator/RuleEngine_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,72 +2,73 @@
 from dataclasses import dataclass
 
 from pytest import mark
 
 from adjudicator.Cache import Cache
 from adjudicator.Executor import Executor
 from adjudicator.Params import Params
-from adjudicator.Rule import Rule, collect_rules, rule
-from adjudicator.RulesEngine import RulesEngine, get
+from adjudicator.rule import ProductionRule, collect_rules, rule
+from adjudicator.RuleEngine import RuleEngine, get
 
 sys.setrecursionlimit(130)
 
 
 @mark.parametrize(
     argnames="cache_impl,is_cached",
     argvalues=[
         (Cache.memory(), True),
         (Cache.none(), False),
     ],
+    ids=["memory", "none"],
 )
 def test__RulesEngine__can_cache_properly(cache_impl: Cache, is_cached: bool) -> None:
     """
     Tests if rule result caching works as expected.
     """
 
     @dataclass(frozen=True)
     class Fibonacci:
         n: int
 
     num_invokations = 0
 
-    @rule
+    @rule()
     def fibonacci(n: int) -> Fibonacci:
         nonlocal num_invokations
         num_invokations += 1
         if n < 2:
             return Fibonacci(n)
         x = get(Fibonacci, n - 1)
         y = get(Fibonacci, n - 2)
         return Fibonacci(x.n + y.n)
 
-    engine = RulesEngine(list(collect_rules()), [], executor=Executor.simple(cache=cache_impl))
+    engine = RuleEngine(list(collect_rules()), [], executor=Executor.simple(cache=cache_impl))
 
     assert engine.get(Fibonacci, Params([0])).n == 0
     assert engine.get(Fibonacci, Params([3])).n == 2
     assert engine.get(Fibonacci, Params([4])).n == 3
     assert engine.get(Fibonacci, Params([5])).n == 5
     assert engine.get(Fibonacci, Params([6])).n == 8
     assert num_invokations == 7 if is_cached else 55
     assert engine.get(Fibonacci, Params([7])).n == 13
     assert num_invokations == 8 if is_cached else 96
 
 
 def test__RulesEngine__picks_correct_rule_for_same_output() -> None:
-    engine = RulesEngine(
+    engine = RuleEngine(
         rules=[
-            Rule(
+            ProductionRule(
                 func=lambda p: int(p.get(str)),
-                input_types={str},
+                input_types=frozenset({str}),
                 output_type=int,
                 id="r1",
             ),
-            Rule(
+            ProductionRule(
                 func=lambda p: int(p.get(bool)),
-                input_types={bool},
+                input_types=frozenset({bool}),
                 output_type=int,
                 id="r2",
             ),
         ],
         facts=[],
     )
 
@@ -77,19 +78,19 @@
 
 
 def test__RulesEngine__injects_facts() -> None:
     @dataclass(frozen=True)
     class CustomType:
         v: int
 
-    engine = RulesEngine(
+    engine = RuleEngine(
         rules=[
-            Rule(
+            ProductionRule(
                 func=lambda p: p.get(CustomType).v,
-                input_types={CustomType},
+                input_types=frozenset({CustomType}),
                 output_type=int,
                 id="r1",
             )
         ],
         facts=[CustomType(42)],
     )
```

### Comparing `python_adjudicator-0.2.1/src/adjudicator/errors.py` & `python_adjudicator-0.3.0/src/adjudicator/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from adjudicator.Rule import Rule
-    from adjudicator.RulesGraph import RulesGraph
+    from adjudicator.rule import ProductionRule
+    from adjudicator.RuleGraph import RuleGraph
     from adjudicator.Signature import Signature
 
 SUBSET_CHAR = "⊆"
 
 
 class RuleResolveError(Exception):
     pass
 
 
 @dataclass
 class NoMatchingRulesError(RuleResolveError):
     sig: Signature
-    graph: RulesGraph
+    graph: RuleGraph
 
     def __str__(self) -> str:
         return f"No rule(s) satisfy the signature {SUBSET_CHAR} {self.sig}" + (
             (
                 f"\nAvailable rules for output type {self.sig.output_type.__name__} are:\n"
-                + "\n".join(f"  {rule.id}: {rule.signature}" for rule in self.graph.rules_for(self.sig.output_type))
+                + "\n".join(
+                    f"  {rule.id}: {rule.signature}" for rule in self.graph.get_production_rules(self.sig.output_type)
+                )
             )
             if self.graph
             else ""
         )
 
 
 @dataclass
 class MultipleMatchingRulesError(RuleResolveError):
     sig: Signature
-    paths: list[list[Rule]]
-    graph: RulesGraph
+    paths: list[list[ProductionRule]]
+    graph: RuleGraph
 
     def __str__(self) -> str:
         return (
             f"Multiple paths through the rules graph satisfy the signature {SUBSET_CHAR} {self.sig}.\n"
             "The following paths were found:\n"
             + "\n\n".join(
                 f"  {idx:>2}: " + "\n      ".join(f"{rule.signature} [rule id: {rule.id}]" for rule in rules)
```

### Comparing `python_adjudicator-0.2.1/PKG-INFO` & `python_adjudicator-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,59 +19,85 @@
 
 # adjudicator
 
 > __Adjudicator__ _(nount_): An adjudicator is a person or body that makes formal judgments on a disputed matter. They
 > are the ones who settle disputes or decide who is right in a disagreement. This could be a judge in a courtroom, an
 > arbitrator in a negotiation, or any person or system given the power to make decisions of this type.
 
-Adjudicator is a framework for type-based rules engines largely inspired by the Pants build system. The rule graph
-consists of nodes which are concrete Python types and edges which are functions that take a set of input types and
-produce an output type.
+Adjudicator is a framework for implementing type-based rule engines largely inspired by the Pants build system. The
+rule graph consists of nodes which are concrete Python types and edges which are functions that take a set of input
+types and produce an output type.
 
 Rules are matched on a set of facts, which populate the possible input types of a rule. Deriving a type may require
 chained execution of rules, which is supported. Global facts may be used to populate a potential input type for all
 rule executions.
 
-In a way, Adjudicator can also be called a dependency injection engine.
-
-```mermaid
-graph LR
-    String --> Rule1 --> Integer
-    String --> Rule2 --> Integer
-    IntegerBase --> Rule2
+The Adjudicator rule engine is designed to be used in a request-response fashion. A request is a set of facts that
+should be used to derive a type. A response is the derived type. The rule engine will execute the rules necessary to
+derive the type and return the response. If a rule was already executed with the same inputs, it will not be executed
+again. For optimal use of the caching mechanism, all types participating in the rule evaluation should be immutable
+and implement a stable hash (e.g. using `@dataclass(frozen=True)` and `tuple` instead of `list`, etc.).
+
+When a mutable type should intentionally participate in the rule evaluation, usually this works automatically because
+the hash of a Python object that does not provide a custom `__hash__()` implementation or disables its hashing is based
+on the object's identity. This means that the hash is stable for the memory allocation of the object, and will not
+change if the object is mutated. For types that do not _support_ hashing, support can be enabled explicitly using the
+`RuleEngine.hashsupport` object.
+
+__Table of Contents__
+
+<!-- table of contents -->
+* [Quickstart](#quickstart)
+* [Installation](#installation)
+* [Future Extensions](#future-extensions)
+<!-- end table of contents -->
+
+## Quickstart
+
+The following example shows how to use Adjudicator to implement a simple "Hello World" application. The rule engine
+invokes the `say_hello()` production rule because a `HelloResponse` is requested and a `HelloRequest` is provided,
+which matches the rule's signature.
+
+<!-- include examples/hello.py code:python -->
+```python
+from dataclasses import dataclass
+from adjudicator import Params, RuleEngine, rule
+
+@dataclass(frozen=True)
+class HelloRequest:
+    name: str
+
+@dataclass(frozen=True)
+class HelloResponse:
+    greeting: str
+
+@rule()
+def say_hello(request: HelloRequest) -> HelloResponse:
+    return HelloResponse(greeting=f"Hello {request.name}!")
+
+engine = RuleEngine()
+engine.load_module(__name__)
+response = engine.get(HelloResponse, Params(HelloRequest(name="World")))
+print(response.greeting)
 ```
+<!-- end include -->
 
-In the above example, an `Integer` can be derived by providing a `String` as a fact and `Rule1` will be executed, or
-by also providing an `IntegerBase` and `Rule2` will be executed.
+A more complex example can be found in the [examples/update_readme.py](examples/update_readme.py) file. That script
+is actually used to keep this README file up to date with the example and the table of contents above. It demonstrates
+how to use the rule engine to generate a file based on a set of rules, leveraging union memberships and rule result
+caching.
 
-__Installation__
+## Installation
 
 Adjudicator is available on PyPI. You need at least Python 3.10.
 
 ```bash
 pip install python-adjudicator
 ```
 
-__Example code__
-
-Check out the [examples/codegen/](examples/codegen/) directory for a simple example of a rules engine that generates
-Terraform code based on a set of Kubernetes-like resources. This example combines the resource management API with
-the rules engine API.
-
-```mermaid
-graph LR
-    AwsAccount["Resource[AwsAccount]"] --> AwsAccountCreation
-    AwsAccount["Resource[AwsAccount]"] --> AwsProviderInitialization
-    TerraformWorkspace["Resource[TerraformWorspace]"] --> TerraformWorkspaceCreation
-```
-
-The advantage of using a rules engine here is that it avoids executing the same rule again if it was already executed
-with the same inputs. It also makes it easier to increase the system's complexity by adding more rules without also
-significantly increasing the complexity of the code.
-
-__Future extensions__
+## Future Extensions
 
 * Currently the rule graph stores rules as connections between types and rules on edges. A more efficient
   representation would be the one illustrated above, where types are connected to rules which are connected to types.
 * The ability to mark facts as required to be consumed. If such a fact is not consumed during the execution of a
   request, an error will be raised.
```

