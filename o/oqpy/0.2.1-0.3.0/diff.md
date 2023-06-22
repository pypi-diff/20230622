# Comparing `tmp/oqpy-0.2.1.tar.gz` & `tmp/oqpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqpy-0.2.1.tar", max compression
+gzip compressed data, was "oqpy-0.3.0.tar", max compression
```

## Comparing `oqpy-0.2.1.tar` & `oqpy-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1510 2022-11-27 03:24:43.621227 oqpy-0.2.1/CITATION.cff
--rw-r--r--   0        0        0    11328 2022-10-20 16:34:51.863893 oqpy-0.2.1/LICENSE
--rw-r--r--   0        0        0       71 2022-10-20 16:34:51.864132 oqpy-0.2.1/NOTICE
--rw-r--r--   0        0        0     6362 2022-11-27 03:24:43.621961 oqpy-0.2.1/README.md
--rw-r--r--   0        0        0     1011 2023-05-18 15:19:04.171749 oqpy-0.2.1/oqpy/__init__.py
--rw-r--r--   0        0        0    13022 2023-05-18 14:52:02.896855 oqpy-0.2.1/oqpy/base.py
--rw-r--r--   0        0        0    13752 2023-05-18 14:52:02.897245 oqpy-0.2.1/oqpy/classical_types.py
--rw-r--r--   0        0        0     4826 2023-05-18 14:52:02.897582 oqpy-0.2.1/oqpy/control_flow.py
--rw-r--r--   0        0        0    22811 2023-05-18 14:52:02.897986 oqpy-0.2.1/oqpy/program.py
--rw-r--r--   0        0        0     2702 2023-05-18 14:52:02.898331 oqpy-0.2.1/oqpy/pulse.py
--rw-r--r--   0        0        0     4435 2023-05-18 14:52:02.898659 oqpy-0.2.1/oqpy/quantum_types.py
--rw-r--r--   0        0        0     8321 2023-05-18 14:52:02.898997 oqpy-0.2.1/oqpy/subroutines.py
--rw-r--r--   0        0        0     2506 2022-10-20 16:34:51.866749 oqpy-0.2.1/oqpy/timing.py
--rw-r--r--   0        0        0     3670 2023-05-18 15:19:04.172581 oqpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 oqpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1957 2023-06-20 21:22:31.425953 oqpy-0.3.0/CITATION.cff
+-rw-r--r--   0        0        0    11328 2022-09-19 17:51:00.552588 oqpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0       71 2022-09-19 17:51:00.552909 oqpy-0.3.0/NOTICE
+-rw-r--r--   0        0        0     6506 2023-06-20 21:22:31.426565 oqpy-0.3.0/README.md
+-rw-r--r--   0        0        0     1011 2023-06-22 18:01:55.965412 oqpy-0.3.0/oqpy/__init__.py
+-rw-r--r--   0        0        0    21295 2023-06-22 18:01:55.966357 oqpy-0.3.0/oqpy/base.py
+-rw-r--r--   0        0        0    14289 2023-06-22 18:01:55.967309 oqpy-0.3.0/oqpy/classical_types.py
+-rw-r--r--   0        0        0     5472 2023-06-22 18:01:55.968896 oqpy-0.3.0/oqpy/control_flow.py
+-rw-r--r--   0        0        0    23815 2023-06-22 18:01:55.970221 oqpy-0.3.0/oqpy/program.py
+-rw-r--r--   0        0        0     2702 2023-06-20 21:40:48.272150 oqpy-0.3.0/oqpy/pulse.py
+-rw-r--r--   0        0        0     4435 2023-05-13 00:40:15.485776 oqpy-0.3.0/oqpy/quantum_types.py
+-rw-r--r--   0        0        0     8337 2023-06-22 18:01:55.971346 oqpy-0.3.0/oqpy/subroutines.py
+-rw-r--r--   0        0        0     3985 2023-06-22 18:01:55.972231 oqpy-0.3.0/oqpy/timing.py
+-rw-r--r--   0        0        0     3663 2023-06-22 18:01:55.973559 oqpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7945 1970-01-01 00:00:00.000000 oqpy-0.3.0/PKG-INFO
```

### Comparing `oqpy-0.2.1/CITATION.cff` & `oqpy-0.3.0/CITATION.cff`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,26 @@
     given-names: Jean-Christophe
     affiliation: "AWS Quantum Technologies"
     orcid: "https://orcid.org/0000-0002-3379-229X"
   - family-names: Chen
     given-names: Li
     affiliation: "AWS Center for Quantum Computing"
     orcid: "https://orcid.org/0000-0002-1700-7503"
+  - family-names: Thorgrimsson
+    given-names: Brandur
+    affiliation: "Atlantic Quantum"
+    orcid: "https://orcid.org/0000-0002-4491-1717"
+  - family-names: Mishra
+    given-names: Anurag
+    affiliation: "AWS Center for Quantum Computing"
+    orcid: "https://orcid.org/0000-0003-1325-4387"
+  - family-names: D'Ewart
+    given-names: Mitch
+    affiliation: "AWS Center for Quantum Computing"
+    orcid: "https://orcid.org/0000-0001-8916-560X"
   - family-names: Sivarajah
     given-names: Prasahnt
     affiliation: "AWS Center for Quantum Computing"
     orcid: "https://orcid.org/0000-0002-9383-8624"
   - family-names: Karalekas
     given-names: Peter
     affiliation: "AWS Center for Quantum Computing"
```

