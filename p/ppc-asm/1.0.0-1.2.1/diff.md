# Comparing `tmp/ppc-asm-1.0.0.tar.gz` & `tmp/ppc-asm-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ppc-asm/ppc-asm/dist/tmpg2fkampw/ppc-asm-1.0.0.tar", last modified: Thu Jun 16 14:32:26 2022, max compression
+gzip compressed data, was "/home/runner/work/ppc-asm/ppc-asm/dist/.tmp-yzft3iou/ppc-asm-1.2.1.tar", last modified: Thu Jun 22 01:32:19 2023, max compression
```

## Comparing `ppc-asm-1.0.0.tar` & `ppc-asm-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/ppc_asm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm/assembler/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/ppc_asm/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/ppc_asm/assembler/custom_ppc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19129 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/ppc_asm/assembler/ppc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/ppc_asm/dol_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-16 14:32:25.000000 ppc-asm-1.0.0/ppc_asm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-16 14:32:25.000000 ppc-asm-1.0.0/ppc_asm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:32:25.000000 ppc-asm-1.0.0/ppc_asm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/ppc_asm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:32:23.000000 ppc-asm-1.0.0/ppc_asm.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/requirements-setuptools.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:32:26.000000 ppc-asm-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/tests/test_custom_ppc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-06-16 14:32:10.000000 ppc-asm-1.0.0/tests/test_ppc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/src/ppc_asm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/src/ppc_asm/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/src/ppc_asm/assembler/custom_ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/src/ppc_asm/assembler/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/src/ppc_asm/dol_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/src/ppc_asm.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:32:19.000000 ppc-asm-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/tests/test_custom_ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-22 01:32:05.000000 ppc-asm-1.2.1/tests/test_ppc.py
```

### Comparing `ppc-asm-1.0.0/.gitignore` & `ppc-asm-1.2.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 # Pyre type checker
 .pyre/
 
 # PyCharm
 /.idea
 
 # Project files
-/ppc_asm/version.py
+/src/ppc_asm/version.py
```

### Comparing `ppc-asm-1.0.0/LICENSE` & `ppc-asm-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ppc-asm-1.0.0/PKG-INFO` & `ppc-asm-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ppc-asm
-Version: 1.0.0
+Version: 1.2.1
 Summary: "library for writing assembly for PowerPC, focused on Nintendo GameCube/Wii"
 Home-page: https://github.com/henriquegemignani/ppc-asm
 Author: Henrique Gemignani Passos Lima
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # ppc-asm
 
 This package provides allows one to easily modify existing Nintendo GameCube or Wii game executables.
```

### Comparing `ppc-asm-1.0.0/ppc_asm/assembler/custom_ppc.py` & `ppc-asm-1.2.1/src/ppc_asm/assembler/custom_ppc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Tuple, Dict
+import typing
 
 from ppc_asm.assembler import ppc
 
 
 class CompositeInstruction(ppc.BaseInstruction):
-    def __init__(self, instructions: Tuple[ppc.BaseInstruction, ...]):
+    def __init__(self, instructions: typing.Tuple[ppc.BaseInstruction, ...]):
         super().__init__()
         self.instructions = instructions
 
-    def bytes_for(self, address: int, symbols: Dict[str, int]):
+    def bytes_for(self, address: int, symbols: typing.Dict[str, int]):
         for instruction in self.instructions:
             yield from instruction.bytes_for(address, symbols=symbols)
             address += instruction.byte_count
 
     def __eq__(self, other):
         return isinstance(other, CompositeInstruction) and other.instructions == self.instructions
 
@@ -23,15 +23,15 @@
 
 class CurrentAddressInstruction(ppc.BaseInstruction):
     def __init__(self, output_register: ppc.GeneralRegister, offset: int):
         super().__init__()
         self.output_register = output_register
         self.offset = offset
 
-    def bytes_for(self, address: int, symbols: Dict[str, int]):
+    def bytes_for(self, address: int, symbols: typing.Dict[str, int]):
         return load_unsigned_32bit(self.output_register, address + self.offset).bytes_for(address, symbols=symbols)
 
     def __eq__(self, other):
         return (isinstance(other, CurrentAddressInstruction) and
                 (other.output_register, other.offset) == (self.output_register, self.offset))
 
     @property
