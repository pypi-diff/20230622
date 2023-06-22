# Comparing `tmp/pymolecule_parser-0.0.2.tar.gz` & `tmp/pymolecule_parser-0.1.0.tar.gz`

## Comparing `pymolecule_parser-0.0.2.tar` & `pymolecule_parser-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/main.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/src/pymolecule_parser/__about__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/src/pymolecule_parser/__init__.py
--rwxr-xr-x   0        0        0     6993 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/src/pymolecule_parser/pymolecule_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/tests/unit_test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/LICENSE
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/README.md
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/workflows/reusable_test.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/src/pymolecule_parser/__about__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/src/pymolecule_parser/__init__.py
+-rwxr-xr-x   0        0        0     8766 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/src/pymolecule_parser/pymolecule_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/tests/unit_test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/README.md
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 pymolecule_parser-0.1.0/PKG-INFO
```

### Comparing `pymolecule_parser-0.0.2/src/pymolecule_parser/pymolecule_parser.py` & `pymolecule_parser-0.1.0/src/pymolecule_parser/pymolecule_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 #!/usr/bin/env python3
 
 import re
 from collections import defaultdict
 
 
-def parse(molecule_str: "str") -> "dict[str, int]":
+def parse(molecule_str: str, strict_mode: bool = False) -> "dict[str, int]":
     """
     Parse the molecule input and return the Atoms object.
 
+    args:
+        molecule_str: str - The molecule string.
+        strict_mode: bool - If True, the molecule string is parsed strictly.
+    return:
+        dict[str, int] - The dictionary of the molecule. The key is the element symbol and the value is the number of atoms.
+
     digit_exclude_zero ::= '1', '2', '3', '4', '5', '6', '7', '8', '9'
     digit ::= '0' | digit_exclude_zero
     natural_number ::= digit_exclude_zero, {digit}
-    atom ::= 'H' | 'He' | 'Li' | 'Be' | 'B' | 'C' | 'N' | 'O' | 'F' | 'Ne' | ... | 'Rg'
+    atom ::= 'H' | 'He' | 'Li' | 'Be' | 'B' | 'C' | 'N' | 'O' | 'F' | 'Ne' | ... | 'Og' (strict_mode=True)
+    atom ::= '[A-Z][a-z]*' (strict_mode=False)
     atom_number ::= { atom, natural_number }
     bra ::= '(' | '[' | '{'
     ket ::= ')' | ']' | '}'
     nests ::= bra, { nests | atom_number }, ket, [natural_number]
     molecule ::= [natural_number], nests | atom_number
     """
 
@@ -46,21 +53,43 @@
             res += tmp
         if res == "":
             return 1
         return int(res)
 
     def atom(string: str) -> str:
         global parser_idx
-        if parser_idx + 2 <= len(string) and string[parser_idx : parser_idx + 2] in elements:
-            parser_idx += 2
-            return string[parser_idx - 2 : parser_idx]
-        elif parser_idx + 1 <= len(string) and string[parser_idx] in elements:
-            parser_idx += 1
-            return string[parser_idx - 1]
-        return ""
+        if strict_mode:
+            if parser_idx + 2 <= len(string) and string[parser_idx : parser_idx + 2] in elements:
+                parser_idx += 2
+                return string[parser_idx - 2 : parser_idx]
+            elif parser_idx + 1 <= len(string) and string[parser_idx] in elements:
+                parser_idx += 1
+                return string[parser_idx - 1]
+            else:
+                re_invalid = re.compile(r"[A-Za-z]+")
+                invalid_match = re.match(re_invalid, string[parser_idx:])
+                if invalid_match is not None:
+                    raise ValueError(f"Error: Parse error. The atom is not in H-Og. invalid atom: {invalid_match.group()}. your argument: {string}. Please check your argument.")
+                else:
+                    return ""
+        else:  # strict_mode=False
+            # Non-strict mode: non-atomic symbols are allowed (e.g.) Xyz, Abc, etc.
+            # atom ::= '[A-Z][a-z]*'
+            re_atom = re.compile(r"[A-Z][a-z]*")
+            atom_match = re.match(re_atom, string[parser_idx:])
+            # invalid atom ::= '[a-z]+' (e.g.) c, abc, xyz, etc.
+            re_invalid = re.compile(r"[a-z]+")
+            invalid_match = re.match(re_invalid, string[parser_idx:])
+            if atom_match is None:
+                if invalid_match is not None:  # Start with lowercase letter, invalid atom
+                    raise ValueError(f"Error: Parse error. The atom is not in regex ([A-Z][a-z]*). invalid atom: {invalid_match.group()}. your argument: {string}. Please check your argument.")
+                else:  # No atom
+                    return ""
+            parser_idx += atom_match.end()
+            return atom_match.group()
 
     def atom_number(string: str) -> "defaultdict[str, int]":
         # atom_number: { atom, natural_number }
         res: defaultdict[str, int] = defaultdict(int)
         while True:
             atom_str = atom(string)
             atom_num = natural_number(string)
