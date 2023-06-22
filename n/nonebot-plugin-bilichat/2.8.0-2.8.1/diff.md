# Comparing `tmp/nonebot_plugin_bilichat-2.8.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.8.0.tar", last modified: Thu Jun 22 10:44:27 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.8.1.tar", last modified: Thu Jun 22 14:45:47 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.8.0.tar` & `nonebot_plugin_bilichat-2.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    34523 2023-06-22 10:44:19.092550 nonebot_plugin_bilichat-2.8.0/LICENSE
--rw-r--r--   0        0        0    12397 2023-06-22 10:44:19.092550 nonebot_plugin_bilichat-2.8.0/README.md
--rw-r--r--   0        0        0     9690 2023-06-22 10:44:19.108550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5513 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16205 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7279 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1677 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    27644 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/newbing.png
--rw-r--r--   0        0        0    59199 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     1363 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2200 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     2941 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-22 10:44:27.468604 nonebot_plugin_bilichat-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-22 14:45:34.022725 nonebot_plugin_bilichat-2.8.1/LICENSE
+-rw-r--r--   0        0        0    12397 2023-06-22 14:45:34.022725 nonebot_plugin_bilichat-2.8.1/README.md
+-rw-r--r--   0        0        0     9690 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5472 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      844 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      871 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16355 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     2773 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2017 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     1363 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2200 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     3082 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-22 14:45:47.622857 nonebot_plugin_bilichat-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.8.0/LICENSE` & `nonebot_plugin_bilichat-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/README.md` & `nonebot_plugin_bilichat-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     bilichat_enable_private: bool = True
     bilichat_enable_self: bool = False
     bilichat_only_self: bool = False
     bilichat_enable_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
-    bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
     bilichat_neterror_retry: int = 3
     bilichat_show_error_msg: bool = True
 
     # basic info
     bilichat_basic_info: bool = True
     bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = "bbot_default"
```

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import base64
+import re
 from datetime import datetime
 from io import BytesIO
 from pathlib import Path
 from typing import List, Optional, Union
 
 import qrcode
 from bilireq.exceptions import ResponseCodeError
@@ -358,14 +359,16 @@
 
         return image.getvalue()
 
     async def style_blue(self):
         import jinja2
         from nonebot_plugin_htmlrender.browser import get_new_page
 
+        from ..lib.browser import pw_font_injecter
+
         style_bule = Path(__file__).parent.parent.joinpath("static", "style_blue")
         video_time = (
             f"{self.hours:02d}:{self.minutes:02d}:{self.seconds:02d}"
             if self.hours
             else f"{self.minutes:02d}:{self.seconds:02d}"
         )
         qr = qrcode.QRCode(border=1)
@@ -413,14 +416,15 @@
                 "fav_count": self.favorite,
                 "share_count": self.share,
                 "qr_code_image": f"data:image/png;base64,{base64.b64encode(qr_image.getvalue()).decode()}",
             }
         )
 
         async with get_new_page() as page:
+            await page.route(re.compile("^https://fonts.bbot/(.+)$"), pw_font_injecter)
             await page.goto(template_path)
             await page.set_content(html, wait_until="networkidle")
             await page.wait_for_timeout(5)
             img_raw = await page.locator(".video").screenshot(
                 type="png",
             )
         return img_raw
```

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,38 @@
   <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>视频详情</title>
     <style>
       @font-face {
         font-family: "van";
-        src: url("./assets/vanfont.ttf");
+        src: url("https://fonts.bbot/?name=vanfont.ttf");
+      }
+      @font-face {
+        font-family: "base";
+        src: url("https://fonts.bbot?name=HarmonyOS_Sans_SC_Medium.ttf");
+      }
+      @font-face {
+        font-family: "emoji";
+        src: url("https://fonts.bbot/?name=nte.ttf");
       }
       .cell,
       .up .condition,
       .video-cover .time,
       .video-cover .category {
         border-radius: 8px;
         color: #fff;
         text-align: center;
         vertical-align: middle;
       }
       * {
         margin: 0;
         padding: 0;
         box-sizing: border-box;
-        font-family: "Microsoft YaHei", sans-serif;
+        font-family: "base", "emoji", sans-serif;
       }
       body {
         display: flex;
         flex-direction: column;
         align-items: center;
         background-color: #e9e9e9;
       }
```

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,26 @@
 <html lang="zh-CN">
   <head>
     <meta charset="UTF-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>AI视频总结</title>
     <style>
+      @font-face {
+        font-family: "base";
+        src: url("https://fonts.bbot?name=HarmonyOS_Sans_SC_Medium.ttf");
+      }
+      @font-face {
+        font-family: "emoji";
+        src: url("https://fonts.bbot?name=nte.ttf");
+      }
+      * {
+        box-sizing: border-box;
+        font-family: "base", "emoji", sans-serif;
+      }
       body,
       html {
         height: 100%;
         margin: 0;
         background-color: #fcf4dc; /* 浅黄色背景 */
       }
```

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/newbing.png` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/newbing.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from io import BytesIO
+import re
 from pathlib import Path
 
 from dynamicadaptor.Content import RichTextDetail, Text
 from minidynamicrender.DynConfig import ConfigInit
 from minidynamicrender.DynText import DynTextRender
 from nonebot.log import logger
 
@@ -41,14 +42,15 @@
             image.convert("RGB").save(bio, "jpeg", optimize=True)
             return bio.getvalue()
 
 
 async def pw_text2image(data: str, src: str):
     import jinja2
     from nonebot_plugin_htmlrender import get_new_page
+    from ..lib.browser import pw_font_injecter
 
     src = "openai" if src == plugin_config.bilichat_openai_model else "newbing"
     data = r"\n".join(data.splitlines())
 
     summary = Path(__file__).parent.parent.joinpath("static", "summary")
     template_env = jinja2.Environment(
         loader=jinja2.FileSystemLoader(summary),
@@ -60,14 +62,15 @@
         **{
             "data": data,
             "src": src,
         }
     )
 
     async with get_new_page() as page:
+        await page.route(re.compile("^https://fonts.bbot/(.+)$"), pw_font_injecter)
         await page.set_viewport_size({"width": 800, "height": 2000})
         await page.goto(template_path)
         await page.set_content(html, wait_until="networkidle")
         await page.wait_for_timeout(5)
         img_raw = await page.get_by_alt_text("main").screenshot(
             type="png",
         )
```

### Comparing `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.0/pyproject.toml` & `nonebot_plugin_bilichat-2.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.8.0"
+version = "2.8.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.8.0/PKG-INFO` & `nonebot_plugin_bilichat-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.8.0
+Version: 2.8.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

