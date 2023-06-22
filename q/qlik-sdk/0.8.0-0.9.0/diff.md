# Comparing `tmp/qlik-sdk-0.8.0.tar.gz` & `tmp/qlik-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlik-sdk-0.8.0.tar", last modified: Tue Jul 19 12:14:53 2022, max compression
+gzip compressed data, was "qlik-sdk-0.9.0.tar", last modified: Fri Jul 22 13:19:13 2022, max compression
```

## Comparing `qlik-sdk-0.8.0.tar` & `qlik-sdk-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.879521 qlik-sdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-07-19 12:14:53.879521 qlik-sdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-07-19 12:14:53.879521 qlik-sdk-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.871521 qlik-sdk-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.875521 qlik-sdk-0.8.0/src/qlik_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.875521 qlik-sdk-0.8.0/src/qlik_sdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)    84483 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    29353 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Data_Files.py
--rw-r--r--   0 runner    (1001) docker     (121)    15670 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)    57511 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Items.py
--rw-r--r--   0 runner    (1001) docker     (121)   888555 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Qix.py
--rw-r--r--   0 runner    (1001) docker     (121)    11444 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Reloads.py
--rw-r--r--   0 runner    (1001) docker     (121)    40486 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    11925 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Themes.py
--rw-r--r--   0 runner    (1001) docker     (121)    27244 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/Users.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/auth_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/generate_signed_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.879521 qlik-sdk-0.8.0/src/qlik_sdk/interceptors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/interceptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/interceptors/retry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/interceptors/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/listable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/qlik.py
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8003 2022-07-19 12:13:56.000000 qlik-sdk-0.8.0/src/qlik_sdk/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 12:14:53.875521 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-07-19 12:14:53.000000 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-19 12:14:53.000000 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 12:14:53.000000 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-19 12:14:53.000000 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-19 12:14:53.000000 qlik-sdk-0.8.0/src/qlik_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.298231 qlik-sdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-07-22 13:19:13.298231 qlik-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-07-22 13:19:13.298231 qlik-sdk-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.294231 qlik-sdk-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.294231 qlik-sdk-0.9.0/src/qlik_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.298231 qlik-sdk-0.9.0/src/qlik_sdk/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)    79769 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29354 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Data_Files.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15418 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57932 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Items.py
+-rw-r--r--   0 runner    (1001) docker     (121)   902589 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Qix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11444 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Reloads.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41730 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Spaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11925 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Themes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27617 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/Users.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/auth_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/generate_signed_token.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.298231 qlik-sdk-0.9.0/src/qlik_sdk/interceptors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/interceptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/interceptors/retry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/interceptors/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/listable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8003 2022-07-22 13:18:24.000000 qlik-sdk-0.9.0/src/qlik_sdk/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 13:19:13.294231 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-07-22 13:19:13.000000 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-22 13:19:13.000000 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 13:19:13.000000 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-22 13:19:13.000000 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-22 13:19:13.000000 qlik-sdk-0.9.0/src/qlik_sdk.egg-info/top_level.txt
```

### Comparing `qlik-sdk-0.8.0/LICENSE` & `qlik-sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/PKG-INFO` & `qlik-sdk-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlik-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Software Development Kit for Qlik Cloud
 Author: qlik-sdk
 Author-email: dev.thulhu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qlik-sdk-0.8.0/README.md` & `qlik-sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/setup.cfg` & `qlik-sdk-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/__init__.py` & `qlik-sdk-0.9.0/src/qlik_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Apps.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
-import warnings
 from dataclasses import asdict, dataclass
 
 from ..auth import Auth, Config
 from ..listable import ListableResource
 from .Qix import Doc
 
 
@@ -248,40 +247,14 @@
             method="PUT",
             params={},
             data=data,
         )
         self.__init__(**response.json())
         return self
 
-    def get_reloads_logs(self, max_items: int = 10) -> ListableResource[ScriptLogMeta]:
-        """
-        Experimental
-        Retrieves the metadata about all script logs stored for an app.
-        Returns an array of ScriptLogMeta objects.
-
-        Parameters
-        ----------
-        """
-        warnings.warn("get_reloads_logs is experimental", UserWarning, stacklevel=2)
-
-        response = self.auth.rest(
-            path="/apps/{appId}/reloads/logs".replace("{appId}", self.attributes.id),
-            method="GET",
-            params={},
-            data=None,
-        )
-        return ListableResource(
-            response=response.json(),
-            cls=ScriptLogMeta,
-            auth=self.auth,
-            path="/apps/{appId}/reloads/logs".replace("{appId}", self.attributes.id),
-            max_items=max_items,
-            query_params={},
-        )
-
     def delete_space(self) -> NxApp:
         """
         Removes space from a specific app.
 
         Parameters
         ----------
         """
