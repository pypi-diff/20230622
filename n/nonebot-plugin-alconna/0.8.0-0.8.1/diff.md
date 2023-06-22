# Comparing `tmp/nonebot-plugin-alconna-0.8.0.tar.gz` & `tmp/nonebot-plugin-alconna-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.8.0.tar", last modified: Thu Jun 22 16:10:33 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.8.1.tar", last modified: Thu Jun 22 16:21:51 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.8.0.tar` & `nonebot-plugin-alconna-0.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.0/LICENSE
--rw-r--r--   0        0        0     1524 2023-06-22 16:05:08.762119 nonebot-plugin-alconna-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.0/README.md
--rw-r--r--   0        0        0     1789 2023-06-22 16:05:08.741761 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0     5053 2023-06-22 16:08:58.794218 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3216 2023-06-22 15:30:18.392103 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2295 2023-06-22 14:54:15.807613 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1524 2023-06-22 16:21:04.954312 nonebot-plugin-alconna-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.1/README.md
+-rw-r--r--   0        0        0     1789 2023-06-22 16:21:04.935845 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0     5109 2023-06-22 16:21:04.974805 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2295 2023-06-22 14:54:15.807613 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.1/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.8.0/LICENSE` & `nonebot-plugin-alconna-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/pyproject.toml` & `nonebot-plugin-alconna-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.8.0"
+version = "0.8.1"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "arclet-alconna<2.0.0, >=1.7.7",
```

### Comparing `nonebot-plugin-alconna-0.8.0/README.md` & `nonebot-plugin-alconna-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .params import assign as assign
 from .params import match_path as match_path
 from .params import match_value as match_value
 from .rule import alconna as alconna
 from .rule import set_output_converter as set_output_converter
 from .config import Config
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 _meta_source = {
     "name": "Alconna 插件",
     "description": "提供 [Alconna](https://github.com/ArcletProject/Alconna) 的 Nonebot2 适配版本与工具",
     "usage": "matcher = on_alconna(...)",
     "homepage": "https://github.com/ArcletProject/Alconna",
     "type": "library",
```

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/__init__.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 mention_user: qqguild
 At: mirai
 kmarkdown: kook
 """
 
 
 def _handle_image(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12, telegram
+    if "file_id" in seg.data:  # ob12
         return Image(seg, id=seg.data["file_id"])
     if "image_key" in seg.data:  # feishu
         return Image(seg, url=seg.data["image_key"])
     if "file_key" in seg.data:  # kook
         return Image(seg, url=seg.data["file_key"])
     if "url" in seg.data:  # ob11, qqguild
         return Image(seg, url=seg.data["url"])
@@ -87,14 +87,15 @@
 
 
 
 _Image = gen_unit(
     Image,
     {
         "image": _handle_image,
+        "photo": lambda seg: Image(seg, id=seg.data["file_id"]),
         "Image": lambda seg: Image(seg, seg.data["url"], seg.data["imageId"]),
     }
 )
 
 
 def _handle_video(seg: MessageSegment):
     if "file_id" in seg.data:  # ob12, telegram
```

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Code = SegmentPattern("code", Entity, Entity.code)
 """该 Pattern 只用于发送"""
 Pre = SegmentPattern("pre", Entity, Entity.pre)
 TextLink = SegmentPattern("text_link", Entity, Entity.text_link)
 TextMention = SegmentPattern("text_mention", Entity, Entity.text_mention)
 CustomEmoji = SegmentPattern("custom_emoji", Entity, Entity.custom_emoji)
 
-Photo = SegmentPattern("photo", File, File.photo)
+Image = Photo = SegmentPattern("photo", File, File.photo)
 Voice = SegmentPattern("voice", File, File.voice)
 Animation = SegmentPattern("animation", File, File.animation)
 Audio = SegmentPattern("audio", File, File.audio)
 Document = SegmentPattern("document", File, File.document)
 Video = SegmentPattern("video", File, File.video)
 
 Sticker = SegmentPattern("sticker", UnCombinFile, UnCombinFile.sticker)
```

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/typings.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.0/PKG-INFO` & `nonebot-plugin-alconna-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.8.0
+Version: 0.8.1
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
```

