# Comparing `tmp/statute_utils-0.3.0.tar.gz` & `tmp/statute_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.3.0.tar", max compression
+gzip compressed data, was "statute_utils-0.3.1.tar", max compression
```

## Comparing `statute_utils-0.3.0.tar` & `statute_utils-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.3.0/README.md
--rw-r--r--   0        0        0     1452 2023-06-22 05:28:27.920655 statute_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      372 2023-06-22 05:28:27.920807 statute_utils-0.3.0/statute_utils/__init__.py
--rw-r--r--   0        0        0     2593 2023-06-22 05:28:27.920932 statute_utils-0.3.0/statute_utils/__main__.py
--rw-r--r--   0        0        0      319 2023-06-22 05:28:27.921068 statute_utils-0.3.0/statute_utils/components/__init__.py
--rw-r--r--   0        0        0    10097 2023-06-22 05:28:27.921249 statute_utils-0.3.0/statute_utils/components/category.py
--rw-r--r--   0        0        0     3528 2023-06-22 05:28:27.921378 statute_utils-0.3.0/statute_utils/components/details.py
--rw-r--r--   0        0        0     4611 2023-06-22 05:28:27.921524 statute_utils-0.3.0/statute_utils/components/rule.py
--rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.3.0/statute_utils/components/short.py
--rw-r--r--   0        0        0     3091 2023-06-22 05:28:27.921786 statute_utils-0.3.0/statute_utils/components/utils.py
--rw-r--r--   0        0        0     5229 2023-06-22 05:28:27.921946 statute_utils-0.3.0/statute_utils/models.py
--rw-r--r--   0        0        0     4619 2023-06-22 05:28:27.922075 statute_utils-0.3.0/statute_utils/names.py
--rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.3.0/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.3.0/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.3.0/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.3.0/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.3.0/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6618 2023-06-22 05:28:27.922797 statute_utils-0.3.0/statute_utils/serials.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.3.1/README.md
+-rw-r--r--   0        0        0     1449 2023-06-22 06:12:44.624813 statute_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-06-22 06:12:44.625409 statute_utils-0.3.1/statute_utils/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-22 05:28:27.921068 statute_utils-0.3.1/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     9434 2023-06-22 06:12:44.626162 statute_utils-0.3.1/statute_utils/components/category.py
+-rw-r--r--   0        0        0     3528 2023-06-22 05:28:27.921378 statute_utils-0.3.1/statute_utils/components/details.py
+-rw-r--r--   0        0        0     4611 2023-06-22 05:28:27.921524 statute_utils-0.3.1/statute_utils/components/rule.py
+-rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.3.1/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3326 2023-06-22 06:12:44.626570 statute_utils-0.3.1/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     2350 2023-06-22 06:12:44.626823 statute_utils-0.3.1/statute_utils/main.py
+-rw-r--r--   0        0        0     5195 2023-06-22 06:12:44.627181 statute_utils-0.3.1/statute_utils/models.py
+-rw-r--r--   0        0        0     4434 2023-06-22 06:12:44.627800 statute_utils-0.3.1/statute_utils/names.py
+-rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.3.1/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.3.1/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.3.1/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.3.1/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.3.1/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6618 2023-06-22 06:11:13.995177 statute_utils-0.3.1/statute_utils/serials.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.3.1/PKG-INFO
```

### Comparing `statute_utils-0.3.0/LICENSE` & `statute_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/README.md` & `statute_utils-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/pyproject.toml` & `statute_utils-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.3.0"
+version = "0.3.1"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
@@ -37,15 +37,15 @@
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
-testpaths = ["tests", "statute_patterns"]
+testpaths = ["tests", "statute_utils"]
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
 [build-system]