### Comparing `oqpy-0.2.1/LICENSE` & `oqpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oqpy-0.2.1/README.md` & `oqpy-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,16 @@
     }
 }
 ```
 
 ## Contributing
 
 We welcome contributions to OQpy including bug fixes, feature requests, etc. To get started, check
-out our [contributing guidelines](CONTRIBUTING.md).
+out our [contributing guidelines](CONTRIBUTING.md). Those who make a nontrivial contribution to the
+source code will be added as an author to the [`CITATION.cff`][citation-file] file (see below).
 
 ## Citation
 
 If you use OQpy in your work or research, please cite it using the metadata in the
 [`CITATION.cff`][citation-file] file in the repository (which includes a
 [Zenodo DOI][zenodo-doi]). You can copy the citation in BibTeX format using the
 ["Cite this repository" widget][citation-widget] in the About section of the
```

### Comparing `oqpy-0.2.1/oqpy/__init__.py` & `oqpy-0.3.0/oqpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 ############################################################################
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 from oqpy.classical_types import *
 from oqpy.control_flow import *
 from oqpy.program import *
 from oqpy.pulse import *
 from oqpy.quantum_types import *
 from oqpy.subroutines import *
 from oqpy.timing import *
```

### Comparing `oqpy-0.2.1/oqpy/classical_types.py` & `oqpy-0.3.0/oqpy/classical_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,19 @@
     OQPyExpression,
     Var,
     make_annotations,
     map_to_ast,
     optional_ast,
     to_ast,
 )
-from oqpy.timing import make_duration
+from oqpy.timing import convert_float_to_duration
 
 if TYPE_CHECKING:
