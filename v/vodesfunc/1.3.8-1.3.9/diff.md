# Comparing `tmp/vodesfunc-1.3.8.tar.gz` & `tmp/vodesfunc-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.8.tar", last modified: Wed May 24 12:08:59 2023, max compression
+gzip compressed data, was "vodesfunc-1.3.9.tar", last modified: Wed Jun 21 22:02:38 2023, max compression
```

## Comparing `vodesfunc-1.3.8.tar` & `vodesfunc-1.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.777507 vodesfunc-1.3.8/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.8/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-05-24 12:08:59.776176 vodesfunc-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 12:08:59.777507 vodesfunc-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.756520 vodesfunc-1.3.8/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.8/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-05-24 12:08:42.000000 vodesfunc-1.3.8/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.8/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.775166 vodesfunc-1.3.8/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.8/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.8/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.8/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.8/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.8/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.8/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32395 2023-05-13 20:45:39.000000 vodesfunc-1.3.8/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.3.8/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12864 2023-05-13 20:45:35.000000 vodesfunc-1.3.8/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.8/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.8/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    14058 2023-05-24 12:07:39.000000 vodesfunc-1.3.8/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.8/vodesfunc/types.py
--rw-rw-rw-   0        0        0     7717 2023-05-04 22:57:47.000000 vodesfunc-1.3.8/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.769662 vodesfunc-1.3.8/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/README.md
+-rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.417457 vodesfunc-1.3.9/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.9/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-06-21 22:02:18.000000 vodesfunc-1.3.9/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.9/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.429459 vodesfunc-1.3.9/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.9/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.9/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.9/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.9/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.9/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.9/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32395 2023-05-13 20:45:39.000000 vodesfunc-1.3.9/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.3.9/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    12864 2023-05-13 20:45:35.000000 vodesfunc-1.3.9/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.9/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.9/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14058 2023-05-24 12:07:39.000000 vodesfunc-1.3.9/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.9/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     6942 2023-06-21 22:00:50.000000 vodesfunc-1.3.9/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.425459 vodesfunc-1.3.9/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.8/LICENSE` & `vodesfunc-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/PKG-INFO` & `vodesfunc-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.8
+Version: 1.3.9
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.8/setup.py` & `vodesfunc-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/aa.py` & `vodesfunc-1.3.9/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/convert.py` & `vodesfunc-1.3.9/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/download.py` & `vodesfunc-1.3.9/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/fonts.py` & `vodesfunc-1.3.9/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/muxing.py` & `vodesfunc-1.3.9/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/parsing.py` & `vodesfunc-1.3.9/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/auto/webhook.py` & `vodesfunc-1.3.9/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/automation.py` & `vodesfunc-1.3.9/vodesfunc/automation.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/denoise.py` & `vodesfunc-1.3.9/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/descale.py` & `vodesfunc-1.3.9/vodesfunc/descale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/misc.py` & `vodesfunc-1.3.9/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/noise.py` & `vodesfunc-1.3.9/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/scale.py` & `vodesfunc-1.3.9/vodesfunc/scale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/types.py` & `vodesfunc-1.3.9/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.8/vodesfunc/util.py` & `vodesfunc-1.3.9/vodesfunc/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import os
 import binascii
 
 core = vs.core
 
 
 __all__: list[str] = [
-    'set_output_source', 'out_src',
     'set_output', 'out',
     'src_file', 'SRC_FILE', 'src', 'source',
 ]
 
 class src_file:
 
     file: Path
@@ -111,56 +110,33 @@
         sub.Popen(f"dgindexnv -i \"{path.name}\" -h -o \"{dgiFile.name}\" -e",
                   shell=True, stdout=sub.DEVNULL, cwd=path.parent.resolve(True)).wait()
         if path.with_suffix('.log').exists() and delete_dgi_log:
             os.remove(path.with_suffix('.log').resolve(True))
         return core.dgdecodenv.DGSource(dgiFile.resolve(True), **kwargs)
 
 
-def set_output(clip: vs.VideoNode, name: str = None, frame_info: bool = False, allow_comp: bool = True) -> vs.VideoNode:
+def set_output(clip: vs.VideoNode, name: str = None, frame_info: bool = False, allow_comp: bool = True, cache: bool | None = None) -> vs.VideoNode:
     """
     Outputs a clip. Less to type.
     Designed to be used with the good ol 'from vodesfunc import *' and the 'out' alias
     """
-    if name is not None:
-        clip = clip.std.SetFrameProp('Name', data=name)
-    if not allow_comp:
-        clip = clip.std.SetFrameProp('_VSPDisableComp', 1)
     if frame_info:
-        output = _print_frameinfo(clip, name)
-        output.set_output(len(vs.get_outputs()))
-    else:
-        clip.set_output(len(vs.get_outputs()))
-
-    return clip
-
-
-def set_output_source(filePath: str | src_file, clip: vs.VideoNode = None, frame_info: bool = False) -> vs.VideoNode:
-    """
-    Outputs your source clip while also outputting the audio for it
-    so scenefiltering becomes less boring
+        clip = _print_frameinfo(clip, name)
 
-    Also returns the clip in case you wanna use it at the start of your script
-    """
-    filePath = filePath if isinstance(filePath, str) else str(filePath.file.resolve())
-
-    if clip is None:
-        clip = src(filePath)
-
-    clip = clip.std.SetFrameProp('Name', data='Source')
-    if frame_info:
-        output = _print_frameinfo(clip, 'Source')
-        output.set_output(len(vs.get_outputs()))
-    else:
+    try:
+        from vspreview import is_preview, set_output as setsu_sucks
+        if cache is None:
+            cache = is_preview()
+        setsu_sucks(clip, name=name, cache=cache, disable_comp=not allow_comp)
+    except:
+        if name is not None:
+            clip = clip.std.SetFrameProp('Name', data=name)
         clip.set_output(len(vs.get_outputs()))
-
-    audio = core.bs.AudioSource(filePath)
-    audio.set_output(len(vs.get_outputs()) + 20)
     return clip
 
-
 def _print_frameinfo(clip: vs.VideoNode, title: str = '') -> vs.VideoNode:
     style = ("sans-serif,20,&H00FFFFFF,&H000000FF,&H00000000,&H00000000,"
              "0,0,0,0,100,100,0,0,1,2,0,7,10,10,10,1")
 
     def FrameProps(n: int, f: vs.VideoFrame, clip: vs.VideoNode) -> vs.VideoNode:
         if "_PictType" in f.props:
             info = f"Frame {n} of {clip.num_frames}\nPicture type: {f.props['_PictType'].decode()}"
@@ -194,9 +170,8 @@
         if len(zone) < 4:
             raise ValueError(f"Zone {zone} is invalid.")
         return True
     else:
         return False
 
 out = set_output
-out_src = set_output_source
 source = src
```

### Comparing `vodesfunc-1.3.8/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.3.9/vodesfunc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.8
+Version: 1.3.9
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.8/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.3.9/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