```

### Comparing `statute_utils-0.3.0/statute_utils/__main__.py` & `statute_utils-0.3.1/statute_utils/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,17 @@
 
 def extract_rules(text: str) -> Iterator[Rule]:
     """If text contains [serialized][serial-pattern] (e.g. _Republic Act No. 386_)
     and [named][named-pattern] rules (_the Civil Code of the Philippines_),
     extract the [`Rules`][rule-model] into their canonical serial variants.
 
     Examples:
-        >>> from statute_patterns import extract_rules
         >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
         >>> list(extract_rules(text)) # get all rules
-        [
-            Rule(cat='ra', id='386'),
-            Rule(cat='ra', id='386'),
-            Rule(cat='spain', id='civil')
-        ]
+        [Rule(cat='ra', id='386'), Rule(cat='ra', id='386'), Rule(cat='spain', id='civil')]
 
     Args:
         text (str): Text to search for statute patterns.
 
     Yields:
         Iterator[Rule]: Serialized Rules and Named Rule patterns
     """  # noqa: E501
@@ -32,15 +27,14 @@
 
 
 def extract_rule(text: str) -> Rule | None:
     """Thin wrapper over [`extract_rules()`][extract-rules]. If text contains a
     matching [`Rule`][rule-model], get the first one found.
 
     Examples:
-        >>> from statute_patterns import extract_rule
         >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
         >>> extract_rule(text)  # get the first matching rule
         Rule(cat='ra', id='386')
 
     Args:
         text (str): Text to search for statute patterns.
 
@@ -54,21 +48,17 @@
 
 
 def count_rules(text: str) -> Iterator[dict]:
     """Based on results from [`extract_rules()`][extract-rules],
     get the count of each unique rule found.
 
     Examples:
-        >>> from statute_patterns import count_rules
         >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
-        >>> list(count_rules(text)): # get unique rules with counts
-        [
-            {'cat': 'ra', 'id': '386', 'mentions': 2},
-            {'cat': 'spain', 'id': 'civil', 'mentions': 1}
-        ]
+        >>> list(count_rules(text)) # get unique rules with counts
+        [{'cat': 'ra', 'id': '386', 'mentions': 2}, {'cat': 'spain', 'id': 'civil', 'mentions': 1}]
 
     Args:
         text (str): Text to search for statute patterns.
 
     Returns:
         Iterator[dict]: Unique rules converted into dicts with their counts
     """  # noqa: E501
```

### Comparing `statute_utils-0.3.0/statute_utils/components/category.py` & `statute_utils-0.3.1/statute_utils/components/category.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
-from enum import Enum
+from enum import StrEnum, auto
 from typing import Self
 
 from pydantic import BaseModel, ConfigDict
 
 
-class StatuteTitleCategory(str, Enum):
+class StatuteTitleCategory(StrEnum):
     """
     A [`Rule`][rule-model] in the Philippines involves various denominations.
     It can be referred to by its
 
     1. `official` title
     2. `serial` title
     3. `short` title
@@ -21,21 +21,21 @@
     --:|:--:|:--:|:--|:--|--:
     `official` | yes | official | full length title | _AN ACT TO PROVIDE PROTECTION TO BUYERS OF REAL ESTATE ON INSTALLMENT PAYMENTS_ | [Statute Details][statute-details]
     `serial` | yes | official | [`Statute Category`][statute-category-model] + serial identifier. | _Republic Act No. 6552_ | [Serial Pattern][serial-pattern] regex matching
     `short`  | no | official | may be declared in body of statute | _Realty Installment Buyer Act_ | [A helper function ][extract-short-title]
     `alias`  | no | unofficial | popular, undocumented means of referring to a statute | _Maceda Law_ | [Named Pattern][named-pattern] regex matching
     """  # noqa: E501
 
-    Official = "official"
-    Serial = "serial"
-    Alias = "alias"
-    Short = "short"
+    Official = auto()
+    Serial = auto()
+    Alias = auto()
+    Short = auto()
 
 
-class StatuteSerialCategory(str, Enum):
+class StatuteSerialCategory(StrEnum):
     """
     ## Application
     This concerns the `serial` title described by the [`Statute Title Category`][statute-title-category-model].
 
     ## Concept
     It would be difficult to identify rules if they were arbitrarily named
     without a fixed point of reference. For instance the _Civil Code of the