@@ -1530,37 +1503,14 @@
                 self_.statement = kvargs["statement"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class Log:
-    """
-
-    Attributes
-    ----------
-    log: str
-      Provides a link to download the log file.
-    """
-
-    log: str = None
-
-    def __init__(self_, **kvargs):
-        if "log" in kvargs:
-            if type(kvargs["log"]).__name__ is self_.__annotations__["log"]:
-                self_.log = kvargs["log"]
-            else:
-                self_.log = kvargs["log"]
-        for k, v in kvargs.items():
-            if k not in getattr(self_, "__annotations__", {}):
-                self_.__setattr__(k, v)
-
-
-@dataclass
 class NxAppCreatePrivileges:
     """
 
     Attributes
     ----------
     canCreate: bool
       Is set to true if the user has privileges to create the resource.
@@ -1867,91 +1817,14 @@
                 self_.targetId = kvargs["targetId"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class ScriptLogList:
-    """
-
-    Attributes
-    ----------
-    data: list[ScriptLogMeta]
-      Array of scriptLogMeta.
-    """
-
-    data: list[ScriptLogMeta] = None
-
-    def __init__(self_, **kvargs):
-        if "data" in kvargs:
-            if type(kvargs["data"]).__name__ is self_.__annotations__["data"]:
-                self_.data = kvargs["data"]
-            else:
-                self_.data = [ScriptLogMeta(**e) for e in kvargs["data"]]
-        for k, v in kvargs.items():
-            if k not in getattr(self_, "__annotations__", {}):
-                self_.__setattr__(k, v)
-
-
-@dataclass
-class ScriptLogMeta:
-    """
-
-    Attributes
-    ----------
-    duration: int
-      Duration of reload (ms).
-    endTime: str
-      Time when reload ended.
-    links: Log
-    reloadId: str
-      Reload identifier.
-    success: bool
-      True if the reload was successful.
-    """
-
-    duration: int = None
-    endTime: str = None
-    links: Log = None
-    reloadId: str = None
-    success: bool = None
-
-    def __init__(self_, **kvargs):
-        if "duration" in kvargs:
-            if type(kvargs["duration"]).__name__ is self_.__annotations__["duration"]:
-                self_.duration = kvargs["duration"]
-            else:
-                self_.duration = kvargs["duration"]
-        if "endTime" in kvargs:
-            if type(kvargs["endTime"]).__name__ is self_.__annotations__["endTime"]:
-                self_.endTime = kvargs["endTime"]
-            else:
-                self_.endTime = kvargs["endTime"]
-        if "links" in kvargs:
-            if type(kvargs["links"]).__name__ is self_.__annotations__["links"]:
-                self_.links = kvargs["links"]
-            else:
-                self_.links = Log(**kvargs["links"])
-        if "reloadId" in kvargs:
-            if type(kvargs["reloadId"]).__name__ is self_.__annotations__["reloadId"]:
-                self_.reloadId = kvargs["reloadId"]
-            else:
-                self_.reloadId = kvargs["reloadId"]
-        if "success" in kvargs:
-            if type(kvargs["success"]).__name__ is self_.__annotations__["success"]:
-                self_.success = kvargs["success"]
-            else:
-                self_.success = kvargs["success"]
-        for k, v in kvargs.items():
-            if k not in getattr(self_, "__annotations__", {}):
-                self_.__setattr__(k, v)
-
-
-@dataclass
 class SymbolFrequency:
     """
 
     Attributes
     ----------
     Frequency: int
       Frequency of the above symbol in the field
@@ -2244,83 +2117,82 @@
         obj = NxApp(**response.json())
         obj.auth = self.auth
         return obj
 
     def import_app(
         self,
         data: FileData,
-        name: str = None,
-        spaceId: str = None,
-        mode: str = None,
         appId: str = None,
-        fileId: str = None,
         fallbackName: str = None,
+        fileId: str = None,
+        mode: str = None,
+        name: str = None,
         NoData: bool = None,
+        spaceId: str = None,
     ) -> NxApp:
         """
         Imports an app into the system.
 
 
-        name: str
-          The name of the target app.
+        appId: str
+          The app ID of the target app when source is qvw file.
 
-        spaceId: str
-          The space ID of the target app.
+        fallbackName: str
+          The name of the target app when source does not have a specified name, applicable if source is qvw file.
+
+        fileId: str
+          The file ID to be downloaded from Temporary Content Service (TCS) and used during import.
 
         mode: str
-          The import mode. In `new` mode (default), the source app will be imported as a new app with generated attributes.
-          In `autoreplace` mode, the attributes from the source app will be retained and imported with the app.
-          The app-id is extracted from the source app and used as the target app-id. If the app exists, it will be replaced.
+          The import mode. In `new` mode (default), the source app will be imported as a new app.
+          In `autoreplace` mode, the app-id is extracted from the source app and used as the target app-id. If the app exists, it will be replaced.
           Approved objects in the target app that are not available in the source app will be removed.
           Non-approved objects in the target app will not be removed.
 
           One of:
 
           • NEW
 
           • AUTOREPLACE
 
-        appId: str
-          The app ID of the target app when source is qvw file.
-
-        fileId: str
-          The file ID to be downloaded from Temporary Content Service (TCS) and used during import.
-
-        fallbackName: str
-          The name of the target app when source does not have a specified name, applicable if source is qvw file.
+        name: str
+          The name of the target app.
 
         NoData: bool
           If NoData is true, the data of the existing app will be kept as is, otherwise it will be replaced by the new incoming data.
 
+        spaceId: str
+          The space ID of the target app.
+
         Parameters
         ----------
-        name: str = None
-        spaceId: str = None
-        mode: str = None
         appId: str = None
-        fileId: str = None
         fallbackName: str = None
+        fileId: str = None
+        mode: str = None
+        name: str = None
         NoData: bool = None
+        spaceId: str = None
         data: FileData
         """
         query_params = {}
-        if name is not None:
-            query_params["name"] = name
-        if spaceId is not None:
-            query_params["spaceId"] = spaceId
-        if mode is not None:
-            query_params["mode"] = mode
         if appId is not None:
             query_params["appId"] = appId
-        if fileId is not None:
-            query_params["fileId"] = fileId
         if fallbackName is not None:
             query_params["fallbackName"] = fallbackName
+        if fileId is not None:
+            query_params["fileId"] = fileId
+        if mode is not None:
+            query_params["mode"] = mode
+        if name is not None:
+            query_params["name"] = name
         if NoData is not None:
             query_params["NoData"] = NoData
+        if spaceId is not None:
+            query_params["spaceId"] = spaceId
 
         try:
             data = asdict(data)
         except:
             data = data
 
         response = self.auth.rest(
@@ -2512,45 +2384,14 @@
             path="/apps/{appId}/media/list/{path}".replace("{appId}", appId).replace(
                 "{path}", path
             ),
             max_items=max_items,
             query_params=query_params,
         )
 
-    def get_reloads_log(self, appId: str, reloadId: str) -> str:
-        """
-        Experimental
-        Retrieves the log of a specific reload.
-        Returns the log as "text/plain; charset=UTF-8".
-
-
-        appId: str
-          Identifier of the app.
-
-        reloadId: str
-          Identifier of the reload.
-
-        Parameters
-        ----------
-        appId: str
-        reloadId: str
-        """
-        warnings.warn("get_reloads_log is experimental", UserWarning, stacklevel=2)
-
-        response = self.auth.rest(
-            path="/apps/{appId}/reloads/logs/{reloadId}".replace(
-                "{appId}", appId
-            ).replace("{reloadId}", reloadId),
-            method="GET",
-            params={},
-            data=None,
-            stream=True,
-        )
-        return response
-
     def create_session_app(self, session_app_id: str) -> NxApp:
         """
         creates an empty session app
 
         Parameters
         ----------
         session_app_id: string the a self generated "app_id" prefixed with SessionApp_
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Data_Files.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Data_Files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
 import io
 import json
 from dataclasses import asdict, dataclass
 
@@ -629,83 +629,83 @@
 class DataFiles:
     def __init__(self, config: Config) -> None:
         self.config = config
         self.auth = Auth(config)
 
     def get_data_files(
         self,
-        connectionId: str = None,
+        allowInternalFiles: bool = None,
         appId: str = None,
-        name: str = None,
-        page: str = None,
+        connectionId: str = None,
         limit: int = 20,
+        name: str = None,
         ownerId: str = None,
-        allowInternalFiles: bool = None,
+        page: str = None,
         sort: str = None,
         max_items: int = 20,
     ) -> ListableResource[DataFileUploadResponse]:
         """
         Get descriptive info for the specified data files.
 
 
-        connectionId: str
-          Return files that reside in the space referenced by the specified DataFiles connection. If this parameter
-          is not specified, the user's personal space is implied.
+        allowInternalFiles: bool
+          If set to false, do not return data files with internal extensions else return all the data files.
 
         appId: str
           Only return files scoped to the specified app. If this parameter is not specified, only files that are not
           scoped to any app are returned. "*" implies all app-scoped files are returned.
 
-        name: str
-          Filter the list of files returned to the given file name.
-
-        page: str
-          If present, the cursor that starts the page of data that is returned.
+        connectionId: str
+          Return files that reside in the space referenced by the specified DataFiles connection. If this parameter
+          is not specified, the user's personal space is implied.
 
         limit: int
           If present, the maximum number of data files to return.
 
+        name: str
+          Filter the list of files returned to the given file name.
+
         ownerId: str
           If present, fetch the data files for the specified owner. If a connectionId is specified in this case, the
           returned list is constrained to the specified space. If connectionId is not specified, then all files owned
           by the specified user are returned regardless of the personal space that a given file resides in.
 
-        allowInternalFiles: bool
-          If set to false, do not return data files with internal extensions else return all the data files.
+        page: str
+          If present, the cursor that starts the page of data that is returned.
 
         sort: str
           The name of the field used to sort the result. By default, the sort order is ascending. Putting a '+' prefix on
           the sort field name explicitly indicates ascending sort order. A '-' prefix indicates a descending sort order.
 
         Parameters
         ----------
-        connectionId: str = None
+        allowInternalFiles: bool = None
         appId: str = None
-        name: str = None
-        page: str = None
+        connectionId: str = None
         limit: int = 20
+        name: str = None
         ownerId: str = None
-        allowInternalFiles: bool = None
+        page: str = None
         sort: str = None
         """
         query_params = {}
-        if connectionId is not None:
-            query_params["connectionId"] = connectionId
+        if allowInternalFiles is not None:
+            query_params["allowInternalFiles"] = allowInternalFiles
         if appId is not None:
             query_params["appId"] = appId
-        if name is not None:
-            query_params["name"] = name
-        if page is not None:
-            query_params["page"] = page
+        if connectionId is not None:
+            query_params["connectionId"] = connectionId
         if limit is not None:
             query_params["limit"] = limit
+        if name is not None:
+            query_params["name"] = name
         if ownerId is not None:
             query_params["ownerId"] = ownerId
-        if allowInternalFiles is not None:
-            query_params["allowInternalFiles"] = allowInternalFiles
+        if page is not None:
+            query_params["page"] = page
         if sort is not None:
             query_params["sort"] = sort
 
         response = self.auth.rest(
             path="/data-files",
             method="GET",
             params=query_params,
@@ -807,75 +807,75 @@
             params={},
             data=data,
         )
 
     def get_connections(
         self,
         appId: str = None,
+        limit: int = 20,
         name: str = None,
-        spaceId: str = None,
-        personal: bool = None,
         page: str = None,
-        limit: int = 20,
+        personal: bool = None,
         sort: str = None,
+        spaceId: str = None,
         max_items: int = 20,
     ) -> ListableResource[ConnectionsResponse]:
         """
         Get the list of built-in connections used by the engine to load/write data files.
         The non-filtered list contains a set of hardcoded connections, along with one connection per team space that
         the given user has access to.
 
 
         appId: str
           If present, get connections with connection strings that are scoped to the given app ID.
 
+        limit: int
+          If present, the maximum number of data file connection records to return.
+
         name: str
           If present, only return connections with the given name.
 
-        spaceId: str
-          If present, only return the connection that accesses data files in the specified space.
-
-        personal: bool
-          If true, only return the connections that access data in a personal space. Default is false.
-
         page: str
           If present, the cursor that starts the page of data that is returned.
 
-        limit: int
-          If present, the maximum number of data file connection records to return.
+        personal: bool
+          If true, only return the connections that access data in a personal space. Default is false.
 
         sort: str
           The name of the field used to sort the result. By default, the sort is ascending. Putting a '+' prefix on
           the sort field name explicitly indicates ascending sort order. A '-' prefix indicates a descending sort order.
 
+        spaceId: str
+          If present, only return the connection that accesses data files in the specified space.
+
         Parameters
         ----------
         appId: str = None
+        limit: int = 20
         name: str = None
-        spaceId: str = None
-        personal: bool = None
         page: str = None
-        limit: int = 20
+        personal: bool = None
         sort: str = None
+        spaceId: str = None
         """
         query_params = {}
         if appId is not None:
             query_params["appId"] = appId
+        if limit is not None:
+            query_params["limit"] = limit
         if name is not None:
             query_params["name"] = name
-        if spaceId is not None:
-            query_params["spaceId"] = spaceId
-        if personal is not None:
-            query_params["personal"] = personal
         if page is not None:
             query_params["page"] = page
-        if limit is not None:
-            query_params["limit"] = limit
+        if personal is not None:
+            query_params["personal"] = personal
         if sort is not None:
             query_params["sort"] = sort
+        if spaceId is not None:
+            query_params["spaceId"] = spaceId
 
         response = self.auth.rest(
             path="/data-files/connections",
             method="GET",
             params=query_params,
             data=None,
         )
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Extensions.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Extensions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
 import io
 import json
 from dataclasses import asdict, dataclass
 
@@ -266,17 +266,15 @@
         self.auth.rest(
             path="/extensions/{id}".replace("{id}", self.id),
             method="DELETE",
             params={},
             data=None,
         )
 
-    def patchs(
-        self, file: io.BufferedReader, data: Extension = None, max_items: int = 10
-    ) -> ListableResource[Extension]:
+    def patch(self, file: io.BufferedReader, data: Extension = None) -> Extension:
         """
         Updates a specific extension with provided data. If a file is provided, the data field is not required.
 
         Parameters
         ----------
         """
 
@@ -293,22 +291,16 @@
         response = self.auth.rest(
             path="/extensions/{id}".replace("{id}", self.id),
             method="PATCH",
             params={},
             data=None,
             files=files_dict,
         )
-        return ListableResource(
-            response=response.json(),
-            cls=Extension,
-            auth=self.auth,
-            path="/extensions/{id}".replace("{id}", self.id),
-            max_items=max_items,
-            query_params={},
-        )
+        self.__init__(**response.json())
+        return self
 
     def get_file(self) -> None:
         """
         Downloads the extension as an archive.
 
         Parameters
         ----------
@@ -461,32 +453,32 @@
             params={},
             data=None,
         )
         obj = Extension(**response.json())
         obj.auth = self.auth
         return obj
 
-    def get_file(self, id: str, filepath: str) -> None:
+    def get_file(self, filepath: str, id: str) -> None:
         """
         Downloads a file from the extension archive.
 
 
-        id: str
-          Extension identifier or its qextFilename.
-
         filepath: str
           Path to the file archive for the specified extension archive. Folders separated with forward slashes.
 
+        id: str
+          Extension identifier or its qextFilename.
+
         Parameters
         ----------
-        id: str
         filepath: str
+        id: str
         """
 
         self.auth.rest(
-            path="/extensions/{id}/file/{filepath}".replace("{id}", id).replace(
+            path="/extensions/{id}/file/{filepath}".replace(
                 "{filepath}", filepath
-            ),
+            ).replace("{id}", id),
             method="GET",
             params={},
             data=None,
         )
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Items.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import asdict, dataclass
 
 from ..auth import Auth, Config
@@ -331,52 +331,52 @@
             data=data,
         )
         self.__init__(**response.json())
         return self
 
     def get_collections(
         self,
+        limit: int = None,
+        name: str = None,
         next: str = None,
         prev: str = None,
-        limit: int = None,
-        sort: str = None,
         query: str = None,
+        sort: str = None,
         type: str = None,
-        name: str = None,
         max_items: int = 10,
     ) -> ListableResource[CollectionResultResponseBody]:
         """
         Returns the collections of an item.
         Finds and returns the collections of an item. This endpoint does not return the user's favorites collection.
 
         Parameters
         ----------
+        limit: int = None
+        name: str = None
         next: str = None
         prev: str = None
-        limit: int = None
-        sort: str = None
         query: str = None
+        sort: str = None
         type: str = None
-        name: str = None
         """
         query_params = {}
+        if limit is not None:
+            query_params["limit"] = limit
+        if name is not None:
+            query_params["name"] = name
         if next is not None:
             query_params["next"] = next
         if prev is not None:
             query_params["prev"] = prev
-        if limit is not None:
-            query_params["limit"] = limit
-        if sort is not None:
-            query_params["sort"] = sort
         if query is not None:
             query_params["query"] = query
+        if sort is not None:
+            query_params["sort"] = sort
         if type is not None:
             query_params["type"] = type
-        if name is not None:
-            query_params["name"] = name
 
         response = self.auth.rest(
             path="/items/{itemId}/collections".replace("{itemId}", self.id),
             method="GET",
             params=query_params,
             data=None,
         )
@@ -387,44 +387,44 @@
             path="/items/{itemId}/collections".replace("{itemId}", self.id),
             max_items=max_items,
             query_params=query_params,
         )
 
     def get_publisheditems(
         self,
+        limit: int = None,
         next: str = None,
         prev: str = None,
-        limit: int = None,
-        sort: str = None,
         resourceType: str = None,
+        sort: str = None,
         max_items: int = 10,
     ) -> ListableResource[CollectionResultResponseBody]:
         """
         Returns published items for a given item.
         Finds and returns the published items for a given item.
 
         Parameters
         ----------
+        limit: int = None
         next: str = None
         prev: str = None
-        limit: int = None
-        sort: str = None
         resourceType: str = None
+        sort: str = None
         """
         query_params = {}
+        if limit is not None:
+            query_params["limit"] = limit
         if next is not None:
             query_params["next"] = next
         if prev is not None:
             query_params["prev"] = prev
-        if limit is not None:
-            query_params["limit"] = limit
-        if sort is not None:
-            query_params["sort"] = sort
         if resourceType is not None:
             query_params["resourceType"] = resourceType
+        if sort is not None:
+            query_params["sort"] = sort
 
         response = self.auth.rest(
             path="/items/{itemId}/publisheditems".replace("{itemId}", self.id),
             method="GET",
             params=query_params,
             data=None,
         )
