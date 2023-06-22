# Comparing `tmp/taipan_di-0.0.6.tar.gz` & `tmp/taipan_di-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.6.tar", max compression
+gzip compressed data, was "taipan_di-0.0.7.tar", max compression
```

## Comparing `taipan_di-0.0.6.tar` & `taipan_di-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0     1063 2023-06-16 20:14:24.052799 taipan_di-0.0.6/LICENSE
--rw-r--r--   0        0        0     3022 2023-06-16 20:14:24.052799 taipan_di-0.0.6/README.md
--rw-r--r--   0        0        0     1004 2023-06-16 20:14:24.052799 taipan_di-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      474 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/__init__.py
--rw-r--r--   0        0        0      140 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     3730 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      673 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      733 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3689 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0      130 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      503 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      625 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      225 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/tools/__init__.py
--rw-r--r--   0        0        0      811 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_factory.py
--rw-r--r--   0        0        0      705 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_link.py
--rw-r--r--   0        0        0     1775 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_registrator.py
--rw-r--r--   0        0        0      415 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       67 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      142 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      148 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_registration_error.py
--rw-r--r--   0        0        0      132 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      148 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      236 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      933 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0     1056 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      544 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/py.typed
--rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 taipan_di-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-22 15:31:06.188720 taipan_di-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2977 2023-06-22 15:31:06.188720 taipan_di-0.0.7/README.md
+-rw-r--r--   0        0        0     1004 2023-06-22 15:31:06.188720 taipan_di-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-06-22 15:31:06.188720 taipan_di-0.0.7/taipan_di/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-22 15:31:06.188720 taipan_di-0.0.7/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-22 15:31:06.188720 taipan_di-0.0.7/taipan_di/classes/registerers/__init__.py
+-rw-r--r--   0        0        0     1833 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/registerers/factory_registerer.py
+-rw-r--r--   0        0        0     2370 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/registerers/pipeline_registerer.py
+-rw-r--r--   0        0        0     1131 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/registerers/service_registerer.py
+-rw-r--r--   0        0        0     2143 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/registerers/singleton_registerer.py
+-rw-r--r--   0        0        0      130 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      423 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      551 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0     1639 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/service_collection.py
+-rw-r--r--   0        0        0      650 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/service_container.py
+-rw-r--r--   0        0        0      681 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/service_provider.py
+-rw-r--r--   0        0        0      205 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/tools/__init__.py
+-rw-r--r--   0        0        0     3692 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/tools/instanciate_service.py
+-rw-r--r--   0        0        0      844 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/tools/pipeline_factory.py
+-rw-r--r--   0        0        0      944 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/classes/tools/pipeline_link.py
+-rw-r--r--   0        0        0      433 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      240 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      241 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/taipan_registration_error.py
+-rw-r--r--   0        0        0      235 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/taipan_resolution_error.py
+-rw-r--r--   0        0        0      250 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      218 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0      582 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/interfaces/base_service_container.py
+-rw-r--r--   0        0        0      971 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/interfaces/base_service_provider.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:31:06.192720 taipan_di-0.0.7/taipan_di/py.typed
+-rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 taipan_di-0.0.7/PKG-INFO
```

### Comparing `taipan_di-0.0.6/LICENSE` & `taipan_di-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.6/README.md` & `taipan_di-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,14 @@
  - Register pipelines easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
- - It is necessary to write an `__init__` function or use `@dataclass`
 
 
 ## Installation
 
 ### Pip
 
 > `pip install taipan-di`
