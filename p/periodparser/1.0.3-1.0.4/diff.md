# Comparing `tmp/periodparser-1.0.3.tar.gz` & `tmp/periodparser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodparser-1.0.3.tar", max compression
+gzip compressed data, was "periodparser-1.0.4.tar", max compression
```

## Comparing `periodparser-1.0.3.tar` & `periodparser-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     4857 2023-06-21 18:31:00.723311 periodparser-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1154 2023-06-21 18:31:00.722309 periodparser-1.0.3/README.md
--rw-r--r--   0        0        0       28 2023-06-21 18:31:00.724310 periodparser-1.0.3/src/periodparser/__init__.py
--rw-r--r--   0        0        0       78 2023-06-21 18:31:00.724310 periodparser-1.0.3/src/periodparser/dict/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-21 18:31:00.725311 periodparser-1.0.3/src/periodparser/dict/keywords.py
--rw-r--r--   0        0        0     2031 2023-06-21 18:31:00.726310 periodparser-1.0.3/src/periodparser/dict/morph.py
--rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.3/src/periodparser/dict/time_words.txt
--rw-r--r--   0        0        0      161 2023-06-21 18:31:00.727310 periodparser-1.0.3/src/periodparser/models/__init__.py
--rw-r--r--   0        0        0     6422 2023-06-21 18:31:00.728311 periodparser-1.0.3/src/periodparser/models/abstract_period.py
--rw-r--r--   0        0        0     2833 2023-06-21 18:31:00.728311 periodparser-1.0.3/src/periodparser/models/dates_raw_data.py
--rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.3/src/periodparser/models/i_has_edges.py
--rw-r--r--   0        0        0     2448 2023-06-21 18:31:00.729312 periodparser-1.0.3/src/periodparser/models/parse_result.py
--rw-r--r--   0        0        0     2288 2023-06-21 18:31:00.730309 periodparser-1.0.3/src/periodparser/models/parser_models.py
--rw-r--r--   0        0        0      234 2023-06-21 18:31:00.731310 periodparser-1.0.3/src/periodparser/models/text_token.py
--rw-r--r--   0        0        0     1002 2023-06-21 18:31:00.732309 periodparser-1.0.3/src/periodparser/recognizers/__init__.py
--rw-r--r--   0        0        0     1139 2023-06-21 18:31:00.733310 periodparser-1.0.3/src/periodparser/recognizers/dates_period_recognizer.py
--rw-r--r--   0        0        0     1469 2023-06-21 18:31:00.733310 periodparser-1.0.3/src/periodparser/recognizers/day_of_week_recognizer.py
--rw-r--r--   0        0        0     1727 2023-06-21 18:31:00.734312 periodparser-1.0.3/src/periodparser/recognizers/days_month_recognizer.py
--rw-r--r--   0        0        0      906 2023-06-21 18:31:00.735312 periodparser-1.0.3/src/periodparser/recognizers/holidays_recognizer.py
--rw-r--r--   0        0        0     1283 2023-06-21 18:31:00.735312 periodparser-1.0.3/src/periodparser/recognizers/month_recognizer.py
--rw-r--r--   0        0        0     1347 2023-06-21 18:31:00.736309 periodparser-1.0.3/src/periodparser/recognizers/part_of_day_recognizer.py
--rw-r--r--   0        0        0     1621 2023-06-21 18:31:00.737311 periodparser-1.0.3/src/periodparser/recognizers/recognizer.py
--rw-r--r--   0        0        0     1231 2023-06-21 18:31:00.738309 periodparser-1.0.3/src/periodparser/recognizers/relative_date_recognizer.py
--rw-r--r--   0        0        0      732 2023-06-21 18:31:00.739309 periodparser-1.0.3/src/periodparser/recognizers/relative_day_recognizer.py
--rw-r--r--   0        0        0     3137 2023-06-21 18:31:00.740311 periodparser-1.0.3/src/periodparser/recognizers/time_recognizer.py
--rw-r--r--   0        0        0     2761 2023-06-21 18:31:00.740311 periodparser-1.0.3/src/periodparser/recognizers/time_span_recognizer.py
--rw-r--r--   0        0        0      726 2023-06-21 18:31:00.741311 periodparser-1.0.3/src/periodparser/recognizers/year_recognizer.py
--rw-r--r--   0        0        0     2538 2023-06-21 18:31:00.742316 periodparser-1.0.3/src/periodparser/sugar.py
--rw-r--r--   0        0        0    11842 2023-06-21 18:31:00.743310 periodparser-1.0.3/src/periodparser/text_parser.py
--rw-r--r--   0        0        0      118 2023-06-21 18:31:00.744312 periodparser-1.0.3/src/periodparser/utils/__init__.py
--rw-r--r--   0        0        0     1043 2023-06-21 18:31:00.745309 periodparser-1.0.3/src/periodparser/utils/helpers.py
--rw-r--r--   0        0        0     4849 2023-06-21 18:31:00.745309 periodparser-1.0.3/src/periodparser/utils/parser_extractors.py
--rw-r--r--   0        0        0      668 2023-06-21 18:31:00.746311 periodparser-1.0.3/src/periodparser/utils/parser_utils.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 periodparser-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4857 2023-06-22 18:05:20.613355 periodparser-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1142 2023-06-22 17:45:56.279467 periodparser-1.0.4/README.md
+-rw-r--r--   0        0        0       28 2023-06-21 18:35:36.491438 periodparser-1.0.4/src/periodparser/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-21 18:31:00.724310 periodparser-1.0.4/src/periodparser/dict/__init__.py
+-rw-r--r--   0        0        0     2828 2023-06-21 18:31:00.725311 periodparser-1.0.4/src/periodparser/dict/keywords.py
+-rw-r--r--   0        0        0     2031 2023-06-21 18:31:00.726310 periodparser-1.0.4/src/periodparser/dict/morph.py
+-rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.4/src/periodparser/dict/time_words.txt
+-rw-r--r--   0        0        0      161 2023-06-21 18:31:00.727310 periodparser-1.0.4/src/periodparser/models/__init__.py
+-rw-r--r--   0        0        0     6422 2023-06-21 18:31:00.728311 periodparser-1.0.4/src/periodparser/models/abstract_period.py
+-rw-r--r--   0        0        0     2833 2023-06-21 18:31:00.728311 periodparser-1.0.4/src/periodparser/models/dates_raw_data.py
+-rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.4/src/periodparser/models/i_has_edges.py
+-rw-r--r--   0        0        0     2448 2023-06-21 18:31:00.729312 periodparser-1.0.4/src/periodparser/models/parse_result.py
+-rw-r--r--   0        0        0     2288 2023-06-21 18:31:00.730309 periodparser-1.0.4/src/periodparser/models/parser_models.py
+-rw-r--r--   0        0        0      234 2023-06-21 18:31:00.731310 periodparser-1.0.4/src/periodparser/models/text_token.py
+-rw-r--r--   0        0        0     1002 2023-06-21 18:31:00.732309 periodparser-1.0.4/src/periodparser/recognizers/__init__.py
+-rw-r--r--   0        0        0     1139 2023-06-21 18:31:00.733310 periodparser-1.0.4/src/periodparser/recognizers/dates_period_recognizer.py
+-rw-r--r--   0        0        0     1469 2023-06-21 18:31:00.733310 periodparser-1.0.4/src/periodparser/recognizers/day_of_week_recognizer.py
+-rw-r--r--   0        0        0     1727 2023-06-21 18:31:00.734312 periodparser-1.0.4/src/periodparser/recognizers/days_month_recognizer.py
+-rw-r--r--   0        0        0      906 2023-06-21 18:31:00.735312 periodparser-1.0.4/src/periodparser/recognizers/holidays_recognizer.py
+-rw-r--r--   0        0        0     1283 2023-06-21 18:31:00.735312 periodparser-1.0.4/src/periodparser/recognizers/month_recognizer.py
+-rw-r--r--   0        0        0     1347 2023-06-21 18:31:00.736309 periodparser-1.0.4/src/periodparser/recognizers/part_of_day_recognizer.py
+-rw-r--r--   0        0        0     1621 2023-06-21 18:31:00.737311 periodparser-1.0.4/src/periodparser/recognizers/recognizer.py
+-rw-r--r--   0        0        0     1231 2023-06-21 18:31:00.738309 periodparser-1.0.4/src/periodparser/recognizers/relative_date_recognizer.py
+-rw-r--r--   0        0        0      732 2023-06-21 18:31:00.739309 periodparser-1.0.4/src/periodparser/recognizers/relative_day_recognizer.py
+-rw-r--r--   0        0        0     3220 2023-06-22 18:05:19.371143 periodparser-1.0.4/src/periodparser/recognizers/time_recognizer.py
+-rw-r--r--   0        0        0     2761 2023-06-21 18:31:00.740311 periodparser-1.0.4/src/periodparser/recognizers/time_span_recognizer.py
+-rw-r--r--   0        0        0      726 2023-06-21 18:31:00.741311 periodparser-1.0.4/src/periodparser/recognizers/year_recognizer.py
+-rw-r--r--   0        0        0     2538 2023-06-21 18:35:36.491949 periodparser-1.0.4/src/periodparser/sugar.py
+-rw-r--r--   0        0        0    11954 2023-06-22 18:05:19.372143 periodparser-1.0.4/src/periodparser/text_parser.py
+-rw-r--r--   0        0        0      118 2023-06-21 18:31:00.744312 periodparser-1.0.4/src/periodparser/utils/__init__.py
+-rw-r--r--   0        0        0     1043 2023-06-21 18:31:00.745309 periodparser-1.0.4/src/periodparser/utils/helpers.py
+-rw-r--r--   0        0        0     4849 2023-06-21 18:31:00.745309 periodparser-1.0.4/src/periodparser/utils/parser_extractors.py
+-rw-r--r--   0        0        0      668 2023-06-21 18:31:00.746311 periodparser-1.0.4/src/periodparser/utils/parser_utils.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 periodparser-1.0.4/PKG-INFO
```

### Comparing `periodparser-1.0.3/pyproject.toml` & `periodparser-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "periodparser"
-version = "1.0.3"
+version = "1.0.4"
 description = "python parser for human readable period dates"
 authors = ["fenn_r <fenrir1121@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/fennr/periodparser"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.3"
+version = "1.0.4"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.8,<4.0"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 black = ">=23.3.0"
```

### Comparing `periodparser-1.0.3/README.md` & `periodparser-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/periodparser)
 ![PyPI - Python Version](https://img.shields.io/pypi/v/periodparser)
 ![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)
 
-
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=git@github.com:fennr/periodparser)
 
 # periodparser
 
 python parser for human-readable period dates
 
 ## Установка