@@ -1368,156 +1368,163 @@
 class Items:
     def __init__(self, config: Config) -> None:
         self.config = config
         self.auth = Auth(config)
 
     def get_items(
         self,
-        next: str = None,
-        prev: str = None,
-        limit: int = None,
-        sort: str = None,
-        resourceType: str = None,
-        resourceSubType: str = None,
-        resourceId: str = None,
-        resourceLink: str = None,
-        spaceId: str = None,
-        shared: bool = None,
         collectionId: str = None,
         createdByUserId: str = None,
+        id: str = None,
+        limit: int = None,
+        name: str = None,
+        next: str = None,
         notCreatedByUserId: str = None,
-        ownerId: str = None,
         notOwnerId: str = None,
-        id: str = None,
+        ownerId: str = None,
+        prev: str = None,
         query: str = None,
-        name: str = None,
+        resourceId: str = None,
+        resourceIds: str = None,
+        resourceLink: str = None,
+        resourceSubType: str = None,
+        resourceType: str = None,
+        shared: bool = None,
+        sort: str = None,
+        spaceId: str = None,
         noActions: bool = None,
         max_items: int = 10,
     ) -> ListableResource[ItemResultResponseBody]:
         """
         Retrieves items that the user has access to.
         Finds and returns items that the user has access to.
 
 
-        next: str
-          The cursor to the next page of resources. Provide either the next or prev cursor, but not both.
+        collectionId: str
+          The collection's unique identifier.
 
-        prev: str
-          The cursor to the previous page of resources. Provide either the next or prev cursor, but not both.
+        createdByUserId: str
+          User's unique identifier.
+
+        id: str
+          The item's unique identifier.
 
         limit: int
           The maximum number of resources to return for a request. The limit must be an integer between 1 and 100 (inclusive).
 
-        sort: str
-          The property of a resource to sort on (default sort is +createdAt). The supported properties are createdAt, updatedAt, and name. A property must be prefixed by + or - to indicate ascending or descending sort order respectively.
+        name: str
+          The case-insensitive string used to search for a resource by name.
 
-        resourceType: str
-          The case-sensitive string used to filter items by resourceType(s). For example '?resourceType=app,qvapp'
+        next: str
+          The cursor to the next page of resources. Provide either the next or prev cursor, but not both.
 
-        resourceSubType: str
-          the case-sensitive string used to filter items by resourceSubType(s). For example '?resourceSubType=chart-monitoring,qix-df,qvd'
+        notCreatedByUserId: str
+          User's unique identifier.
 
-        resourceId: str
-          The case-sensitive string used to search for an item by resourceId. If resourceId is provided, then resourceType must be provided. Provide either the resourceId or resourceLink, but not both.
+        notOwnerId: str
+          Owner identifier.
 
-        resourceLink: str
-          The case-sensitive string used to search for an item by resourceLink. If resourceLink is provided, then resourceType must be provided. Provide either the resourceId or resourceLink, but not both.
+        ownerId: str
+          Owner identifier.
 
-        spaceId: str
-          The space's unique identifier (supports \'personal\' as spaceId).
+        prev: str
+          The cursor to the previous page of resources. Provide either the next or prev cursor, but not both.
 
-        shared: bool
-          Whether or not to return items in a shared space.
+        query: str
+          The case-insensitive string used to search for a resource by name or description.
 
-        collectionId: str
-          The collection's unique identifier.
+        resourceId: str
+          The case-sensitive string used to search for an item by resourceId. If resourceId is provided, then resourceType must be provided. Provide either the resourceId or resourceLink, but not both.
 
-        createdByUserId: str
-          User's unique identifier.
+        resourceIds: str
+          The case-sensitive strings used to search for an item by resourceIds. The maximum number of resourceIds it supports is 100. If resourceIds is provided, then resourceType must be provided. For example '?resourceIds=appId1,appId2'
 
-        notCreatedByUserId: str
-          User's unique identifier.
+        resourceLink: str
+          The case-sensitive string used to search for an item by resourceLink. If resourceLink is provided, then resourceType must be provided. Provide either the resourceId or resourceLink, but not both.
 
-        ownerId: str
-          Owner identifier.
+        resourceSubType: str
+          the case-sensitive string used to filter items by resourceSubType(s). For example '?resourceSubType=chart-monitoring,qix-df,qvd'
 
-        notOwnerId: str
-          Owner identifier.
+        resourceType: str
+          The case-sensitive string used to filter items by resourceType(s). For example '?resourceType=app,qvapp'
 
-        id: str
-          The item's unique identifier.
+        shared: bool
+          Whether or not to return items in a shared space.
 
-        query: str
-          The case-insensitive string used to search for a resource by name or description.
+        sort: str
+          The property of a resource to sort on (default sort is +createdAt). The supported properties are createdAt, updatedAt, and name. A property must be prefixed by + or - to indicate ascending or descending sort order respectively.
 
-        name: str
-          The case-insensitive string used to search for a resource by name.
+        spaceId: str
+          The space's unique identifier (supports \'personal\' as spaceId).
 
         noActions: bool
           If set to true, the user's available actions for each item will not be evaluated meaning the actions-array will be omitted from the response (reduces response time).
 
         Parameters
         ----------
-        next: str = None
-        prev: str = None
-        limit: int = None
-        sort: str = None
-        resourceType: str = None
-        resourceSubType: str = None
-        resourceId: str = None
-        resourceLink: str = None
-        spaceId: str = None
-        shared: bool = None
         collectionId: str = None
         createdByUserId: str = None
+        id: str = None
+        limit: int = None
+        name: str = None
+        next: str = None
         notCreatedByUserId: str = None
-        ownerId: str = None
         notOwnerId: str = None
-        id: str = None
+        ownerId: str = None
+        prev: str = None
         query: str = None
-        name: str = None
+        resourceId: str = None
+        resourceIds: str = None
+        resourceLink: str = None
+        resourceSubType: str = None
+        resourceType: str = None
+        shared: bool = None
+        sort: str = None
+        spaceId: str = None
         noActions: bool = None
         """
         query_params = {}
-        if next is not None:
-            query_params["next"] = next
-        if prev is not None:
-            query_params["prev"] = prev
-        if limit is not None:
-            query_params["limit"] = limit
-        if sort is not None:
-            query_params["sort"] = sort
-        if resourceType is not None:
-            query_params["resourceType"] = resourceType
-        if resourceSubType is not None:
-            query_params["resourceSubType"] = resourceSubType
-        if resourceId is not None:
-            query_params["resourceId"] = resourceId
-        if resourceLink is not None:
-            query_params["resourceLink"] = resourceLink
-        if spaceId is not None:
-            query_params["spaceId"] = spaceId
-        if shared is not None:
-            query_params["shared"] = shared
         if collectionId is not None:
             query_params["collectionId"] = collectionId
         if createdByUserId is not None:
             query_params["createdByUserId"] = createdByUserId
+        if id is not None:
+            query_params["id"] = id
+        if limit is not None:
+            query_params["limit"] = limit
+        if name is not None:
+            query_params["name"] = name
+        if next is not None:
+            query_params["next"] = next
         if notCreatedByUserId is not None:
             query_params["notCreatedByUserId"] = notCreatedByUserId
-        if ownerId is not None:
-            query_params["ownerId"] = ownerId
         if notOwnerId is not None:
             query_params["notOwnerId"] = notOwnerId
-        if id is not None:
-            query_params["id"] = id
+        if ownerId is not None:
+            query_params["ownerId"] = ownerId
+        if prev is not None:
+            query_params["prev"] = prev
         if query is not None:
             query_params["query"] = query