```

### Comparing `ppc-asm-1.0.0/ppc_asm/assembler/ppc.py` & `ppc-asm-1.2.1/src/ppc_asm/assembler/ppc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import dataclasses as _dataclasses
 import struct as _struct
-from typing import Optional, Callable, Tuple, Dict, Union
+import typing as _typing
 
 
 def _pack(*args):
     return _struct.pack(*args)
 
 
-JumpTarget = Union[str, int]
+JumpTarget = _typing.Union[str, int]
 
 
 @_dataclasses.dataclass(frozen=True)
 class Register:
     number: int
 
 
@@ -24,29 +24,29 @@
 
 class FloatRegister(Register):
     def __repr__(self):
         return f"f{self.number}"
 
 
 class BaseInstruction:
-    label: Optional[str]
-    name: Optional[str] = None
+    label: str | None
+    name: str | None = None
 
     def __init__(self):
         self.label = None
 
     def with_label(self, label: str) -> BaseInstruction:
         self.label = label
         return self
 
     def with_name(self, name: str):
         self.name = name
         return self
 
-    def bytes_for(self, address: int, symbols: Dict[str, int]):
+    def bytes_for(self, address: int, symbols: dict[str, int]):
         raise NotImplementedError()
 
     def __eq__(self, other):
         raise NotImplementedError()
 
     @property
     def byte_count(self):
@@ -56,15 +56,15 @@
 class Instruction(BaseInstruction):
     value: int
 
     def __init__(self, value: int):
         super().__init__()
         self.value = value
 
-    def bytes_for(self, address: int, symbols: Dict[str, int]):
+    def bytes_for(self, address: int, symbols: dict[str, int]):
         return iter(_pack(">I", self.value))
 
     def __eq__(self, other):
         return isinstance(other, Instruction) and self.value == other.value
 
     def __repr__(self):
         if self.name is None:
@@ -72,15 +72,15 @@
         return f"<{self.name}>"
 
     @property
     def byte_count(self):
         return 4
 
     @classmethod
-    def compose(cls, data: Tuple[Tuple[int, int, bool], ...]):
+    def compose(cls, data: tuple[tuple[int, int, bool], ...]):
         value = 0
         bits_left = 32
         for item, bit_size, signed in data:
             bits_left -= bit_size
             if signed:
                 assert -(1 << (bit_size - 1)) <= item < (1 << (bit_size - 1))
                 if item < 0:
@@ -90,45 +90,45 @@
             value += item << bits_left
 
         assert bits_left == 0
         return cls(value)
 
 
 class AddressDependantInstruction(BaseInstruction):
-    def __init__(self, factory: Callable[[int], Tuple[Tuple[int, int, bool], ...]]):
+    def __init__(self, factory: _typing.Callable[[int], tuple[tuple[int, int, bool], ...]]):
         super().__init__()
         self.factory = factory
 
-    def bytes_for(self, address: int, symbols: Dict[str, int]):
+    def bytes_for(self, address: int, symbols: dict[str, int]):
         yield from Instruction.compose(self.factory(address)).bytes_for(address, symbols=symbols)
 
     def __eq__(self, other):
         return isinstance(other, AddressDependantInstruction) and self.factory == other.factory
 
     @property
     def byte_count(self):
         return 4
 
 
 class RelativeAddressInstruction(BaseInstruction):
     def __init__(self,
                  address_or_symbol: JumpTarget,
-                 factory: Callable[[int, int], Tuple[Tuple[int, int, bool], ...]]):
+                 factory: _typing.Callable[[int, int], tuple[tuple[int, int, bool], ...]]):
         super().__init__()
         self.address_or_symbol = address_or_symbol
         self.factory = factory
 
-    def concrete_instruction(self, instruction_address: int, symbols: Dict[str, int]) -> Instruction:
+    def concrete_instruction(self, instruction_address: int, symbols: dict[str, int]) -> Instruction:
         if isinstance(self.address_or_symbol, str):
             address = symbols[self.address_or_symbol]
         else:
             address = self.address_or_symbol
         return Instruction.compose(self.factory(address, instruction_address))
 
-    def bytes_for(self, instruction_address: int, symbols: Dict[str, int]):
+    def bytes_for(self, instruction_address: int, symbols: dict[str, int]):
         instruction = self.concrete_instruction(instruction_address, symbols=symbols)
         yield from instruction.bytes_for(instruction_address, symbols=symbols)
 
     def __eq__(self, other):
         return isinstance(other, RelativeAddressInstruction) and (self.factory == other.factory and
                                                                   self.address_or_symbol == other.address_or_symbol)
 
