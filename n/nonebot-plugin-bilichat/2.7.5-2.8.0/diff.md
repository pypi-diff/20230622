# Comparing `tmp/nonebot_plugin_bilichat-2.7.5.tar.gz` & `tmp/nonebot_plugin_bilichat-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.7.5.tar", last modified: Wed Jun 21 16:07:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.8.0.tar", last modified: Thu Jun 22 10:44:27 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.7.5.tar` & `nonebot_plugin_bilichat-2.8.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0    34523 2023-06-21 16:06:54.416686 nonebot_plugin_bilichat-2.7.5/LICENSE
--rw-r--r--   0        0        0    13120 2023-06-21 16:06:54.416686 nonebot_plugin_bilichat-2.7.5/README.md
--rw-r--r--   0        0        0     9690 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5513 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16205 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7279 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1363 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-21 16:07:04.985378 nonebot_plugin_bilichat-2.7.5/pyproject.toml
--rw-r--r--   0        0        0    14695 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-22 10:44:19.092550 nonebot_plugin_bilichat-2.8.0/LICENSE
+-rw-r--r--   0        0        0    12397 2023-06-22 10:44:19.092550 nonebot_plugin_bilichat-2.8.0/README.md
+-rw-r--r--   0        0        0     9690 2023-06-22 10:44:19.108550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5513 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16205 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-22 10:44:19.112550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7279 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1677 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     1363 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2200 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     2941 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-22 10:44:19.116550 nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-22 10:44:27.468604 nonebot_plugin_bilichat-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.7.5/LICENSE` & `nonebot_plugin_bilichat-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/README.md` & `nonebot_plugin_bilichat-2.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,45 +50,37 @@
 
 ## 📖 介绍
 
 视频链接解析，并根据其内容生成**基本信息**、**词云**和**内容总结**
 
 <details>
 <summary>手机端视图</summary>
+注: 此图片已过时，预期下个版本就会进行更换
 
 ![](docs/mobile.png)
 </details>
 
 <details>
 <summary>基本信息</summary>
 
-![](docs/basic.png)
+![bbot_default](docs/bbot_default.png)
+
+![style_blue](docs/style_blue.png)
 </details>
 
 <details>
 <summary>词云</summary>
 
 ![](docs/wordcloud.png)
 </details>
 
 <details>
 <summary>视频总结</summary>
 
-```markdown
-## 总结
-高通第二代骁龙7+的工程机，拥有台积电4nm工艺，CPU规格和骁龙8+一模一样，GPU规格上是新的Adreno 700架构，性能表现出众，能效曲线稍逊于8+，但中低频段能效水平相同，终端机价格如果能做到1500-2000元，竞争力还是很足的。 
-
-## 要点
-- 💻 第二代骁龙7+拥有台积电4nm工艺和与骁龙8+一样的CPU规格。
-- 🎮 新的Adreno 700架构GPU规格性能强，比上一代7Gen1强了超过一倍。
-- 📈 能效曲线稍逊于8+，但中低频段能效水平相同。
-- 💰 如果终端机价格做到1500-2000元，竞争力还是很足的。
-- 🧪 高通自己也意识到骁龙7系列的竞争力问题，这也使其成了必须要解决的一个问题。
-- 🕹️ 7+ Gen2就是8+的CPU，旗舰规格下放，最大的受益者是大型游戏。
-```
+![](docs/summary.png)
 
 </details>
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
```

#### html2text {}

```diff
@@ -1,30 +1,20 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
-ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![](docs/basic.png)
-è¯äº ![](docs/wordcloud.png)   è§é¢æ»ç» ```markdown ## æ»ç»
-é«éç¬¬äºä»£éªé¾7+çå·¥ç¨æºï¼æ¥æå°ç§¯çµ4nmå·¥èºï¼CPUè§æ ¼åéªé¾8+ä¸æ¨¡ä¸æ ·ï¼GPUè§æ ¼ä¸æ¯æ°çAdreno
-700æ¶æï¼æ§è½è¡¨ç°åºä¼ï¼è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åï¼ç»ç«¯æºä»·æ ¼å¦æè½åå°1500-
-2000åï¼ç«äºåè¿æ¯å¾è¶³çã ## è¦ç¹ - ð»
-ç¬¬äºä»£éªé¾7+æ¥æå°ç§¯çµ4nmå·¥èºåä¸éªé¾8+ä¸æ ·çCPUè§æ ¼ã -
-ð® æ°çAdreno
-700æ¶æGPUè§æ ¼æ§è½å¼ºï¼æ¯ä¸ä¸ä»£7Gen1å¼ºäºè¶è¿ä¸åã - ð
-è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
-å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
-é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
-- ð¹ï¸ 7+
-Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
-```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ææºç«¯è§å¾ æ³¨: æ­¤å¾çå·²è¿æ¶ï¼é¢æä¸ä¸ªçæ¬å°±ä¼è¿è¡æ´æ¢
+![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/bbot_default.png) !
+[style_blue](docs/style_blue.png)   è¯äº ![](docs/wordcloud.png)
+è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨
+nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
+nb plugin install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
 ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
 pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
 poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
 plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