-        if name is not None:
-            query_params["name"] = name
+        if resourceId is not None:
+            query_params["resourceId"] = resourceId
+        if resourceIds is not None:
+            query_params["resourceIds"] = resourceIds
+        if resourceLink is not None:
+            query_params["resourceLink"] = resourceLink
+        if resourceSubType is not None:
+            query_params["resourceSubType"] = resourceSubType
+        if resourceType is not None:
+            query_params["resourceType"] = resourceType
+        if shared is not None:
+            query_params["shared"] = shared
+        if sort is not None:
+            query_params["sort"] = sort
+        if spaceId is not None:
+            query_params["spaceId"] = spaceId
         if noActions is not None:
             query_params["noActions"] = noActions
 
         response = self.auth.rest(
             path="/items",
             method="GET",
             params=query_params,
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Qix.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Qix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# QIX 12.1351.0
+# QIX 12.1414.0
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass
 
 from ..rpc import RpcSession
@@ -114,14 +114,90 @@
                 self_.qEndIndex = kvargs["qEndIndex"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
+class BookmarkFieldVerifyResultState:
+    """
+
+    Attributes
+    ----------
+    """
+
+    def __init__(self_, **kvargs):
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
+class BookmarkFieldVerifyWarning:
+    """
+
+    Attributes
+    ----------
+    qState: str
+      Alternate State *
+    qField: str
+      Field Name *
+    qVerifyResult: str
+      Field/values verfication result *
+      Defines result of ApplyAndVerify.
+      One of:
+
+      • NOT_VERIFIED
+
+      • FIELD_VALUE_MATCH_ALL
+
+      • FIELD_MISSING
+
+      • FIELD_VALUE_MISSING
+    qWarningMsg: str
+    """
+
+    qState: str = None
+    qField: str = None
+    qVerifyResult: str = "NOT_VERIFIED"
+    qWarningMsg: str = None
+
+    def __init__(self_, **kvargs):
+        if "qState" in kvargs:
+            if type(kvargs["qState"]).__name__ is self_.__annotations__["qState"]:
+                self_.qState = kvargs["qState"]
+            else:
+                self_.qState = kvargs["qState"]
+        if "qField" in kvargs:
+            if type(kvargs["qField"]).__name__ is self_.__annotations__["qField"]:
+                self_.qField = kvargs["qField"]
+            else:
+                self_.qField = kvargs["qField"]
+        if "qVerifyResult" in kvargs:
+            if (
+                type(kvargs["qVerifyResult"]).__name__
+                is self_.__annotations__["qVerifyResult"]
+            ):
+                self_.qVerifyResult = kvargs["qVerifyResult"]
+            else:
+                self_.qVerifyResult = kvargs["qVerifyResult"]
+        if "qWarningMsg" in kvargs:
+            if (
+                type(kvargs["qWarningMsg"]).__name__
+                is self_.__annotations__["qWarningMsg"]
+            ):
+                self_.qWarningMsg = kvargs["qWarningMsg"]
+            else:
+                self_.qWarningMsg = kvargs["qWarningMsg"]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
 class CalendarStrings:
     """
 
     Attributes
     ----------
     qDayNames: list[str]
       List of short day names.
@@ -771,18 +847,21 @@
 
     Attributes
     ----------
     qSuccess: bool
       The reload is successful if True.
     qScriptLogFile: str
       Path to the script log file.
+    qEndedWithMemoryConstraint: bool
+      true if memory limits were exhausted during reload.
     """
 
     qSuccess: bool = None
     qScriptLogFile: str = None
+    qEndedWithMemoryConstraint: bool = None
 
     def __init__(self_, **kvargs):
         if "qSuccess" in kvargs:
             if type(kvargs["qSuccess"]).__name__ is self_.__annotations__["qSuccess"]:
                 self_.qSuccess = kvargs["qSuccess"]
             else:
                 self_.qSuccess = kvargs["qSuccess"]
@@ -790,14 +869,22 @@
             if (
                 type(kvargs["qScriptLogFile"]).__name__
                 is self_.__annotations__["qScriptLogFile"]
             ):
                 self_.qScriptLogFile = kvargs["qScriptLogFile"]
             else:
                 self_.qScriptLogFile = kvargs["qScriptLogFile"]
+        if "qEndedWithMemoryConstraint" in kvargs:
+            if (
+                type(kvargs["qEndedWithMemoryConstraint"]).__name__
+                is self_.__annotations__["qEndedWithMemoryConstraint"]
+            ):
+                self_.qEndedWithMemoryConstraint = kvargs["qEndedWithMemoryConstraint"]
+            else:
+                self_.qEndedWithMemoryConstraint = kvargs["qEndedWithMemoryConstraint"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class DriveType:
@@ -3318,30 +3405,41 @@
 
     Attributes
     ----------
     qTypes: list[str]
       List of object types.
     qData: JsonObject
       Set of data.
+    qIncludePatches: bool
+      Include the bookmark patches. Patches can be very large and may make the list result unmanageable.
     """
 
     qTypes: list[str] = None
     qData: JsonObject = None
+    qIncludePatches: bool = None
 
     def __init__(self_, **kvargs):
         if "qTypes" in kvargs:
             if type(kvargs["qTypes"]).__name__ is self_.__annotations__["qTypes"]:
                 self_.qTypes = kvargs["qTypes"]
             else:
                 self_.qTypes = kvargs["qTypes"]
         if "qData" in kvargs:
             if type(kvargs["qData"]).__name__ is self_.__annotations__["qData"]:
                 self_.qData = kvargs["qData"]
             else:
                 self_.qData = JsonObject(**kvargs["qData"])
+        if "qIncludePatches" in kvargs:
+            if (
+                type(kvargs["qIncludePatches"]).__name__
+                is self_.__annotations__["qIncludePatches"]
+            ):
+                self_.qIncludePatches = kvargs["qIncludePatches"]
+            else:
+                self_.qIncludePatches = kvargs["qIncludePatches"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class NxGetObjectOptions:
@@ -4633,14 +4731,51 @@
                 self_.qId = kvargs["qId"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
+class NxTempBookmarkOptions:
+    """
+
+    Attributes
+    ----------
+    qIncludeVariables: bool
+      IncludeVariables If true all variables will be stored in the temporary bookmark
+    qIncludeAllPatches: bool
+      IncludeAllPatches If true all patches will be stored in the temporary bookmark, if false ObjectIdsToPatch will determine what patches to include
+    """
+
+    qIncludeVariables: bool = None
+    qIncludeAllPatches: bool = None
+
+    def __init__(self_, **kvargs):
+        if "qIncludeVariables" in kvargs:
+            if (
+                type(kvargs["qIncludeVariables"]).__name__
+                is self_.__annotations__["qIncludeVariables"]
+            ):
+                self_.qIncludeVariables = kvargs["qIncludeVariables"]
+            else:
+                self_.qIncludeVariables = kvargs["qIncludeVariables"]
+        if "qIncludeAllPatches" in kvargs:
+            if (
+                type(kvargs["qIncludeAllPatches"]).__name__
+                is self_.__annotations__["qIncludeAllPatches"]
+            ):
+                self_.qIncludeAllPatches = kvargs["qIncludeAllPatches"]
+            else:
+                self_.qIncludeAllPatches = kvargs["qIncludeAllPatches"]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
 class NxTickCell:
     """
 
     Attributes
     ----------
     qText: str
       Tick's label.
@@ -6800,14 +6935,79 @@
     def __init__(self_, **kvargs):
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
+class TransformAppParameters:
+    """
+
+    Attributes
+    ----------
+    qName: str
+      The name (title) of the application
+    qSpaceId: str
+      ID of the space where the app is to be created. Empty value implies Personal space
+    qScriptParameterPrefix: str
+      Prefix to be used on inserted ScriptParameters, only applicable for template apps
+    """
+
+    qName: str = None
+    qSpaceId: str = None
+    qScriptParameterPrefix: str = None
+
+    def __init__(self_, **kvargs):
+        if "qName" in kvargs:
+            if type(kvargs["qName"]).__name__ is self_.__annotations__["qName"]:
+                self_.qName = kvargs["qName"]
+            else:
+                self_.qName = kvargs["qName"]
+        if "qSpaceId" in kvargs:
+            if type(kvargs["qSpaceId"]).__name__ is self_.__annotations__["qSpaceId"]:
+                self_.qSpaceId = kvargs["qSpaceId"]
+            else:
+                self_.qSpaceId = kvargs["qSpaceId"]
+        if "qScriptParameterPrefix" in kvargs:
+            if (
+                type(kvargs["qScriptParameterPrefix"]).__name__
+                is self_.__annotations__["qScriptParameterPrefix"]
+            ):
+                self_.qScriptParameterPrefix = kvargs["qScriptParameterPrefix"]
+            else:
+                self_.qScriptParameterPrefix = kvargs["qScriptParameterPrefix"]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
+class TransformAppResult:
+    """
+
+    Attributes
+    ----------
+    qAppId: str
+      ID of created App
+    """
+
+    qAppId: str = None
+
+    def __init__(self_, **kvargs):
+        if "qAppId" in kvargs:
+            if type(kvargs["qAppId"]).__name__ is self_.__annotations__["qAppId"]:
+                self_.qAppId = kvargs["qAppId"]
+            else:
+                self_.qAppId = kvargs["qAppId"]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
 class UndoInfo:
     """
     Displays information about the number of possible undos and redos. Is the layout for UndoInfoDef.
 
     Attributes
     ----------
     qUndoCount: int
@@ -7508,14 +7708,16 @@
       • EXT or FUNC_GROUP_EXTERNAL
 
       • PROB or FUNC_GROUP_PROBABILITY
 
       • ARRAY or FUNC_GROUP_ARRAY
 
       • LEG or FUNC_GROUP_LEGACY
+
+      • DB or FUNC_GROUP_DB_NATIVE
     qFieldFlag: bool
       If set to true, the definition is related to a field.
       This parameter is optional. The default value is false.
     qMT: str
       Type of the data.
 
       One of:
@@ -7656,40 +7858,87 @@
                 self_.qFGList = [FunctionGroup(**e) for e in kvargs["qFGList"]]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
+class BookmarkApplyAndVerifyResult:
+    """
+
+    Attributes
+    ----------
+    qApplySuccess: bool
+      Apply successfully or not *
+    qWarnings: list[BookmarkFieldVerifyWarning]
+      Field values verfication result *
+    """
+
+    qApplySuccess: bool = None
+    qWarnings: list[BookmarkFieldVerifyWarning] = None
+
+    def __init__(self_, **kvargs):
+        if "qApplySuccess" in kvargs:
+            if (
+                type(kvargs["qApplySuccess"]).__name__
+                is self_.__annotations__["qApplySuccess"]
+            ):
+                self_.qApplySuccess = kvargs["qApplySuccess"]
+            else:
+                self_.qApplySuccess = kvargs["qApplySuccess"]
+        if "qWarnings" in kvargs:
+            if type(kvargs["qWarnings"]).__name__ is self_.__annotations__["qWarnings"]:
+                self_.qWarnings = kvargs["qWarnings"]
+            else:
+                self_.qWarnings = [
+                    BookmarkFieldVerifyWarning(**e) for e in kvargs["qWarnings"]
+                ]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
 class BookmarkListDef:
     """
     Defines the list of bookmarks.
 
     Attributes
     ----------
     qType: str
       Type of the list.
     qData: JsonObject
       Data
+    qIncludePatches: bool
+      Include the bookmark patches. Patches can be very large and may make the list result unmanageable.
     """
 
     qType: str = None
     qData: JsonObject = None
+    qIncludePatches: bool = None
 
     def __init__(self_, **kvargs):
         if "qType" in kvargs:
             if type(kvargs["qType"]).__name__ is self_.__annotations__["qType"]:
                 self_.qType = kvargs["qType"]
             else:
                 self_.qType = kvargs["qType"]
         if "qData" in kvargs:
             if type(kvargs["qData"]).__name__ is self_.__annotations__["qData"]:
                 self_.qData = kvargs["qData"]
             else:
                 self_.qData = JsonObject(**kvargs["qData"])
+        if "qIncludePatches" in kvargs:
+            if (
+                type(kvargs["qIncludePatches"]).__name__
+                is self_.__annotations__["qIncludePatches"]
+            ):
+                self_.qIncludePatches = kvargs["qIncludePatches"]
+            else:
+                self_.qIncludePatches = kvargs["qIncludePatches"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class BookmarkVariableItem:
@@ -9445,14 +9694,38 @@
         """
         params = {}
         params["qId"] = qId
         handle = -1 if not hasattr(self, "qHandle") else self.qHandle
         response = self._session.send("ApplyBookmark", handle, **params)["qSuccess"]
         return response
 
+    def apply_and_verify_bookmark(self, qId: str) -> BookmarkApplyAndVerifyResult:
+        """
+        Experimental
+        Applies a bookmark and verifies result dataset against originally selected values.
+        The operation is successful if qApplySuccess is set to true. qWarnings lists state and field with unmatching values
+
+
+        qId: str
+          Identifier of the bookmark.
+
+        """
+        warnings.warn(
+            "ApplyAndVerifyBookmark is experimental", UserWarning, stacklevel=2
+        )
+        params = {}
+        params["qId"] = qId
+        handle = -1 if not hasattr(self, "qHandle") else self.qHandle
+        response = self._session.send("ApplyAndVerifyBookmark", handle, **params)[
+            "qResult"
+        ]
+        obj = BookmarkApplyAndVerifyResult(**response)
+        obj._session = self._session
+        return obj
+
     def clone_bookmark(self, qId: str) -> str:
         """
         Clones a bookmark.
         The identifier is set by the engine.
 
 
         qId: str
@@ -10275,14 +10548,16 @@
 
         • QVX for QVX file
 
         • JSON for JSON format
 
         • KML for KML file
 
+        • PARQUET for PARQUET file
+
         FileType:
 
         Recognized file formats are:
 
         • CSV for Delimited
 
         • FIX for Fixed Record
@@ -10301,14 +10576,16 @@
 
         • QVX for QVX file
 
         • JSON for JSON format
 
         • KML for KML file
 
+        • PARQUET for PARQUET file
+
 
         qConnectionId: str
           Identifier of the connection file.
 
         qRelativePath: str
           Path of the connection file.
 
@@ -10351,14 +10628,16 @@
 
         • QVX for QVX file
 
         • JSON for JSON format
 
         • KML for KML file
 
+        • PARQUET for PARQUET file
+
 
         qConnectionId: str
           Identifier of the connection.
 
         qRelativePath: str
           Path of the connection file.
 
@@ -10407,14 +10686,16 @@
 
         • QVX for QVX file
 
         • JSON for JSON format
 
         • KML for KML file
 
+        • PARQUET for PARQUET file
+
 
         qConnectionId: str
           Identifier of the connection.
 
         qRelativePath: str
           Path of the connection file.
 
@@ -10468,14 +10749,16 @@
 
         • QVX for QVX file
 
         • JSON for JSON format
 
         • KML for KML file
 
+        • PARQUET for PARQUET file
+
 
         qConnectionId: str
           Identifier of the connection.
 
         qRelativePath: str
           Path of the connection file.
 
@@ -11138,14 +11421,82 @@
         """
         params = {}
         params["qProhibit"] = qProhibit
         handle = -1 if not hasattr(self, "qHandle") else self.qHandle
         response = self._session.send("SetProhibitBinaryLoad", handle, **params)
         return response
 
+    def transform_app(
+        self, qDstParameters: TransformAppParameters
+    ) -> TransformAppResult:
+        """
+        Transform current app into an instance of the targeted mode
+
+
+        qDstParameters: TransformAppParameters
+          Attributes that should be set in the new app.
+
+        """
+        params = {}
+        params["qDstParameters"] = qDstParameters
+        handle = -1 if not hasattr(self, "qHandle") else self.qHandle
+        response = self._session.send("TransformApp", handle, **params)["qResult"]
+        obj = TransformAppResult(**response)
+        obj._session = self._session
+        return obj
+
+    def create_temporary_bookmark(
+        self, qOptions: NxTempBookmarkOptions, qObjectIdsToPatch: list[str] = None
+    ) -> object:
+        """
+        Experimental
+        Create temporary bookmark
+        CreateTemporaryBookmark method is only supported in SaaS Editions of Qlik Sense.
+
+
+        qOptions: NxTempBookmarkOptions
+          Options for the temporary bookmark
+
+        qObjectIdsToPatch: list[str]
+          Add softpatches for this objects if available. If empty all softpatches are added to the bookmark. This is ignored if IncludePatches is false.
+
+        """
+        warnings.warn(
+            "CreateTemporaryBookmark is experimental", UserWarning, stacklevel=2
+        )
+        params = {}
+        params["qOptions"] = qOptions
+        if qObjectIdsToPatch is not None:
+            params["qObjectIdsToPatch"] = qObjectIdsToPatch
+        handle = -1 if not hasattr(self, "qHandle") else self.qHandle
+        response = self._session.send("CreateTemporaryBookmark", handle, **params)
+        return response
+
+    def apply_temporary_bookmark(self, qId: str) -> bool:
+        """
+        Experimental
+        Apply temporary bookmark identified by Id.
+        ApplyTemporaryBookmark method is only supported in SaaS Editions of Qlik Sense.
+
+
+        qId: str
+          Identifier of the temporary selection state
+
+        """
+        warnings.warn(
+            "ApplyTemporaryBookmark is experimental", UserWarning, stacklevel=2
+        )
+        params = {}
+        params["qId"] = qId
+        handle = -1 if not hasattr(self, "qHandle") else self.qHandle
+        response = self._session.send("ApplyTemporaryBookmark", handle, **params)[
+            "qReturn"
+        ]
+        return response
+
     def open(self, qNoData: bool = None) -> RpcSession:
         if not hasattr(self, "_session"):
             self._session = self.auth.rpc(self.attributes.id)
         session = self._session.open()
         params = {"qDocName": self.attributes.id}
         if qNoData is not None:
             params["qNoData"] = qNoData
@@ -12290,14 +12641,16 @@
 
     • QVX for QVX file
 
     • JSON for JSON format
 
     • KML for KML file
 
+    • PARQUET for PARQUET file
+
     Attributes
     ----------
     qType: str
       Type of the file.
 
       One of:
 
@@ -12318,14 +12671,16 @@
       • XML or FILE_TYPE_XML
 
       • QVX or FILE_TYPE_QVX
 
       • JSON or FILE_TYPE_JSON
 
       • KML or FILE_TYPE_KML
+
+      • PARQUET or FILE_TYPE_PARQUET
     qLabel: str
       One of:
 
       • Embedded labels (field names are present in the file)
 
       • No labels
 
@@ -12603,14 +12958,16 @@
       • EXT or FUNC_GROUP_EXTERNAL
 
       • PROB or FUNC_GROUP_PROBABILITY
 
       • ARRAY or FUNC_GROUP_ARRAY
 
       • LEG or FUNC_GROUP_LEGACY
+
+      • DB or FUNC_GROUP_DB_NATIVE
     qSignature: str
       Signature of the script function.
       Gives general information about the function.
     """
 
     qName: str = None
     qGroup: str = None
@@ -12817,14 +13174,30 @@
 
 
         """
         handle = -1 if not hasattr(self, "qHandle") else self.qHandle
         response = self._session.send("Apply", handle)["qSuccess"]
         return response
 
+    def apply_and_verify(self) -> BookmarkApplyAndVerifyResult:
+        """
+        Experimental
+        Applies a bookmark and verify result dataset against originally selected values.
+
+        The operation is successful if qApplySuccess is set to true. qWarnings lists state and field with unmatching values
+
+
+        """
+        warnings.warn("ApplyAndVerify is experimental", UserWarning, stacklevel=2)
+        handle = -1 if not hasattr(self, "qHandle") else self.qHandle
+        response = self._session.send("ApplyAndVerify", handle)["qResult"]
+        obj = BookmarkApplyAndVerifyResult(**response)
+        obj._session = self._session
+        return obj
+
     def publish(self) -> object:
         """
         Publishes a bookmark.
         This operation is not applicable for Qlik Sense Desktop.
 
 
         """
@@ -12873,30 +13246,52 @@
     Attributes
     ----------
     qInfo: NxInfo
       Information about the bookmark.
       This parameter is mandatory.
     qMetaDef: NxMetaDef
       Definition of the dynamic properties.
+    qIncludeVariables: bool
+      If true all variables will be stored in the bookmark.
+    qDistinctValues: bool
+      If true all selected values will be stored distinct, i.e. searchstrings will not be kept.
     """
 
     qInfo: NxInfo = None
     qMetaDef: NxMetaDef = None
+    qIncludeVariables: bool = None
+    qDistinctValues: bool = None
 
     def __init__(self_, **kvargs):
         if "qInfo" in kvargs:
             if type(kvargs["qInfo"]).__name__ is self_.__annotations__["qInfo"]:
                 self_.qInfo = kvargs["qInfo"]
             else:
                 self_.qInfo = NxInfo(**kvargs["qInfo"])
         if "qMetaDef" in kvargs:
             if type(kvargs["qMetaDef"]).__name__ is self_.__annotations__["qMetaDef"]:
                 self_.qMetaDef = kvargs["qMetaDef"]
             else:
                 self_.qMetaDef = NxMetaDef(**kvargs["qMetaDef"])
+        if "qIncludeVariables" in kvargs:
+            if (
+                type(kvargs["qIncludeVariables"]).__name__
+                is self_.__annotations__["qIncludeVariables"]
+            ):
+                self_.qIncludeVariables = kvargs["qIncludeVariables"]
+            else:
+                self_.qIncludeVariables = kvargs["qIncludeVariables"]
+        if "qDistinctValues" in kvargs:
+            if (
+                type(kvargs["qDistinctValues"]).__name__
+                is self_.__annotations__["qDistinctValues"]
+            ):
+                self_.qDistinctValues = kvargs["qDistinctValues"]
+            else:
+                self_.qDistinctValues = kvargs["qDistinctValues"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class GenericDimension:
@@ -16659,15 +17054,15 @@
     qIsOpenedWithoutData: bool
       If set to true, it means that the app was opened without loading its data.
     qIsSessionApp: bool
       If set to true, the app is a Session App, i.e. not persistent.
     qThumbnail: StaticContentUrl
       App thumbnail.
     qIsBDILiveMode: bool
-      If set to true, the app is in BDI Live Mode.
+      If set to true, the app is in BDI Direct Query Mode.
     qIsDirectQueryMode: bool
       If set to true, the app is in Direct Query Mode.
     qUnsupportedFeatures: list[NxFeature]
       Array of features not supported by the app.
     """
 
     qTitle: str = None
@@ -22705,24 +23100,29 @@
       Note that on the contrary, the qStateCounts parameter counts the excluded values as alternative values.
       This parameter is optional.
     qInitialDataFetch: list[NxPage]
       Fetches an initial data set.
     qExpressions: list[NxListObjectExpressionDef]
       Lists the expressions in the list object.
       This parameter is optional.
+    qDirectQuerySimplifiedView: bool
+      If set to true, reduces the set of states returned.
+      Supported for Direct Query mode only.
+      Default is false.
     """
 
     qStateName: str = None
     qLibraryId: str = None
     qDef: NxInlineDimensionDef = None
     qAutoSortByState: NxAutoSortByStateDef = None
     qFrequencyMode: str = "NX_FREQUENCY_NONE"
     qShowAlternatives: bool = None
     qInitialDataFetch: list[NxPage] = None
     qExpressions: list[NxListObjectExpressionDef] = None
+    qDirectQuerySimplifiedView: bool = None
 
     def __init__(self_, **kvargs):
         if "qStateName" in kvargs:
             if (
                 type(kvargs["qStateName"]).__name__
                 is self_.__annotations__["qStateName"]
             ):
@@ -22784,14 +23184,22 @@
                 is self_.__annotations__["qExpressions"]
             ):
                 self_.qExpressions = kvargs["qExpressions"]
             else:
                 self_.qExpressions = [
                     NxListObjectExpressionDef(**e) for e in kvargs["qExpressions"]
                 ]
+        if "qDirectQuerySimplifiedView" in kvargs:
+            if (
+                type(kvargs["qDirectQuerySimplifiedView"]).__name__
+                is self_.__annotations__["qDirectQuerySimplifiedView"]
+            ):
+                self_.qDirectQuerySimplifiedView = kvargs["qDirectQuerySimplifiedView"]
+            else:
+                self_.qDirectQuerySimplifiedView = kvargs["qDirectQuerySimplifiedView"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class NxBookmark:
@@ -25293,14 +25701,16 @@
 
           • PROB or FUNC_GROUP_PROBABILITY
 
           • ARRAY or FUNC_GROUP_ARRAY
 
           • LEG or FUNC_GROUP_LEGACY
 
+          • DB or FUNC_GROUP_DB_NATIVE
+
         """
         params = {}
         if qGroup is not None:
             params["qGroup"] = qGroup
         handle = -1 if not hasattr(self, "qHandle") else self.qHandle
         response = self._session.send("GetFunctions", handle, **params)["qFunctions"]
         return [Function(e) for e in response]
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Reloads.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Reloads.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Spaces.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Spaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import asdict, dataclass
 
 from ..auth import Auth, Config
@@ -237,57 +237,57 @@
         )
         obj = Assignment(**response.json())
         obj.auth = self.auth
         return obj
 
     def get_shares(
         self,
-        name: str = None,
-        resourceId: str = None,
-        resourceType: str = None,
         groupId: str = None,
-        userId: str = None,
         limit: int = 10,
+        name: str = None,
         next: str = None,
         prev: str = None,
+        resourceId: str = None,
+        resourceType: str = None,
+        userId: str = None,
         max_items: int = 10,
     ) -> ListableResource[Share]:
         """
         Experimental
         Retrieves the shares of the space matching the query.
 
         Parameters
         ----------
-        name: str = None
-        resourceId: str = None
-        resourceType: str = None
         groupId: str = None
-        userId: str = None
         limit: int = 10
+        name: str = None
         next: str = None
         prev: str = None
+        resourceId: str = None
+        resourceType: str = None
+        userId: str = None
         """
         warnings.warn("get_shares is experimental", UserWarning, stacklevel=2)
         query_params = {}
-        if name is not None:
-            query_params["name"] = name
-        if resourceId is not None:
-            query_params["resourceId"] = resourceId
-        if resourceType is not None:
-            query_params["resourceType"] = resourceType
         if groupId is not None:
             query_params["groupId"] = groupId
-        if userId is not None:
-            query_params["userId"] = userId
         if limit is not None:
             query_params["limit"] = limit
+        if name is not None:
+            query_params["name"] = name
         if next is not None:
             query_params["next"] = next
         if prev is not None:
             query_params["prev"] = prev
+        if resourceId is not None:
+            query_params["resourceId"] = resourceId
+        if resourceType is not None:
+            query_params["resourceType"] = resourceType
+        if userId is not None:
+            query_params["userId"] = userId
 
         response = self.auth.rest(
             path="/spaces/{spaceId}/shares".replace("{spaceId}", self.id),
             method="GET",
             params=query_params,
             data=None,
         )
@@ -557,14 +557,39 @@
                 self_.names = kvargs["names"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
+class FineGrainedLicense:
+    """
+
+    Attributes
+    ----------
+    fineGrainedAppEnabled: bool
+    """
+
+    fineGrainedAppEnabled: bool = None
+
+    def __init__(self_, **kvargs):
+        if "fineGrainedAppEnabled" in kvargs:
+            if (
+                type(kvargs["fineGrainedAppEnabled"]).__name__
+                is self_.__annotations__["fineGrainedAppEnabled"]
+            ):
+                self_.fineGrainedAppEnabled = kvargs["fineGrainedAppEnabled"]
+            else:
+                self_.fineGrainedAppEnabled = kvargs["fineGrainedAppEnabled"]
+        for k, v in kvargs.items():
+            if k not in getattr(self_, "__annotations__", {}):
+                self_.__setattr__(k, v)
+
+
+@dataclass
 class Share:
     """
 
     Attributes
     ----------
     assigneeId: str
       The userId or groupId based on the type.
@@ -982,80 +1007,80 @@
 class Spaces:
     def __init__(self, config: Config) -> None:
         self.config = config
         self.auth = Auth(config)
 
     def get_spaces(
         self,
-        type: str = None,
         action: str = None,
-        sort: str = None,
-        name: str = None,
-        ownerId: str = None,
         limit: int = 10,
+        name: str = None,
         next: str = None,
+        ownerId: str = None,
         prev: str = None,
+        sort: str = None,
+        type: str = None,
         max_items: int = 10,
     ) -> ListableResource[Space]:
         """
         Retrieves spaces that the current user has access to and match the query.
 
 
-        type: str
-          Type(s) of space to filter. For example, "?type=managed,shared".
-
         action: str
           Action on space. For example, "?action=publish".
 
-        sort: str
-          Field to sort by. Prefix with +/- to indicate asc/desc. For example, "?sort=+name" to sort ascending on Name. Supported fields are "type", "name" and "createdAt".
+        limit: int
+          Maximum number of spaces to return.
 
         name: str
           Space name to search and filter for. Case-insensitive open search with wildcards both as prefix and suffix. For example, "?name=fin" will get "finance", "Final" and "Griffin".
 
-        ownerId: str
-          Space ownerId to filter by. For example, "?ownerId=123".
-
-        limit: int
-          Maximum number of spaces to return.
-
         next: str
           The next page cursor. Next links make use of this.
 
+        ownerId: str
+          Space ownerId to filter by. For example, "?ownerId=123".
+
         prev: str
           The previous page cursor. Previous links make use of this.
 
+        sort: str
+          Field to sort by. Prefix with +/- to indicate asc/desc. For example, "?sort=+name" to sort ascending on Name. Supported fields are "type", "name" and "createdAt".
+
+        type: str
+          Type(s) of space to filter. For example, "?type=managed,shared".
+
         Parameters
         ----------
-        type: str = None
         action: str = None
-        sort: str = None
-        name: str = None
-        ownerId: str = None
         limit: int = 10
+        name: str = None
         next: str = None
+        ownerId: str = None
         prev: str = None
+        sort: str = None
+        type: str = None
         """
         query_params = {}
-        if type is not None:
-            query_params["type"] = type
         if action is not None:
             query_params["action"] = action
-        if sort is not None:
-            query_params["sort"] = sort
-        if name is not None:
-            query_params["name"] = name
-        if ownerId is not None:
-            query_params["ownerId"] = ownerId
         if limit is not None:
             query_params["limit"] = limit
+        if name is not None:
+            query_params["name"] = name
         if next is not None:
             query_params["next"] = next
+        if ownerId is not None:
+            query_params["ownerId"] = ownerId
         if prev is not None:
             query_params["prev"] = prev
+        if sort is not None:
+            query_params["sort"] = sort
+        if type is not None:
+            query_params["type"] = type
 
         response = self.auth.rest(
             path="/spaces",
             method="GET",
             params=query_params,
             data=None,
         )
@@ -1123,14 +1148,35 @@
             cls=Space,
             auth=self.auth,
             path="/spaces/filter",
             max_items=max_items,
             query_params={},
         )
 
+    def get_shares_license(self) -> FineGrainedLicense:
+        """
+        Experimental
+        Get licenses for fine-grained.
+
+
+        Parameters
+        ----------
+        """
+        warnings.warn("get_shares_license is experimental", UserWarning, stacklevel=2)
+
+        response = self.auth.rest(
+            path="/spaces/shares/license",
+            method="GET",
+            params={},
+            data=None,
+        )
+        obj = FineGrainedLicense(**response.json())
+        obj.auth = self.auth
+        return obj
+
     def get_types(self, max_items: int = 10) -> ListableResource[str]:
         """
         Gets a list of distinct space types.
 
 
         Parameters
         ----------
@@ -1170,196 +1216,196 @@
             params={},
             data=None,
         )
         obj = Space(**response.json())
         obj.auth = self.auth
         return obj
 
-    def delete_assignment(self, spaceId: str, assignmentId: str) -> None:
+    def delete_assignment(self, assignmentId: str, spaceId: str) -> None:
         """
         Deletes an assignment.
 
 
-        spaceId: str
-          The ID of the space of the assignment.
-
         assignmentId: str
           The ID of the assignment to delete.
 
+        spaceId: str
+          The ID of the space of the assignment.
+
         Parameters
         ----------
-        spaceId: str
         assignmentId: str
+        spaceId: str
         """
 
         self.auth.rest(
             path="/spaces/{spaceId}/assignments/{assignmentId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{assignmentId}", assignmentId),
+                "{assignmentId}", assignmentId
+            ).replace("{spaceId}", spaceId),
             method="DELETE",
             params={},
             data=None,
         )
 