@@ -94,15 +94,15 @@
 
     Knowing the path to a [`Rule`][rule-model], we can later [extract its contents][statute-details].
 
     Examples:
         >>> StatuteSerialCategory
         <enum 'StatuteSerialCategory'>
         >>> StatuteSerialCategory._member_map_
-        {'RepublicAct': <StatuteSerialCategory.RepublicAct: 'ra'>, 'CommonwealthAct': <StatuteSerialCategory.CommonwealthAct: 'ca'>, 'Act': <StatuteSerialCategory.Act: 'act'>, 'Constitution': <StatuteSerialCategory.Constitution: 'const'>, 'Spain': <StatuteSerialCategory.Spain: 'spain'>, 'BatasPambansa': <StatuteSerialCategory.BatasPambansa: 'bp'>, 'PresidentialDecree': <StatuteSerialCategory.PresidentialDecree: 'pd'>, 'ExecutiveOrder': <StatuteSerialCategory.ExecutiveOrder: 'eo'>, 'LetterOfInstruction': <StatuteSerialCategory.LetterOfInstruction: 'loi'>, 'VetoMessage': <StatuteSerialCategory.VetoMessage: 'veto'>, 'RulesOfCourt': <StatuteSerialCategory.RulesOfCourt: 'roc'>, 'BarMatter': <StatuteSerialCategory.BarMatter: 'rule_bm'>, 'AdministrativeMatter': <StatuteSerialCategory.AdministrativeMatter: 'rule_am'>, 'ResolutionEnBanc': <StatuteSerialCategory.ResolutionEnBanc: 'rule_reso'>, 'CircularOCA': <StatuteSerialCategory.CircularOCA: 'oca_cir'>, 'CircularSC': <StatuteSerialCategory.CircularSC: 'sc_cir'>}
+        {'RepublicAct': 'ra', 'CommonwealthAct': 'ca', 'Act': 'act', 'Constitution': 'const', 'Spain': 'spain', 'BatasPambansa': 'bp', 'PresidentialDecree': 'pd', 'ExecutiveOrder': 'eo', 'LetterOfInstruction': 'loi', 'VetoMessage': 'veto', 'RulesOfCourt': 'roc', 'BarMatter': 'rule_bm', 'AdministrativeMatter': 'rule_am', 'ResolutionEnBanc': 'rule_reso', 'CircularOCA': 'oca_cir', 'CircularSC': 'sc_cir'}
     """  # noqa: E501
 
     RepublicAct = "ra"
     CommonwealthAct = "ca"
     Act = "act"
     Constitution = "const"
     Spain = "spain"
@@ -114,21 +114,26 @@
     RulesOfCourt = "roc"
     BarMatter = "rule_bm"
     AdministrativeMatter = "rule_am"
     ResolutionEnBanc = "rule_reso"
     CircularOCA = "oca_cir"
     CircularSC = "sc_cir"
 
+    def __repr__(self) -> str:
+        """Uses the value of the member `ra` instead of the the Enum default
+        `<StatuteSerialCategory.RepublicAct: 'ra'>`"""
+        return str.__repr__(self.value)
+
     @classmethod
     def from_value(cls, v: str) -> Self | None:
         """Using value, get the member, else return None.
 
         Examples:
             >>> StatuteSerialCategory.from_value('ra')
