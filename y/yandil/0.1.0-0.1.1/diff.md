# Comparing `tmp/yandil-0.1.0.tar.gz` & `tmp/yandil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.1.0.tar", max compression
+gzip compressed data, was "yandil-0.1.1.tar", max compression
```

## Comparing `yandil-0.1.0.tar` & `yandil-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2023-06-21 18:50:46.521116 yandil-0.1.0/README.md
--rw-r--r--   0        0        0      817 2023-06-21 18:51:43.093824 yandil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0     8588 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     2573 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      255 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     2308 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-21 18:50:46.525116 yandil-0.1.0/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 17:48:56.767189 yandil-0.1.1/README.md
+-rw-r--r--   0        0        0      817 2023-06-22 17:49:49.976006 yandil-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0     8588 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1020 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3002 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      255 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     2364 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.1/PKG-INFO
```

### Comparing `yandil-0.1.0/README.md` & `yandil-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/pyproject.toml` & `yandil-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.1.0"
+version = "0.1.1"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 
@@ -30,15 +30,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.1.1"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.1.0/src/yandil/configuration/configuration_container.py` & `yandil-0.1.1/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/container.py` & `yandil-0.1.1/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/declarative/decorators.py` & `yandil-0.1.1/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/dependency.py` & `yandil-0.1.1/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/dependency_filler.py` & `yandil-0.1.1/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/discovery/class_discovery.py` & `yandil-0.1.1/src/yandil/discovery/class_discovery.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 from ast import Call, ClassDef, FunctionDef, Name, parse
 from dataclasses import dataclass
 from importlib import import_module
 from os import path
 from os.path import relpath, splitext
-from typing import Iterator, Set, Type
+from typing import Iterable, Set, Type
 
 
 @dataclass(frozen=True)
 class ClassData:
     module_file_path: str
     class_name: str
 
     def to_class(self, sources_root_path: str) -> Type:
         module_path_without_ext = splitext(self.module_file_path)[0]
         module_rel_path = relpath(module_path_without_ext, sources_root_path)
         module = import_module(module_rel_path.replace(path.sep, "."))
         return getattr(module, self.class_name)
 
 
-def discover_classes_from_module(module_file_path: str) -> Iterator[ClassDef]:
+def discover_classes_from_module(module_file_path: str) -> Iterable[ClassDef]:
     with open(module_file_path, "r", encoding="utf-8") as file:
         module_ast = parse(file.read())
 
     for node in module_ast.body:
         if isinstance(node, ClassDef):
             yield node
 
 
-def transform_class_nodes_to_class_data(class_nodes: Iterator[ClassDef], module_file_path: str) -> Iterator[ClassData]:
+def exclude_abstract_classes(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
+    def __is_abstract_class_node(node: ClassDef) -> bool:
+        for base in node.bases:
+            if isinstance(base, Name) and base.id in {"Protocol", "Generic", "ABC"}:
+                return True
+        return False
+
+    for class_node in class_nodes:
+        if not __is_abstract_class_node(class_node):
+            yield class_node
+
+
+def transform_class_nodes_to_class_data(class_nodes: Iterable[ClassDef], module_file_path: str) -> Iterable[ClassData]:
     for class_node in class_nodes:
         yield ClassData(
             module_file_path=module_file_path,
             class_name=class_node.name,
         )
 
 
-def exclude_classes_without_public_methods(class_nodes: Iterator[ClassDef]) -> Iterator[ClassDef]:
+def exclude_classes_without_public_methods(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
     for class_node in class_nodes:
         if class_defines_public_methods(class_node):
             yield class_node
 
 
 def class_defines_public_methods(class_node: ClassDef) -> bool:
     for node in class_node.body:
         if not isinstance(node, FunctionDef) or node.name.startswith("_"):
             continue
         return True
     return False
 
 
-def exclude_dataclasses(class_nodes: Iterator[ClassDef]) -> Iterator[ClassDef]:
+def exclude_dataclasses(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
     for class_node in class_nodes:
         if class_has_any_decorator(class_node, {"dataclass"}):
             continue
         yield class_node
 
 
 def class_has_any_decorator(class_node: ClassDef, decorator_names: Set[str]) -> bool:
@@ -66,12 +78,12 @@
 
         if decorator_id in decorator_names:
             return True
     return False
 
 
 def exclude_classes_without_decorators(
-    class_nodes: Iterator[ClassDef], decorator_names: Set[str]
-) -> Iterator[ClassDef]:
+    class_nodes: Iterable[ClassDef], decorator_names: Set[str]
+) -> Iterable[ClassDef]:
     for class_node in class_nodes:
         if class_has_any_decorator(class_node, decorator_names):
             yield class_node
```

### Comparing `yandil-0.1.0/src/yandil/discovery/module_discovery.py` & `yandil-0.1.1/src/yandil/discovery/module_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pkgutil
 from dataclasses import dataclass
 from importlib.machinery import FileFinder
 from os.path import join
-from typing import Iterator, Optional, Set
+from typing import Iterable, Optional, Set
 
 
 @dataclass(frozen=True)
 class ModuleData:
     module_name: str
     module_path: str
 
 
-def discover_modules(base_path: str, exclude_modules: Optional[Set[str]] = None) -> Iterator[ModuleData]:
+def discover_modules(base_path: str, exclude_modules: Optional[Set[str]] = None) -> Iterable[ModuleData]:
     if exclude_modules is None:
         exclude_modules = set()
 
     for module_finder, module_name, is_pkg in pkgutil.iter_modules([base_path]):
         if module_name in exclude_modules:
             continue
```

### Comparing `yandil-0.1.0/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.1.1/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.1.1/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable, Optional, Set
 
 from yandil.container import Container, default_container
 from yandil.discovery.class_discovery import (
     ClassData,
     discover_classes_from_module,
+    exclude_abstract_classes,
     exclude_classes_without_public_methods,
     exclude_dataclasses,
     transform_class_nodes_to_class_data,
 )
 from yandil.discovery.module_discovery import discover_modules
 
 
@@ -43,13 +44,13 @@
 
     def __get_classes_discover_iterable(
         self,
         module_file_path: str,
         should_exclude_classes_without_public_methods: bool,
         should_exclude_dataclasses: bool,
     ) -> Iterable[ClassData]:
-        iterable = discover_classes_from_module(module_file_path)
+        iterable = exclude_abstract_classes(discover_classes_from_module(module_file_path))
         if should_exclude_classes_without_public_methods:
             iterable = exclude_classes_without_public_methods(iterable)
         if should_exclude_dataclasses:
             iterable = exclude_dataclasses(iterable)
         return transform_class_nodes_to_class_data(iterable, module_file_path)
```

### Comparing `yandil-0.1.0/src/yandil/typing_tools.py` & `yandil-0.1.1/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.0/PKG-INFO` & `yandil-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

