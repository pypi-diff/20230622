# Comparing `tmp/citation_report-0.1.4.tar.gz` & `tmp/citation_report-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_report-0.1.4.tar", max compression
+gzip compressed data, was "citation_report-0.1.5.tar", max compression
```

## Comparing `citation_report-0.1.4.tar` & `citation_report-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:17:10.404107 citation_report-0.1.4/LICENSE
--rw-r--r--   0        0        0      149 2023-06-21 15:20:34.271243 citation_report-0.1.4/citation_report/__init__.py
--rw-r--r--   0        0        0     6097 2023-06-21 15:20:17.992985 citation_report-0.1.4/citation_report/__main__.py
--rw-r--r--   0        0        0     1751 2023-06-21 15:17:00.053497 citation_report-0.1.4/citation_report/published_report.py
--rw-r--r--   0        0        0     3233 2023-06-21 15:20:49.835556 citation_report-0.1.4/citation_report/publisher.py
--rw-r--r--   0        0        0     1377 2023-06-21 15:19:04.186541 citation_report-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 citation_report-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:17:10.404107 citation_report-0.1.5/LICENSE
+-rw-r--r--   0        0        0      163 2023-06-22 10:48:32.510065 citation_report-0.1.5/citation_report/__init__.py
+-rw-r--r--   0        0        0     7629 2023-06-22 10:51:16.600868 citation_report-0.1.5/citation_report/main.py
+-rw-r--r--   0        0        0     1787 2023-06-22 10:49:27.462730 citation_report-0.1.5/citation_report/published_report.py
+-rw-r--r--   0        0        0     3165 2023-06-22 10:52:31.001537 citation_report-0.1.5/citation_report/publisher.py
+-rw-r--r--   0        0        0     1353 2023-06-22 10:49:58.585605 citation_report-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 citation_report-0.1.5/PKG-INFO
```

### Comparing `citation_report-0.1.4/LICENSE` & `citation_report-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.4/citation_report/__main__.py` & `citation_report-0.1.5/citation_report/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from collections.abc import Iterator
 from typing import Self
 
 from dateutil.parser import parse
 from pydantic import BaseModel, Field
 
 from .published_report import REPORT_PATTERN
-from .publisher import OFFG, PHIL, SCRA, get_publisher_label
+from .publisher import ReportOffg, ReportPhil, ReportSCRA, get_publisher_label
+
+
+def is_eq(a: str | None, b: str | None) -> bool:
+    """Checks if string `a` is not None, string `b` is not None and both
+    `a` and `b` are equal."""
+    return all([a, b, a == b])
 
 
 class Report(BaseModel):
     """The [REPORT_PATTERN][report-pattern] is a `re.Pattern` object that
     contains pre-defined regex group names. These group names can be mapped
     to the `Report` model's fields:
 
@@ -43,62 +49,98 @@
         title="Report Publisher",
         description="Shorthand label of the publisher involved, e.g. SCRA, Phil. Offg",
         max_length=5,
     )
     volume: str | None = Field(
         None,
         title="Volume Number",
-        description=(
-            "Publisher volume number - may not be a full digit since it can"
-            " exceptionally include letters."
-        ),
+        description=("Can exceptionally include letters e.g. vol 1a"),
         max_length=10,
     )
     page: str | None = Field(
         None,
         title="Page Number",
-        description="The page number of the publisher volume involved",
+        description="Page number can have letters, e.g. 241a",
         max_length=5,
     )
     volpubpage: str | None = Field(
         None,
         title="Volume Publisher Page",
-        description="Full expression of the report citation",
+        description="Full expression of report citation",
         max_length=20,
     )
     report_date: datetime.date | None = Field(
         None,
         title="Report Date",
         description="Exceptionally, report citations reference dates.",
     )
 
+    def __repr__(self) -> str:
+        return f"<Report {str(self)}>"
+
     def __str__(self) -> str:
         return self.volpubpage or ""
 
+    def __eq__(self, other: Self) -> bool:
+        """Naive equality checks will only compare direct values,
+        exceptionally, when volume, publisher and page are provided,
+        must compare all three values with each other.
+
+        Examples:
+            >>> a = Report(volume='10', publisher='Phil.', page='25')
+            >>> b = Report(volume='10', publisher='Phil.')
+            >>> a == b
+            False
+            >>> c = Report(volume='10', publisher='SCRA', page='25')
+            >>> a == c
+            False
+            >>> d = Report(volume='10', publisher='Phil.', page='25')
+            >>> a == d
+            True
+
+        Args:
+            other[Self]: The other Citation being compared
+
+        Returns:
+            bool: Whether values are equal
+        """
+        opt_1 = is_eq(self.volpubpage, other.volpubpage)
+        opt_2 = is_eq(self.phil, other.phil)
+        opt_3 = is_eq(self.scra, other.scra)
+        opt_4 = is_eq(self.offg, other.offg)
+        opt_5 = all(
+            [
+                is_eq(self.publisher, other.publisher),
+                is_eq(self.volume, other.volume),
+                is_eq(self.page, other.page),
+            ]
+        )
+        return any([opt_1, opt_2, opt_3, opt_4, opt_5])
+
     @property
     def phil(self):
-        return self.volpubpage if self.publisher == PHIL.label else None
+        return self.volpubpage if self.publisher == ReportPhil.label else None
 
     @property
     def scra(self):
-        return self.volpubpage if self.publisher == SCRA.label else None
+        return self.volpubpage if self.publisher == ReportSCRA.label else None
 
     @property
     def offg(self):
-        return self.volpubpage if self.publisher == OFFG.label else None
+        return self.volpubpage if self.publisher == ReportOffg.label else None
 
     @classmethod
-    def extract_report(cls, text: str) -> Iterator[Self]:
+    def extract_reports(cls, text: str) -> Iterator[Self]:
         """Given sample legalese `text`, extract all Supreme Court `Report` patterns.
 
         Examples:
             >>> sample = "250 Phil. 271, 271-272, Jan. 1, 2019"