@@ -153,9 +182,9 @@
     molecule_str = molecule_str.replace(" ", "")  # remove all spaces
     # special characters [-=≡] are removed
     molecule_str = re.sub(r"[-=≡]", "", molecule_str)
     global parser_idx
     parser_idx = 0
     bra_list = ["(", "[", "{"]
     ket_list = [")", "]", "}"]
-    elements: "list[str]" = ["H", "He", "Li", "Be", "B", "C", "N", "O", "F", "Ne", "Na", "Mg", "Al", "Si", "P", "S", "Cl", "Ar", "K", "Ca", "Sc", "Ti", "V", "Cr", "Mn", "Fe", "Co", "Ni", "Cu", "Zn", "Ga", "Ge", "As", "Se", "Br", "Kr", "Rb", "Sr", "Y", "Zr", "Nb", "Mo", "Tc", "Ru", "Rh", "Pd", "Ag", "Cd", "In", "Sn", "Sb", "Te", "I", "Xe", "Cs", "Ba", "La", "Ce", "Pr", "Nd", "Pm", "Sm", "Eu", "Gd", "Tb", "Dy", "Ho", "Er", "Tm", "Yb", "Lu", "Hf", "Ta", "W", "Re", "Os", "Ir", "Pt", "Au", "Hg", "Tl", "Pb", "Bi", "Po", "At", "Rn", "Fr", "Ra", "Ac", "Th", "Pa", "U", "Np", "Pu", "Am", "Cm", "Bk", "Cf", "Es", "Fm", "Md", "No", "Lr", "Rf", "Db", "Sg", "Bh", "Hs", "Mt", "Ds", "Rg"]
+    elements: "list[str]" = ["H", "He", "Li", "Be", "B", "C", "N", "O", "F", "Ne", "Na", "Mg", "Al", "Si", "P", "S", "Cl", "Ar", "K", "Ca", "Sc", "Ti", "V", "Cr", "Mn", "Fe", "Co", "Ni", "Cu", "Zn", "Ga", "Ge", "As", "Se", "Br", "Kr", "Rb", "Sr", "Y", "Zr", "Nb", "Mo", "Tc", "Ru", "Rh", "Pd", "Ag", "Cd", "In", "Sn", "Sb", "Te", "I", "Xe", "Cs", "Ba", "La", "Ce", "Pr", "Nd", "Pm", "Sm", "Eu", "Gd", "Tb", "Dy", "Ho", "Er", "Tm", "Yb", "Lu", "Hf", "Ta", "W", "Re", "Os", "Ir", "Pt", "Au", "Hg", "Tl", "Pb", "Bi", "Po", "At", "Rn", "Fr", "Ra", "Ac", "Th", "Pa", "U", "Np", "Pu", "Am", "Cm", "Bk", "Cf", "Es", "Fm", "Md", "No", "Lr", "Rf", "Db", "Sg", "Bh", "Hs", "Mt", "Ds", "Rg", "Cn", "Nh", "Fl", "Mc", "Lv", "Ts", "Og"]
     return molecule(molecule_str)
```

### Comparing `pymolecule_parser-0.0.2/.gitignore` & `pymolecule_parser-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.2/LICENSE` & `pymolecule_parser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.2/pyproject.toml` & `pymolecule_parser-0.1.0/pyproject.toml`

 * *Files identical despite different names*