```

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
 from ..model.exception import AbortError, BingChatResponseException
 from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
-from .text_to_image import rich_text2image
+from .text_to_image import t2i
 
 cookies = (
     {}
     if plugin_config.bilichat_newbing_cookie == "no_login"
     else json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 )
 
@@ -133,26 +133,23 @@
             if len(ai_summary) > 50:
                 cache.episodes[cid].newbing = ai_summary
                 cache.save()
                 meaning = True
             # 小于 50 认为无意义
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure")
-                cache.episodes[cid].newbing = f"视频(专栏) {cache.id} 总结失败: {ai_summary}"
+                return f"视频(专栏) {cache.id} 总结失败: {ai_summary}", False
 
         elif cache.episodes[cid].newbing == "Refusal to answer":
             return BING_APOLOGY.read_bytes(), False
         else:
             meaning = True
             logger.info("Using cached newbing summarization")
 
-        if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结", "new Bing"):
-            return img, meaning
-        else:
-            return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].newbing}", meaning
+        return await t2i(cache.episodes[cid].newbing or "视频无法总结", "new Bing"), meaning
     except BingChatResponseException as e:
         logger.error(f"Video(Column) {cache.id} summary failed: {e}")
         cache.episodes[cid].newbing = "Refusal to answer"
         cache.save()
         return BING_APOLOGY.read_bytes(), False
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
```

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from loguru import logger
 
 from ..config import plugin_config
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .openai import get_small_size_transcripts, get_summarise_prompt, openai_req
-from .text_to_image import rich_text2image
+from .text_to_image import t2i
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
     small_size_transcripts = get_small_size_transcripts(title, sub)
     prompt = get_summarise_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
@@ -37,18 +37,15 @@
 
             if ai_summary.response:
                 cache.episodes[cid].openai = ai_summary.response
                 cache.save()
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
                 return f"视频(专栏) {cache.id} 总结失败: 响应内容异常\n{ai_summary.raw}"
-        if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结", plugin_config.bilichat_openai_model):
-            return img
-        else:
-            return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].openai}"
+        return await t2i(cache.episodes[cid].openai or "视频无法总结", plugin_config.bilichat_openai_model)
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
     except Exception as e:
         capture_exception()
         logger.exception(f"Video(Column) {cache.id} summary failed: {e}")
         return f"视频(专栏) {cache.id} 总结失败: {e}"
```

### Comparing `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.5/pyproject.toml` & `nonebot_plugin_bilichat-2.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.7.5"
+version = "2.8.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.7.5/PKG-INFO` & `nonebot_plugin_bilichat-2.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.7.5
+Version: 2.8.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -88,45 +88,37 @@
 
 ## 📖 介绍
 
 视频链接解析，并根据其内容生成**基本信息**、**词云**和**内容总结**
 
 <details>
 <summary>手机端视图</summary>
+注: 此图片已过时，预期下个版本就会进行更换
 
 ![](docs/mobile.png)
 </details>
 
 <details>
 <summary>基本信息</summary>
 
-![](docs/basic.png)
+![bbot_default](docs/bbot_default.png)
+
+![style_blue](docs/style_blue.png)
 </details>
 
 <details>
 <summary>词云</summary>
 
 ![](docs/wordcloud.png)
 </details>
 
 <details>
 <summary>视频总结</summary>
 
-```markdown
-## 总结
-高通第二代骁龙7+的工程机，拥有台积电4nm工艺，CPU规格和骁龙8+一模一样，GPU规格上是新的Adreno 700架构，性能表现出众，能效曲线稍逊于8+，但中低频段能效水平相同，终端机价格如果能做到1500-2000元，竞争力还是很足的。 
-
-## 要点
-- 💻 第二代骁龙7+拥有台积电4nm工艺和与骁龙8+一样的CPU规格。
-- 🎮 新的Adreno 700架构GPU规格性能强，比上一代7Gen1强了超过一倍。
-- 📈 能效曲线稍逊于8+，但中低频段能效水平相同。
-- 💰 如果终端机价格做到1500-2000元，竞争力还是很足的。
-- 🧪 高通自己也意识到骁龙7系列的竞争力问题，这也使其成了必须要解决的一个问题。
-- 🕹️ 7+ Gen2就是8+的CPU，旗舰规格下放，最大的受益者是大型游戏。
-```
+![](docs/summary.png)
 
 </details>
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
@@ -24,30 +24,20 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
-ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![](docs/basic.png)
-è¯äº ![](docs/wordcloud.png)   è§é¢æ»ç» ```markdown ## æ»ç»
-é«éç¬¬äºä»£éªé¾7+çå·¥ç¨æºï¼æ¥æå°ç§¯çµ4nmå·¥èºï¼CPUè§æ ¼åéªé¾8+ä¸æ¨¡ä¸æ ·ï¼GPUè§æ ¼ä¸æ¯æ°çAdreno
-700æ¶æï¼æ§è½è¡¨ç°åºä¼ï¼è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åï¼ç»ç«¯æºä»·æ ¼å¦æè½åå°1500-
-2000åï¼ç«äºåè¿æ¯å¾è¶³çã ## è¦ç¹ - ð»
-ç¬¬äºä»£éªé¾7+æ¥æå°ç§¯çµ4nmå·¥èºåä¸éªé¾8+ä¸æ ·çCPUè§æ ¼ã -
-ð® æ°çAdreno
-700æ¶æGPUè§æ ¼æ§è½å¼ºï¼æ¯ä¸ä¸ä»£7Gen1å¼ºäºè¶è¿ä¸åã - ð
-è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
-å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
-é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
-- ð¹ï¸ 7+
-Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
-```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ææºç«¯è§å¾ æ³¨: æ­¤å¾çå·²è¿æ¶ï¼é¢æä¸ä¸ªçæ¬å°±ä¼è¿è¡æ´æ¢
+![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/bbot_default.png) !
+[style_blue](docs/style_blue.png)   è¯äº ![](docs/wordcloud.png)
+è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨
+nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
+nb plugin install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
 ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
 pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
 poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
 plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
```

