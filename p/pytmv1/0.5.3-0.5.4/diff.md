# Comparing `tmp/pytmv1-0.5.3.tar.gz` & `tmp/pytmv1-0.5.4.tar.gz`

## Comparing `pytmv1-0.5.3.tar` & `pytmv1-0.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.3/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.3/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10938 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3203 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.3/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.3/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.3/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.4/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.4/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10938 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3203 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.4/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.4/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.4/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.4/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.4/PKG-INFO
```

### Comparing `pytmv1-0.5.3/src/pytmv1/__init__.py` & `pytmv1-0.5.4/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/caller.py` & `pytmv1-0.5.4/src/pytmv1/caller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     SubmitFileToSandboxResp,
 )
 from .results import MultiResult, Result
 
 log: Logger = logging.getLogger(__name__)
 
 
+@lru_cache(maxsize=None)
 def client(
     name: str,
     token: str,
     url: str,
     pool_connections: int = 1,
     pool_maxsize: int = 1,
     connect_timeout: int = 30,
@@ -91,15 +92,14 @@
             pool_maxsize,
             connect_timeout,
             read_timeout,
         )
     )
 
 
-@lru_cache(maxsize=None)
 class Client:
     def __init__(self, core: Core):
         self._core = core
 
     def add_alert_note(
         self, alert_id: str, note: str
     ) -> Result[AddAlertNoteResp]:
```

### Comparing `pytmv1-0.5.3/src/pytmv1/core.py` & `pytmv1-0.5.4/src/pytmv1/core.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/exceptions.py` & `pytmv1-0.5.4/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/mapper.py` & `pytmv1-0.5.4/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/results.py` & `pytmv1-0.5.4/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/utils.py` & `pytmv1-0.5.4/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/model/commons.py` & `pytmv1-0.5.4/src/pytmv1/model/commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Status,
 )
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
         alias_generator = to_lower_camel
+        allow_populate_by_field_name = True
 
 
 class BaseConsumable(BaseModel):
     ...
 
 
 def _get_task_id(headers: List[Dict[str, str]]) -> Optional[str]:
```

### Comparing `pytmv1-0.5.3/src/pytmv1/model/enums.py` & `pytmv1-0.5.4/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/model/requests.py` & `pytmv1-0.5.4/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/src/pytmv1/model/responses.py` & `pytmv1-0.5.4/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/LICENSE.txt` & `pytmv1-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/README.md` & `pytmv1-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/pyproject.toml` & `pytmv1-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.3/PKG-INFO` & `pytmv1-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