+    from typing import Literal
+
     from oqpy.program import Program
 
 __all__ = [
     "pi",
     "ArrayVar",
     "BoolVar",
     "IntVar",
@@ -152,36 +154,36 @@
 
 
 class Identifier(OQPyExpression):
     """Base class to specify constant symbols."""
 
     name: str
 
-    def __init__(self, name: str) -> None:
-        self.type = None
+    def __init__(self, name: str, ast_type: ast.ClassicalType) -> None:
         self.name = name
+        self.type = ast_type
 
     def to_ast(self, program: Program) -> ast.Expression:
         return ast.Identifier(name=self.name)
 
 
-pi = Identifier(name="pi")
+pi = Identifier(name="pi", ast_type=ast.FloatType())
 
 
 class _ClassicalVar(Var, OQPyExpression):
     """Base type for variables with classical type.
 
     Subclasses should supply the type_cls class variable.
     """
 
     type_cls: Type[ast.ClassicalType]
 
     def __init__(
         self,
-        init_expression: AstConvertible | None = None,
+        init_expression: AstConvertible | Literal["input", "output"] | None = None,
         name: str | None = None,
         needs_declaration: bool = True,
         annotations: Sequence[str | tuple[str, str]] = (),
         **type_kwargs: Any,
     ):
         name = name or "".join([random.choice(string.ascii_letters) for _ in range(10)])
         super().__init__(name, needs_declaration=needs_declaration)
@@ -192,14 +194,18 @@
     def to_ast(self, program: Program) -> ast.Identifier:
         """Converts the OQpy variable into an ast node."""
         program._add_var(self)
         return ast.Identifier(self.name)
 
     def make_declaration_statement(self, program: Program) -> ast.Statement:
         """Make an ast statement that declares the OQpy variable."""
+        if isinstance(self.init_expression, str) and self.init_expression in ("input", "output"):
+            return ast.IODeclaration(
+                ast.IOKeyword[self.init_expression], self.type, self.to_ast(program)
+            )
         init_expression_ast = optional_ast(program, self.init_expression)
         stmt = ast.ClassicalDeclaration(self.type, self.to_ast(program), init_expression_ast)
         stmt.annotations = make_annotations(self.annotations)
         return stmt
 
 
 class BoolVar(_ClassicalVar):
@@ -291,41 +297,41 @@
     base_type: ast.FloatType = float64
 
     def __class_getitem__(cls, item: ast.FloatType) -> Callable[..., ComplexVar]:
         return functools.partial(cls, base_type=item)
 
     def __init__(
         self,
-        init_expression: AstConvertible | None = None,
+        init_expression: AstConvertible | Literal["input", "output"] | None = None,
         *args: Any,
         base_type: ast.FloatType = float64,
         **kwargs: Any,
     ) -> None:
         assert isinstance(base_type, ast.FloatType)
         self.base_type = base_type
 
-        if not isinstance(init_expression, (complex, type(None), OQPyExpression)):
+        if not isinstance(init_expression, (complex, type(None), str, OQPyExpression)):
             init_expression = complex(init_expression)  # type: ignore[arg-type]
         super().__init__(init_expression, *args, **kwargs, base_type=base_type)
 
 
 class DurationVar(_ClassicalVar):
     """An oqpy variable with duration type."""
 
     type_cls = ast.DurationType
 
     def __init__(
         self,
-        init_expression: AstConvertible | None = None,
+        init_expression: AstConvertible | Literal["input", "output"] | None = None,
         name: str | None = None,
         *args: Any,
         **type_kwargs: Any,
     ) -> None:
-        if init_expression is not None:
-            init_expression = make_duration(init_expression)
+        if init_expression is not None and not isinstance(init_expression, str):
+            init_expression = convert_float_to_duration(init_expression)
         super().__init__(init_expression, name, *args, **type_kwargs)
 
 
 class StretchVar(_ClassicalVar):
     """An oqpy variable with stretch type."""
 
     type_cls = ast.StretchType
@@ -370,16 +376,18 @@
             )
         elif isinstance(base_type_instance, ComplexVar):
             array_base_type = base_type_instance.type_cls(base_type=base_type_instance.base_type)
         else:
             array_base_type = base_type_instance.type_cls()
 
         # Automatically handle Duration array.
-        if base_type is DurationVar and kwargs["init_expression"]:
-            kwargs["init_expression"] = (make_duration(i) for i in kwargs["init_expression"])
+        if base_type is DurationVar and kwargs["init_expression"] is not None:
+            kwargs["init_expression"] = (
+                convert_float_to_duration(i) for i in kwargs["init_expression"]
+            )
 
         super().__init__(
             *args,
             **kwargs,
             dimensions=[ast.IntegerLiteral(dimension) for dimension in dimensions],
             base_type=array_base_type,
         )
```

### Comparing `oqpy-0.2.1/oqpy/control_flow.py` & `oqpy-0.3.0/oqpy/control_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 from oqpy.classical_types import (
     AstConvertible,
     DurationVar,
     IntVar,
     _ClassicalVar,
     convert_range,
 )
