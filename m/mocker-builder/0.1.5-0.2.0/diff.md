# Comparing `tmp/mocker-builder-0.1.5.tar.gz` & `tmp/mocker-builder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mocker-builder-0.1.5.tar", last modified: Mon May  8 19:15:37 2023, max compression
+gzip compressed data, was "dist/mocker-builder-0.2.0.tar", last modified: Thu Jun 22 12:50:28 2023, max compression
```

## Comparing `mocker-builder-0.1.5.tar` & `mocker-builder-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/PKG-INFO
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    21572 2023-03-30 13:19:39.000000 mocker-builder-0.1.5/README.md
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       77 2022-10-09 14:25:42.000000 mocker-builder-0.1.5/mocker_builder/__init__.py
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    30235 2023-05-08 19:05:16.000000 mocker-builder-0.1.5/mocker_builder/mocker_builder.py
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/PKG-INFO
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)      267 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)        1 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       45 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/requires.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       15 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/top_level.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       38 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/setup.cfg
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)     1704 2023-03-24 10:06:37.000000 mocker-builder-0.1.5/setup.py
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/PKG-INFO
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    21572 2023-03-30 13:19:39.000000 mocker-builder-0.2.0/README.md
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       77 2022-10-09 14:25:42.000000 mocker-builder-0.2.0/mocker_builder/__init__.py
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    31703 2023-06-22 10:21:33.000000 mocker-builder-0.2.0/mocker_builder/mocker_builder.py
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)      267 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)        1 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       45 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/requires.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       15 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/mocker_builder.egg-info/top_level.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       38 2023-06-22 12:50:28.000000 mocker-builder-0.2.0/setup.cfg
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)     1704 2023-03-24 10:06:37.000000 mocker-builder-0.2.0/setup.py
```

### Comparing `mocker-builder-0.1.5/PKG-INFO` & `mocker-builder-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-builder
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python library to build mock tests dynamicaly using the mocker feature from pytest-mock lib
 Home-page: https://github.com/tgc77/mocker_builder
 Author: Tiago G Cunha
 Author-email: tikx.batera@gmail.com
 License: MIT
 Project-URL: Documentation, https://mocker-builder.readthedocs.io
 Project-URL: Source, https://github.com/tgc77/mocker_builder
```

### Comparing `mocker-builder-0.1.5/README.md` & `mocker-builder-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mocker-builder-0.1.5/mocker_builder/mocker_builder.py` & `mocker-builder-0.2.0/mocker_builder/mocker_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     Callable,
     Dict,
     Generic,
     List,
     NewType,
     Optional,
     Tuple,
