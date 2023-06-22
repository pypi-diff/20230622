# Comparing `tmp/bipl-0.1.2.tar.gz` & `tmp/bipl-0.2.4.tar.gz`

## Comparing `bipl-0.1.2.tar` & `bipl-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.2/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.2/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.2/hatch_build.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.2.4/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.4/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.4/hatch_build.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.4/PKG-INFO
```

### Comparing `bipl-0.1.2/src/bipl/io/__init__.py` & `bipl-0.2.4/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_dzi.py` & `bipl-0.2.4/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_libs.py` & `bipl-0.2.4/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_openslide.py` & `bipl-0.2.4/src/bipl/io/_openslide.py`

 * *Files 7% similar despite different names*

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
@@ -182,7 +186,16 @@
 
     def get(self, key: str) -> Item:
         name = key.encode()
         w, h = c_int64(), c_int64()
         OSD.openslide_get_associated_image_dimensions(self.ptr, name, byref(w),
                                                       byref(h))
         return _Item((h.value, w.value, 3), name, self)
+
+    @property
+    def bbox(self) -> tuple[slice, slice]:
+        y, x = (
+            int(self._tags.get(f'openslide.bounds-{ax}', 0)) for ax in 'yx')
+        h, w = (
+            int(self._tags.get(f'openslide.bounds-{ax}', 0)) or None
+            for ax in ('height', 'width'))
+        return slice(y, h), slice(x, w)
```

### Comparing `bipl-0.1.2/src/bipl/io/_slide.py` & `bipl-0.2.4/src/bipl/io/_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from bisect import bisect_right
 from pathlib import Path
 from typing import final
 
 import cv2
 import numpy as np
-from glow import memoize
+from glow import memoize, shared_call, weak_memoize
 
 from ._openslide import Openslide
 from ._slide_bases import REGISTRY, Driver, Item, Lod, normalize
 from ._tiff import Tiff
 
 # TODO: inside Slide.open import ._slide.registry,
 # TODO: and in ._slide.registry do registration and DLL loading
@@ -21,15 +21,17 @@
 
 Openslide.register('bif mrxs ndpi scn svs svsslide tif tiff vms vmu')
 Tiff.register('svs tif tiff')
 
 _MAX_BYTES = int(os.environ.get('GLOW_SLIDE_BYTES') or 102_400)
 
 
-@memoize(capacity=_MAX_BYTES, policy='lru')
+@shared_call  # merge duplicate calls
+@weak_memoize  # reuse result if it's already exist, but used by someone else
+@memoize(capacity=_MAX_BYTES, policy='lru')  # keep LRU for unused results
 def _cached_open(path: Path) -> Slide:
     if not path.exists():
         raise FileNotFoundError(path)
 
     if tps := REGISTRY.get(path.suffix):
         last_exc = BaseException()
         for tp in reversed(tps):  # Loop over types to find non-failing
@@ -88,14 +90,15 @@
             elif key := item.key:
                 self.extras[key] = item
 
         self.pools = *sorted(lods.keys()),
         self.lods = *(lods[pool] for pool in self.pools),
         self.shape = self.lods[0].shape
         self.spacing = self.lods[0].spacing
+        self.bbox = driver.bbox
 
         self.extras |= driver.named_items()
         self.driver = driver_cls.__name__
 
     def __reduce__(self) -> tuple:
         return Slide.open, (self.path, )
 
@@ -107,21 +110,20 @@
         return f'{type(self).__name__}({line})'
 
     def best_lod_for(self, pool: float) -> tuple[int, Lod]:
         """Gives the most detailed LOD below `pool`"""
         idx = max(bisect_right(self.pools, pool) - 1, 0)
         return self.pools[idx], self.lods[idx]
 
-    def pool(self, zoom: int) -> Lod:
+    def pool(self, zoom: float, *, eps: float = 0.01) -> Lod:
         """Use like `slide.pool(4)[y0:y1, x0:x1]` call"""
-        p, lod = self.best_lod_for(zoom)
+        p, lod = self.best_lod_for(zoom * max(1, 1 + eps))
         if p == zoom:
             return lod