-            >>> report = next(Report.extract(sample))
+            >>> report = next(Report.extract_reports(sample))
             >>> type(report)
-            citation_report.__main__.Report
+            <class 'citation_report.main.Report'>
             >>> report.volpubpage
             '250 Phil. 271'
 
         Args:
             text (str): Text containing report citations.
 
         Yields:
@@ -141,32 +183,34 @@
 
         Returns:
             str | None: The value of the key `report_type` in the `data` dict.
         """
         if report_type.lower() in ["scra", "phil", "offg"]:
             if candidate := data.get(report_type):
                 try:
-                    obj = next(cls.extract_report(candidate))
+                    obj = next(cls.extract_reports(candidate))
                     # will get the @property of the Report with the same name
                     if hasattr(obj, report_type):
                         return obj.__getattribute__(report_type)
                 except StopIteration:
                     return None
         return None
 
     @classmethod
     def get_unique(cls, text: str) -> list[str]:
         """Will only get `Report` volpubpages (string) from the text. This
         is used later in `citation_utils` to prevent duplicate citations.
 
         Examples:
             >>> text = "(22 Phil. 303; 22 Phil. 303; 176 SCRA 240; Peñalosa v. Tuason, 22 Phil. 303, 313 (1912); Heirs of Roxas v. Galido, 108 Phil. 582 (1960)); Valmonte v. PCSO, supra; Bugnay Const. and Dev. Corp. v. Laron, 176 SCRA 240 (1989)"
-            >>> Report.get_unique(text)
-            ['22 Phil. 303', '108 Phil. 582', '176 SCRA 240']
+            >>> len(Report.get_unique(text))
+            3
+            >>> set(Report.get_unique(text)) == {'22 Phil. 303', '176 SCRA 240', '108 Phil. 582'}
+            True
 
         Args:
             text (str): Text to search for report patterns
 
         Returns:
             list[str]: Unique report `volpubpage` strings found in the text
         """  # noqa: E501
-        return list({r.volpubpage for r in cls.extract_report(text) if r.volpubpage})
+        return list({r.volpubpage for r in cls.extract_reports(text) if r.volpubpage})
```

### Comparing `citation_report-0.1.4/citation_report/published_report.py` & `citation_report-0.1.5/citation_report/published_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from re import Pattern
 
 from citation_date import REPORT_DATE_REGEX
 
-from .publisher import OFFG, PHIL, SCRA
+from .publisher import ReportOffg, ReportPhil, ReportSCRA
 
 PUBLISHERS_REGEX = rf"""
     (?P<publisher>
-        {SCRA.regex}| # contains SCRA_PUB group name
-        {PHIL.regex}| # contains PHIL_PUB group name
-        {OFFG.regex} # contains OG_PUB group name
+        {ReportSCRA.regex}| # contains SCRA_PUB group name
+        {ReportPhil.regex}| # contains PHIL_PUB group name
+        {ReportOffg.regex} # contains OG_PUB group name
     )
 """
 """A partial regex string containing the Publisher options available."""
 
 
 volume = r"""
     \b