@@ -35,49 +34,61 @@
 [Poetry](https://python-poetry.org/) is a Python dependency management and packaging tool. I actually use it for this project.
 
 > `poetry add taipan-di`
 
 
 ## Usage
 
-First, you have to create a `DependencyCollection` in which you will register your services. Each `DependencyCollection` is independant and contain different services.
+First, you have to create a `ServiceCollection` in which you will register your services. Each `ServiceCollection` is independant and contain different services.
 
-> `services = DependencyCollection()`
+```python
+services = ServiceCollection()
+```
 
-Then, register your services as you wish. They can be registered as factories or singletons using the following methods :
+Then, register your services as you wish. You can initiate registrations processes via 2 ways :
 
- - `services.register_factory(InterfaceType, ImplementationType)`
- - `services.register_singleton(InterfaceType, ImplementationType)`
+```python
+services.register(Type)
+services.register_pipeline(Type)
+```
 
-You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
+For "standard" registration, you have to first choose the scope and then how you wish the instances to be created. Examples :
 
- - `services.register_factory_creator(Type, lambda provider: create(provider))`
- - `services.register_singleton_creator(Type, lambda provider: create(provider))`
- - `services.register_singleton_instance(Type, instance)`
+```python
+services.register(Type).as_factory().with_implementation(ChildType)
+services.register(Type).as_singleton().with_self()
+services.register(Type).as_singleton().with_instance(instance)
+services.register(Type).as_factory().with_creator(lambda provider: create(provider))
+```
 
-You can also register pipelines. Examples are given in the test files.
+For pipeline registration, all you have to do is add the links that constitute the pipeline and register it as a singleton or a factory. Example :
 
-Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
+```python
+services.register_pipeline(Type).add(Link1).add(Link2).as_factory()
+```
 
-> `provider = services.build()`<br/>
-> `resolved = provider.resolve(InterfaceType)`
+Once your services are registered, you have to build a service provider which will be used to resolve services : 
 
-If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
+```python
+provider = services.build()
+resolved = provider.resolve(Type)
+```
+
+If `Type` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `ServiceCollection`.
 
 
 ## Inspirations
 
-This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements.
+This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements and wishes.
 
 I also took inspiration from the [*injector*](https://pypi.org/project/injector/) library and .Net's dependency injection system.
 
 
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
- - Modify the registration process / methods to better handle type conditions and protocols
  - Create configuration from environment or configuration files
```

### Comparing `taipan_di-0.0.6/pyproject.toml` & `taipan_di-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.6"
+version = "0.0.7"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
```

### Comparing `taipan_di-0.0.6/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.7/taipan_di/classes/tools/instanciate_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     TypeVar,
     Union,
     ForwardRef,
     cast,
 )
 from typing_extensions import Protocol
 
-from taipan_di.interfaces import BaseDependencyProvider
-from taipan_di.errors import TaipanInjectionError, TaipanTypeError
+from taipan_di.interfaces import BaseServiceProvider
+from taipan_di.errors import TaipanInjectionError, TaipanResolutionError
 
 __all__ = ["instanciate_service"]
 
 S = TypeVar("S")
 
 Undefined = NewType("Undefined", int)
 
@@ -80,35 +80,35 @@
 
     return parameters
 
 
 def _resolve_function_kwargs(
     parameters_name: Tuple[str, ...],
     parameters: Dict[str, Parameter],
-    provider: BaseDependencyProvider,
+    provider: BaseServiceProvider,
 ) -> Dict[str, Any]:
     resolved_kwargs = {}
 
     for name in parameters_name:
         if provider.contains(parameters[name].type):
             resolved_kwargs[name] = provider.resolve(parameters[name].type)
             continue
 
         if parameters[name].default is not Undefined:
             resolved_kwargs[name] = parameters[name].default
 
     return resolved_kwargs
 
 
-def instanciate_service(service: Type[S], provider: BaseDependencyProvider) -> S:
+def instanciate_service(service: Type[S], provider: BaseServiceProvider) -> S:
     constructor = getattr(service, "__init__")
 
     # ignore abstract class initialiser and protocol initialisers
     if constructor in [ABC.__init__, _no_init] or constructor.__name__ == "_no_init":
-        raise TaipanTypeError(
+        raise TaipanResolutionError(
             f"{str(service)} has no __init__, cannot instanciate the service"
         )
 
     # Add class definition to dependency injection
     parameters = _inspect_function_arguments(constructor)
     parameters_name = tuple([p for p in parameters.keys() if p != "self"])
```

### Comparing `taipan_di-0.0.6/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.7/taipan_di/classes/scopes/singleton_scope.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from typing import Any, Callable, Type, TypeVar, cast
+from typing import Callable, Generic, Type, TypeVar
 
-from taipan_di.interfaces import BaseDependencyProvider, BaseScope
+from taipan_di.interfaces import BaseServiceProvider
 
 __all__ = ["SingletonScope"]
 
 T = TypeVar("T")
 
 
-class SingletonScope(BaseScope):
-    def __init__(self, creator: Callable[[BaseDependencyProvider], Any]) -> None:
+class SingletonScope(Generic[T]):
+    def __init__(self, creator: Callable[[BaseServiceProvider], T]) -> None:
         self._creator = creator
         self._memoized_instance = None
 
-    def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
+    def get_instance(self, container: BaseServiceProvider) -> T:
         if self._memoized_instance is None:
             self._memoized_instance = self._creator(container)
 
-        result = cast(type, self._memoized_instance)
-        return result
+        return self._memoized_instance
```

### Comparing `taipan_di-0.0.6/taipan_di/classes/tools/pipeline_factory.py` & `taipan_di-0.0.7/taipan_di/classes/tools/pipeline_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Generic, List, TypeVar
 
 from taipan_di.classes.tools import PipelineLink
 from taipan_di.errors import TaipanRegistrationError
 
 __all__ = ["PipelineFactory"]
 
@@ -9,15 +10,15 @@
 U = TypeVar("U")
 
 
 class PipelineFactory(Generic[T, U]):
     def __init__(self) -> None:
         self._links: List[PipelineLink[T, U]] = []
 
-    def add(self, link: PipelineLink[T, U]) -> "PipelineFactory[T, U]":
+    def add(self, link: PipelineLink[T, U]) -> PipelineFactory[T, U]:
         self._links.append(link)
         return self
 
     def build(self) -> PipelineLink[T, U]:
         if len(self._links) == 0:
             raise TaipanRegistrationError(
                 f"Pipeline[{str(T)}, {str(U)}] is empty ! Add at least one link"
```

### Comparing `taipan_di-0.0.6/taipan_di/classes/tools/pipeline_link.py` & `taipan_di-0.0.7/taipan_di/classes/tools/pipeline_link.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,37 @@
+from __future__ import annotations
+
 import abc
 from typing import Callable, Generic, Optional, TypeVar
 
 __all__ = ["PipelineLink"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class PipelineLink(Generic[T, U], metaclass=abc.ABCMeta):
+    """
+    A component of a pipeline.
+
+    When writing your own links, you only have to write the `_handle` method.
+    """
+
     def __init__(self) -> None:
         self._next = None
 
-    def _set_next(self, next: "PipelineLink[T, U]") -> "PipelineLink[T, U]":
+    def _set_next(self, next: PipelineLink[T, U]) -> PipelineLink[T, U]:
         self._next = next
         return self._next
 
     def exec(self, request: T) -> Optional[U]:
+        """
+        Execute the pipeline that starts at this link.
+        """
+
         next_function = self._next.exec if self._next is not None else lambda req: None
 
         return self._handle(request, next_function)
 
     @abc.abstractmethod
     def _handle(self, request: T, next: Callable[[T], Optional[U]]) -> Optional[U]:
         return next(request)
```

### Comparing `taipan_di-0.0.6/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.7/taipan_di/interfaces/base_service_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import abc
-from typing import Type, TypeVar
+from typing import Any, Type, TypeVar, Protocol
 
-__all__ = ["BaseDependencyProvider"]
+__all__ = ["BaseServiceProvider"]
 
 T = TypeVar("T")
 
 
-class BaseDependencyProvider(metaclass=abc.ABCMeta):
-    @classmethod
-    def __subclasshook__(cls, subclass):
-        return (
-            hasattr(subclass, "contains")
-            and callable(subclass.contains)
-            and hasattr(subclass, "resolve")
-            and callable(subclass.resolve)
-            or NotImplemented
-        )
+class BaseServiceProvider(Protocol):
+    """
+    The `BaseServiceProvider` contains the services that were registered and allows for
+    their resolution via the `resolve` method.
+    """
 
     @abc.abstractmethod
-    def contains(self, type: Type) -> bool:
+    def contains(self, type: Type[Any]) -> bool:
         """
         Checks if the requested type is registered in the provider's services
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def resolve(self, type: Type[T]) -> T:
         """
         Resolve a service along with its dependencies if it is registered in the provider.
         It it isn't, a TaipanUnregisteredError is raised.
 
         Warning : Depending on how the services were registered, the instance provided might
-        not be of the requested type.
+        not be of the requested type. This would not happen if type hinting is respected.
         """
         raise NotImplementedError
```

### Comparing `taipan_di-0.0.6/PKG-INFO` & `taipan_di-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.6
+Version: 0.0.7
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -39,15 +39,14 @@
  - Register pipelines easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
- - It is necessary to write an `__init__` function or use `@dataclass`
 
 
 ## Installation
 
 ### Pip
 
 > `pip install taipan-di`
@@ -57,50 +56,62 @@
 [Poetry](https://python-poetry.org/) is a Python dependency management and packaging tool. I actually use it for this project.
 
 > `poetry add taipan-di`
 
 
 ## Usage
 
-First, you have to create a `DependencyCollection` in which you will register your services. Each `DependencyCollection` is independant and contain different services.
+First, you have to create a `ServiceCollection` in which you will register your services. Each `ServiceCollection` is independant and contain different services.
 
-> `services = DependencyCollection()`
+```python
+services = ServiceCollection()
+```
 
-Then, register your services as you wish. They can be registered as factories or singletons using the following methods :
+Then, register your services as you wish. You can initiate registrations processes via 2 ways :
 
- - `services.register_factory(InterfaceType, ImplementationType)`
- - `services.register_singleton(InterfaceType, ImplementationType)`
+```python
+services.register(Type)
+services.register_pipeline(Type)
+```
 
-You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
+For "standard" registration, you have to first choose the scope and then how you wish the instances to be created. Examples :
 
- - `services.register_factory_creator(Type, lambda provider: create(provider))`
- - `services.register_singleton_creator(Type, lambda provider: create(provider))`
- - `services.register_singleton_instance(Type, instance)`
+```python
+services.register(Type).as_factory().with_implementation(ChildType)
+services.register(Type).as_singleton().with_self()
+services.register(Type).as_singleton().with_instance(instance)
+services.register(Type).as_factory().with_creator(lambda provider: create(provider))
+```
 
-You can also register pipelines. Examples are given in the test files.
+For pipeline registration, all you have to do is add the links that constitute the pipeline and register it as a singleton or a factory. Example :
 
-Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
+```python
+services.register_pipeline(Type).add(Link1).add(Link2).as_factory()
+```
 
-> `provider = services.build()`<br/>
-> `resolved = provider.resolve(InterfaceType)`
+Once your services are registered, you have to build a service provider which will be used to resolve services : 
 
-If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
+```python
+provider = services.build()
+resolved = provider.resolve(Type)
+```
+
+If `Type` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `ServiceCollection`.
 
 
 ## Inspirations
 
-This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements.
+This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements and wishes.
 
 I also took inspiration from the [*injector*](https://pypi.org/project/injector/) library and .Net's dependency injection system.
 
 
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
- - Modify the registration process / methods to better handle type conditions and protocols
  - Create configuration from environment or configuration files
```

