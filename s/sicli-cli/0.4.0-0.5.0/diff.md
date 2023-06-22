# Comparing `tmp/sicli_cli-0.4.0.tar.gz` & `tmp/sicli_cli-0.5.0.tar.gz`

## Comparing `sicli_cli-0.4.0.tar` & `sicli_cli-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/examples/congrat.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/exceptions.py
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/main.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/types.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/sicli/utils.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/tests/test_main.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/LICENSE
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/README.md
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 sicli_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/examples/congrat.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/__about__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/argument.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/exceptions.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/main.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/types.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/sicli/utils.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/tests/test_main.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 sicli_cli-0.5.0/PKG-INFO
```

### Comparing `sicli_cli-0.4.0/examples/congrat.py` & `sicli_cli-0.5.0/examples/congrat.py`

 * *Files identical despite different names*

### Comparing `sicli_cli-0.4.0/sicli/main.py` & `sicli_cli-0.5.0/sicli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sys
 from argparse import ArgumentParser
 from collections.abc import Iterable, Sequence
 from typing import Any, Literal, Annotated, Tuple, Union, List
 from enum import Enum
+from dataclasses import asdict
 import inspect
 from sicli.utils import (
     isgeneric,
     unwrap_generic_alias,
     get_signature,
     snake_to_lower_kebab_case,
     lenient_issubclass,
 )
 from sicli.types import AnyCallable
 from sicli.exceptions import SicliException
+from sicli.argument import Arg
 
 
 class Sicli:
     """Wrapper for parser that can parse function signatures."""
 
     _parser: ArgumentParser
 
@@ -86,15 +88,15 @@
                 # we do it only for options because argparse is raising
                 # `'required' is an invalid argument for positionals`
                 kwargs = {"required": True} | kwargs
 
             if (
                 kwargs.get("default") is not None
                 and kwargs.get("nargs") != "*"
-                and not kwargs.get("action") == "store_true"
+                and kwargs.get("action") != "store_true"
             ):
                 # Always respect the existence of default value
                 # (except when flag and when multiple arguments)
                 kwargs = {"nargs": "?"} | kwargs
 
             param_name = param.name
 
@@ -118,53 +120,60 @@
         """Unwrap type, help, args and kwargs from `Annotated`."""
 
         origin, args = unwrap_generic_alias(type_annotation)
 
         if origin is not Annotated:
             return type_annotation, [], {}
 
-        type_ = args[0]
+        args = list(args)
+        type_ = args.pop(0)
         varargs = []
         kwargs = {}
 
         for arg in args:
             if isinstance(arg, str):
                 kwargs["help"] = arg
             elif isinstance(arg, list):
                 varargs.extend(arg)
-            elif isinstance(arg, dict):
-                kwargs |= arg
+            elif isinstance(arg, Arg):
+                override_kwargs = {k: v for (k, v) in asdict(arg).items() if v is not None}
+                kwargs |= override_kwargs
+            else:
+                raise SicliException(
+                    f"`Annotated` arguments after the first one must be values of"
+                    "type `str`, `list`, or `sicli.Arg`, got {arg} instead"
+                )
 
         return type_, varargs, kwargs
 
     def _add_single_command(self, function: AnyCallable) -> None:
         parser = self._parser
         self._consume_function(function, parser)
-        parser.set_defaults(__function=function)
+        parser.set_defaults(__sicli_function=function)
 
     def _add_multiple_commands(self, functions: Iterable[AnyCallable]) -> None:
         subparsers = self._parser.add_subparsers()
         for function in functions:
             parser = subparsers.add_parser(
                 snake_to_lower_kebab_case(function.__name__),
                 help=inspect.getdoc(function) or None,
             )
             self._consume_function(function, parser)
-            parser.set_defaults(__function=function)
+            parser.set_defaults(__sicli_function=function)
 
     def add_commands(self, functions: AnyCallable | Iterable[AnyCallable]) -> None:
         if isinstance(functions, Iterable):
             self._add_multiple_commands(functions)
         else:
             self._add_single_command(functions)
 
     def __call__(self, args: list[str] | None = None) -> Any:
         parsed_args = self._parser.parse_args(args)
         kwargs = vars(parsed_args)