-from oqpy.timing import make_duration
+from oqpy.timing import convert_float_to_duration
 
 ClassicalVarT = TypeVar("ClassicalVarT", bound=_ClassicalVar)
 
 if TYPE_CHECKING:
     from oqpy.program import Program
 
 
-__all__ = ["If", "Else", "ForIn", "While"]
+__all__ = ["If", "Else", "ForIn", "While", "Range"]
 
 
 @contextlib.contextmanager
 def If(program: Program, condition: OQPyExpression) -> Iterator[None]:
     """Context manager for doing conditional evaluation.
 
     .. code-block:: python
@@ -122,29 +122,51 @@
 
     if isinstance(iterator, range):
         # A range can only be iterated over integers.
         assert identifier_type is IntVar, "A range can only be looped over an integer."
         set_declaration = convert_range(program, iterator)
     elif isinstance(iterator, Iterable):
         if identifier_type is DurationVar:
-            iterator = (make_duration(i) for i in iterator)
+            iterator = (convert_float_to_duration(i) for i in iterator)
 
         set_declaration = ast.DiscreteSet([to_ast(program, i) for i in iterator])
-    elif isinstance(iterator, _ClassicalVar):
-        set_declaration = to_ast(program, iterator)
-        assert isinstance(set_declaration, ast.Identifier), type(set_declaration)
     else:
-        raise TypeError(f"'{type(iterator)}' object is not iterable")
+        set_declaration = to_ast(program, iterator)
 
     stmt = ast.ForInLoop(
         identifier_type.type_cls(), var.to_ast(program), set_declaration, state.body
     )
     program._add_statement(stmt)
 
 
+class Range:
+    """AstConvertible which creates an integer range.
+
+    Unlike builtin python range, this allows the components to be AstConvertible,
+    instead of just int.
+    """
+
+    def __init__(self, start: AstConvertible, stop: AstConvertible, step: AstConvertible = 1):
+        self.start = start
+        self.stop = stop
+        self.step = step
+
+    def to_ast(self, program: Program) -> ast.Expression:
+        """Convert to an ast.RangeDefinition."""
+        return ast.RangeDefinition(
+            to_ast(program, self.start),
+            ast.BinaryExpression(
+                lhs=to_ast(program, self.stop),
+                op=ast.BinaryOperator["-"],
+                rhs=ast.IntegerLiteral(value=1),
+            ),
+            to_ast(program, self.step) if self.step != 1 else None,
+        )
+
+
 @contextlib.contextmanager
 def While(program: Program, condition: OQPyExpression) -> Iterator[None]:
     """Context manager for looping a repeating a portion of a program while a condition is True.
 
     .. code-block:: python
 
         i = IntVar(1)
```

### Comparing `oqpy-0.2.1/oqpy/program.py` & `oqpy-0.3.0/oqpy/program.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Var,
     expr_matches,
     map_to_ast,
     optional_ast,
     to_ast,
 )
 from oqpy.pulse import FrameVar, PortVar, WaveformVar
