# Comparing `tmp/nonebot-plugin-alconna-0.7.0.tar.gz` & `tmp/nonebot-plugin-alconna-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.7.0.tar", last modified: Thu Jun  1 09:05:07 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.8.0.tar", last modified: Thu Jun 22 16:10:33 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.7.0.tar` & `nonebot-plugin-alconna-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.7.0/LICENSE
--rw-r--r--   0        0        0     1524 2023-06-01 08:47:38.630190 nonebot-plugin-alconna-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8521 2023-06-01 08:55:17.953962 nonebot-plugin-alconna-0.7.0/README.md
--rw-r--r--   0        0        0     1789 2023-06-01 08:53:41.996763 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3116 2023-05-31 10:32:51.341066 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2094 2023-05-31 10:32:51.240029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8601 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1524 2023-06-22 16:05:08.762119 nonebot-plugin-alconna-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.0/README.md
+-rw-r--r--   0        0        0     1789 2023-06-22 16:05:08.741761 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0     5053 2023-06-22 16:08:58.794218 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3216 2023-06-22 15:30:18.392103 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2295 2023-06-22 14:54:15.807613 nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.0/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.7.0/LICENSE` & `nonebot-plugin-alconna-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/pyproject.toml` & `nonebot-plugin-alconna-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.7.0"
+version = "0.8.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "arclet-alconna<2.0.0, >=1.7.7",
@@ -39,15 +39,15 @@
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-adapter-feishu>=2.0.0b8",
     "nonebot-adapter-console>=0.3.2",
     "nonebot-adapter-ding>=2.0.0a16",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-minecraft>=0.1.1",
     "nonebot-adapter-ntchat>=0.3.5",
-    "nonebot-adapter-qqguild>=0.2.2",
+    "nonebot-adapter-qqguild>=0.2.3",
     "nonebot-adapter-telegram>=0.1.0b10",
 ]
 
 [tool.pdm.build]
 includes = [
     "src/nonebot_plugin_alconna",
 ]
```

### Comparing `nonebot-plugin-alconna-0.7.0/README.md` & `nonebot-plugin-alconna-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,32 +75,35 @@
 assert res.matched
 assert res.query("target").data['user_id'] == '123'
 ```
 
 通用标注:
 
 ```python
-from nonebot.adapters.onebot.v12 import Message as Ob12M, MessageSegment as Ob12MS
-from nonebot.adapters.onebot.v11 import Message as Ob11M, MessageSegment as Ob11MS
+from nonebot.adapters.onebot.v12 import Message as Ob12Msg, MessageSegment as Ob12MS
+from nonebot.adapters.onebot.v11 import Message as Ob11Msg, MessageSegment as Ob11MS
 from nonebot_plugin_alconna.adapters import At
 from arclet.alconna import Alconna, Args
 
-msg1 = Ob12M(["Hello!", Ob12MS.mention("123")])
-print(msg1)  # Hello![mention:user_id=123]
-msg2 = Ob11M(["Hello!", Ob11MS.at(123)])
-print(msg2)  # Hello![CQ:at,qq=123]
+msg1 = Ob12Msg(["Hello!", Ob12MS.mention("123")]) # Hello![mention:user_id=123]
+msg2 = Ob11Msg(["Hello!", Ob11MS.at(123)]) # Hello![CQ:at,qq=123]
+
 
 alc = Alconna("Hello!", Args["target", At])
 res1 = alc.parse(msg1)
 assert res1.matched
-assert res1.query("target").data['user_id'] == '123'
+target = res1.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
 
 res2 = alc.parse(msg2)
 assert res2.matched
