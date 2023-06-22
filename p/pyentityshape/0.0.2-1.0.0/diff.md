# Comparing `tmp/pyentityshape-0.0.2.tar.gz` & `tmp/pyentityshape-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyentityshape-0.0.2.tar", max compression
+gzip compressed data, was "pyentityshape-1.0.0.tar", max compression
```

## Comparing `pyentityshape-0.0.2.tar` & `pyentityshape-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-06-22 16:30:47.249674 pyentityshape-0.0.2/LICENSE
--rw-r--r--   0        0        0      205 2023-06-22 18:21:02.155359 pyentityshape-0.0.2/README.md
--rw-r--r--   0        0        0     1641 2023-06-22 18:02:01.315781 pyentityshape-0.0.2/entityshape/__init__.py
--rw-r--r--   0        0        0      167 2023-06-22 17:49:57.400423 pyentityshape-0.0.2/entityshape/exceptions.py
--rw-r--r--   0        0        0     3115 2023-06-22 18:20:52.671943 pyentityshape-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 pyentityshape-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 16:30:47.249674 pyentityshape-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1009 2023-06-22 21:04:46.239611 pyentityshape-1.0.0/README.md
+-rw-r--r--   0        0        0     1725 2023-06-22 21:04:46.226277 pyentityshape-1.0.0/entityshape/__init__.py
+-rw-r--r--   0        0        0      446 2023-06-22 21:01:22.634718 pyentityshape-1.0.0/entityshape/enums.py
+-rw-r--r--   0        0        0      167 2023-06-22 17:49:57.400423 pyentityshape-1.0.0/entityshape/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:14:54.501995 pyentityshape-1.0.0/entityshape/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-06-22 19:34:42.343203 pyentityshape-1.0.0/entityshape/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      814 2023-06-22 19:34:42.343203 pyentityshape-1.0.0/entityshape/models/__pycache__/property_value.cpython-311.pyc
+-rw-r--r--   0        0        0     6892 2023-06-22 20:39:39.790500 pyentityshape-1.0.0/entityshape/models/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0      823 2023-06-22 19:38:04.854916 pyentityshape-1.0.0/entityshape/models/__pycache__/statement_value.cpython-311.pyc
+-rw-r--r--   0        0        0      245 2023-06-22 19:34:08.339605 pyentityshape-1.0.0/entityshape/models/property_value.py
+-rw-r--r--   0        0        0     3970 2023-06-22 21:04:46.216277 pyentityshape-1.0.0/entityshape/models/result.py
+-rw-r--r--   0        0        0      252 2023-06-22 19:37:57.434849 pyentityshape-1.0.0/entityshape/models/statement_value.py
+-rw-r--r--   0        0        0     3115 2023-06-22 21:06:07.860724 pyentityshape-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 pyentityshape-1.0.0/PKG-INFO
```

### Comparing `pyentityshape-0.0.2/LICENSE` & `pyentityshape-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyentityshape-0.0.2/entityshape/__init__.py` & `pyentityshape-1.0.0/entityshape/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from typing import Any, Dict
-
 import requests
 from pydantic import BaseModel
 
 from entityshape.exceptions import ApiError, EidError, LangError, QidError
+from entityshape.models.result import Result
 
 
 class EntityShape(BaseModel):
     """This class models the entityshape API
     It has a default timeout of 10 seconds
 
     The API currently only support items"""
 
     qid = ""  # item
     eid = ""  # entityshape
     lang = ""  # language
     timeout: int = 10
-    result: Dict[Any, Any] = {}
+    result: Result = Result()
 
     def __check__(self):
         if not self.lang:
             raise LangError("We only support 2 and 3 letter language codes")
         if not self.eid:
             raise EidError("We need an entityshape EID")
         if not self.qid:
             raise QidError("We need an item QID")
 
-    def get_result(self) -> Dict[Any, Any]:
+    def get_result(self) -> Result:
         """This method checks if we got the 3 parameters we need and
         gets the results and return them"""
         self.__check__()
         url = f"http://entityshape.toolforge.org/api?entity={self.qid}&entityschema={self.eid}&language={self.lang}"
         response = requests.get(url, timeout=self.timeout)
         if response.status_code == 200:
-            self.result = response.json()
+            print(response.json())
+            self.result = Result(**response.json())
+            self.result.analyze()
             # print(self.result)
             return self.result
         else:
             raise ApiError(f"Got {response.status_code} from the entityshape API")
 
     # def check_lang(self):
     #     if not self.lang or 4 > len(self.lang) > 1:
```

### Comparing `pyentityshape-0.0.2/pyproject.toml` & `pyentityshape-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyEntityshape"
-version = "0.0.2"
+version = "1.0.0"
 description = "Python library to validate Wikidata items using the entityshape API."
 authors = ["Dennis Priskorn <68460690+dpriskorn@users.noreply.github.com>"]
 license = "GPLv3+"
 readme = "README.md"
 repository = "https://github.com/dpriskorn/PyEntityshape"
 keywords = ["entityshape API", "wikidata", "entityschema", "entity validation"]
 classifiers = [
```