@@ -300,27 +300,27 @@
                                 (0, 3, False),
                                 (0, 1, False),
                                 (0, 1, False),
                                 (input_register.number, 5, False),
                                 (literal, 16, True)))
 
 
-def cmp(bf, l, ra: GeneralRegister, rb: GeneralRegister):
+def cmp(bf, unused, ra: GeneralRegister, rb: GeneralRegister):
     """
     https://www.ibm.com/support/knowledgecenter/ssw_aix_72/assembler/idalangref_cmp_instr.html
     :param bf: Specifies Condition Register Field 0-7 which indicates result of compare.
-    :param l: Must be set to 0 for the 32-bit subset architecture.
+    :param unused: Must be set to 0 for the 32-bit subset architecture.
     :param ra: Specifies source general-purpose register for operation.
     :param rb: Specifies source general-purpose register for operation.
     :return:
     """
     return Instruction.compose(((31, 6, False),
                                 (bf, 3, False),
                                 (0, 1, False),
-                                (l, 1, False),
+                                (unused, 1, False),
                                 (ra.number, 5, False),
                                 (rb.number, 5, False),
                                 (0, 10, False),
                                 (0, 1, False),
                                 ))
 
 
@@ -394,23 +394,41 @@
     jumps to the given address, if last comparison was a successful equality
     """
     bo = 12  # Branch if condition true (BO=12)
     bi = 2  # condition: equals
     return _conditional_branch(bo, bi, address_or_symbol, relative=relative)
 
 
+def bgt(address_or_symbol: JumpTarget, relative: bool = False):
+    """
+    jumps to the given address, if last comparison was a successful equality
+    """
+    bo = 12  # Branch if condition false (BO=4)
+    bi = 1  # condition: less than
+    return _conditional_branch(bo, bi, address_or_symbol, relative=relative)
+
+
 def bge(address_or_symbol: JumpTarget, relative: bool = False):
     """
     jumps to the given address, if last comparison was a successful equality
     """
     bo = 4  # Branch if condition false (BO=4)
     bi = 0  # condition: less than
     return _conditional_branch(bo, bi, address_or_symbol, relative=relative)
 
 
+def ble(address_or_symbol: JumpTarget, relative: bool = False):
+    """
+    jumps to the given address, if last comparison was a successful equality
+    """
+    bo = 4  # Branch if condition false (BO=4)
+    bi = 1  # condition: less than
+    return _conditional_branch(bo, bi, address_or_symbol, relative=relative)
+
+
 def bne(address_or_symbol: JumpTarget, relative: bool = False):
     """
     jumps to the given address, if last comparison was a successful equality
     """
     bo = 4  # Branch if condition false (BO=4)
     bi = 2  # condition: equals
     return _conditional_branch(bo, bi, address_or_symbol, relative=relative)
@@ -551,7 +569,14 @@
 
 def mfspr(output_register: GeneralRegister, special_register):
     """
     Move from Special-Purpose Register
     https://www.ibm.com/support/knowledgecenter/ssw_aix_72/assembler/idalangref_mfspr_spr_instrs.html
     """
     return _special_register_op(output_register, special_register, 339, 31)
+
+
+def mulli(output_register: GeneralRegister, input_register: GeneralRegister, literal: int):
+    return Instruction.compose(((7, 6, False),
+                                (output_register.number, 5, False),
+                                (input_register.number, 5, False),
+                                (literal, 16, True)))
```

### Comparing `ppc-asm-1.0.0/ppc_asm/dol_file.py` & `ppc-asm-1.2.1/src/ppc_asm/dol_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from __future__ import annotations
 
 import dataclasses
 import struct
 from pathlib import Path
-from typing import Tuple, Optional, BinaryIO, Iterable, List, Dict, Union
+from typing import BinaryIO, Iterable, Tuple, Union
 
 from ppc_asm import assembler
 
+__all__ = [
+    "Section",
+    "DolHeader",
+    "Symbol",
+    "DolEditor",
+    "DolFile"
+]
+
 _NUM_TEXT_SECTIONS = 7
 _NUM_DATA_SECTIONS = 11
 _NUM_SECTIONS = _NUM_TEXT_SECTIONS + _NUM_DATA_SECTIONS
 
 
 @dataclasses.dataclass(frozen=True)
 class Section:
     offset: int
     base_address: int
     size: int
 
 
 @dataclasses.dataclass(frozen=True)
 class DolHeader:
-    sections: Tuple[Section, ...]
+    sections: tuple[Section, ...]
     bss_address: int
     bss_size: int
     entry_point: int
 
     @classmethod
     def from_bytes(cls, data: bytes) -> DolHeader:
         struct_format = f">{_NUM_SECTIONS}L"
@@ -44,33 +52,33 @@
         args.extend(section.offset for section in self.sections)
         args.extend(section.base_address for section in self.sections)
         args.extend(section.size for section in self.sections)
         args.extend([self.bss_address, self.bss_size, self.entry_point])
 
         return struct.pack(f">{_NUM_SECTIONS}L{_NUM_SECTIONS}L{_NUM_SECTIONS}LLLL", *args) + (b"\x00" * 0x1C)
 
-    def section_for_address(self, address: int) -> Optional[Section]:
+    def section_for_address(self, address: int) -> Section | None:
         for section in self.sections:
             relative_to_base = address - section.base_address
             if 0 <= relative_to_base < section.size:
                 return section
 
-    def offset_for_address(self, address: int) -> Optional[int]:
+    def offset_for_address(self, address: int) -> int | None:
         section = self.section_for_address(address)
         if section is not None:
             return section.offset + (address - section.base_address)
         return None
 
 
 Symbol = Union[int, str, Tuple[str, int]]
 
 
 class DolEditor:
     header: DolHeader
-    symbols: Dict[str, int]
+    symbols: dict[str, int]
 
     def __init__(self, header: DolHeader):
         self.header = header
         self.symbols = {}
 
     def resolve_symbol(self, address_or_symbol: Symbol) -> int:
         if isinstance(address_or_symbol, tuple):
@@ -98,22 +106,22 @@
         return self._seek_and_read(offset, size)
 
     def write(self, address_or_symbol: Symbol, code_points: Iterable[int]):
         offset = self.offset_for_address(self.resolve_symbol(address_or_symbol))
         self._seek_and_write(offset, bytes(code_points))
 
     def write_instructions(self, address_or_symbol: Symbol,
-                           instructions: List[assembler.BaseInstruction]):
+                           instructions: list[assembler.BaseInstruction]):
         address = self.resolve_symbol(address_or_symbol)
         self.write(address, assembler.assemble_instructions(address, instructions, symbols=self.symbols))
 
 
 class DolFile(DolEditor):
-    symbols: Dict[str, int]
-    dol_file: Optional[BinaryIO] = None
+    symbols: dict[str, int]
+    dol_file: BinaryIO | None = None
     editable: bool = False
 
     def __init__(self, dol_path: Path):
         with dol_path.open("rb") as f:
             header_bytes = f.read(0x100)
 
         self.dol_path = dol_path
```

### Comparing `ppc-asm-1.0.0/ppc_asm.egg-info/PKG-INFO` & `ppc-asm-1.2.1/src/ppc_asm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ppc-asm
-Version: 1.0.0
+Version: 1.2.1
 Summary: "library for writing assembly for PowerPC, focused on Nintendo GameCube/Wii"
 Home-page: https://github.com/henriquegemignani/ppc-asm
 Author: Henrique Gemignani Passos Lima
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # ppc-asm
 
 This package provides allows one to easily modify existing Nintendo GameCube or Wii game executables.
```

### Comparing `ppc-asm-1.0.0/setup.cfg` & `ppc-asm-1.2.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -9,30 +9,29 @@
 	LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 zip_safe = True
-packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
-	pytest-asyncio
 	pytest-mock
 	mock>=4.0
+	pre-commit
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ppc-asm-1.0.0/tests/test_custom_ppc.py` & `ppc-asm-1.2.1/tests/test_custom_ppc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from ppc_asm import assembler
 from ppc_asm.assembler import custom_ppc, ppc
 
 
 @pytest.mark.parametrize("value", [-1, 0x100000000])
 def test_load_unsigned_32bit_invalid(value):
     with pytest.raises(AssertionError):
```

### Comparing `ppc-asm-1.0.0/tests/test_ppc.py` & `ppc-asm-1.2.1/tests/test_ppc.py`

 * *Files identical despite different names*