-assert res2.query("target").data['qq'] == 123
+target = res2.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
 ```
 
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
```

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .params import assign as assign
 from .params import match_path as match_path
 from .params import match_value as match_value
 from .rule import alconna as alconna
 from .rule import set_output_converter as set_output_converter
 from .config import Config
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 _meta_source = {
     "name": "Alconna 插件",
     "description": "提供 [Alconna](https://github.com/ArcletProject/Alconna) 的 Nonebot2 适配版本与工具",
     "usage": "matcher = on_alconna(...)",
     "homepage": "https://github.com/ArcletProject/Alconna",
     "type": "library",
```

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,7 +68,10 @@
 Video = SegmentPattern("video", File, File.video)
 
 Sticker = SegmentPattern("sticker", UnCombinFile, UnCombinFile.sticker)
 VideoNote = SegmentPattern("video_note", UnCombinFile, UnCombinFile.video_note)
 
 Mentions = UnionPattern([Mention, TextMention, TextLink])
 """联合接收 Mention, TextMention, TextLink, 不能用于发送"""
+
+Videos = UnionPattern([Video, Animation])
+"""联合接收 Video, Animation, 不能用于发送"""
```

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.8.0/src/nonebot_plugin_alconna/typings.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Awaitable, Callable, Generic, Literal, TypeVar, Union
 from typing_extensions import ParamSpec, TypeAlias
 
 from nepattern import BasePattern, MatchFailed, PatternModel
 from nonebot.internal.adapter.message import Message, MessageSegment
 from tarina import lang
 
+T = TypeVar("T")
 TMS = TypeVar("TMS", bound=MessageSegment)
 P = ParamSpec("P")
 
 
 class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
     def __init__(
         self,
@@ -44,22 +45,27 @@
         return self.call(*args, **kwargs)  # type: ignore
 
 
 OutputType = Literal["help", "shortcut", "completion"]
 TConvert: TypeAlias = Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
 
 
-def _isinstance(seg: MessageSegment, accepts: set[str]):
-    return seg if seg.type.lower() in accepts else None
-
+def _isinstance(seg: MessageSegment, mapping: dict[str, Callable[[MessageSegment], Any]]):
+    if (key := seg.type) not in mapping:
+        return
+    if res := mapping[key](seg):
+        return res
+    else:
+        return
 
 def gen_unit(
-    name: str, accepts: set[str], additional: Callable[..., bool] | None = None
-) -> BasePattern[MessageSegment]:
+    model: type[T], mapping: dict[str, Callable[[MessageSegment], Any]], additional: Callable[..., bool] | None = None
+) -> BasePattern[T]:
     return BasePattern(
-        name,
+        model.__name__,
         PatternModel.TYPE_CONVERT,
-        Any,
-        lambda self, x: _isinstance(x, accepts),
+        model,
+        lambda self, x: _isinstance(x, mapping),
         accepts=[MessageSegment],
+        alias=model.__name__,
         validators=[additional] if additional else [],
     )
```

### Comparing `nonebot-plugin-alconna-0.7.0/PKG-INFO` & `nonebot-plugin-alconna-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.7.0
+Version: 0.8.0
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -86,32 +86,35 @@
 assert res.matched
 assert res.query("target").data['user_id'] == '123'
 ```
 
 通用标注:
 
 ```python
-from nonebot.adapters.onebot.v12 import Message as Ob12M, MessageSegment as Ob12MS
-from nonebot.adapters.onebot.v11 import Message as Ob11M, MessageSegment as Ob11MS
+from nonebot.adapters.onebot.v12 import Message as Ob12Msg, MessageSegment as Ob12MS
+from nonebot.adapters.onebot.v11 import Message as Ob11Msg, MessageSegment as Ob11MS
 from nonebot_plugin_alconna.adapters import At
 from arclet.alconna import Alconna, Args
 
-msg1 = Ob12M(["Hello!", Ob12MS.mention("123")])
-print(msg1)  # Hello![mention:user_id=123]
-msg2 = Ob11M(["Hello!", Ob11MS.at(123)])
-print(msg2)  # Hello![CQ:at,qq=123]
+msg1 = Ob12Msg(["Hello!", Ob12MS.mention("123")]) # Hello![mention:user_id=123]
+msg2 = Ob11Msg(["Hello!", Ob11MS.at(123)]) # Hello![CQ:at,qq=123]
+
 
 alc = Alconna("Hello!", Args["target", At])
 res1 = alc.parse(msg1)
 assert res1.matched
-assert res1.query("target").data['user_id'] == '123'
+target = res1.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
 
 res2 = alc.parse(msg2)
 assert res2.matched
-assert res2.query("target").data['qq'] == 123
+target = res2.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
 ```
 
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
```