-    def get_assignment(self, spaceId: str, assignmentId: str) -> Assignment:
+    def get_assignment(self, assignmentId: str, spaceId: str) -> Assignment:
         """
         Retrieves a single assignment by ID.
 
 
-        spaceId: str
-          The ID of the space of the assignment.
-
         assignmentId: str
           The ID of the assignment to retrieve.
 
+        spaceId: str
+          The ID of the space of the assignment.
+
         Parameters
         ----------
-        spaceId: str
         assignmentId: str
+        spaceId: str
         """
 
         response = self.auth.rest(
             path="/spaces/{spaceId}/assignments/{assignmentId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{assignmentId}", assignmentId),
+                "{assignmentId}", assignmentId
+            ).replace("{spaceId}", spaceId),
             method="GET",
             params={},
             data=None,
         )
         obj = Assignment(**response.json())
         obj.auth = self.auth
         return obj
 
     def set_assignment(
-        self, spaceId: str, assignmentId: str, data: AssignmentUpdate
+        self, assignmentId: str, spaceId: str, data: AssignmentUpdate
     ) -> Assignment:
         """
         Experimental
         Updates a single assignment by ID. The complete list of roles must be provided.
 
 
-        spaceId: str
-          The ID of the space of the assignment.
-
         assignmentId: str
           The ID of the assignment to update.
 
+        spaceId: str
+          The ID of the space of the assignment.
+
         Parameters
         ----------
-        spaceId: str
         assignmentId: str
+        spaceId: str
         data: AssignmentUpdate
         """
         warnings.warn("set_assignment is experimental", UserWarning, stacklevel=2)
 
         try:
             data = asdict(data)
         except:
             data = data
 
         response = self.auth.rest(
             path="/spaces/{spaceId}/assignments/{assignmentId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{assignmentId}", assignmentId),