@@ -19,10 +18,9 @@
 
 ## Пример
 
 ```python
 import periodparser as pp
 
 result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
-print(result.dates[
-          0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
-```
+print(result.dates[0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
+```
```

### Comparing `periodparser-1.0.3/src/periodparser/dict/keywords.py` & `periodparser-1.0.4/src/periodparser/dict/keywords.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/dict/morph.py` & `periodparser-1.0.4/src/periodparser/dict/morph.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/dict/time_words.txt` & `periodparser-1.0.4/src/periodparser/dict/time_words.txt`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/models/abstract_period.py` & `periodparser-1.0.4/src/periodparser/models/abstract_period.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/models/dates_raw_data.py` & `periodparser-1.0.4/src/periodparser/models/dates_raw_data.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/models/parse_result.py` & `periodparser-1.0.4/src/periodparser/models/parse_result.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/models/parser_models.py` & `periodparser-1.0.4/src/periodparser/models/parser_models.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/__init__.py` & `periodparser-1.0.4/src/periodparser/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/dates_period_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/dates_period_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/day_of_week_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/day_of_week_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/days_month_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/days_month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/holidays_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/holidays_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/month_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/part_of_day_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/part_of_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/relative_date_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/relative_date_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/relative_day_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/relative_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/time_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/time_recognizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..models import AbstractPeriod, DatesRawData
 from ..models.parser_models import FixPeriod
 from .recognizer import Recognizer
 
 
 class TimeRecognizer(Recognizer):
     regex_pattern = r"([rvgd])?([fot])?(Q|H)?(h|(0)(h)?)((0)e?)?([rvgd])?"
-
+    counter = 0
     def parse_match(self, data: DatesRawData, match, now: datetime) -> bool:
         if (
             match.group(5) is not None
             or match.group(6) is not None
             or match.group(4) is not None
             or match.group(1) is not None
             or match.group(9)
@@ -68,12 +68,13 @@
                 date.time = timedelta(seconds=hours * 60 * 60 + minutes * 60)
                 s, e = match.span()
                 to_time = data.tokens[s]
                 data.replace_tokens_by_dates(s, (e - s), date)
                 if match.group(2) == "t":
                     data.return_tokens(s, "t", to_time)
             # if 0 <= hours <= 23:
-
-            return True
+            self.counter += 1
+            if self.counter < 99:
+                return True
         #  if match.group(5) is not None or match.group(6) is not None or match.group(4) is not None or match.group(1) is not None or match.group(9):
 
         return False
```

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/time_span_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/time_span_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/recognizers/year_recognizer.py` & `periodparser-1.0.4/src/periodparser/recognizers/year_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/sugar.py` & `periodparser-1.0.4/src/periodparser/sugar.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/text_parser.py` & `periodparser-1.0.4/src/periodparser/text_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,18 @@
             elif resolution == FixPeriod.DAY:
                 date_to += timedelta(days=7)
             elif resolution == FixPeriod.WEEK:
                 date_to = date_to.replace(month=date_to.month + 1)
             elif resolution == FixPeriod.MONTH:
                 date_to = date_to.replace(year=date_to.year + 1)
             else:
-                date_to = date_to.replace(hour=date_to.hour + 12)
+                try:
+                    date_to = date_to.replace(hour=date_to.hour + 12)
+                except ValueError:
+                    date_to += timedelta(days=1)
 
         date_to_save = DateTimeToken()
         date_to_save.date_from = from_token.date_from
         date_to_save.date_to = date_to
         date_to_save.type = DateTimeTokenType.PERIOD
         date_to_save.has_time = from_token.has_time or to_token.has_time
     else:
```

### Comparing `periodparser-1.0.3/src/periodparser/utils/helpers.py` & `periodparser-1.0.4/src/periodparser/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/utils/parser_extractors.py` & `periodparser-1.0.4/src/periodparser/utils/parser_extractors.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/src/periodparser/utils/parser_utils.py` & `periodparser-1.0.4/src/periodparser/utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.3/PKG-INFO` & `periodparser-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodparser
-Version: 1.0.3
+Version: 1.0.4
 Summary: python parser for human readable period dates
 Home-page: https://github.com/fennr/periodparser
 Author: fenn_r
 Author-email: fenrir1121@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,14 @@
 Project-URL: Repository, https://github.com/fennr/periodparser
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/periodparser)
 ![PyPI - Python Version](https://img.shields.io/pypi/v/periodparser)
 ![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)
 
-
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=git@github.com:fennr/periodparser)
 
 # periodparser
 
 python parser for human-readable period dates
 
 ## Установка
@@ -35,10 +34,10 @@
 
 ## Пример
 
 ```python
 import periodparser as pp
 
 result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
-print(result.dates[
-          0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
+print(result.dates[0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
 ```
+
```