-from oqpy.timing import make_duration
+from oqpy.timing import convert_duration_to_float, convert_float_to_duration
 
 __all__ = ["Program"]
 
 
 class ProgramState:
     """Represents the current program state at a particular context level.
 
@@ -87,23 +87,26 @@
         self.finalize_if_clause()
         self.body.append(stmt)
 
 
 class Program:
     """A builder class for OpenQASM/OpenPulse programs."""
 
-    def __init__(self, version: Optional[str] = "3.0") -> None:
+    DURATION_MAX_DIGITS = 12
+
+    def __init__(self, version: Optional[str] = "3.0", simplify_constants: bool = True) -> None:
         self.stack: list[ProgramState] = [ProgramState()]
         self.defcals: dict[
             tuple[tuple[str, ...], str, tuple[str, ...]], ast.CalibrationDefinition
         ] = {}
         self.subroutines: dict[str, ast.SubroutineDefinition] = {}
         self.externs: dict[str, ast.ExternDeclaration] = {}
         self.declared_vars: dict[str, Var] = {}
         self.undeclared_vars: dict[str, Var] = {}
+        self.simplify_constants = simplify_constants
 
         if version is None or (
             len(version.split(".")) in [1, 2]
             and all([item.isnumeric() for item in version.split(".")])
         ):
             self.version = version
         else:
@@ -234,15 +237,15 @@
         openpulse_types = ast.PortType, ast.FrameType, ast.WaveformType
         for extern_statement in self.externs.values():
             for arg in extern_statement.arguments:
                 if isinstance(arg.type, openpulse_types):
                     openpulse_externs.append(extern_statement)
                     break
             else:
-                if isinstance(extern_statement.return_type.type, openpulse_types):
+                if isinstance(extern_statement.return_type, openpulse_types):
                     openpulse_externs.append(extern_statement)
                 else:
                     openqasm_externs.append(extern_statement)
         if openpulse_externs:
             openqasm_externs.append(ast.CalibrationStatement(body=openpulse_externs))
         return openqasm_externs
 
@@ -359,15 +362,15 @@
 
     def delay(
         self, time: AstConvertible, qubits_or_frames: AstConvertible | Iterable[AstConvertible] = ()
     ) -> Program:
         """Apply a delay to a set of qubits or frames."""
         if not isinstance(qubits_or_frames, Iterable):
             qubits_or_frames = [qubits_or_frames]
-        ast_duration = to_ast(self, make_duration(time))
+        ast_duration = to_ast(self, convert_float_to_duration(time))
         ast_qubits_or_frames = map_to_ast(self, qubits_or_frames)
         self._add_statement(ast.DelayInstruction(ast_duration, ast_qubits_or_frames))
         return self
 
     def barrier(self, qubits_or_frames: Iterable[AstConvertible]) -> Program:
         """Apply a barrier to a set of qubits or frames."""
         ast_qubits_or_frames = map_to_ast(self, qubits_or_frames)
@@ -388,40 +391,45 @@
     def capture(self, frame: AstConvertible, kernel: AstConvertible) -> Program:
         """Capture signal integrated against a kernel on a particular frame."""
         self.function_call("capture", [frame, kernel])
         return self
 
     def set_phase(self, frame: AstConvertible, phase: AstConvertible) -> Program:
         """Set the phase of a particular frame."""
-        self.function_call("set_phase", [frame, phase])
+        # We use make_float to force phase to be a unitless (i.e. non-duration) quantity.
+        # Users are expected to keep track the units that are not expressible in openqasm
+        # such as s^{-1}. For instance, in 2 * oqpy.pi * tppi * DurationVar(1e-8),
+        # tppi is a float but has a frequency unit. This will coerce the result type
+        # to a float by assuming the duration should be represented in seconds."
+        self.function_call("set_phase", [frame, convert_duration_to_float(phase)])
         return self
 
     def shift_phase(self, frame: AstConvertible, phase: AstConvertible) -> Program:
         """Shift the phase of a particular frame."""
-        self.function_call("shift_phase", [frame, phase])
+        self.function_call("shift_phase", [frame, convert_duration_to_float(phase)])
         return self
 
     def set_frequency(self, frame: AstConvertible, freq: AstConvertible) -> Program:
         """Set the frequency of a particular frame."""
-        self.function_call("set_frequency", [frame, freq])
+        self.function_call("set_frequency", [frame, convert_duration_to_float(freq)])
         return self
 
     def shift_frequency(self, frame: AstConvertible, freq: AstConvertible) -> Program:
         """Shift the frequency of a particular frame."""
-        self.function_call("shift_frequency", [frame, freq])
+        self.function_call("shift_frequency", [frame, convert_duration_to_float(freq)])
         return self
 
     def set_scale(self, frame: AstConvertible, scale: AstConvertible) -> Program:
         """Set the amplitude scaling of a particular frame."""
-        self.function_call("set_scale", [frame, scale])
+        self.function_call("set_scale", [frame, convert_duration_to_float(scale)])
         return self
 
     def shift_scale(self, frame: AstConvertible, scale: AstConvertible) -> Program:
         """Shift the amplitude scaling of a particular frame."""
-        self.function_call("shift_scale", [frame, scale])
+        self.function_call("shift_scale", [frame, convert_duration_to_float(scale)])
         return self
 
     def returns(self, expression: AstConvertible) -> Program:
         """Return a statement from a function definition or a defcal statement."""
         self._add_statement(ast.ReturnStatement(to_ast(self, expression)))
         return self
 
@@ -468,18 +476,22 @@
             raise RuntimeError("Pragmas must be global")
         self._add_statement(ast.Pragma(command))
         return self
 
     def _do_assignment(self, var: AstConvertible, op: str, value: AstConvertible) -> None:
         """Helper function for variable assignment operations."""
         if isinstance(var, classical_types.DurationVar):
-            value = make_duration(value)
+            value = convert_float_to_duration(value)
+        var_ast = to_ast(self, var)
+        if isinstance(var_ast, ast.IndexExpression):
+            assert isinstance(var_ast.collection, ast.Identifier)
+            var_ast = ast.IndexedIdentifier(name=var_ast.collection, indices=[var_ast.index])
         self._add_statement(
             ast.ClassicalAssignment(
-                to_ast(self, var),
+                var_ast,
                 ast.AssignmentOperator[op],
                 to_ast(self, value),
             )
         )
 
     def do_expression(self, expression: AstConvertible) -> Program:
         """Add a statement which evaluates a given expression without assigning the output."""
```

### Comparing `oqpy-0.2.1/oqpy/pulse.py` & `oqpy-0.3.0/oqpy/pulse.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.2.1/oqpy/quantum_types.py` & `oqpy-0.3.0/oqpy/quantum_types.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.2.1/oqpy/subroutines.py` & `oqpy-0.3.0/oqpy/subroutines.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from mypy_extensions import VarArg
 from openpulse import ast
 
 import oqpy.program
 from oqpy.base import AstConvertible, OQPyExpression, make_annotations, to_ast
 from oqpy.classical_types import OQFunctionCall, _ClassicalVar
 from oqpy.quantum_types import Qubit
-from oqpy.timing import make_duration
+from oqpy.timing import convert_float_to_duration
 
 __all__ = ["subroutine", "annotate_subroutine", "declare_extern", "declare_waveform_generator"]
 
 SubroutineParams = [oqpy.Program, VarArg(AstConvertible)]
 
 
 def subroutine(
@@ -102,15 +102,15 @@
             return_type = output.type
             body.append(ast.ReturnStatement(to_ast(inner_prog, output)))
         elif output is None:
             return_type = None
             if type_hints.get("return", False):
                 return_hint = type_hints["return"]()
                 if isinstance(return_hint, _ClassicalVar):
-                    return_type = return_hint
+                    return_type = return_hint.type
                 elif return_hint is not None:
                     raise ValueError(
                         f"Type hint for return variable on subroutine {name} is not an oqpy classical type."
                     )
         else:
             raise ValueError(
                 "Output type of subroutine {name} was neither oqpy expression nor None."
@@ -172,15 +172,15 @@
 
     """
     arg_names = list(zip(*(args)))[0]
     arg_types = list(zip(*(args)))[1]
     extern_decl = ast.ExternDeclaration(
         ast.Identifier(name),
         [ast.ExternArgument(type=t) for t in arg_types],
-        ast.ExternArgument(type=return_type),
+        return_type,
     )
     extern_decl.annotations = make_annotations(annotations)
 
     def call_extern(*call_args: AstConvertible, **call_kwargs: AstConvertible) -> OQFunctionCall:
         new_args = list(call_args) + [None] * len(call_kwargs)
 
         # Testing that the number of arguments is equal to what's defined by the prototype
