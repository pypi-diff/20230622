# Comparing `tmp/pybox-toolkit-0.1.9.dev79.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev79.tar", last modified: Thu Jun 22 11:00:47 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev81.tar", last modified: Thu Jun 22 16:51:10 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev79.tar` & `pybox-toolkit-0.1.9.dev81.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-22 08:25:42.000000 pybox-toolkit-0.1.9.dev79/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.9.dev79/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:02:46.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:29:38.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:51:10.287623 pybox-toolkit-0.1.9.dev81/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.279623 pybox-toolkit-0.1.9.dev81/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev79/pyproject.toml` & `pybox-toolkit-0.1.9.dev81/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 name = "pybox-toolkit"
 dynamic = ["version"]
 authors = [
     { name = "mguichard", email = "m.guichard@student.tudelft.nl" },
     { name = "rstular", email = "r.stular@student.tudelft.nl" },
 ]
 description = "A toolkit used within the PyBox project"
-dependencies = [
-    "sympy~=1.12",
-    "typing_extensions~=4.5.0"
-]
+dependencies = ["sympy~=1.12"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.ewi.tudelft.nl/cse2000-software-project/2022-2023-q4/cluster-00/group-13c/group-13c-contributors/-/tree/main/toolkit"
 
 [tool.setuptools_scm]
 root = ".."
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
+
+[tool.setuptools.package-data]
+toolkit = ["py.typed"]
```

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """Toolkit is a library for creating and testing formulas."""
 
-from typing import Any, Callable, Optional, Union
 from sys import stdout
-import mpmath
+from typing import Any, Callable, Optional, Union
 
+import mpmath
 import sympy
 from sympy.core.basic import Basic as SympyBasic
-from typing_extensions import Type, Self
 
 from toolkit import test
-from toolkit.typing import Unit, BaseUnit, _UnitClassParser
+from toolkit.typing import BaseUnit, Unit, _UnitClassParser
 from toolkit.utils import (
-    parse_interval,
-    map_dictionary_value,
-    map_dictionary_key,
     ArgumentException,
     DocumentationException,
     RangeException,
     RuntimeException,
     TestingException,
-    ex_assert,
+    map_dictionary_key,
+    map_dictionary_value,
 )
 
+
 class BaseFormula:
     """
     Contains information about a formula, including:
             - Parameter ranges
             - Labels
             - Documentation
     """
 
-    formulas: list[Self] = []
+    formulas: list["BaseFormula"] = []
     outputs: list[tuple[str, Unit]] = []
     test_class: test.ToolkitTests = None
 
     def __init__(self, function: Callable[..., Any], **kwargs):
         if "outputs" not in kwargs:
             raise ArgumentException(
                 f"Function '{function.__qualname__}' does not have any outputs defined"
@@ -51,15 +49,15 @@
 	'''
             )
 
         self.__dict__.update(kwargs)
         self.docs: str = function.__doc__
         self.function: Callable[..., Any] = function
         self.num_args: int = function.__code__.co_argcount
-        self.arg_names: list[str] = function.__code__.co_varnames[:self.num_args]
+        self.arg_names: list[str] = function.__code__.co_varnames[: self.num_args]
         self.name: str = function.__qualname__.replace("_", " ").title()
         self.variable_types: dict[str, BaseUnit] = {}
 
         for variable in self.arg_names:
             if variable not in function.__annotations__:
                 raise ArgumentException(
                     f"Variable '{variable}' in '{function.__qualname__}' is missing a type"
@@ -70,15 +68,17 @@
 
         for output_name, output_type in self.outputs:
             self.variable_types[output_name] = output_type
             self.check_variable(output_name, output_type)
 
         BaseFormula.formulas.append(self)
 
-    def prepare_output_list(self, output_list: list[dict[str, BaseUnit]]) -> list[dict[str, BaseUnit]]:
+    def prepare_output_list(
+        self, output_list: list[dict[str, BaseUnit]]
+    ) -> list[dict[str, BaseUnit]]:
         """Prepare a list of dictionaries of outputs by:
             1. Checking variables are in their physical range or are a choice
             2. Variables are not a complex type returned by mpmath
             3. Converting all mpmath specific types to default types
 
         Args:
             output_list (list[dict[str, BaseUnit]]]): list of outputs
@@ -119,15 +119,15 @@
             variable (str): Name of the variable
             variable_class (Unit): Unit class of the variable
 
         Raises:
             ArgumentException: If the variable class is not derived from Unit
         """
 
-    def run_tests(self, output_stream = stdout) -> bool:
+    def run_tests(self, output_stream=stdout) -> bool:
         """Run all tests for this formula
 
         Raises:
             TestingException: If the formula does not have a test class
 
         Returns:
             bool: True if all tests passed, False otherwise
@@ -137,48 +137,47 @@
             raise TestingException(
                 f"Cannot run tests for: '{self.function.__qualname__}', a test class was not provided."
             )
         return test.run_testcase(self.test_class, output_stream).wasSuccessful()
 
 
 def __formula(
-    function_class: Type[BaseFormula],
+    function_class: type[BaseFormula],
     function: Optional[Callable[..., Any]],
     **kwargs,
-) -> BaseFormula:
+) -> Callable[[Optional[Callable[..., Any]]], BaseFormula]:
     """The expression used in a decorator is evaluated before use, so passing in variables to the wrapper
     will actually evaluate the wrapper before passing in the function.
     We can use currying to bypass this by returning a new wrapper that actually gets the function as an argument.
 
     Args:
-        function_class (Type[BaseFormula]): Formula class (type).
-        function (Optional[Callable[..., Any]]): Function to be wrapped.
+        function_class (type[BaseFormula]): Formula class (type).
+        function (Callable[..., Any]): Function to be wrapped.
 
     Returns:
-        BaseFormula: Wrapped formula object.
+        Callable[[Optional[Callable[..., Any]]], BaseFormula]: Wrapped formula object.
     """
     if function:
         return function_class(function)
 
-    def wrapper(function: Optional[Callable[..., Any]]) -> BaseFormula:
+    def wrapper(function: Callable[..., Any]) -> BaseFormula:
         return function_class(function, **kwargs)
 
     return wrapper
 
+
 class _PureFormula(BaseFormula):
     def __init__(self, function: Callable[..., SympyBasic], **kwargs):
         super().__init__(function, **kwargs)
         self.variable_symbols: dict[str, sympy.Symbol] = {}
 
         for variable in self.variable_types:
             self.variable_symbols[variable] = sympy.Symbol(variable)
 
-        sympy_function_inputs = [
-            self.variable_symbols[i] for i in self.arg_names
-        ]
+        sympy_function_inputs = [self.variable_symbols[i] for i in self.arg_names]
         sympy_function = function(*sympy_function_inputs)
         if not isinstance(sympy_function, tuple):
             sympy_function = (sympy_function,)
 
         self.sympy_equations = tuple(
             sympy.Eq(equation, self.variable_symbols[output[0]])
             for (equation, output) in zip(sympy_function, self.outputs)
@@ -239,51 +238,57 @@
                 ),
                 dic_list,
             )
         )
 
         return results
 
-    def __call__(
-        self, *args: tuple[Unit, ...], **kwargs
-    ) -> list[dict[str, float]]:
+    def __call__(self, *args: tuple[Unit, ...], **kwargs) -> list[dict[str, float]]:
         """Execute the formula with the provided arguments
 
         Raises:
             RangeException: If any of the arguments are outside of their physical range
 
         Returns:
             list[dict[str, float]]: List of dictionaries containing outputs of the formula
                                           (one dictionary per possible solution)
         """
         if len(args) == self.num_args or set(kwargs) == set(self.arg_names):
-            inputs = args if len(args) == self.num_args else [kwargs[i] for i in self.arg_names]
+            inputs = (
+                args
+                if len(args) == self.num_args
+                else [kwargs[i] for i in self.arg_names]
+            )
             for name, value in zip(self.arg_names, inputs):
                 if not self.variable_types[name].possible(value):
                     raise RangeException(
                         f"Variable '{name}' outside of physical range or choices."
                     )
 
             result = self.function(*args, **kwargs)
             if not isinstance(result, tuple):
                 result = (result,)
-            return self.prepare_output_list([dict(zip(map(lambda x: x[0], self.outputs), result))])
+            return self.prepare_output_list(
+                [dict(zip(map(lambda x: x[0], self.outputs), result))]
+            )
 
         for name, value in kwargs.items():
             if not self.variable_types[name].possible(value):
                 raise RangeException(
                     f"Variable '{name}' outside of physical range or choices."
                 )
 
         argument_list = tuple(sorted((i for i in kwargs)))
         non_argument_list = sorted((i for i in self.variable_types if i not in kwargs))
         if argument_list in self.cached_lambdas:
-            return self.prepare_output_list(self.execute_lambda_dictionary_list(
-                self.cached_lambdas[argument_list], kwargs, argument_list
-            ))
+            return self.prepare_output_list(
+                self.execute_lambda_dictionary_list(
+                    self.cached_lambdas[argument_list], kwargs, argument_list
+                )
+            )
 
         known_symbols = [self.variable_symbols[arg] for arg in argument_list]
         unknown_symbols = [self.variable_symbols[sym] for sym in non_argument_list]
 
         # This shit either returns a dictionary of independent variables
         # or a list of tuples of dependent equations
         solved = sympy.solve(self.sympy_equations, *unknown_symbols)
@@ -300,56 +305,66 @@
             # in physical range checks
             solved = [map_dictionary_key(str, solved)]
 
         # We map over the dictionaries entries to get the lambdas tied to each variable
         lambdifieds = list(
             map(
                 lambda dic: map_dictionary_value(
-                    lambda equation: sympy.lambdify(known_symbols, equation, modules = "math"),
+                    lambda equation: sympy.lambdify(
+                        known_symbols, equation, modules="math"
+                    ),
                     dic,
                 ),
                 solved,
             )
         )
 
         self.cached_lambdas[argument_list] = lambdifieds
 
-        return self.prepare_output_list(self.execute_lambda_dictionary_list(lambdifieds, kwargs, argument_list))
+        return self.prepare_output_list(
+            self.execute_lambda_dictionary_list(lambdifieds, kwargs, argument_list)
+        )
 
 
 class _ImpureFormula(BaseFormula):
-    def __call__(self, *args: tuple[Unit, ...], **kwargs) -> list[dict[str, float, int]]:
+    def __call__(
+        self, *args: tuple[Unit, ...], **kwargs
+    ) -> list[dict[str, Union[float, int]]]:
         """Call the impure formula.
 
         Raises:
             RangeException: If any of the arguments are outside of their physical range.
 
         Returns:
             Any: output arguments.
         """
         function_arguments = self.arg_names
         if len(args) == self.num_args:
             inputs = args
         else:
             if set(kwargs) != set(function_arguments):
-                raise ArgumentException(f"""Keyword arguments for impure expression must match its arguments:
-                {tuple(kwargs)} does not match {function_arguments} for {self.name}.""")
+                raise ArgumentException(
+                    f"""Keyword arguments for impure expression must match its arguments:
+                {tuple(kwargs)} does not match {function_arguments} for {self.name}."""
+                )
             inputs = [kwargs[i] for i in self.arg_names]
 
         for name, value in zip(self.arg_names, inputs):
             if not self.variable_types[name].possible(value):
                 raise RangeException(
                     # Idea, add function to get the last part of the error message
-                    f"Variable '{name}' outside of physical range or choices." 
+                    f"Variable '{name}' outside of physical range or choices."
                 )
 
         result = self.function(*args, **kwargs)
         if not isinstance(result, tuple):
             result = (result,)
-        return self.prepare_output_list([dict(zip(map(lambda x: x[0], self.outputs), result))])
+        return self.prepare_output_list(
+            [dict(zip(map(lambda x: x[0], self.outputs), result))]
+        )
 
     def check_variable(self, variable: str, variable_type_instance: Unit):
         """Parse a variable and add it to the parsed_ranges dictionary
 
         Args:
             variable (str): Name of the variable
             variable_class (Unit): Unit class of the variable
@@ -358,14 +373,15 @@
             ArgumentException: If the variable class is not derived from Unit
         """
         if not isinstance(variable_type_instance, BaseUnit):
             raise ArgumentException(
                 f"Variable '{variable}' has a class not derived from BaseUnit"
             )
 
+
 def PureFormula(  # pylint: disable=invalid-name
     func: Optional[Callable[..., SympyBasic]] = None, **kwargs
 ) -> _PureFormula:
     """Annotation for the pure formulas.
     These formulas can only contain sympy functions and operations, and must return a single sympy expression.
 
     The advantage of using this annotation is that the formula will support expressing
```

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/test/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Testing framework for formula scripts"""
 
 from __future__ import annotations
 
 import unittest
 from sys import stdout
-from typing import TYPE_CHECKING, Callable, TextIO, Union
+from typing import TYPE_CHECKING, Any, Callable, TextIO, Union
 from unittest import TestResult
 
-from typing_extensions import Any
-
 from toolkit.utils import TestingException
 
 if TYPE_CHECKING:
     from toolkit import BaseFormula
 
 
 def compare_floats(first: float, second: float, epsilon: float = 0.00001) -> bool:
@@ -38,18 +36,15 @@
 
     Returns:
         bool: whether the entries are equal
     """
     return all((compare_floats(value, second[key])) for key, value in first.items())
 
 
-def compare_result(
-    result: dict[str, float] | list[dict[str, float]],
-    expected: dict[str, float] | list[dict[str, float]],
-) -> bool:
+def compare_result(result: list[dict[str, float]], expected: list[dict[str, float]]) -> bool:
     """Compares a result and expected from toolkit
 
     Args:
         result (dict[str, float] | list[dict[str, float]]): result value
         expected (dict[str, float] | list[dict[str, float]]): expected value
 
     Returns:
@@ -88,22 +83,19 @@
         return new_test
 
 
 # Have a dummy of this production runs in the browser
 class ToolkitTests(unittest.TestCase, metaclass=TestClassSetup):
     """Base class for all tests"""
 
-    function: Callable[..., Any]
+    __qualname__: str
+    function: BaseFormula
     documented_tests: list[tuple[dict[str, Any], list[dict[str, Any]]]]
 
-    def documented_test(
-        self,
-        arguments: dict[str, Any] = None,
-        expected: Union[dict[str, Any], list[dict[str, Any]]] = None,
-    ):
+    def documented_test(self, arguments: dict[str, Any], expected: Union[dict[str, Any], list[dict[str, Any]]]):
         """Run a documented test
 
         Args:
             arguments (dict[str, Any], optional): Argument values to test with. Defaults to None.
             expected (Union[dict[str, Any], list[dict[str, Any]]], optional): Expected values. Defaults to None.
 
         Raises:
```

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev79/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev81/src/toolkit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Miscelaneous utilities for the toolkit"""
 
 from math import copysign, isnan
 from collections.abc import Iterable
-from typing import Callable
-from typing_extensions import TypeVar
+from typing import Callable, TypeVar
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
+
 class ToolkitException(Exception):
     """Base class for exceptions in the toolkit."""
 
 
 class RangeException(ToolkitException):
     """Exception raised for invalid range or out-of range variables."""
 
@@ -24,14 +24,15 @@
 class DocumentationException(ToolkitException):
     """Exception raised for invalid/missing documentation."""
 
 
 class TestingException(ToolkitException):
     """Exception raised for invalid/missing/failing tests."""
 
+
 class RuntimeException(ToolkitException):
     """Exception raised for general runtime errors."""
 
 
 def ex_assert(condition: bool, exception: Exception):
     """Raise an exception if a condition is not met
 
@@ -41,30 +42,32 @@
 
     Raises:
         exception: If condition is not met
     """
     if not condition:
         raise exception
 
+
 _EPSILON = 10**-7
 
 _UNICODE_DIGITS = {
     "0": "⁰",
     "1": "¹",
     "2": "²",
     "3": "³",
     "4": "⁴",
     "5": "⁵",
     "6": "⁶",
     "7": "⁷",
     "8": "⁸",
     "9": "⁹",
-    "-": "⁻"
+    "-": "⁻",
 }
 
+
 def parse_interval(interval_string: str) -> tuple[float, float]:
     """
     Expects input of the form:
     (a, b) (a, b] [a, b) [a, b]
     Parses it into a list of 2 elements which are an inclusive range.
 
     Args:
@@ -80,108 +83,140 @@
     interval: tuple[float, float] = (
         float(components[0][1:]) + (_EPSILON if components[0][0] == "(" else 0),
         float(components[1][:-1]) - (_EPSILON if components[1][-1] == ")" else 0),
     )
 
     return interval
 
+
 def stringify_interval(interval: tuple[float, float]) -> str:
     """
     Turns a physical range back into its string representation.
     Args:
         interval (tuple[float, float]): interval in tuple form
 
     Returns:
         str: interval in string form
     """
     # We try to undo the epsilon for clarity, but this will not work if the original input was non-integral
-    if interval[0] == float('inf'):
+    if interval[0] == float("inf"):
         bottom_range = "(inf, "
     else:
-        bottom_range = f"({int(interval[0])}, " if (interval[0] - _EPSILON).is_integer() else f"[{interval[0]}, "
+        bottom_range = (
+            f"({int(interval[0])}, "
+            if (interval[0] - _EPSILON).is_integer()
+            else f"[{interval[0]}, "
+        )
 
-    if interval[1] == float('inf'):
+    if interval[1] == float("inf"):
         top_range = "inf)"
     else:
-        top_range = f"{int(interval[1] - _EPSILON)})" if (interval[1] + _EPSILON).is_integer() else f"{interval[1]}]"
+        top_range = (
+            f"{int(interval[1] - _EPSILON)})"
+            if (interval[1] + _EPSILON).is_integer()
+            else f"{interval[1]}]"
+        )
 
     return bottom_range + top_range
 
+
 def _safe_div(dividend: float, divisor: float) -> float:
     """
     Float division, with infinity returned if dividing by 0
     Args:
         dividend (float): float being divided
         divisor (float): float dividing
 
     Returns:
         float: Result of regular division, or infinity if the divisor is 0
     """
     if divisor == 0:
         return copysign(float("inf"), dividend)
     return dividend / divisor
 
+
 def _safe_min(args: Iterable[float]) -> float:
     """
     Calculate the minimum of an iterable, without returning nan
     Args:
         args (Iterable[float]): iterable for which to find a minimum
 
     Returns:
         float: minimum of args, ignoring nan
     """
     filtered_args = (arg for arg in args if not isnan(arg))
     return min(filtered_args)
 
+
 def _safe_max(args: Iterable[float]) -> float:
     """
     Calculate the maximum of an iterable, without returning nan
     Args:
         args (Iterable[float]): iterable for which to find a maximum
 
     Returns:
         float: maximum of args, ignoring nan
     """
     filtered_args = (arg for arg in args if not isnan(arg))
     return max(filtered_args)
 
-def physical_range_division(prange_a: tuple[float, float], prange_b: tuple[float, float]) -> tuple[float, float]:
+
+def physical_range_division(
+    prange_a: tuple[float, float], prange_b: tuple[float, float]
+) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a / b
     Args:
         prange_a (tuple[float, float]): physical range of 'a'
         prange_b (tuple[float, float]): physical range of 'b'
 
     Returns:
         tuple[float, float]: physical range of 'a / b'
     """
-    range_combinations = (_safe_div(prange_a[0], prange_b[0]), _safe_div(prange_a[0], prange_b[1]),
-                          _safe_div(prange_a[1], prange_b[0]), _safe_div(prange_a[1], prange_b[1]))
+    range_combinations = (
+        _safe_div(prange_a[0], prange_b[0]),
+        _safe_div(prange_a[0], prange_b[1]),
+        _safe_div(prange_a[1], prange_b[0]),
+        _safe_div(prange_a[1], prange_b[1]),
+    )
     if prange_b[0] <= 0 <= prange_b[1]:
-        range_combinations = (*range_combinations,
-                               copysign(float("inf"), prange_a[0]), copysign(float("inf"), prange_a[1]))
+        range_combinations = (
+            *range_combinations,
+            copysign(float("inf"), prange_a[0]),
+            copysign(float("inf"), prange_a[1]),
+        )
     return (_safe_min(range_combinations), _safe_max(range_combinations))
 
-def physical_range_multiplication(prange_a: tuple[float, float], prange_b: tuple[float, float]) -> tuple[float, float]:
+
+def physical_range_multiplication(
+    prange_a: tuple[float, float], prange_b: tuple[float, float]
+) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a * b
     Args:
         prange_a (tuple[float, float]): physical range of 'a'
         prange_b (tuple[float, float]): physical range of 'b'
 
     Returns:
         tuple[float, float]: physical range of 'a * b'
     """
-    range_combinations = (prange_a[0] * prange_b[0], prange_a[0] * prange_b[1],
-                          prange_a[1] * prange_b[0], prange_a[1] * prange_b[1])
+    range_combinations = (
+        prange_a[0] * prange_b[0],
+        prange_a[0] * prange_b[1],
+        prange_a[1] * prange_b[0],
+        prange_a[1] * prange_b[1],
+    )
     return (_safe_min(range_combinations), _safe_max(range_combinations))
 
-def physical_range_power(prange: tuple[float, float], power: int) -> tuple[float, float]:
+
+def physical_range_power(
+    prange: tuple[float, float], power: int
+) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a ** n
     Args:
         prange (tuple[float, float]): physical range of 'a'
         power (int): exponentiating power
 
@@ -189,39 +224,45 @@
         tuple[float, float]: physical range of 'a ** n'
     """
     if power % 2 == 0:
         if prange[0] <= 0 and prange[1] <= 0:
             return (prange[1] ** power, prange[0] ** power)
 
         if prange[0] <= 0 <= prange[1]:
-            return (prange[0] * prange[1] ** power if prange[0] < 0 else 0,
-                    prange[1] ** power)
+            return (
+                prange[0] * prange[1] ** power if prange[0] < 0 else 0,
+                prange[1] ** power,
+            )
     else:
         if prange[0] <= 0 and prange[1] <= 0:
             return (prange[0] ** power, prange[1] ** power)
 
         if prange[0] <= 0 <= prange[1]:
             max_power = max(abs(prange[0]), prange[1]) ** (power - 1)
-            return (prange[0] * max_power if prange[0] < 0 else 0,
-                    prange[1] * max_power)
+            return (
+                prange[0] * max_power if prange[0] < 0 else 0,
+                prange[1] * max_power,
+            )
 
     # prange[0] >= 0 here
     return (prange[0] ** power, prange[1] ** power)
 
+
 def exponent_unicode(exponent: int) -> str:
     """
     Get the unicode superscript of an integer
     Args:
         exponent (int): integer exponent
 
     Returns:
         str: exponent unicode
     """
     return "".join(_UNICODE_DIGITS[digit] for digit in str(exponent))
 
+
 def map_dictionary_value(
     function: Callable[[U], V], dictionary: dict[T, U]
 ) -> dict[T, V]:
     """Map a function over the values of a dictionary
 
     Args:
         function (Callable[[U], V]): Mapping function
```