-    Type,
     TypeVar,
     Union,
 )
 from unittest.mock import (
     MagicMock,
     DEFAULT,
     _patch as _PatchType,
@@ -43,16 +42,18 @@
 TypeNew = TypeVar('TypeNew', bound=Any)
 NewCallableType = TypeVar('NewCallableType', bound=Optional[Callable])
 ReturnValueType = TypeVar('ReturnValueType', bound=Optional[Any])
 SideEffectType = TypeVar('SideEffectType', bound=Optional[Union[Callable, List]])
 MockMetadataKwargsType = TypeVar('MockMetadataKwargsType', bound=Dict[str, Any])
 FixtureType = TypeVar('FixtureType', bound=Callable[..., object])
 _Patch = TypeVar('_Patch', bound=_PatchType)
+TypeSpec = TypeVar('TypeSpec', bound=Optional[Callable[..., object]])
+TypeAutoSpec = TypeVar('TypeAutoSpec', bound=Optional[Union[bool, object]])
 
-__version__ = "0.1.5"
+__version__ = "0.2.0"
 
 
 class MockerBuilderWarning:
     """Base class for all warnings emitted by mocker-builder"""
 
     @staticmethod
     def warn(message: str):
@@ -134,14 +135,22 @@
     def create(self) -> bool:
         return self.patch_kwargs.get('create')
 
     @property
     def new_callable(self) -> NewCallableType:
         return self.patch_kwargs.get('new_callable')
 
+    @property
+    def spec(self) -> TypeSpec:
+        return self.patch_kwargs.get('spec')
+
+    @property
+    def autospec(self) -> TypeAutoSpec:
+        return self.patch_kwargs.get('autospec')
+
 
 try:
     import asyncio
 
     def _asyncio_future(result: Any) -> asyncio.Future:
         """Function called when patching async ``return_value``.
 
@@ -213,16 +222,22 @@
             )
 
         _patch = Patcher._mocker.mock_module.patch(
             mock_metadata.target_path,
             **mock_metadata.patch_kwargs
         )
         _mocked = _patch.start()
-        if (not mock_metadata.new) and (not mock_metadata.new_callable):
-            _mocked.mock_add_spec(spec=Type[_TMockType])
+        if all([
+            mock_metadata.new == DEFAULT,
+            not mock_metadata.new_callable,
+            not mock_metadata.spec,
+            not mock_metadata.autospec
+        ]):
+            _mocked.mock_add_spec(spec=_mocked)
+
         mock_metadata.is_active = True
         Patcher._mocker._patches.append(_patch)
         mock_metadata._patch = _patch
         mock_metadata._mock = _mocked
         Patcher._mocked_metadata.append(mock_metadata)
 
         if hasattr(_mocked, "reset_mock"):
@@ -230,14 +245,29 @@
 
         _tmock_patch = TMocker.PatchType(
             mock_metadata
         )
         return _tmock_patch
 
     @staticmethod
+    def mock_configure(mock_metadata: TMockMetadata) -> TMocker.PatchType:
+        mock_metadata._patch.stop()
+        mock_metadata.is_active = False
+        mock_configure = mock_metadata.patch_kwargs.pop('mock_configure')
+        mock_metadata.patch_kwargs.update(mock_configure)
+        try:
+            Patcher._mocker._patches.remove(mock_metadata._patch)
+        except ValueError:
+            print("Opss!", mock_metadata._patch, "Not found!")
+
+        return Patcher.dispatch(
+            mock_metadata
+        )
+
+    @staticmethod
     def _clean_up():
         """Our way to clean up patched data from mocker fixture."""
         print("\n######################## cleaning up ########################")
         for mock_metadata in Patcher._mocked_metadata:
             if not mock_metadata.is_active:
                 try:
                     Patcher._mocker._patches.remove(mock_metadata._patch)
@@ -287,15 +317,18 @@
         self,
         mock_metadata_kwargs: MockMetadataKwargsType
     ):
         kwargs = {}
         for attr in self._mock_keys_validate:
             value = mock_metadata_kwargs.get(attr)
             if value:
-                if attr in ['mock_configure', 'mock_kwargs']:
+                if attr in [
+                    'mock_configure',
+                    'mock_kwargs'
+                ]:
                     if isinstance(value, dict):
                         for key, data in value.items():
                             kwargs.update({key: data})
                         continue
                 kwargs.update({attr: value})
         self._mock_metadata.patch_kwargs = kwargs
 
@@ -510,14 +543,25 @@
             print(f"Mock {self.__get_mock()} started")
 
         def stop(self):
             self.__mock_metadata._patch.stop()
             self.__mock_metadata.is_active = False
             print(f"Mock {self.__get_mock()} stopped")
 
+        def configure_mock(self, **mock_configure: Dict):
+            if self.__mock_metadata.mock_configure:
+                self.__mock_metadata.mock_configure.update(mock_configure)
+            else:
+                self.__mock_metadata.mock_configure = mock_configure
+
+            _tpath = Patcher.mock_configure(
+                self.__mock_metadata
+            )
+            self.__mock_metadata = _tpath.__mock_metadata
+
     PatchType = _TPatch[_TMockType]
 
 
 TFixtureContentType = TypeVar('TFixtureContentType')
 
 
 class MockerBuilder(ABC):
```

### Comparing `mocker-builder-0.1.5/mocker_builder.egg-info/PKG-INFO` & `mocker-builder-0.2.0/mocker_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-builder
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python library to build mock tests dynamicaly using the mocker feature from pytest-mock lib
 Home-page: https://github.com/tgc77/mocker_builder
 Author: Tiago G Cunha
 Author-email: tikx.batera@gmail.com
 License: MIT
 Project-URL: Documentation, https://mocker-builder.readthedocs.io
 Project-URL: Source, https://github.com/tgc77/mocker_builder
```

### Comparing `mocker-builder-0.1.5/setup.py` & `mocker-builder-0.2.0/setup.py`

 * *Files identical despite different names*