-            <StatuteSerialCategory.RepublicAct: 'ra'>
+            'ra'
 
         Args:
             v (str): The value to match
 
         Returns:
             Self | None: The member, if available.
         """
@@ -232,31 +237,19 @@
     def generate(
         cls,
         official: str | None = None,
         serial: str | None = None,
         short: str | None = None,
         aliases: list[str] | None = None,
     ):
+        if official:
+            yield cls(category=StatuteTitleCategory.Official, text=official)
+
+        if serial:
+            yield cls(category=StatuteTitleCategory.Serial, text=serial)
+
         if aliases:
             for title in aliases:
                 if title and title != "":
-                    yield cls(
-                        category=StatuteTitleCategory.Alias,
-                        text=title,
-                    )
+                    yield cls(category=StatuteTitleCategory.Alias, text=title)
         if short:
-            yield cls(
-                category=StatuteTitleCategory.Short,
-                text=short,
-            )
-
-        if serial:
-            yield cls(
-                category=StatuteTitleCategory.Serial,
-                text=serial,
-            )
-
-        if official:
-            yield cls(
-                category=StatuteTitleCategory.Official,
-                text=official,
-            )
+            yield cls(category=StatuteTitleCategory.Short, text=short)
```

### Comparing `statute_utils-0.3.0/statute_utils/components/details.py` & `statute_utils-0.3.1/statute_utils/components/details.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/statute_utils/components/rule.py` & `statute_utils-0.3.1/statute_utils/components/rule.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/statute_utils/components/short.py` & `statute_utils-0.3.1/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/statute_utils/components/utils.py` & `statute_utils-0.3.1/statute_utils/components/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     return yaml.nodes.MappingNode("tag:yaml.org,2002:map", value)
 
 
 yaml.add_representer(dict, represent_ordereddict)
 
 
 def walk(nodes: list[dict]):
+    """Converts raw nodes into a suitably formatted object for `yaml.dump()`.
+    Without this, there would be no formatting of content and the ordering
+    of the key-value pairs would not be in sync with the intended design.
+    """
     if isinstance(nodes, list):
         revised_nodes = []
         for node in nodes:
             data = []
             if node.get("item"):
                 candidate = node["item"]
                 if candidate := str(node["item"]).strip():
```

### Comparing `statute_utils-0.3.0/statute_utils/models.py` & `statute_utils-0.3.1/statute_utils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,9 +137,8 @@
         word `and` to get the individual component identifiers.
         """
         for match in self.pattern.finditer(text):
             for sp in self.collection:
                 if match.lastgroup == sp.group_name:
                     if candidates := sp.digits_in_match.search(match.group(0)):
                         for d in split_digits(candidates.group(0)):
-                            c = sp.cat
-                            yield Rule(cat=c, id=d)
+                            yield Rule(cat=sp.cat, id=d)
```

### Comparing `statute_utils-0.3.0/statute_utils/names.py` & `statute_utils-0.3.1/statute_utils/names.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 from .recipes import CONST, ROC, SP_CIVIL, SP_COMMERCE, SP_PENAL
 
 
 def make_spanish(name: str, regex: str):
     return NamedPattern(
         name=f"Old {name.title()} Code",
         regex_base=regex,
-        rule=Rule(
-            cat=StatuteSerialCategory.Spain,
-            id=name,
-        ),
+        rule=Rule(cat=StatuteSerialCategory.Spain, id=name),
     )
 
 
 spain_civil = make_spanish("civil", SP_CIVIL)
 spain_commerce = make_spanish("commerce", SP_COMMERCE)
 spain_penal = make_spanish("penal", SP_PENAL)
 spain_codes = [spain_civil, spain_commerce, spain_penal]
@@ -25,18 +22,15 @@
     regex_base=r"""
         (?: (?:New|NEW|The|THE)\s)?
         (?: (?<![Ss]panish\s)(?<![Oo]ld\s))
         (Civil|CIVIL)\s+(Code|CODE)
         (?: (?:\s+of\s+the\s+Philippines)|(?:\s+of\s+1950))?
         (?: (?!\s+of\s+1889))
     """,