+                "{assignmentId}", assignmentId
+            ).replace("{spaceId}", spaceId),
             method="PUT",
             params={},
             data=data,
         )
         obj = Assignment(**response.json())
         obj.auth = self.auth
         return obj
 
-    def delete_share(self, spaceId: str, shareId: str) -> None:
+    def delete_share(self, shareId: str, spaceId: str) -> None:
         """
         Experimental
         Deletes a Share.
 
 
-        spaceId: str
-          The ID of the space to which the share belongs.
-
         shareId: str
           The ID of the share to delete.
 
+        spaceId: str
+          The ID of the space to which the share belongs.
+
         Parameters
         ----------
-        spaceId: str
         shareId: str
+        spaceId: str
         """
         warnings.warn("delete_share is experimental", UserWarning, stacklevel=2)
 
         self.auth.rest(
             path="/spaces/{spaceId}/shares/{shareId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{shareId}", shareId),
+                "{shareId}", shareId
+            ).replace("{spaceId}", spaceId),
             method="DELETE",
             params={},
             data=None,
         )
 
-    def get_share(self, spaceId: str, shareId: str) -> Share:
+    def get_share(self, shareId: str, spaceId: str) -> Share:
         """
         Experimental
         Retrieves a single share by ID.
 
 
-        spaceId: str
-          The ID of the space to which the share belongs.
-
         shareId: str
           The ID of the share to retrieve.
 
+        spaceId: str
+          The ID of the space to which the share belongs.
+
         Parameters
         ----------
-        spaceId: str
         shareId: str
+        spaceId: str
         """
         warnings.warn("get_share is experimental", UserWarning, stacklevel=2)
 
         response = self.auth.rest(
             path="/spaces/{spaceId}/shares/{shareId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{shareId}", shareId),
+                "{shareId}", shareId
+            ).replace("{spaceId}", spaceId),
             method="GET",
             params={},
             data=None,
         )
         obj = Share(**response.json())
         obj.auth = self.auth
         return obj
 
-    def patch_share(self, spaceId: str, shareId: str, data: SharePatch) -> Share:
+    def patch_share(self, shareId: str, spaceId: str, data: SharePatch) -> Share:
         """
         Experimental
         Patches (updates) a share (partially).
 
 
-        spaceId: str
-          The ID of the space to which the share belongs.
-
         shareId: str
           The ID of the share to update.
 
+        spaceId: str
+          The ID of the space to which the share belongs.
+
         Parameters
         ----------
-        spaceId: str
         shareId: str
+        spaceId: str
         data: SharePatch
         """
         warnings.warn("patch_share is experimental", UserWarning, stacklevel=2)
 
         try:
             data = asdict(data)
         except:
             data = data
 
         response = self.auth.rest(
             path="/spaces/{spaceId}/shares/{shareId}".replace(
-                "{spaceId}", spaceId
-            ).replace("{shareId}", shareId),
+                "{shareId}", shareId
+            ).replace("{spaceId}", spaceId),
             method="PATCH",
             params={},
             data=data,
         )
         obj = Share(**response.json())
         obj.auth = self.auth
         return obj
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Themes.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Themes.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/apis/Users.py` & `qlik-sdk-0.9.0/src/qlik_sdk/apis/Users.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 # This is spectacularly generated code by spectacular v0.0.0 based on
-# Qlik Cloud Services 0.348.2
+# Qlik Cloud Services 0.384.10
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import asdict, dataclass
 from typing import Union
 
 from ..auth import Auth, Config
 from ..listable import ListableResource
 
 
 @dataclass
 class User:
     """
+    A user object.
 
     Attributes
     ----------
     id: str
       The unique user identifier.
     name: str
       The name of the user.
     subject: str
       The unique user identitier from an identity provider.
     tenantId: str
       The tenant that the user belongs too.
     assignedGroups: list[object]
+      An array of group references.
     assignedRoles: list[object]
+      An array of role references.
     created: str
       Deprecated. Use `createdAt` instead.
     createdAt: str
       The timestamp for when the user record was created.
     email: str
       The email address for the user.
     inviteExpiry: float
       The number of seconds until the user invitation will expire.
     lastUpdated: str
       Deprecated. Use `lastUpdatedAt` instead.
     lastUpdatedAt: str
       The timestamp for when the user record was last updated.
     links: object
+      Pagination links to the user.
     locale: str
       Represents the end-user's language tag.
     picture: str
       A static url linking to the avatar of the user.
     preferredLocale: str
       Represents the end-user's preferred language tag.
     preferredZoneinfo: str
@@ -201,34 +205,36 @@
                 self_.zoneinfo = kvargs["zoneinfo"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
     def delete(self) -> None:
         """
