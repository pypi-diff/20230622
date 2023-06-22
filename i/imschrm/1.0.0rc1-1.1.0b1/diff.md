# Comparing `tmp/imschrm-1.0.0rc1.tar.gz` & `tmp/imschrm-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imschrm-1.0.0rc1.tar", last modified: Thu Jul 22 05:36:32 2021, max compression
+gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-wztb7eka\imschrm-1.1.0b1.tar", last modified: Thu Jun 22 15:52:51 2023, max compression
```

## Comparing `imschrm-1.0.0rc1.tar` & `imschrm-1.1.0b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.183542 imschrm-1.0.0rc1/
--rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.0.0rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     3702 2021-07-22 05:36:32.699917 imschrm-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2021-07-22 05:34:53.000000 imschrm-1.0.0rc1/README.md
--rw-rw-rw-   0        0        0       42 2021-07-22 05:36:32.699917 imschrm-1.0.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1329 2021-07-22 05:32:26.000000 imschrm-1.0.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.183542 imschrm-1.0.0rc1/src/
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.183542 imschrm-1.0.0rc1/src/main/
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.183542 imschrm-1.0.0rc1/src/main/python/
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.542959 imschrm-1.0.0rc1/src/main/python/imschrm/
--rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.0.0rc1/src/main/python/imschrm/__init__.py
--rw-rw-rw-   0        0        0    38857 2021-06-02 18:29:37.000000 imschrm-1.0.0rc1/src/main/python/imschrm/_gcpy_codepoints.py
--rw-rw-rw-   0        0        0     3640 2021-07-22 05:14:45.000000 imschrm-1.0.0rc1/src/main/python/imschrm/cli.py
--rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.0.0rc1/src/main/python/imschrm/doc_sequence.py
--rw-rw-rw-   0        0        0    11195 2021-07-22 05:30:27.000000 imschrm-1.0.0rc1/src/main/python/imschrm/hrm.py
-drwxrwxrwx   0        0        0        0 2021-07-22 05:36:32.183542 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/
--rw-rw-rw-   0        0        0     3702 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-07-22 05:36:31.000000 imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.843247 imschrm-1.1.0b1/
+-rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2981 2023-06-22 15:52:51.837227 imschrm-1.1.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2023-06-22 15:26:04.000000 imschrm-1.1.0b1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 15:52:51.846256 imschrm-1.1.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-06-22 15:24:41.000000 imschrm-1.1.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.126332 imschrm-1.1.0b1/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.132368 imschrm-1.1.0b1/src/main/
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.138361 imschrm-1.1.0b1/src/main/python/
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.659756 imschrm-1.1.0b1/src/main/python/imschrm/
+-rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b1/src/main/python/imschrm/__init__.py
+-rw-rw-rw-   0        0        0     3640 2021-07-22 05:14:45.000000 imschrm-1.1.0b1/src/main/python/imschrm/cli.py
+-rw-rw-rw-   0        0        0   366016 2022-04-06 16:51:28.000000 imschrm-1.1.0b1/src/main/python/imschrm/codepoint_sets.py
+-rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.1.0b1/src/main/python/imschrm/doc_sequence.py
+-rw-rw-rw-   0        0        0    11595 2023-06-22 15:09:58.000000 imschrm-1.1.0b1/src/main/python/imschrm/hrm.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.417122 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/top_level.txt
```

### Comparing `imschrm-1.0.0rc1/LICENSE.txt` & `imschrm-1.1.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imschrm-1.0.0rc1/README.md` & `imschrm-1.1.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
      __  _  _  ____   ___  _  _  ____  _  _ 
     (  )( \/ )/ ___) / __)/ )( \(  _ \( \/ )
      )( / \/ \\___ \( (__ ) __ ( )   // \/ \
     (__)\_)(_/(____/ \___)\_)(_/(__\_)\_)(_/
 
 ## Introduction
 
-_imschrm_ validates [IMSC](https://www.w3.org/TR/ttml-imsc1.1) documents against the [IMSC Hypothetical Render Model
-(HRM)](https://www.w3.org/TR/ttml-imsc1.1/#hypothetical-render-model), which constrains document complexity.
+_imschrm_ validates [IMSC](https://www.w3.org/TR/ttml-imsc/) documents against the [IMSC Hypothetical Render Model
+(HRM)](https://www.w3.org/TR/2023/CR-imsc-hrm-20230622/), which constrains document complexity.
 
 _imschrm_ consists of a library and command line application written in pure Python, and uses
 [ttconv](https://github.com/sandflow/ttconv).
 
 ## Known issues
 
 Issues are tracked at https://github.com/sandflow/imscHRM/issues.
@@ -78,8 +78,7 @@
 
 ```sh
 pipenv install --dev
 mkdir build
 export PYTHONPATH=src/main/python
 pipenv run python src/main/python/imschrm/cli.py src/test/resources/ttml/fail001.ttml
 ```
-
```

### Comparing `imschrm-1.0.0rc1/setup.py` & `imschrm-1.1.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
   name='imschrm', 
-  version='1.0.0rc1',
+  version='1.1.0b1',
   description='Validates IMSC documents against the IMSC HRM',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Sandflow Consulting LLC',
   author_email='info@sandflow.com',
   url='https://www.sandflow.com',
   project_urls={
```

### Comparing `imschrm-1.0.0rc1/src/main/python/imschrm/cli.py` & `imschrm-1.1.0b1/src/main/python/imschrm/cli.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.0.0rc1/src/main/python/imschrm/doc_sequence.py` & `imschrm-1.1.0b1/src/main/python/imschrm/doc_sequence.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.0.0rc1/src/main/python/imschrm/hrm.py` & `imschrm-1.1.0b1/src/main/python/imschrm/hrm.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from numbers import Number
 import logging
 
 import ttconv.isd
 import ttconv.style_properties as styles
 import ttconv.model
 
-from ._gcpy_codepoints import GCPY_12 
+from .codepoint_sets import GCPY_12, RENGI_06
 
 LOGGER = logging.getLogger(__name__)
 
 _BDRAW = 12
 _GCPY_BASE = 12
 _GCPY_OTHER = 3
 
@@ -53,31 +53,33 @@
 _IPD = 1
 
 @dataclass
 class ISDStatistics:
   dur: Number = 0 # HRM ISD time
   dur_d: Number = 0 # HRM background drawing time
   nbg_total: Number = 0 # Number of backgrounds drawn
+  clear: bool = False # Whether the root container had to be cleared
   dur_t: Number = 0 # HRM text drawing time
   ngra_t: Number = 0 # Total Normalized Rendered Glyph Area
   gcpy_count: Number = 0 # Total number of glyphs copied
   gren_count: Number = 0 # Total number of glyphs rendered
+  is_empty: bool = False # Does the ISD contain any content
 
 
 class EventHandler:
   '''Allows a callee to inform the caller of events that occur during processing. Typically
   overridden by the caller.
   '''
   
   @staticmethod
   def _format_message(msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     return (
       f"{msg} at {float(time_offset):.3f}s (doc #{doc_index})\n"
       f"  available time: {float(available_time):.3f}s | HRM time: {float(stats.dur):.3f}\n"
-      f"  Glyph copy count: {stats.gcpy_count} | render count: {stats.gren_count} | Background draw count: {stats.nbg_total}\n"
+      f"  Glyph copy count: {stats.gcpy_count} | render count: {stats.gren_count} | Background draw count: {stats.nbg_total} | Clear: {stats.clear}\n"
     )
 
 
   def info(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     LOGGER.info(EventHandler._format_message(msg, doc_index, time_offset, available_time, stats))
 
   def warn(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
@@ -95,34 +97,36 @@
   `isd_iterator` returns a sequence of tuplets `(begin, ISD)`, where `ISD` is an ISD instance whose
   active interval starts at `begin` seconds and ends immediately before the `begin` value of the next 
   ISD. Errors, warnings and info messages are signalled through callbacks on the `event_handler`.
   '''
 
   hrm = HRM()
 
-  last_offset = 0
+  last_render_time = -_IPD
 
   for doc_index, (time_offset, isd) in enumerate(isd_iterator):
 
-    if time_offset < last_offset:
+    if time_offset <= last_render_time:
       raise RuntimeError("ISDs are not in order of increasing offset")
 
-    stats = hrm.next_isd(isd, doc_index)
+    stats = hrm.next_isd(isd)
 
-    avail_render_time = _IPD if doc_index == 0 else time_offset - last_offset
+    avail_render_time = min(_IPD, time_offset - last_render_time)
 
-    if stats.dur > avail_render_time:
-      event_handler.error("Rendering time exceeded", doc_index, time_offset, avail_render_time, stats)
+    event_handler.debug("Processed document", doc_index, time_offset, avail_render_time, stats)
 
-    if stats.ngra_t > 1:
-      event_handler.error("NGBS exceeded", doc_index, time_offset, avail_render_time, stats)
+    if not stats.is_empty:
+      if stats.dur > avail_render_time:
+        event_handler.error("Rendering time exceeded", doc_index, time_offset, avail_render_time, stats)
 
-    event_handler.debug("Processed document", doc_index, time_offset, avail_render_time, stats)
+      if stats.ngra_t > _NGBS:
+        event_handler.error("NGBS exceeded", doc_index, time_offset, avail_render_time, stats)
+
+      last_render_time = time_offset
 
-    last_offset = time_offset
 
 @dataclass(frozen=True)
 class _Glyph:
   char: str
   color : styles.ColorType
   font_family: typing.Tuple[typing.Union[str, styles.GenericFontFamilyType]]
   font_size: styles.LengthType
@@ -137,69 +141,78 @@
 
   def __init__(self):
     self.back_buffer: typing.Set[_Glyph] = set()
     self.isd_stats: ISDStatistics = None
     
   def next_isd(
     self,
-    isd: typing.Type[ttconv.isd.ISD],
-    index_n: int,
+    isd: typing.Type[ttconv.isd.ISD]
     ) -> ISDStatistics:
 
     self.isd_stats = ISDStatistics()
 
-    self._compute_dur_t(isd, index_n)
+    self._compute_dur_t(isd)
 
-    self._compute_dur_d(isd, index_n)
+    self._compute_dur_d(isd)
 
     self.isd_stats.dur = self.isd_stats.dur_t + self.isd_stats.dur_d
 
     return self.isd_stats
 
   def _compute_dur_d(
     self,
-    isd: typing.Type[ttconv.isd.ISD],
-    index_n: int
+    isd: typing.Type[ttconv.isd.ISD]
     ):
 
-    draw_area = 0 if index_n == 0 else 1
+    self.isd_stats.is_empty = True
+
+    draw_area = 0
 
     if isd is not None:
       for region in isd.iter_regions():
 
         if not _is_presented_region(region):
           continue
 
+        self.isd_stats.is_empty = False
+
         nbg = 0
 
         for element in region.dfs_iterator():
 
           # should body elements really be excluded? -> NO
           # should transparent backgrounds really be counted? -> NO
           # should span and br really be included -> yes for now
+          # should br really be included -> no
+
+          if isinstance(element, ttconv.model.Br):
+            continue
 
           bg_color = element.get_style(styles.StyleProperties.BackgroundColor)
 
           if bg_color is not None:
             if bg_color.ident is not styles.ColorType.Colorimetry.RGBA8:
               raise RuntimeError(f"Unsupported colorimetry system: {bg_color.ident}")
 
             if bg_color.components[3] != 0:
               nbg += 1
 
         draw_area += _region_normalized_size(region) * nbg
 
         self.isd_stats.nbg_total += nbg
 
+    draw_area += 0 if self.isd_stats.is_empty else 1
+
+    self.isd_stats.clear = draw_area != 0
+
     self.isd_stats.dur_d = draw_area / _BDRAW
 
   def _compute_dur_t(
     self,
-    isd: typing.Type[ttconv.isd.ISD],
-    _index_n: int
+    isd: typing.Type[ttconv.isd.ISD]
     ):
 
     front_buffer = set()
 
     if isd is not None:
 
       for region in isd.iter_regions():
@@ -267,15 +280,15 @@
   return font_size.value * font_size.value / 10000
 
 def _compute_ren_g(char: str):
 
   if len(char) != 1:
     raise ValueError("Argument must be a string of length 1")
 
-  return _REN_G_CJK if 0x4E00 <= ord(char) <= 0x9FFF else _REN_G_OTHER
+  return _REN_G_CJK if ord(char) in RENGI_06 else _REN_G_OTHER
 
 def _compute_gcpy(char: str):
 
   if len(char) != 1:
     raise ValueError("Argument must be a string of length 1")
 
   return _GCPY_BASE if ord(char) in GCPY_12 else _GCPY_OTHER
```

### Comparing `imschrm-1.0.0rc1/src/main/python/imschrm.egg-info/SOURCES.txt` & `imschrm-1.1.0b1/src/main/python/imschrm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 src/main/python/imschrm.egg-info/PKG-INFO
 src/main/python/imschrm.egg-info/SOURCES.txt
 src/main/python/imschrm.egg-info/dependency_links.txt
 src/main/python/imschrm.egg-info/entry_points.txt
 src/main/python/imschrm.egg-info/requires.txt
 src/main/python/imschrm.egg-info/top_level.txt
 src/main/python/imschrm/__init__.py
-src/main/python/imschrm/_gcpy_codepoints.py
 src/main/python/imschrm/cli.py
+src/main/python/imschrm/codepoint_sets.py
 src/main/python/imschrm/doc_sequence.py
 src/main/python/imschrm/hrm.py
 src/main/python/imschrm.egg-info/PKG-INFO
 src/main/python/imschrm.egg-info/SOURCES.txt
 src/main/python/imschrm.egg-info/dependency_links.txt
 src/main/python/imschrm.egg-info/entry_points.txt
 src/main/python/imschrm.egg-info/requires.txt
```