-    rule=Rule(
-        cat=StatuteSerialCategory.RepublicAct,
-        id="386",
-    ),
+    rule=Rule(cat=StatuteSerialCategory.RepublicAct, id="386"),
     matches=[
         "NEW CIVIL CODE",
         "The Civil Code of the Philippines",
         "Civil Code of 1950",
     ],
     excludes=[
         "Spanish Civil Code",
@@ -48,18 +42,15 @@
     name="Revised Penal Code",
     regex_base=r"""
         (?: (?:The|THE)\s)?
         (?: (?<![Ss]panish\s)(?<![Oo]ld\s))
         (Revised|REVISED)\s+(Penal|PENAL)\s+(Code|CODE)
         (?: (?:\s+of\s+the\s+Philippines)|(?:\s+\(RPC\)))?
     """,
-    rule=Rule(
-        cat=StatuteSerialCategory.Act,
-        id="3815",
-    ),
+    rule=Rule(cat=StatuteSerialCategory.Act, id="3815"),
     matches=[
         "Revised Penal Code (RPC)",
         "The Revised Penal Code of the Philippines",
         "Revised Penal Code",
     ],
     excludes=[
         "The Penal Code",
@@ -69,18 +60,15 @@
 )
 
 
 def make_const(year: int):
     return NamedPattern(
         name=f"{year} Constitution",
         regex_base=rf"{year}\s+(?:{CONST})",
-        rule=Rule(
-            cat=StatuteSerialCategory.Constitution,
-            id=f"{year}",
-        ),
+        rule=Rule(cat=StatuteSerialCategory.Constitution, id=f"{year}"),
     )
 
 
 const_1987: NamedPattern = make_const(1987)
 const_1973: NamedPattern = make_const(1973)
 const_1935: NamedPattern = make_const(1935)
 const_years = [const_1987, const_1973, const_1935]
@@ -107,35 +95,29 @@
     name="Corporation Code of 1980",
     regex_base=r"""
         (?: (?:The|THE)\s)?
         (?: (?<![Rr]evised\s)(?<!REVISED\s))
         (?: Corporation|CORPORATION)\s+(?:Code|CODE)
         (?: (?:\s+of\s+the\s+Philippines)|(?:\s+of\s+1980))?
     """,
-    rule=Rule(
-        cat=StatuteSerialCategory.BatasPambansa,
-        id="68",
-    ),
+    rule=Rule(cat=StatuteSerialCategory.BatasPambansa, id="68"),
     matches=[
         "THE CORPORATION CODE",
         "Corporation Code of 1980",
         "Corporation Code of the Philippines",
     ],
     excludes=["Revised Corporation Code"],
 )
 corpcode_revised = NamedPattern(
     name="Corporation Code of 2021",
     regex_base=r"""
         (?:[Rr]evised|REVISED)\s+(?:Corporation|CORPORATION)\s+(?:Code|CODE)
         (?: (?:\s+of\s+the\s+Philippines)|(?:\s+of\s+2021))?
     """,
-    rule=Rule(
-        cat=StatuteSerialCategory.RepublicAct,
-        id="11232",
-    ),
+    rule=Rule(cat=StatuteSerialCategory.RepublicAct, id="11232"),
     matches=[
         "Revised Corporation Code",
         "Revised Corporation Code of the Philippines",
         "Revised Corporation Code of 2021",
     ],
     excludes=["The Corporation Code"],
 )
@@ -156,18 +138,15 @@
         )|
         (?:
             of\s+
             the\s+
             CPR
         )
     """,
-    rule=Rule(
-        cat=StatuteSerialCategory.RulesOfCourt,
-        id="cpr",
-    ),
+    rule=Rule(cat=StatuteSerialCategory.RulesOfCourt, id="cpr"),
     matches=[
         "Code of Professional Responsibility (CPR)",
         "Code of Professional Responsibility",
         "CODE OF PROFESSIONAL RESPONSIBILITY",
         "of the CPR",
     ],
     excludes=["The Corporation Code"],
```

### Comparing `statute_utils-0.3.0/statute_utils/recipes/digits.py` & `statute_utils-0.3.1/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/statute_utils/recipes/spain.py` & `statute_utils-0.3.1/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/statute_utils/serials.py` & `statute_utils-0.3.1/statute_utils/serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.0/PKG-INFO` & `statute_utils-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