-        assert zoom % p == 0, 'fractional pooling is not supported'
-        return lod.downscale(zoom // p)
+        return lod.rescale(p / zoom)
 
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
         """Retrieves tile"""
         # TODO: Ignore step, always redirect to self.lods[0].__getitem__
         slices = normalize(key, self.shape)
 
         step0, step1 = (s.step for s in slices)
```

### Comparing `bipl-0.1.2/src/bipl/io/_slide_bases.py` & `bipl-0.2.4/src/bipl/io/_slide_bases.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,34 +58,38 @@
         return self.crop(slices)
 
     @final
     def __array__(self) -> np.ndarray:
         """Reads whole LOD in single call"""
         return self[:, :]
 
-    def downscale(self, pool: int) -> Lod:
-        if pool == 1:
+    def rescale(self, scale: float) -> Lod:
+        if scale == 1:
             return self
         h, w, c = self.shape
         return ProxyLod(
-            (h // pool, w // pool, c),
-            (self.spacing * pool if self.spacing else None),
-            pool,
+            # TODO: round/ceil/floor ?
+            (round(h * scale), round(w * scale), c),
+            (self.spacing / scale if self.spacing else None),
+            scale,
             self.base if isinstance(self, ProxyLod) else self,
         )
 
 
 @dataclass(frozen=True)
 class ProxyLod(Lod):
-    pool: int
+    scale: float
     base: Lod
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
-        src_slices = *(slice(s.start * self.pool, s.stop * self.pool)
-                       for s in slices),
+        src_slices = *[
+            # TODO: round/ceil/floor ?
+            slice(round(s.start / self.scale), round(s.stop / self.scale))
+            for s in slices
+        ],
         image = self.base[src_slices]
 
         shape = *((s.stop - s.start) for s in slices),
         return cv2.resize(image, shape[::-1], interpolation=cv2.INTER_AREA)
 
 
 class Driver:
@@ -114,7 +118,11 @@
     def keys(self) -> list[str]:
         """List of names for named items"""
         return []
 
     def get(self, key: str) -> Item:
         """Gives named item"""
         raise NotImplementedError
+
+    @property
+    def bbox(self) -> tuple[slice, slice]:
+        return slice(None), slice(None)
```

### Comparing `bipl-0.1.2/src/bipl/io/_tiff.py` & `bipl-0.2.4/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/ops/_mosaic.py` & `bipl-0.2.4/src/bipl/ops/_mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,19 +291,16 @@
     """
     stride: int
     source: Iterable[Tile]
 
     def __iter__(self) -> Iterator[Tile]:
         for t in self.source:
             vec = *(c // self.stride for c in t.vec),
-            yield Tile(
-                idx=t.idx,
-                vec=vec,  # type: ignore[arg-type]
-                data=t.data[::self.stride, ::self.stride],
-            )
+            data = t.data[::self.stride, ::self.stride]
+            yield Tile(idx=t.idx, vec=vec, data=data)  # type: ignore[arg-type]
 
 
 @dataclass
 class _TiledArrayView(_View):
     """
     Extracts tiles from array.
     Yields same-sized tiles with overlaps.
@@ -318,15 +315,16 @@
 
         ih, iw = self.ishape
         step = self.m.step // scale
         pad = self.m.overlap // (scale * 2)
 
         mh, mw = (ih * step), (iw * step)
         if mask.shape[:2] != (mh, mw):
-            mask_pad = [(0, s1 - s0) for s0, s1 in zip(mask.shape, (mh, mw))]
+            mask_pad = [(0, max(0, s1 - s0))
+                        for s0, s1 in zip(mask.shape, (mh, mw))]
             mask = np.pad(mask, mask_pad)[:mh, :mw]
 
         if self.m.overlap:
             kernel = np.ones((3, 3), dtype='u1')
             mask = cv2.dilate(mask, kernel, iterations=pad)
 
         if pad:
```

### Comparing `bipl-0.1.2/src/bipl/ops/_util.py` & `bipl-0.2.4/src/bipl/ops/_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-__all__ = ['get_trapz', 'probs_to_hsv']
+__all__ = ['get_trapz', 'probs_to_rgb_heatmap']
 
 import cv2
 import numpy as np
 
 
-def probs_to_hsv(prob: np.ndarray) -> np.ndarray:
+def probs_to_rgb_heatmap(prob: np.ndarray) -> np.ndarray:
     """Converts probability array of (H W C) shape to (H W 3) RGB image"""
     assert prob.ndim == 3
+    h, w, c = prob.shape
     if not prob.size:
-        return np.empty((*prob.shape[:2], 3), dtype='u1')
+        return np.empty((h, w, 3), dtype='u1')
 
     hue = prob.argmax(-1).astype('u1')
     value = prob.max(-1)
     if value.dtype != 'u1':
         value *= 255
         value = value.round().astype('u1')
 
-    hue_lut = (np.arange(256) * (127 / prob.shape[2])).round().astype('u1')
+    hue_lut = np.zeros(256, 'u1')
+    hue_lut[:c] = np.linspace(0, 127, c, endpoint=False, dtype='u1')
     hsv = cv2.merge([
         cv2.LUT(hue, hue_lut),
-        np.broadcast_to(np.uint8(255), prob.shape[:2]),
+        np.broadcast_to(np.uint8(255), (h, w)),
         value,
     ])
     return cv2.cvtColor(hsv, cv2.COLOR_HSV2RGB)
 
 
 def get_trapz(step: int, overlap: int) -> np.ndarray:
     """Returns trapezional window kernel to apply stiching"""
```

### Comparing `bipl-0.1.2/LICENSE` & `bipl-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/README.md` & `bipl-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/hatch_build.py` & `bipl-0.2.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/pyproject.toml` & `bipl-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.1.2"
+version = "0.2.4"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
-    "glow~=0.12.0",
+    "glow~=0.12.7",
     "imagecodecs",
     "lxml",
     "numpy~=1.21",
     "opencv-python~=4.0",
     "tqdm",
 ]
 
@@ -47,25 +47,25 @@
 dev-core = [
     "flake8~=6.0.0",
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
-    "mypy~=0.990",
-    "pytest~=6.0",
-    "ruff~=0.0.264",
+    "mypy~=1.3.0",
+    "pytest~=7.3",
+    "ruff~=0.0.270",
     "yapf~=0.33.0",
 ]
 dev = [
     "bipl[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
-    "typing-extensions~=4.4",
+    "typing-extensions~=4.6",
 ]
 dev-wemake = [
     "bipl[dev-core]",
     "wemake-python-styleguide~=0.15.0",
 ]
 
 [project.urls]
```

### Comparing `bipl-0.1.2/PKG-INFO` & `bipl-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.1.2
+Version: 0.2.4
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
@@ -33,34 +33,34 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Requires-Dist: glow~=0.12.0
+Requires-Dist: glow~=0.12.7
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
 Requires-Dist: numpy~=1.21
 Requires-Dist: opencv-python~=4.0
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: bipl[dev-core]; extra == 'dev'
 Requires-Dist: flake8-alphabetize; extra == 'dev'
-Requires-Dist: typing-extensions~=4.4; extra == 'dev'
+Requires-Dist: typing-extensions~=4.6; extra == 'dev'
 Provides-Extra: dev-core
 Requires-Dist: flake8-pie; extra == 'dev-core'
 Requires-Dist: flake8-pyi; extra == 'dev-core'
 Requires-Dist: flake8-pyproject; extra == 'dev-core'
 Requires-Dist: flake8-simplify; extra == 'dev-core'
 Requires-Dist: flake8~=6.0.0; extra == 'dev-core'
 Requires-Dist: isort; extra == 'dev-core'
-Requires-Dist: mypy~=0.990; extra == 'dev-core'
-Requires-Dist: pytest~=6.0; extra == 'dev-core'
-Requires-Dist: ruff~=0.0.264; extra == 'dev-core'
+Requires-Dist: mypy~=1.3.0; extra == 'dev-core'
+Requires-Dist: pytest~=7.3; extra == 'dev-core'
+Requires-Dist: ruff~=0.0.270; extra == 'dev-core'
 Requires-Dist: yapf~=0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: bipl[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Description-Content-Type: text/markdown
 
 # BIPL is a Big Image Python Library
```