-        Deletes a user resource.
+        Delete user by ID
+        Deletes the requested user.
 
         Parameters
         ----------
         """
 
         self.auth.rest(
             path="/users/{userId}".replace("{userId}", self.id),
             method="DELETE",
             params={},
             data=None,
         )
 
-    def patch(self, data: UserJSONPatchArray) -> None:
+    def patch(self, data: JSONPatchArray) -> None:
         """
-        Updates a user resource.
+        Update user by ID
+        Updates fields for a user resource
 
         Parameters
         ----------
-        data: UserJSONPatchArray
+        data: JSONPatchArray
         """
 
         try:
             data = asdict(data)
         except:
             data = data
 
@@ -239,14 +245,15 @@
             data=data,
         )
 
 
 @dataclass
 class Filter:
     """
+    An advanced query filter to be used for complex user querying in the tenant.
 
     Attributes
     ----------
     filter: str
       The advanced filtering to be applied the query. All conditional statements within this query parameter are case insensitive.
     """
 
@@ -260,126 +267,129 @@
                 self_.filter = kvargs["filter"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class Metadata:
+class JSONPatch:
     """
+    A JSON Patch document as defined in http://tools.ietf.org/html/rfc6902.
 
     Attributes
     ----------
-    valid_roles: list[str]
-      List of system roles to which the user can be assigned.
+    op: str
+      The operation to be performed.
+    path: str
+      A JSON Pointer.
+    value: Union[str,bool,list,list]
+      The value to be used for this operation.
     """
 
-    valid_roles: list[str] = None
+    op: str = None
+    path: str = None
+    value: Union[str, bool, list, list] = None
 
     def __init__(self_, **kvargs):
-        if "valid_roles" in kvargs:
-            if (
-                type(kvargs["valid_roles"]).__name__
-                is self_.__annotations__["valid_roles"]
-            ):
-                self_.valid_roles = kvargs["valid_roles"]
+        if "op" in kvargs:
+            if type(kvargs["op"]).__name__ is self_.__annotations__["op"]:
+                self_.op = kvargs["op"]
             else:
-                self_.valid_roles = kvargs["valid_roles"]
+                self_.op = kvargs["op"]
+        if "path" in kvargs:
+            if type(kvargs["path"]).__name__ is self_.__annotations__["path"]:
+                self_.path = kvargs["path"]
+            else:
+                self_.path = kvargs["path"]
+        if "value" in kvargs:
+            if type(kvargs["value"]).__name__ is self_.__annotations__["value"]:
+                self_.value = kvargs["value"]
+            else:
+                self_.value = kvargs["value"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class UserCount:
+class JSONPatchArray:
     """
+    An array of JSON Patch documents
 
     Attributes
     ----------
-    total: float
     """
 
-    total: float = None
-
     def __init__(self_, **kvargs):
-        if "total" in kvargs:
-            if type(kvargs["total"]).__name__ is self_.__annotations__["total"]:
-                self_.total = kvargs["total"]
-            else:
-                self_.total = kvargs["total"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class UserJSONPatch:
+class Metadata:
     """
-    A JSON Patch document as defined in http://tools.ietf.org/html/rfc6902.
+    An object containing the metadata for the user configuration.
 
     Attributes
     ----------
-    op: str
-      The operation to be performed.
-    path: str
-      A JSON Pointer.
-    value: Union[str,bool,list]
-      The value to be used for this operation.
+    valid_roles: list[str]
+      List of system roles to which the user can be assigned.
     """
 
-    op: str = None
-    path: str = None
-    value: Union[str, bool, list] = None
+    valid_roles: list[str] = None
 
     def __init__(self_, **kvargs):
-        if "op" in kvargs:
-            if type(kvargs["op"]).__name__ is self_.__annotations__["op"]:
-                self_.op = kvargs["op"]
-            else:
-                self_.op = kvargs["op"]
-        if "path" in kvargs:
-            if type(kvargs["path"]).__name__ is self_.__annotations__["path"]:
-                self_.path = kvargs["path"]
-            else:
-                self_.path = kvargs["path"]
-        if "value" in kvargs:
-            if type(kvargs["value"]).__name__ is self_.__annotations__["value"]:
-                self_.value = kvargs["value"]
+        if "valid_roles" in kvargs:
+            if (
+                type(kvargs["valid_roles"]).__name__
+                is self_.__annotations__["valid_roles"]
+            ):
+                self_.valid_roles = kvargs["valid_roles"]
             else:
-                self_.value = kvargs["value"]
+                self_.valid_roles = kvargs["valid_roles"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
-class UserJSONPatchArray:
+class UserCount:
     """
-    An array of JSON Patch documents
+    The result object for the user count.
 
     Attributes
     ----------
+    total: float
+      The total number of users in the tenant.
     """
 
+    total: float = None
+
     def __init__(self_, **kvargs):
+        if "total" in kvargs:
+            if type(kvargs["total"]).__name__ is self_.__annotations__["total"]:
+                self_.total = kvargs["total"]
+            else:
+                self_.total = kvargs["total"]
         for k, v in kvargs.items():
             if k not in getattr(self_, "__annotations__", {}):
                 self_.__setattr__(k, v)
 
 
 @dataclass
 class UserPostSchema:
     """
 
     Attributes
     ----------
     subject: str
       The unique user identitier from an identity provider.
-    assignedGroups: list[object]
     assignedRoles: list[object]
+      An array of role reference identifiers.
     email: str
       The email address for the user. This is a required field when inviting a user.
     name: str
       The name of the user.
     picture: str
       A static url linking to the avatar of the user.
     roles: list[str]
@@ -387,37 +397,28 @@
     status: str
       The status of the created user within the tenant.
     tenantId: str
       The tenant that the user will belong too.
     """
 
     subject: str = None
-    assignedGroups: list[object] = None
     assignedRoles: list[object] = None
     email: str = None
     name: str = None
     picture: str = None
     roles: list[str] = None
     status: str = None
     tenantId: str = None
 
     def __init__(self_, **kvargs):
         if "subject" in kvargs:
             if type(kvargs["subject"]).__name__ is self_.__annotations__["subject"]:
                 self_.subject = kvargs["subject"]
             else:
                 self_.subject = kvargs["subject"]
-        if "assignedGroups" in kvargs:
-            if (
-                type(kvargs["assignedGroups"]).__name__
-                is self_.__annotations__["assignedGroups"]
-            ):
-                self_.assignedGroups = kvargs["assignedGroups"]
-            else:
-                self_.assignedGroups = kvargs["assignedGroups"]
         if "assignedRoles" in kvargs:
             if (
                 type(kvargs["assignedRoles"]).__name__
                 is self_.__annotations__["assignedRoles"]
             ):
                 self_.assignedRoles = kvargs["assignedRoles"]
             else:
@@ -460,15 +461,17 @@
 @dataclass
 class UsersClass:
     """
 
     Attributes
     ----------
     data: list[User]
+      List of users.
     links: object
+      Pagination links
     """
 
     data: list[User] = None
     links: object = None
 
     def __init__(self_, **kvargs):
         if "data" in kvargs:
@@ -489,71 +492,45 @@
 class Users:
     def __init__(self, config: Config) -> None:
         self.config = config
         self.auth = Auth(config)
 
     def get_users(
         self,
-        tenantId: str = None,
-        subject: str = None,
         email: str = None,
-        status: str = None,
-        role: str = None,
+        endingBefore: str = None,
         fields: str = None,
+        filter: str = None,
         limit: float = 20,
+        next: str = None,
+        prev: str = None,
+        role: str = None,
         sort: str = "+name",
         sortBy: str = None,
         sortOrder: str = None,
         startingAfter: str = None,
-        endingBefore: str = None,
-        filter: str = None,
-        next: str = None,
-        prev: str = None,
+        status: str = None,
+        subject: str = None,
+        tenantId: str = None,
         max_items: int = 20,
     ) -> ListableResource[User]:
         """
-        Retrieves a list of users matching the query.
+        List users
+        Returns a list of users using cursor-based pagination.
 
 
-        tenantId: str
-          The tenant ID to filter by. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
-
-        subject: str
-          The subject to filter by. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
-
         email: str
           The email to filter by. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
 
-        status: str
-          The status to filter by. Supports multiple values delimited by commas. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
-
-        role: str
-          The role to filter by. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
+        endingBefore: str
+          Get users with IDs that are lower than the target user ID. Cannot be used in conjunction with startingAfter. Deprecated. Use `prev` instead.
 
         fields: str
           A comma-delimited string of the requested fields per entity. If the 'links' value is omitted, then the entity HATEOAS link will also be omitted.
 