```

### Comparing `citation_report-0.1.4/citation_report/publisher.py` & `citation_report-0.1.5/citation_report/publisher.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,53 +7,47 @@
 
 
 class PublisherStyle(BaseModel):
     """Each publisher is represented by a regex expression `regex`.
     The `group_name` should be present in the `regex`.
     """
 
-    label: str = Field(
-        ...,
-        title="Report style",
-        description="Use for uniformity"
-    )
+    label: str = Field(..., title="Report style", description="Use for uniformity")
     group_name: str = Field(
         ...,
         title="Regex group name",
-        description="Custom regex group that identifies the publisher"
+        description="Custom regex group that identifies the publisher",
     )
     regex: str = Field(
         ...,
         title="Regular expression",
-        description=(
-            "The regex expression that can be used to extract the various"
-            " publisher styles, e.g. 'Phil.' or 'Phil. Report', 'SCRA' or"
-            " 'S.C.R.A. Note that all expressions are eventually combined in"
-            " `REPORT_PATTERN`."
+        description=(  # noqa: E501
+            "Extract various publisher styles, e.g. 'Phil.' or 'Phil. Report', 'SCRA'"
+            " or 'S.C.R.A. All expressions eventually combined in `REPORT_PATTERN`."
         ),
     )
 
     @property
     def pattern(self) -> Pattern:
         return re.compile(self.regex, re.I | re.X)
 
 
-PHIL = PublisherStyle(
+ReportPhil = PublisherStyle(
     label="Phil.",
     group_name="PHIL_PUB",
     regex=rf"(?P<PHIL_PUB>phil{separator}(rep)?{separator})",
 )  # e.g .4 Phil. Rep., 545
 
-SCRA = PublisherStyle(
+ReportSCRA = PublisherStyle(
     label="SCRA",
     group_name="SCRA_PUB",
     regex=r"(?P<SCRA_PUB>SCRA)",
 )
 
-OFFG = PublisherStyle(
+ReportOffg = PublisherStyle(
     label="O.G.",
     group_name="OG_PUB",
     regex=rf"""(?P<OG_PUB>
                 (
                     (
                         o
                         {separator}
@@ -104,10 +98,10 @@
     Args:
         match (Match): Based on a prior `re.search` or `re.finditer`
             result on text
 
     Returns:
         str | None: The first matching publisher found
     """
-    for src in [PHIL, SCRA, OFFG]:
+    for src in [ReportPhil, ReportSCRA, ReportOffg]:
         if match.group(src.group_name):
             return src.label
```

### Comparing `citation_report-0.1.4/pyproject.toml` & `citation_report-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "citation-report"
-version = "0.1.4"
+version = "0.1.5"
 description = "Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
-license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-report"
 documentation = "https://justmars.github.io/citation-report"
 classifiers = [
   "Topic :: Text Processing :: General",
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
@@ -40,9 +39,9 @@
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
 [build-system]
-requires = ["poetry-core>=1.1.12"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `citation_report-0.1.4/PKG-INFO` & `citation_report-0.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: citation-report
-Version: 0.1.4
+Version: 0.1.5
 Summary: Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG.
 Home-page: https://lawsql.com
-License: MIT
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
 Requires-Dist: citation-date (>=0.1.5,<0.2.0)
 Requires-Dist: pydantic (>=2.0b3)
 Project-URL: Documentation, https://justmars.github.io/citation-report
```