@@ -196,22 +196,22 @@
             except ValueError:
                 raise TypeError(f"{name}() got an unexpected keyword argument '{k}'.")
 
             if k_idx < len(call_args):
                 raise TypeError(f"{name}() got multiple values for argument '{k}'.")
 
             if type(arg_types[k_idx]) == ast.DurationType:
-                new_args[k_idx] = make_duration(call_kwargs[k])
+                new_args[k_idx] = convert_float_to_duration(call_kwargs[k])
             else:
                 new_args[k_idx] = call_kwargs[k]
 
         # Casting floats into durations for the non-keyword arguments
         for i, a in enumerate(call_args):
             if type(arg_types[i]) == ast.DurationType:
-                new_args[i] = make_duration(a)
+                new_args[i] = convert_float_to_duration(a)
         return OQFunctionCall(name, new_args, return_type, extern_decl=extern_decl)
 
     return call_extern
 
 
 def declare_waveform_generator(
     name: str,
```

### Comparing `oqpy-0.2.1/pyproject.toml` & `oqpy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqpy"
-version = "0.2.1"
+version = "0.3.0"
 description = "Generating OpenQASM 3 + OpenPulse in Python"
 authors = ["OQpy Contributors <oqpy-contributors@amazon.com>"]
 license = "Apache-2.0"
 include = ["CITATION.cff", "NOTICE"]
 readme = "README.md"
 repository = "https://github.com/openqasm/oqpy"
 keywords = ["openqasm", "quantum"]
@@ -13,15 +13,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 # 0.4 loosens the antlr4-python3-runtime constraints
-openpulse = ">=0.4.1,<0.5.0"
+openpulse = ">=0.4.2"
 numpy = [
     {version = ">=1.14.5", python = ">=3.7,<3.8"},
     {version = ">=1.17.3", python = ">=3.8,<3.9"},
     {version = ">=1.19.3", python = ">=3.9,<3.10"},
     {version = ">=1.21.6", python = ">=3.10,<3.11"},
     {version = ">=1.22.0", python = ">=3.11"}
 ]
```

### Comparing `oqpy-0.2.1/PKG-INFO` & `oqpy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oqpy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generating OpenQASM 3 + OpenPulse in Python
 Home-page: https://github.com/openqasm/oqpy
 License: Apache-2.0
 Keywords: openqasm,quantum
 Author: OQpy Contributors
 Author-email: oqpy-contributors@amazon.com
 Requires-Python: >=3.7,<4.0
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: mypy-extensions (>=0.2.0)
 Requires-Dist: numpy (>=1.14.5) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: numpy (>=1.17.3) ; python_version >= "3.8" and python_version < "3.9"
 Requires-Dist: numpy (>=1.19.3) ; python_version >= "3.9" and python_version < "3.10"
 Requires-Dist: numpy (>=1.21.6) ; python_version >= "3.10" and python_version < "3.11"
 Requires-Dist: numpy (>=1.22.0) ; python_version >= "3.11"
-Requires-Dist: openpulse (>=0.4.1,<0.5.0)
+Requires-Dist: openpulse (>=0.4.2)
 Requires-Dist: typing-extensions (>=3.10.0.2) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/openqasm/oqpy
 Description-Content-Type: text/markdown
 
 # OQpy: Generating OpenQASM 3 + OpenPulse in Python
 
 The goal of `oqpy` ("ock-pie") is to make it easy to generate OpenQASM 3 + OpenPulse in Python. The
@@ -173,15 +173,16 @@
     }
 }
 ```
 
 ## Contributing
 
 We welcome contributions to OQpy including bug fixes, feature requests, etc. To get started, check
-out our [contributing guidelines](CONTRIBUTING.md).
+out our [contributing guidelines](CONTRIBUTING.md). Those who make a nontrivial contribution to the
+source code will be added as an author to the [`CITATION.cff`][citation-file] file (see below).
 
 ## Citation
 
 If you use OQpy in your work or research, please cite it using the metadata in the
 [`CITATION.cff`][citation-file] file in the repository (which includes a
 [Zenodo DOI][zenodo-doi]). You can copy the citation in BibTeX format using the
 ["Cite this repository" widget][citation-widget] in the About section of the
```