-        limit: float
-          The number of user entries to retrieve.
-
-        sort: str
-          The field to sort by, with +/- prefix indicating sort order
-
-        sortBy: str
-          The user parameter to sort by. Deprecated. Use `sort` instead.
-
-        sortOrder: str
-          The sort order, either ascending or descending. Deprecated. Use `sort` instead.
-
-        startingAfter: str
-          Get users with IDs that are higher than the target user ID. Cannot be used in conjunction with endingBefore. Deprecated. Use `next` instead.
-
-        endingBefore: str
-          Get users with IDs that are lower than the target user ID. Cannot be used in conjunction with startingAfter. Deprecated. Use `prev` instead.
-
         filter: str
           The advanced filtering to use for the query. Refer to [RFC 7644](https://datatracker.ietf.org/doc/rfc7644/) for the syntax. Cannot be combined with any of the fields marked as deprecated. All conditional statements within this query parameter are case insensitive.
 
           The following fields support the `eq` operator: `id`, `subject`, `name`, `email`, `status`, `clientId`, `assignedRoles.id` `assignedRoles.name`, `assignedGroups.id`, `assignedGroupsAssignedRoles.name`
 
           Additionally, the following fields support the `co` operator: `name`, `email`, `subject`
 
@@ -563,82 +540,123 @@
           (id eq "62716ab404a7bd8626af9bd6" or id eq "62716ac4c7e500e13ff5fa22") and (status eq "active" or status eq "disabled")
           ```
 
           ```
           name co "query" or email co "query" or subject co "query" or id eq "query" or assignedRoles.name eq "query"
           ```
 
+          Any filters for status must be grouped together and applied to the whole query.
+
+          Valid:
+
+          ```
+          (name eq "Bob" or name eq "Alice") and (status eq "active" or status eq "disabled")
+          ```
+
+          Invalid:
+
+          ```
+          name eq "Bob" or name eq "Alice" and (status eq "active" or status eq "disabled")
+          ```
+
+        limit: float
+          The number of user entries to retrieve.
+
         next: str
           Get users that come after this cursor value when sorted. Cannot be used in conjunction with `prev`.
 
         prev: str
           Get users that come before this cursor value when sorted. Cannot be used in conjunction with `next`.
 
+        role: str
+          The role to filter by. Deprecated.
+
+        sort: str
+          The field to sort by, with +/- prefix indicating sort order
+
+        sortBy: str
+          The user parameter to sort by. Deprecated. Use `sort` instead.
+
+        sortOrder: str
+          The sort order, either ascending or descending. Deprecated. Use `sort` instead.
+
+        startingAfter: str
+          Get users with IDs that are higher than the target user ID. Cannot be used in conjunction with endingBefore. Deprecated. Use `next` instead.
+
+        status: str
+          The status to filter by. Supports multiple values delimited by commas. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
+
+        subject: str
+          The subject to filter by. Deprecated. Use the new `filter` parameter to provide an advanced query filter.
+
+        tenantId: str
+          The tenant ID to filter by. Deprecated.
+
         Parameters
         ----------
-        tenantId: str = None
-        subject: str = None
         email: str = None
-        status: str = None
-        role: str = None
+        endingBefore: str = None
         fields: str = None
+        filter: str = None
         limit: float = 20
+        next: str = None
+        prev: str = None
+        role: str = None
         sort: str = "+name"
         sortBy: str = None
         sortOrder: str = None
         startingAfter: str = None
-        endingBefore: str = None
-        filter: str = None
-        next: str = None
-        prev: str = None
+        status: str = None
+        subject: str = None
+        tenantId: str = None
         """
         query_params = {}
-        if tenantId is not None:
-            query_params["tenantId"] = tenantId
-            warnings.warn("tenantId is deprecated", DeprecationWarning, stacklevel=2)
-        if subject is not None:
-            query_params["subject"] = subject
-            warnings.warn("subject is deprecated", DeprecationWarning, stacklevel=2)
         if email is not None:
             query_params["email"] = email
             warnings.warn("email is deprecated", DeprecationWarning, stacklevel=2)
-        if status is not None:
-            query_params["status"] = status
-            warnings.warn("status is deprecated", DeprecationWarning, stacklevel=2)
-        if role is not None:
-            query_params["role"] = role
-            warnings.warn("role is deprecated", DeprecationWarning, stacklevel=2)
+        if endingBefore is not None:
+            query_params["endingBefore"] = endingBefore
+            warnings.warn(
+                "endingBefore is deprecated", DeprecationWarning, stacklevel=2
+            )
         if fields is not None:
             query_params["fields"] = fields
+        if filter is not None:
+            query_params["filter"] = filter
         if limit is not None:
             query_params["limit"] = limit
+        if next is not None:
+            query_params["next"] = next
+        if prev is not None:
+            query_params["prev"] = prev
+        if role is not None:
+            query_params["role"] = role
+            warnings.warn("role is deprecated", DeprecationWarning, stacklevel=2)
         if sort is not None:
             query_params["sort"] = sort
         if sortBy is not None:
             query_params["sortBy"] = sortBy
             warnings.warn("sortBy is deprecated", DeprecationWarning, stacklevel=2)
         if sortOrder is not None:
             query_params["sortOrder"] = sortOrder
             warnings.warn("sortOrder is deprecated", DeprecationWarning, stacklevel=2)
         if startingAfter is not None:
             query_params["startingAfter"] = startingAfter
             warnings.warn(
                 "startingAfter is deprecated", DeprecationWarning, stacklevel=2
             )
-        if endingBefore is not None:
-            query_params["endingBefore"] = endingBefore
-            warnings.warn(
-                "endingBefore is deprecated", DeprecationWarning, stacklevel=2
-            )
-        if filter is not None:
-            query_params["filter"] = filter
-        if next is not None:
-            query_params["next"] = next
-        if prev is not None:
-            query_params["prev"] = prev
+        if status is not None:
+            query_params["status"] = status
+            warnings.warn("status is deprecated", DeprecationWarning, stacklevel=2)
+        if subject is not None:
+            query_params["subject"] = subject
+            warnings.warn("subject is deprecated", DeprecationWarning, stacklevel=2)
+        if tenantId is not None:
+            query_params["tenantId"] = tenantId
+            warnings.warn("tenantId is deprecated", DeprecationWarning, stacklevel=2)
 
         response = self.auth.rest(
             path="/users",
             method="GET",
             params=query_params,
             data=None,
         )
@@ -649,20 +667,17 @@
             path="/users",
             max_items=max_items,
             query_params=query_params,
         )
 
     def create(self, data: UserPostSchema) -> User:
         """
-        Creates a user in a given tenant.
-        Creates and returns a user in a given tenant. Note that only creating invited status users is supported for users of the given tenant.
-
+        Create user
+        Creates an invited user.
 
-        Authorization: str
-          The JWT used for authentication. Send the JWT in the Authorization header using the Bearer schema.
 
         Parameters
         ----------
         data: UserPostSchema
         """
 
         try:
@@ -678,27 +693,29 @@
         )
         obj = User(**response.json())
         obj.auth = self.auth
         return obj
 
     def count(self, tenantId: str = None) -> UserCount:
         """
+        Count users
         Returns the number of users in a given tenant
 
 
         tenantId: str
           The tenant ID to filter by.
 
         Parameters
         ----------
         tenantId: str = None
         """
         query_params = {}
         if tenantId is not None:
             query_params["tenantId"] = tenantId
+            warnings.warn("tenantId is deprecated", DeprecationWarning, stacklevel=2)
 
         response = self.auth.rest(
             path="/users/actions/count",
             method="GET",
             params=query_params,
             data=None,
         )
@@ -706,59 +723,60 @@
         obj.auth = self.auth
         return obj
 
     def filter(
         self,
         data: Filter,
         fields: str = None,
-        sort: str = "+name",
+        limit: float = 20,
         next: str = None,
         prev: str = None,
-        limit: float = 20,
+        sort: str = "+name",
         max_items: int = 20,
     ) -> ListableResource[User]:
         """
-        Retrieves a list of users matching the filter using advanced query string.
+        Filter users
+        Retrieves a list of users matching the filter using an advanced query string.
 
 
         fields: str
           A comma-delimited string of the requested fields per entity. If the 'links' value is omitted, then the entity HATEOAS link will also be omitted.
 
-        sort: str
-          The field to sort by, with +/- prefix indicating sort order
+        limit: float
+          The number of user entries to retrieve.
 
         next: str
           Get users with IDs that are higher than the target user ID. Cannot be used in conjunction with prev.
 
         prev: str
           Get users with IDs that are lower than the target user ID. Cannot be used in conjunction with next.
 
-        limit: float
-          The number of user entries to retrieve.
+        sort: str
+          The field to sort by, with +/- prefix indicating sort order
 
         Parameters
         ----------
         fields: str = None
-        sort: str = "+name"
+        limit: float = 20
         next: str = None
         prev: str = None
-        limit: float = 20
+        sort: str = "+name"
         data: Filter
         """
         query_params = {}
         if fields is not None:
             query_params["fields"] = fields
-        if sort is not None:
-            query_params["sort"] = sort
+        if limit is not None:
+            query_params["limit"] = limit
         if next is not None:
             query_params["next"] = next
         if prev is not None:
             query_params["prev"] = prev
-        if limit is not None:
-            query_params["limit"] = limit
+        if sort is not None:
+            query_params["sort"] = sort
 
         try:
             data = asdict(data)
         except:
             data = data
 
         response = self.auth.rest(
@@ -774,14 +792,15 @@
             path="/users/actions/filter",
             max_items=max_items,
             query_params=query_params,
         )
 
     def get_me(self) -> any:
         """
+        Get my user
         Redirects to retrieve the user resource associated with the JWT claims.
 
 
         Parameters
         ----------
         """
 
@@ -791,35 +810,37 @@
             params={},
             data=None,
         )
         return response.json()
 
     def get_metadata(self) -> Metadata:
         """
-        Returns the metadata with regard to the user configuration.
-        Deprecated, use GET /v1/roles instead.
+        Deprecated
+        Get configuration metadata
+        Returns the metadata with regard to the user configuration. Deprecated, use GET /v1/roles instead.
 
 
         Parameters
         ----------
         """
+        warnings.warn("get_metadata is deprecated", DeprecationWarning, stacklevel=2)
 
         response = self.auth.rest(
             path="/users/metadata",
             method="GET",
             params={},
             data=None,
         )
         obj = Metadata(**response.json())
         obj.auth = self.auth
         return obj
 
     def get(self, userId: str) -> User:
         """
-        Returns the requested user.
+        Get user by ID
         Returns the requested user.
 
 
         userId: str
           The user's unique identifier
 
         Parameters
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/auth.py` & `qlik-sdk-0.9.0/src/qlik_sdk/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,27 +28,30 @@
     config: Config
     rest: RestClientInstance
     """
     rest method can be used to make raw calls against Qlik Cloud
 
     Parameters
     ----------
-    app_id: str
     method: str, default GET
         string HTTP verb
     path: str
         representing the api endpoint ex: `/users/me`
     data: dict, optional
         Dictionary, list of tuples, bytes, or file-like object to send in the body of the Request.
     params: dict, optional
         Dictionary, list of tuples or bytes to send in the query string for the Request.
-    headers: dict, optional
-        Dictionary of HTTP Headers to send with the Request
     files: dict, optional
         Dictionary of {filename: fileobject} files to multipart upload.
+    headers: dict, optional
+        Dictionary of HTTP Headers to send with the Request
+    stream: bool, optional, default True
+        if False, the response content will be immediately downloaded.
+    timeout: int optional, default 10
+        How many seconds to wait for the server to send data before giving up
 
     Attributes
     ----------
     interceptors: Interceptors
 
     Examples
     ----------
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/config.py` & `qlik-sdk-0.9.0/src/qlik_sdk/config.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/generate_signed_token.py` & `qlik-sdk-0.9.0/src/qlik_sdk/generate_signed_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import string
+import time
 from typing import List
 
 import jwt
 
 
 def _generate_id(length: int) -> str:
     return "".join(random.choices(string.ascii_letters + string.digits, k=length))
@@ -11,16 +12,16 @@
 
 def generate_signed_token(
     crt: str,
     sub: str,
     sub_type: str,
     name: str,
     email: str,
-    expires_in: str,
-    not_before: str,
+    expires_in: int,
+    not_before: int,
     issuer: str,
     keyid: str,
     email_verified: bool = True,
     jti: str = None,
     groups: List[str] = [],
     algorithm: str = "RS256",
     audience: str = "qlik.api/login/jwt-session",
@@ -89,14 +90,15 @@
         "subType": sub_type,
         "name": name,
         "email": email,
         "email_verified": email_verified,
         "groups": groups,
         "exp": expires_in,
         "nbf": not_before,
+        "iat": int(time.time()),
         "iss": issuer,
         "aud": audience,
     }
     singning_options = {"kid": keyid}
     token = jwt.encode(
         payload=claims, key=crt, algorithm=algorithm, headers=singning_options
     )
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/interceptors/retry_response.py` & `qlik-sdk-0.9.0/src/qlik_sdk/interceptors/retry_response.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/interceptors/types.py` & `qlik-sdk-0.9.0/src/qlik_sdk/interceptors/types.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/listable.py` & `qlik-sdk-0.9.0/src/qlik_sdk/listable.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/qlik.py` & `qlik-sdk-0.9.0/src/qlik_sdk/qlik.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/rest.py` & `qlik-sdk-0.9.0/src/qlik_sdk/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         path: str,
         method: HTTPMethods = "GET",
         data=None,
         files=None,
         params: dict = None,
         headers: dict = None,
         stream: bool = False,
+        timeout: int = 10,
     ) -> requests.Response:
         """
         rest sends a request
         """
         if not self.base_url:
             raise NoUrlException("Caller has no 'base_url'")
         if not path.startswith("/api/v1/"):
@@ -118,19 +119,20 @@
             files=files,
             headers=headers,
             params=params,
         )
 
         req = reduce(lambda d, f: f(d), self._interceptors["request"].handlers, req)
         with requests.Session() as session:
-            session.stream = stream
             prepared = req.prepare()
             try:
-                res = session.send(prepared)
-            except Exception as exc:
+                res = session.send(prepared, timeout=timeout, stream=stream)
+            except requests.exceptions.Timeout:
+                raise ConnectionException("Connection Timeout: " + self.base_url)
+            except requests.exceptions.RequestException as exc:
                 raise ConnectionException("Connection Error: " + self.base_url) from exc
 
             res = reduce(
                 lambda r, f: f(r), self._interceptors["response"].handlers, res
             )
 
             try:
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk/rpc.py` & `qlik-sdk-0.9.0/src/qlik_sdk/rpc.py`

 * *Files identical despite different names*

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk.egg-info/PKG-INFO` & `qlik-sdk-0.9.0/src/qlik_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlik-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Software Development Kit for Qlik Cloud
 Author: qlik-sdk
 Author-email: dev.thulhu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qlik-sdk-0.8.0/src/qlik_sdk.egg-info/SOURCES.txt` & `qlik-sdk-0.9.0/src/qlik_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