-        function: AnyCallable | None = kwargs.pop("__function", None)
+        function: AnyCallable | None = kwargs.pop("__sicli_function", None)
         if function is None:
             self._parser.print_help()
             sys.exit()
         return function(**kwargs)
 
 
 def run(
```

### Comparing `sicli_cli-0.4.0/sicli/utils.py` & `sicli_cli-0.5.0/sicli/utils.py`

 * *Files identical despite different names*

### Comparing `sicli_cli-0.4.0/tests/test_main.py` & `sicli_cli-0.5.0/tests/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections.abc import Iterable, Sequence
 from typing import Annotated, List, Literal
 from sicli import run
 import pytest
+from sicli.argument import Arg
 
 
 def test_basic():
     def f(x: str):
         return x
 
     assert run(f, ["a"]) == "a"
@@ -93,28 +94,36 @@
         assert run(f, ["--x", "NaN"])
 
 
 def test_annotated_wrapped_type():
     def f(
         x: Annotated[int, "help for x"],
         *,
-        y: Annotated[Literal[3, 4], "help for y", {}] = 3,
+        y: Annotated[Literal[3, 4], "help for y"] = 3,
     ):
         return x, y
 
     assert run(f, ["1", "--y", "4"]) == (1, 4)
 
 
 def test_annotated_name_override():
     def f(*, x: Annotated[int, ["-n", "--number"]]):
         return x
 
     assert run(f, ["-n", "34"]) == 34
     assert run(f, ["--number", "34"]) == 34
 
+def test_annotated_kwrags_override():
+    def f(*, x: Annotated[list[int], Arg(help="help", type=lambda _: 1, nargs=2)]):
+        return x
+
+    assert run(f, ["--x", "4", "2"]) == [1, 1]
+
+    with pytest.raises(SystemExit):
+        run(f, ["--x", "1"])
 
 def test_subcommands():
     def sub_1(*, x: int):
         return x
 
     def sub_2(*, y: int):
         return y
```

### Comparing `sicli_cli-0.4.0/.gitignore` & `sicli_cli-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sicli_cli-0.4.0/LICENSE` & `sicli_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sicli_cli-0.4.0/README.md` & `sicli_cli-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -106,34 +106,34 @@
 - Keyword-only arguments (after `*`) are mapped to options.
 
 ### Default values
 Default values for both types of arguments are mapped, as your intuition would suggest, to default arguments in CLI. For flags, default value is always `False` and don't have to be set.
 
 ### Types
 
-#### `typing.Annotated[T, help, args, kwargs]`
+#### `typing.Annotated[T, ...]`
 `Annotated` in Python is the way to store metadata inside a valid type.
-So, `sicli` uses
-- first argument as the type and does whatever would be done with it
+So, `sicli` the following metadata
+- first argument as the type and does whatever would be done with it without `Annotated` wrapper.
 - argument of type `str` as help for this argument. 
 - argument of type `list` as names for argument. 
-- argument of type `dict` to merge it with `*kwargs` for `argparse.ArgumentParser.add_argument` (see `argparse` docs).
+- argument of `sici.Arg` dataclass will be merged with `*kwargs` for `argparse.ArgumentParser.add_argument` (see `argparse` docs).
 
 Example:
 ```python
 
 >>> import sicli
 >>> from typing import Annotated as Ann
 >>> def divide(
 ...     *,
 ...     numbers: Ann[
 ...         list[int],
 ...         "Numbers to divide",
 ...         ["+n", "+numbers"],
-...         {"nargs": 2},
+...         sicli.Arg(nargs=2),
 ...     ],
 ... ):
 ...     print(numbers[0] / numbers[1])
 ... 
 >>> sicli.run(divide, ["+numbers", "1", "2"], prefix_chars="-+")
 0.5
 
@@ -159,24 +159,24 @@
 #### `bool`
 `bool` is interpreted as flag. Its default value is always `False` and shouldn't be set.
 
 #### Other types
 Any other primitive type that you would pass to `type` argument in `argparse.ArgumentParser.add_argument` would work. For instance, `int`, `str`, `Path`.
 
 #### Overriding types
-You can use `dict` in `Annotated` to override type for `argparse.ArgumentParser.add_argument`:
+You can override type for `argparse.ArgumentParser.add_argument`:
 ```python
 def example(
-    s: Annotated[str, {"type": ascii}],
+    s: Annotated[str, sicli.Arg(type=ascii)],
 ):
 ```
 You could've used `ascii` directly as type annotation here if you don't care that your type checker will complain.
 
 #### Limitations
-Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3], {}]]`). Only `Annotated` can wrap other generic types.
+Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3]]]`). Only `Annotated` can wrap other generic types.
 
 ## Requirements
 No dependencies are needed, only pure Python ≥ `3.10`.
 
 ## Installation
 Install from PyPI:
 ```
