# Comparing `tmp/bipl-0.2.2.tar.gz` & `tmp/bipl-0.2.3.tar.gz`

## Comparing `bipl-0.2.2.tar` & `bipl-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.2/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.2/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.2/hatch_build.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.2.3/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.3/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.3/hatch_build.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.3/PKG-INFO
```

### Comparing `bipl-0.2.2/src/bipl/io/__init__.py` & `bipl-0.2.3/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/io/_dzi.py` & `bipl-0.2.3/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/io/_libs.py` & `bipl-0.2.3/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/io/_openslide.py` & `bipl-0.2.3/src/bipl/io/_openslide.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,24 +139,28 @@
         weakref.finalize(self, OSD.openslide_close, self.ptr)
 
         self._tags = self._get_metadata()
 
         bg_hex = self._tags.get('openslide.background-color', 'FFFFFF')
         self.bg_color: np.ndarray = np.frombuffer(bytes.fromhex(bg_hex), 'u1')
 
-        self.spacing = None
+        self.spacing = self._spacing()
+
+    def _spacing(self) -> float | None:
         mpp = (self._tags.get(f'openslide.mpp-{ax}') for ax in 'yx')
         if s := [float(m) for m in mpp if m]:
-            self.spacing = float(np.mean(s))
+            return float(np.mean(s))
+
+        if self._tags.get('tiff.ResolutionUnit') != 'centimeter':
+            return None
+        resolution = (self._tags.get(f'tiff.{ax}Resolution') for ax in 'YX')
+        if s := [(10_000 / float(v)) for v in resolution if v]:
+            return float(np.mean(s))
 
-        # TODO: handle offsets
-        # self.offset = *(int(self._tags.get(f'openslide.bounds-{ax}', 0))
-        #                 for ax in 'yx'),
-        # self.size = *(int(self._tags.get(f'openslide.bounds-{ax}', lim))
-        #               for ax, lim in zip(('height', 'width'), self.shape)),
+        return None
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}({addressof(self.ptr.contents):0x})'
 
     def _get_metadata(self) -> dict[str, str]:
         names = OSD.openslide_get_property_names(self.ptr)
         return {
```

### Comparing `bipl-0.2.2/src/bipl/io/_slide.py` & `bipl-0.2.3/src/bipl/io/_slide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/io/_slide_bases.py` & `bipl-0.2.3/src/bipl/io/_slide_bases.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/io/_tiff.py` & `bipl-0.2.3/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/ops/_mosaic.py` & `bipl-0.2.3/src/bipl/ops/_mosaic.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/src/bipl/ops/_util.py` & `bipl-0.2.3/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/LICENSE` & `bipl-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/README.md` & `bipl-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/hatch_build.py` & `bipl-0.2.3/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.2/pyproject.toml` & `bipl-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.2.2"
+version = "0.2.3"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.2.2/PKG-INFO` & `bipl-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.2.2
+Version: 0.2.3
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