```

### Comparing `sicli_cli-0.4.0/pyproject.toml` & `sicli_cli-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sicli_cli-0.4.0/PKG-INFO` & `sicli_cli-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sicli-cli
-Version: 0.4.0
+Version: 0.5.0
 Summary: Build simple command line tools easily and declaratively
 Project-URL: Documentation, https://github.com/unknown/sicli#readme
 Project-URL: Issues, https://github.com/immanelg/sicli/issues
 Project-URL: Source, https://github.com/immanelg/sicli
 Author: immanelg
 License-Expression: MIT
 License-File: LICENSE
@@ -124,34 +124,34 @@
 - Keyword-only arguments (after `*`) are mapped to options.
 
 ### Default values
 Default values for both types of arguments are mapped, as your intuition would suggest, to default arguments in CLI. For flags, default value is always `False` and don't have to be set.
 
 ### Types
 
-#### `typing.Annotated[T, help, args, kwargs]`
+#### `typing.Annotated[T, ...]`
 `Annotated` in Python is the way to store metadata inside a valid type.
-So, `sicli` uses
-- first argument as the type and does whatever would be done with it
+So, `sicli` the following metadata
+- first argument as the type and does whatever would be done with it without `Annotated` wrapper.
 - argument of type `str` as help for this argument. 
 - argument of type `list` as names for argument. 
-- argument of type `dict` to merge it with `*kwargs` for `argparse.ArgumentParser.add_argument` (see `argparse` docs).
+- argument of `sici.Arg` dataclass will be merged with `*kwargs` for `argparse.ArgumentParser.add_argument` (see `argparse` docs).
 
 Example:
 ```python
 
 >>> import sicli
 >>> from typing import Annotated as Ann
 >>> def divide(
 ...     *,
 ...     numbers: Ann[
 ...         list[int],
 ...         "Numbers to divide",
 ...         ["+n", "+numbers"],
-...         {"nargs": 2},
+...         sicli.Arg(nargs=2),
 ...     ],
 ... ):
 ...     print(numbers[0] / numbers[1])
 ... 
 >>> sicli.run(divide, ["+numbers", "1", "2"], prefix_chars="-+")
 0.5
 
@@ -177,24 +177,24 @@
 #### `bool`
 `bool` is interpreted as flag. Its default value is always `False` and shouldn't be set.
 
 #### Other types
 Any other primitive type that you would pass to `type` argument in `argparse.ArgumentParser.add_argument` would work. For instance, `int`, `str`, `Path`.
 
 #### Overriding types
-You can use `dict` in `Annotated` to override type for `argparse.ArgumentParser.add_argument`:
+You can override type for `argparse.ArgumentParser.add_argument`:
 ```python
 def example(
-    s: Annotated[str, {"type": ascii}],
+    s: Annotated[str, sicli.Arg(type=ascii)],
 ):
 ```
 You could've used `ascii` directly as type annotation here if you don't care that your type checker will complain.
 
 #### Limitations
-Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3], {}]]`). Only `Annotated` can wrap other generic types.
+Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3]]]`). Only `Annotated` can wrap other generic types.
 
 ## Requirements
 No dependencies are needed, only pure Python ≥ `3.10`.
 
 ## Installation
 Install from PyPI:
 ```
```

