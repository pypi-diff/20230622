# Comparing `tmp/keqing-1.0.0.tar.gz` & `tmp/keqing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keqing-1.0.0.tar", max compression
+gzip compressed data, was "keqing-1.0.1.tar", max compression
```

## Comparing `keqing-1.0.0.tar` & `keqing-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0     1084 2023-04-18 12:19:28.364059 keqing-1.0.0/LICENSE
--rw-r--r--   0        0        0      929 2023-04-18 14:10:55.488281 keqing-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3881 2023-04-18 12:42:40.554569 keqing-1.0.0/README.md
--rw-r--r--   0        0        0    12631 2023-04-18 14:10:30.699671 keqing-1.0.0/src/keqing/__init__.py
--rw-r--r--   0        0        0       50 2023-04-18 12:28:22.912333 keqing-1.0.0/src/keqing/__main__.py
--rw-r--r--   0        0        0      289 2023-04-18 14:10:54.653347 keqing-1.0.0/src/keqing/basic/global_const.py
--rw-r--r--   0        0        0     3294 2023-04-18 12:31:16.240678 keqing-1.0.0/src/keqing/basic/model.py
--rw-r--r--   0        0        0     1752 2023-04-18 12:28:22.913416 keqing-1.0.0/src/keqing/method/diff.py
--rw-r--r--   0        0        0     2206 2023-04-18 14:10:30.699671 keqing-1.0.0/src/keqing/method/network.py
--rw-r--r--   0        0        0      142 2023-04-18 12:31:16.240678 keqing-1.0.0/src/keqing/method/nominatim.py
--rw-r--r--   0        0        0      181 2023-04-18 12:31:16.240678 keqing-1.0.0/src/keqing/method/overpass_bbox.py
--rw-r--r--   0        0        0      477 2023-04-18 12:31:16.240678 keqing-1.0.0/src/keqing/method/overpass_geocode.py
--rw-r--r--   0        0        0      818 2023-04-18 12:48:19.005528 keqing-1.0.0/src/keqing/method/parse_url.py
--rw-r--r--   0        0        0     2582 2023-04-18 12:49:18.386300 keqing-1.0.0/src/keqing/method/parse_xml.py
--rw-r--r--   0        0        0     1754 2023-04-18 12:28:22.913416 keqing-1.0.0/src/keqing/method/query.py
--rw-r--r--   0        0        0        9 2023-04-18 12:28:22.913416 keqing-1.0.0/src/keqing/method/stream_read.py
--rw-r--r--   0        0        0        0 2023-04-18 12:28:22.913416 keqing-1.0.0/src/keqing/method/stream_write.py
--rw-r--r--   0        0        0      890 2023-04-18 12:28:22.914416 keqing-1.0.0/src/keqing/method/transform.py
--rw-r--r--   0        0        0     1840 2023-04-18 12:28:22.914416 keqing-1.0.0/src/keqing/type/constraint.py
--rw-r--r--   0        0        0      528 2023-04-18 12:28:22.914416 keqing-1.0.0/src/keqing/type/data.py
--rw-r--r--   0        0        0     5980 2023-04-18 12:31:16.241680 keqing-1.0.0/src/keqing/type/element.py
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 keqing-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-18 12:19:28.364059 keqing-1.0.1/LICENSE
+-rw-r--r--   0        0        0      929 2023-06-22 08:42:05.168126 keqing-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 2023-04-18 19:39:07.284572 keqing-1.0.1/README.md
+-rw-r--r--   0        0        0    13779 2023-06-08 00:07:02.498288 keqing-1.0.1/src/keqing/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-18 19:39:07.285573 keqing-1.0.1/src/keqing/__main__.py
+-rw-r--r--   0        0        0       51 2023-05-21 20:05:26.016529 keqing-1.0.1/src/keqing/basic/__init__.py
+-rw-r--r--   0        0        0      303 2023-06-22 08:41:48.058699 keqing-1.0.1/src/keqing/basic/global_const.py
+-rw-r--r--   0        0        0     3294 2023-04-18 19:39:07.286645 keqing-1.0.1/src/keqing/basic/model.py
+-rw-r--r--   0        0        0      228 2023-05-21 20:05:26.016529 keqing-1.0.1/src/keqing/method/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-18 17:09:04.346746 keqing-1.0.1/src/keqing/method/diff.py
+-rw-r--r--   0        0        0     2582 2023-06-22 07:55:06.017120 keqing-1.0.1/src/keqing/method/network.py
+-rw-r--r--   0        0        0      142 2023-04-18 19:39:07.287644 keqing-1.0.1/src/keqing/method/nominatim.py
+-rw-r--r--   0        0        0      864 2023-04-18 19:39:07.287644 keqing-1.0.1/src/keqing/method/parse_url.py
+-rw-r--r--   0        0        0     2550 2023-06-22 07:57:24.345402 keqing-1.0.1/src/keqing/method/parse_xml.py
+-rw-r--r--   0        0        0     2458 2023-06-22 08:39:21.221428 keqing-1.0.1/src/keqing/method/query.py
+-rw-r--r--   0        0        0       11 2023-04-18 19:39:07.288644 keqing-1.0.1/src/keqing/method/stream_read.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:09:04.348746 keqing-1.0.1/src/keqing/method/stream_write.py
+-rw-r--r--   0        0        0     1231 2023-05-21 20:05:26.017975 keqing-1.0.1/src/keqing/method/transform.py
+-rw-r--r--   0        0        0        0 2023-05-21 20:05:26.017975 keqing-1.0.1/src/keqing/plugin/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-21 20:05:26.017975 keqing-1.0.1/src/keqing/plugin/overpass/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-21 20:05:26.017975 keqing-1.0.1/src/keqing/plugin/overpass/overpass_bbox.py
+-rw-r--r--   0        0        0      477 2023-05-21 20:05:26.018982 keqing-1.0.1/src/keqing/plugin/overpass/overpass_geocode.py
+-rw-r--r--   0        0        0       72 2023-05-21 20:05:26.018982 keqing-1.0.1/src/keqing/type/__init__.py
+-rw-r--r--   0        0        0     1842 2023-04-18 19:39:07.288644 keqing-1.0.1/src/keqing/type/constraint.py
+-rw-r--r--   0        0        0      528 2023-04-18 17:09:04.349746 keqing-1.0.1/src/keqing/type/data.py
+-rw-r--r--   0        0        0     5964 2023-06-22 07:47:03.709178 keqing-1.0.1/src/keqing/type/element.py
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 keqing-1.0.1/PKG-INFO
```

### Comparing `keqing-1.0.0/LICENSE` & `keqing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keqing-1.0.0/pyproject.toml` & `keqing-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 224b 6571 696e 6722 0d0a  ame = "Keqing"..
-00000020: 7665 7273 696f 6e20 3d20 2231 2e30 2e30  version = "1.0.0
+00000020: 7665 7273 696f 6e20 3d20 2231 2e30 2e31  version = "1.0.1
 00000030: 220d 0a64 6573 6372 6970 7469 6f6e 203d  "..description =
 00000040: 2022 4120 6e6f 6e2d 6461 7461 6261 7365   "A non-database
 00000050: 2050 7974 686f 6e20 6261 7365 204f 534d   Python base OSM
 00000060: 2064 6174 6120 7061 7273 6572 2c20 7769   data parser, wi
 00000070: 7468 2053 514c 206f 7065 7261 7469 6f6e  th SQL operation
 00000080: 2073 696d 756c 6174 6564 2e22 0d0a 6175   simulated."..au
 00000090: 7468 6f72 7320 3d20 5b22 e5bf abe4 b990  thors = ["......
 000000a0: e79a 84e8 8081 e9bc a0e5 ae9d e5ae 9d20  ............... 
 000000b0: 3c6b 6561 6974 6961 6e78 696e 6d61 696c  <keaitianxinmail
 000000c0: 4071 712e 636f 6d3e 225d 0d0a 6c69 6365  @qq.com>"]..lice
 000000d0: 6e73 6520 3d20 224d 4954 220d 0a72 6561  nse = "MIT"..rea
 000000e0: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
-000000f0: 220d 0a72 6570 6f73 6974 6f72 793d 2268  "..repository="h
-00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000110: 6d2f 4f53 4d43 6869 6e61 2f4b 6571 696e  m/OSMChina/Keqin
-00000120: 6722 0d0a 636c 6173 7369 6669 6572 733d  g"..classifiers=
-00000130: 5b0d 0a20 2020 2020 2020 2022 5072 6f67  [..        "Prog
+000000f0: 220d 0a72 6570 6f73 6974 6f72 7920 3d20  "..repository = 
+00000100: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000110: 636f 6d2f 4f53 4d43 6869 6e61 2f4b 6571  com/OSMChina/Keq
+00000120: 696e 6722 0d0a 636c 6173 7369 6669 6572  ing"..classifier
+00000130: 7320 3d20 5b0d 0a20 2020 2022 5072 6f67  s = [..    "Prog
 00000140: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000150: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
-00000160: 2c0d 0a20 2020 2020 2020 2022 4c69 6365  ,..        "Lice
-00000170: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000180: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000190: 7365 222c 0d0a 2020 2020 2020 2020 224f  se",..        "O
-000001a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001c0: 7422 2c0d 0a20 2020 205d 0d0a 7061 636b  t",..    ]..pack
-000001d0: 6167 6573 203d 205b 7b69 6e63 6c75 6465  ages = [{include
-000001e0: 203d 2022 7372 632f 6b65 7169 6e67 227d   = "src/keqing"}
+00000160: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
+00000170: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000180: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
+00000190: 0d0a 2020 2020 224f 7065 7261 7469 6e67  ..    "Operating
+000001a0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000001b0: 6465 7065 6e64 656e 7422 2c0d 0a5d 0d0a  dependent",..]..
+000001c0: 7061 636b 6167 6573 203d 205b 7b20 696e  packages = [{ in
+000001d0: 636c 7564 6520 3d20 226b 6571 696e 6722  clude = "keqing"
+000001e0: 2c20 6672 6f6d 203d 2022 7372 6322 207d  , from = "src" }
 000001f0: 5d0d 0a0d 0a5b 746f 6f6c 2e70 6f65 7472  ]....[tool.poetr
 00000200: 792e 6465 7065 6e64 656e 6369 6573 5d0d  y.dependencies].
 00000210: 0a70 7974 686f 6e20 3d20 225e 332e 3822  .python = "^3.8"
 00000220: 0d0a 7265 7175 6573 7473 203d 2022 5e32  ..requests = "^2
 00000230: 2e32 382e 3222 0d0a 0d0a 5b74 6f6f 6c2e  .28.2"....[tool.
 00000240: 706f 6574 7279 2e67 726f 7570 2e70 726f  poetry.group.pro
 00000250: 642e 6465 7065 6e64 656e 6369 6573 5d0d  d.dependencies].
```

### Comparing `keqing-1.0.0/README.md` & `keqing-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Keqing
 
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword?ref=badge_shield)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FOSMChina%2FKeqing.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FKeqing?ref=badge_shield)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 ![](https://img.shields.io/badge/stable--version-v0.6.0-green)
-![PyPI](https://img.shields.io/pypi/v/Keqing-Sword)
+![PyPI](https://img.shields.io/pypi/v/Keqing)
 
 A non-database Python base OSM data parser, with SQL operation simulated 
 
 [English](https://github.com/OSMChina/Keqing/#english) [简体中文](https://github.com/OSMChina/Keqing/#简体中文)
 
 ----------
 
@@ -46,28 +46,28 @@
 
 List alternatives that may be close and similar to this item, but have a different purpose
 
 ## Roadmap
 
 ### Prior to version 1.0
 
-1. Improve the Diff work in the initial stage
+1. Can read and write files normally
 
-2. Can read and write files normally
-
-3. Officially renamed to Keqing (namespace reserved)
+2. Officially renamed to Keqing (namespace reserved)
 
 ### After version 1.0
 
 1. Accelerate the construction of multiple input and output streams
 
 2. Introduce coverage test
 
 3. Introduce the select statement, you can customize the query (expected to be released as 2.0)
 
+4. Improve the Diff work in the initial stage
+
 ## Source of project name
 
 ACGN waifu of project leader @Jyunhou :
 
 <a herf="https://zh.wikipedia.org/wiki/%E5%8E%9F%E7%A5%9E%E8%A7%92%E8%89%B2%E5%88%97%E8%A1%A8#%E7%92%83%E6%9C%88%E4%B8%83%E6%98%9F"><img alt="Keqing" src="https://avatars.githubusercontent.com/u/45530478?v=4" width=249px></a>
 
 ----------
@@ -106,22 +106,22 @@
 ## KQS:NOT
 
 列举出可能与本项目相近，相似，但目的并非一致的替代品
 
 ## Roadmap
 
 ### 1.0版本之前
-1. 初期完善Diff工作
-2. 能够正常读写到文件
-3. 正式重命名为Keqing（已预留命名空间）
+1. 能够正常读写到文件
+2. 正式重命名为Keqing（已预留命名空间）
 
 ### 1.0版本之后
 1. 加快建设多种输入输出流
 2. 引入覆盖率测试
 3. 引入select语句，可以自定义查询（预计作为2.0发布）
+4. 初期完善Diff工作
 
 ## 命名来源
 
 项目Leader @Jyunhou 钦点：
 
 <a herf="https://zh.wikipedia.org/wiki/%E5%8E%9F%E7%A5%9E%E8%A7%92%E8%89%B2%E5%88%97%E8%A1%A8#%E7%92%83%E6%9C%88%E4%B8%83%E6%98%9F"><img alt="Keqing" src="https://avatars.githubusercontent.com/u/45530478?v=4" width=249px></a>
```

#### html2text {}

```diff
@@ -1,44 +1,43 @@
 # Keqing [![FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=shield)](https://
-app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-
-Keqing_Sword?ref=badge_shield) [Code_style:_black] ![](https://img.shields.io/
-badge/stable--version-v0.6.0-green) ![PyPI](https://img.shields.io/pypi/v/
-Keqing-Sword) A non-database Python base OSM data parser, with SQL operation
-simulated [English](https://github.com/OSMChina/Keqing/#english) [ç®ä½ä¸­æ]
-(https://github.com/OSMChina/Keqing/#ç®ä½ä¸­æ) ---------- ###### English
-This project is a Python-based manipulation library for `.osm` files ## Use the
-example Demo ### Quick Start ```python import keqing map = keqing.Waifu()
-map.read(mode="file", file_path="map.osm") ``` ### Get `name` ### Generate
-`.osm` file based on input **For more examples, see the [README file](/docs/
-README.md) in `/docs`, which lists the various functions of Keqing in detail**
-## Features ### Pypy friendly This package don't depend on any package, so it's
-compatible with latest pypy. Now it depends on requests package to fetch
-network data. ### Pure in memory Don't need any database environment, just a
-fast and out-of-the-box tool. ## KQS: NOT List alternatives that may be close
-and similar to this item, but have a different purpose ## Roadmap ### Prior to
-version 1.0 1. Improve the Diff work in the initial stage 2. Can read and write
-files normally 3. Officially renamed to Keqing (namespace reserved) ### After
+git%2Bgithub.com%2FOSMChina%2FKeqing.svg?type=shield)](https://app.fossa.com/
+projects/git%2Bgithub.com%2FOSMChina%2FKeqing?ref=badge_shield) [Code_style:
+black] ![](https://img.shields.io/badge/stable--version-v0.6.0-green) ![PyPI]
+(https://img.shields.io/pypi/v/Keqing) A non-database Python base OSM data
+parser, with SQL operation simulated [English](https://github.com/OSMChina/
+Keqing/#english) [ç®ä½ä¸­æ](https://github.com/OSMChina/Keqing/
+#ç®ä½ä¸­æ) ---------- ###### English This project is a Python-based
+manipulation library for `.osm` files ## Use the example Demo ### Quick Start
+```python import keqing map = keqing.Waifu() map.read(mode="file",
+file_path="map.osm") ``` ### Get `name` ### Generate `.osm` file based on input
+**For more examples, see the [README file](/docs/README.md) in `/docs`, which
+lists the various functions of Keqing in detail** ## Features ### Pypy friendly
+This package don't depend on any package, so it's compatible with latest pypy.
+Now it depends on requests package to fetch network data. ### Pure in memory
+Don't need any database environment, just a fast and out-of-the-box tool. ##
+KQS: NOT List alternatives that may be close and similar to this item, but have
+a different purpose ## Roadmap ### Prior to version 1.0 1. Can read and write
+files normally 2. Officially renamed to Keqing (namespace reserved) ### After
 version 1.0 1. Accelerate the construction of multiple input and output streams
 2. Introduce coverage test 3. Introduce the select statement, you can customize
-the query (expected to be released as 2.0) ## Source of project name ACGN waifu
-of project leader @Jyunhou : [Keqing] ---------- ###### ç®ä½ä¸­æ
+the query (expected to be released as 2.0) 4. Improve the Diff work in the
+initial stage ## Source of project name ACGN waifu of project leader @Jyunhou :
+[Keqing] ---------- ###### ç®ä½ä¸­æ
 æ¬é¡¹ç®æ¯ä¸ä¸ªåºäºPythonçå¯¹`.osm`æä»¶çè®¿é®åº ## ä½¿ç¨ç¤ºä¾
 Demo ### å¿«éå¼å§ ```python import keqing map = keqing.Waifu() map.read
 (mode="file", file_path="map.osm") ``` ### è·å`name` ###
 åºäºè¾å¥çæ`.osm`æä»¶ **æ´å¤ç¤ºä¾å¯è§`/docs`ä¸­[READMEæä»¶](/
 docs/README.md)ï¼è¯¦ç»ååºäºKeqingçåç§åè½** ## ç¹æ§ ### Pypy
 åå¥½ è¿ä¸ªåä¸ä¾èµä»»ä½åï¼æä»¥å®å¼å®¹ææ°çpypyã
 ç°å¨å®ä¾èµäºrequestsåæ¥è·åç½ç»æ°æ®ã ### çº¯åå­å
 ä¸éè¦ä»»ä½æ°æ®åºç¯å¢ï¼åªæ¯ä¸ä¸ªå¿«éä¸å¼ç®±å³ç¨çå·¥å·ã
 ## KQS:NOT
 åä¸¾åºå¯è½ä¸æ¬é¡¹ç®ç¸è¿ï¼ç¸ä¼¼ï¼ä½ç®çå¹¶éä¸è´çæ¿ä»£å
-## Roadmap ### 1.0çæ¬ä¹å 1. åæå®åDiffå·¥ä½ 2.
-è½å¤æ­£å¸¸è¯»åå°æä»¶ 3.
+## Roadmap ### 1.0çæ¬ä¹å 1. è½å¤æ­£å¸¸è¯»åå°æä»¶ 2.
 æ­£å¼éå½åä¸ºKeqingï¼å·²é¢çå½åç©ºé´ï¼ ### 1.0çæ¬ä¹å 1.
 å å¿«å»ºè®¾å¤ç§è¾å¥è¾åºæµ 2. å¼å¥è¦ççæµè¯ 3.
-å¼å¥selectè¯­å¥ï¼å¯ä»¥èªå®ä¹æ¥è¯¢ï¼é¢è®¡ä½ä¸º2.0åå¸ï¼ ##
-å½åæ¥æº é¡¹ç®Leader @Jyunhou é¦ç¹ï¼ [Keqing] ---------- ## License [!
-[FOSSA Status](https://app.fossa.com/api/projects/
+å¼å¥selectè¯­å¥ï¼å¯ä»¥èªå®ä¹æ¥è¯¢ï¼é¢è®¡ä½ä¸º2.0åå¸ï¼ 4.
+åæå®åDiffå·¥ä½ ## å½åæ¥æº é¡¹ç®Leader @Jyunhou é¦ç¹ï¼ [Keqing]
+---------- ## License [![FOSSA Status](https://app.fossa.com/api/projects/
 git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=large)](https://
 app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-
 Keqing_Sword?ref=badge_large)
```

### Comparing `keqing-1.0.0/src/keqing/__init__.py` & `keqing-1.0.1/src/keqing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import time
 from typing import Dict, List
 from xml.dom import minidom
 from xml.etree import ElementTree as ET
 from xml.etree.ElementTree import Element, ElementTree
 
-from keqing.basic.global_const import KEQING_CORE_NAME, KEQING_START_ID, KEQING_VERSION
-from keqing.method.network import get_server, get_headers
-from keqing.method.parse import parse_node, parse_way, parse_relation, pre_parse_classify
-from keqing.method.transform import prefix_abbreviation
-from keqing.basic.model import BaseOsmModel
-from keqing.type.constraint import Bounds, Member
-from keqing.type.element import Node, Relation, Way
+from .basic.global_const import (
+    KEQING_CORE_NAME,
+    KEQING_START_ID,
+    KEQING_VERSION,
+)
+from .basic.model import BaseOsmModel
+from .method.network import get_headers, get_server
+from .method.parse_xml import (
+    parse_node,
+    parse_relation,
+    parse_way,
+    pre_parse_classify,
+)
+from .method.transform import prefix_normalization
+from .type.constraint import Bounds, Member
+from .type.element import Node, Relation, Way
 
 
 class Waifu:
     def __init__(self):
         self.node_dict: Dict[int, Node] = {}
         self.bounds_list: List[Bounds] = []
         self.version: str = "0.6"
@@ -53,15 +62,23 @@
                     + str(len(self.bounds_list))
                     + "\n"
                 )
                 + "=============================="
             )
         )
 
-    def read(self, mode=None, file_path="", text="", url="", fpath="", data_driver=""):
+    def read(
+        self,
+        mode=None,
+        file_path="",
+        text="",
+        url="",
+        fpath="",
+        data_driver="",
+    ):
         def pre_read_warn(mode: str, file_path: str, text: str, url: str):
             if url != "" and (mode != "network" and mode != "n"):
                 if ("http://" in url) or ("https://" in url):
                     print(
                         "WARN:You may intent to request from network, but you enter another mode."
                     )
             if mode == "text" or mode == "t":
@@ -99,21 +116,48 @@
             raise TypeError(f"Unexpected read mode: {mode}")
 
         time_end = time.time()
         print("[TIME]: " + str(round((time_end - time_start), 3)) + "s" + "\n")
         self.meow()
 
     def read_file(self, file_path: str):
-        tree: ElementTree = ET.parse(file_path)
-        root: Element = tree.getroot()
-        pre_parse_classify(self.node_dict, self.way_dict, self.relation_dict, self.bounds_list, root)
+        try:
+            tree: ElementTree = ET.parse(file_path)
+            root: Element = tree.getroot()
+            pre_parse_classify(
+                self.node_dict,
+                self.way_dict,
+                self.relation_dict,
+                self.bounds_list,
+                root,
+            )
+        except FileNotFoundError:
+            print("Error: 文件不存在，请检查文件路径")
+        except PermissionError:
+            print("Error: 无权访问文件，请检查文件权限")
+        except ET.ParseError:
+            print("Error: XML 解析失败，请检查文件内容是否为有效的 XML 格式")
+        except Exception as e:
+            print(f"Error: 发生未知错误 - {str(e)}")
+
 
     def read_memory(self, text: str):
-        root: Element = ET.fromstring(text)
-        pre_parse_classify(self.node_dict, self.way_dict, self.relation_dict, self.bounds_list, root)
+        try:
+            root: Element = ET.fromstring(text)
+            pre_parse_classify(
+                self.node_dict,
+                self.way_dict,
+                self.relation_dict,
+                self.bounds_list,
+                root,
+            )
+        except ET.ParseError:
+            print("Error: XML 解析失败，请检查文本内容是否为有效的 XML 格式")
+        except Exception as e:
+            print(f"Error: 发生未知错误 - {str(e)}")
 
     def read_network(self, mode="api", server="OSM", quantity="", **kwargs):
         # version problem haven't been introduced
         if quantity != "":
             if quantity == "area":
                 # parse SWNE
                 self.read_network_area()
@@ -149,32 +193,38 @@
     ):
         def have_multi_elements(element_id) -> bool:
             if "," in element_id:
                 # have comma or space between multi element
                 return True
 
         if have_multi_elements(element_id):
+            # if flag_allow_batch_download
             self.read_network_element_batch(element_id)
         else:
             if (
-                (type == "node" or type == "n")
-                or (type == "way" or type == "w")
-                or (type == "relation" or type == "r")
+                prefix_normalization(type) == "node"
+                or prefix_normalization(type) == "way"
+                or prefix_normalization(type) == "relation"
             ):
                 import requests
 
                 pure_id = (
                     element_id.replace("n", "")
                     .replace("w", "")
                     .replace("r", "")
                 )
                 if "v" in pure_id:
                     version = pure_id.split("v")[1]
                     pure_id = pure_id.split("v")[0]
-                url = get_server(server) + prefix_abbreviation(type,mode="p2prefix") + "/" + pure_id
+                url = (
+                    get_server(server)
+                    + prefix_normalization(type, mode="p2prefix")
+                    + "/"
+                    + pure_id
+                )
                 headers = get_headers()
                 print("url:", url)
                 print("headers:", headers)
                 response = requests.get(url=url, headers=headers).text
                 print(response)
                 self.read_memory(response)
             else:
@@ -185,17 +235,15 @@
     def read_network_element_batch(
         self, element_id=None, mode="api", server="OSM"
     ):
         # it can be string or list
         # https://wiki.openstreetmap.org/wiki/API_v0.6#Multi_fetch:_GET_/api/0.6/[nodes|ways|relations]?#parameters
         pass
 
-
     def write(self, mode=None, file_path="", data_driver=""):
-
         def is_limit_valid(ignore=False):
             # conduct limit check
             # for ele in nwr
             # if ele.is_limit_valid=True
             return True
 
         if mode == "file":
```

### Comparing `keqing-1.0.0/src/keqing/basic/model.py` & `keqing-1.0.1/src/keqing/basic/model.py`

 * *Files identical despite different names*

### Comparing `keqing-1.0.0/src/keqing/method/diff.py` & `keqing-1.0.1/src/keqing/method/diff.py`

 * *Files identical despite different names*

### Comparing `keqing-1.0.0/src/keqing/method/parse_xml.py` & `keqing-1.0.1/src/keqing/method/parse_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List
 from xml.etree.ElementTree import Element
 
+from ..type.constraint import Bounds, Member
+from ..type.element import Node, Relation, Way
 
-from keqing.type.constraint import Member, Bounds
-from keqing.type.element import Node, Way, Relation
 
 def parse(element: Element):
     # judge whether is N/W/R then invoke function.
     pass
 
 
 def pre_parse_classify(node_dict, way_dict, relation_dict, bounds_list, root):
@@ -21,15 +21,14 @@
         elif element.tag == "bounds":
             bounds_list.append(Bounds(element.attrib))
         else:
             # raise TypeError('Unexpected element tag type: ' + element.tag)
             pass
 
 
-
 def parse_node(node_dict, element: Element):
     attrib: Dict[str, str] = element.attrib
     tag_dict: Dict[str, str] = {}
     for sub_element in element:
         tag_dict[sub_element.attrib["k"]] = sub_element.attrib["v"]
     node_dict[int(attrib["id"])] = Node(attrib, tag_dict)
 
@@ -67,12 +66,8 @@
             )
         elif sub_element.tag == "tag":
             tag_dict[sub_element.attrib["k"]] = sub_element.attrib["v"]
         else:
             raise TypeError(
                 f"Unexpected element tag type: {sub_element.tag} in Relation"
             )
-    relation_dict[int(attrib["id"])] = Relation(
-        attrib, tag_dict, member_list
-    )
-
-
+    relation_dict[int(attrib["id"])] = Relation(attrib, tag_dict, member_list)
```

### Comparing `keqing-1.0.0/src/keqing/method/query.py` & `keqing-1.0.1/src/keqing/method/query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,54 @@
-from keqing.keqing import Waifu
-
-
-def remove_comment(query_content:str)->str:
-    # line comment
+def remove_comment(query_content: str) -> str:
+    # priority: block comment > line comment
     # block comment
+    # suggestion: regex
+    # line comment
+    query_content = query_content.split("\n")
+    query_content_judge = [line.replace(" ", "") for line in query_content]
+    query_content_none_comment = []
+    for i in range(len(query_content_judge)):
+        if i[:2] != "//":
+            query_content_none_comment.append(line)
+    query_content = "".join(query_content)
+    # warning: if a line not begin with comment, it't comment won't be removed, I still waiting for a good method.
     pass
     return query_content
 
-def query_in_type(type:list, query_content:str)-> Waifu:
-    return Waifu()
+
+# def query_in_type(type: list, query_content: str) -> Waifu:
+#     return Waifu()
+# 不能直接返回Waifu，因为并不打算撤销这套__init__里放单独一个waifu的结构。这里只能返回其他内容（如xml/json）再在waifu里面parse它
+
 
 def overpass_query(query_content: str) -> None:
     print("NOTE: currently only support basic ql")
     lines = (
-        remove_comment(query_content).replace("\n", "")
+        remove_comment(query_content)
+        .replace("\n", "")
         .replace("(", "")
         .replace(")", "")
         .split(";")
     )
     types = ["node", "way", "relation"] + ["nw", "nr", "wr", "nwr"]
     operations = set()
     for line in lines:
         for type in types:
             if type in line:
-                operations=operations.union(set([line]))
+                operations = operations.union(set([line]))
     print(operations)
-    for operation in operations:
-        # type:list=operation.jianceleixing
-        # actions:list=operation.fenliqitayaosu
-        # temp:Waifu=Waifu()
-        # for i in actions:
-        #     # i就是[k=v]
-        #     temp=query_in_type(type,query_content)
-        # 最后剩下的就是逐层查询完了以后的，可以是空
-        pass # 分离出逐次查询
+    # for operation in operations:
+    #     # type:list=operation.jianceleixing
+    #     # actions:list=operation.fenliqitayaosu
+    #     # temp:Waifu=Waifu()
+    #     # for i in actions:
+    #     #     # i就是[k=v]
+    #     #     temp=query_in_type(type,query_content)
+    #     # 最后剩下的就是逐层查询完了以后的，可以是空
+    #     pass # 分离出逐次查询
 
 
 def ganyu_query(query_content: str) -> None:
     pass
 
 
 def query(query_content: str, query_language: str) -> None:
@@ -51,11 +62,11 @@
     ]
     name_list_ganyu = ["Ganyu", "Yeyang"]
     if query_language in name_list_overpass:
         overpass_query(query_content)
     if query_language in name_list_ganyu:
         ganyu_query(query_content)
 
-query(
-    open("../../../tests/overpassql/telecommunication.overpassql"),
-    "Overpass"
-)
+
+# query(
+#     open("../../../tests/overpassql/telecommunication.overpassql"), "Overpass"
+# )
```

### Comparing `keqing-1.0.0/src/keqing/type/constraint.py` & `keqing-1.0.1/src/keqing/type/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         self.min_lon: float = float(attrib["minlon"])
         self.max_lat: float = float(attrib["maxlat"])
         self.max_lon: float = float(attrib["maxlon"])
         self.origin: str = attrib.get("origin", "")
 
     def align_serialization(self) -> str:
         serialize_format = "SB_WB_NB_EB"
+
         # another choise is don't use B in output_format, and use A/B insteal of P/N for plus or minus sign
         def num_serialization(degree: float):
             if degree >= 0:
                 return "P" + str(degree).replace(".", "D")
             else:
                 return str(degree).replace("-", "N").replace(".", "D")
```

### Comparing `keqing-1.0.0/src/keqing/type/data.py` & `keqing-1.0.1/src/keqing/type/data.py`

 * *Files identical despite different names*

### Comparing `keqing-1.0.0/src/keqing/type/element.py` & `keqing-1.0.1/src/keqing/type/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Dict, List
 
-from keqing.basic.model import BaseOsmModel
+
+
 from .constraint import Member
+from .. import BaseOsmModel
+
 
 # TODO
 # limit check should be conduct while modify
 
 
 class Node(BaseOsmModel):
     upstream_way: list = [0]
@@ -107,15 +110,15 @@
         pass
 
     def get_upstream_relation(self, order=-1):
         if order == -1:
             return self.upstream_relation
         else:
             return self.upstream_relation[order]
-        
+
     def is_limit_valid(self):
         # if len<API_LIMIT_MAX_ELEMENT_TAGS:
         # if len>0 and len<API_LIMIT_MAX_WAY_NODES:
         return True
 
 
 class Relation(BaseOsmModel):
@@ -159,8 +162,8 @@
         if order == -1:
             return self.upstream_relation
         else:
             return self.upstream_relation[order]
 
     def is_limit_valid(self):
         # if len<API_LIMIT_MAX_RELATION_MEMBERS
-        return True
+        return True
```

### Comparing `keqing-1.0.0/PKG-INFO` & `keqing-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keqing
-Version: 1.0.0
+Version: 1.0.1
 Summary: A non-database Python base OSM data parser, with SQL operation simulated.
 Home-page: https://github.com/OSMChina/Keqing
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: keaitianxinmail@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/OSMChina/Keqing
 Description-Content-Type: text/markdown
 
 # Keqing
 
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword?ref=badge_shield)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FOSMChina%2FKeqing.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FKeqing?ref=badge_shield)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 ![](https://img.shields.io/badge/stable--version-v0.6.0-green)
-![PyPI](https://img.shields.io/pypi/v/Keqing-Sword)
+![PyPI](https://img.shields.io/pypi/v/Keqing)
 
 A non-database Python base OSM data parser, with SQL operation simulated 
 
 [English](https://github.com/OSMChina/Keqing/#english) [简体中文](https://github.com/OSMChina/Keqing/#简体中文)
 
 ----------
 
@@ -67,28 +67,28 @@
 
 List alternatives that may be close and similar to this item, but have a different purpose
 
 ## Roadmap
 
 ### Prior to version 1.0
 
-1. Improve the Diff work in the initial stage
+1. Can read and write files normally
 
-2. Can read and write files normally
-
-3. Officially renamed to Keqing (namespace reserved)
+2. Officially renamed to Keqing (namespace reserved)
 
 ### After version 1.0
 
 1. Accelerate the construction of multiple input and output streams
 
 2. Introduce coverage test
 
 3. Introduce the select statement, you can customize the query (expected to be released as 2.0)
 
+4. Improve the Diff work in the initial stage
+
 ## Source of project name
 
 ACGN waifu of project leader @Jyunhou :
 
 <a herf="https://zh.wikipedia.org/wiki/%E5%8E%9F%E7%A5%9E%E8%A7%92%E8%89%B2%E5%88%97%E8%A1%A8#%E7%92%83%E6%9C%88%E4%B8%83%E6%98%9F"><img alt="Keqing" src="https://avatars.githubusercontent.com/u/45530478?v=4" width=249px></a>
 
 ----------
@@ -127,22 +127,22 @@
 ## KQS:NOT
 
 列举出可能与本项目相近，相似，但目的并非一致的替代品
 
 ## Roadmap
 
 ### 1.0版本之前
-1. 初期完善Diff工作
-2. 能够正常读写到文件
-3. 正式重命名为Keqing（已预留命名空间）
+1. 能够正常读写到文件
+2. 正式重命名为Keqing（已预留命名空间）
 
 ### 1.0版本之后
 1. 加快建设多种输入输出流
 2. 引入覆盖率测试
 3. 引入select语句，可以自定义查询（预计作为2.0发布）
+4. 初期完善Diff工作
 
 ## 命名来源
 
 项目Leader @Jyunhou 钦点：
 
 <a herf="https://zh.wikipedia.org/wiki/%E5%8E%9F%E7%A5%9E%E8%A7%92%E8%89%B2%E5%88%97%E8%A1%A8#%E7%92%83%E6%9C%88%E4%B8%83%E6%98%9F"><img alt="Keqing" src="https://avatars.githubusercontent.com/u/45530478?v=4" width=249px></a>
```

#### html2text {}

```diff
@@ -1,55 +1,54 @@
-Metadata-Version: 2.1 Name: keqing Version: 1.0.0 Summary: A non-database
+Metadata-Version: 2.1 Name: keqing Version: 1.0.1 Summary: A non-database
 Python base OSM data parser, with SQL operation simulated. Home-page: https://
 github.com/OSMChina/Keqing License: MIT Author: å¿«ä¹çèé¼ å®å® Author-
 email: keaitianxinmail@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
 Requires-Dist: requests (>=2.28.2,<3.0.0) Project-URL: Repository, https://
 github.com/OSMChina/Keqing Description-Content-Type: text/markdown # Keqing [!
 [FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=shield)](https://
-app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-
-Keqing_Sword?ref=badge_shield) [Code_style:_black] ![](https://img.shields.io/
-badge/stable--version-v0.6.0-green) ![PyPI](https://img.shields.io/pypi/v/
-Keqing-Sword) A non-database Python base OSM data parser, with SQL operation
-simulated [English](https://github.com/OSMChina/Keqing/#english) [ç®ä½ä¸­æ]
-(https://github.com/OSMChina/Keqing/#ç®ä½ä¸­æ) ---------- ###### English
-This project is a Python-based manipulation library for `.osm` files ## Use the
-example Demo ### Quick Start ```python import keqing map = keqing.Waifu()
-map.read(mode="file", file_path="map.osm") ``` ### Get `name` ### Generate
-`.osm` file based on input **For more examples, see the [README file](/docs/
-README.md) in `/docs`, which lists the various functions of Keqing in detail**
-## Features ### Pypy friendly This package don't depend on any package, so it's
-compatible with latest pypy. Now it depends on requests package to fetch
-network data. ### Pure in memory Don't need any database environment, just a
-fast and out-of-the-box tool. ## KQS: NOT List alternatives that may be close
-and similar to this item, but have a different purpose ## Roadmap ### Prior to
-version 1.0 1. Improve the Diff work in the initial stage 2. Can read and write
-files normally 3. Officially renamed to Keqing (namespace reserved) ### After
+git%2Bgithub.com%2FOSMChina%2FKeqing.svg?type=shield)](https://app.fossa.com/
+projects/git%2Bgithub.com%2FOSMChina%2FKeqing?ref=badge_shield) [Code_style:
+black] ![](https://img.shields.io/badge/stable--version-v0.6.0-green) ![PyPI]
+(https://img.shields.io/pypi/v/Keqing) A non-database Python base OSM data
+parser, with SQL operation simulated [English](https://github.com/OSMChina/
+Keqing/#english) [ç®ä½ä¸­æ](https://github.com/OSMChina/Keqing/
+#ç®ä½ä¸­æ) ---------- ###### English This project is a Python-based
+manipulation library for `.osm` files ## Use the example Demo ### Quick Start
+```python import keqing map = keqing.Waifu() map.read(mode="file",
+file_path="map.osm") ``` ### Get `name` ### Generate `.osm` file based on input
+**For more examples, see the [README file](/docs/README.md) in `/docs`, which
+lists the various functions of Keqing in detail** ## Features ### Pypy friendly
+This package don't depend on any package, so it's compatible with latest pypy.
+Now it depends on requests package to fetch network data. ### Pure in memory
+Don't need any database environment, just a fast and out-of-the-box tool. ##
+KQS: NOT List alternatives that may be close and similar to this item, but have
+a different purpose ## Roadmap ### Prior to version 1.0 1. Can read and write
+files normally 2. Officially renamed to Keqing (namespace reserved) ### After
 version 1.0 1. Accelerate the construction of multiple input and output streams
 2. Introduce coverage test 3. Introduce the select statement, you can customize
-the query (expected to be released as 2.0) ## Source of project name ACGN waifu
-of project leader @Jyunhou : [Keqing] ---------- ###### ç®ä½ä¸­æ
+the query (expected to be released as 2.0) 4. Improve the Diff work in the
+initial stage ## Source of project name ACGN waifu of project leader @Jyunhou :
+[Keqing] ---------- ###### ç®ä½ä¸­æ
 æ¬é¡¹ç®æ¯ä¸ä¸ªåºäºPythonçå¯¹`.osm`æä»¶çè®¿é®åº ## ä½¿ç¨ç¤ºä¾
 Demo ### å¿«éå¼å§ ```python import keqing map = keqing.Waifu() map.read
 (mode="file", file_path="map.osm") ``` ### è·å`name` ###
 åºäºè¾å¥çæ`.osm`æä»¶ **æ´å¤ç¤ºä¾å¯è§`/docs`ä¸­[READMEæä»¶](/
 docs/README.md)ï¼è¯¦ç»ååºäºKeqingçåç§åè½** ## ç¹æ§ ### Pypy
 åå¥½ è¿ä¸ªåä¸ä¾èµä»»ä½åï¼æä»¥å®å¼å®¹ææ°çpypyã
 ç°å¨å®ä¾èµäºrequestsåæ¥è·åç½ç»æ°æ®ã ### çº¯åå­å
 ä¸éè¦ä»»ä½æ°æ®åºç¯å¢ï¼åªæ¯ä¸ä¸ªå¿«éä¸å¼ç®±å³ç¨çå·¥å·ã
 ## KQS:NOT
 åä¸¾åºå¯è½ä¸æ¬é¡¹ç®ç¸è¿ï¼ç¸ä¼¼ï¼ä½ç®çå¹¶éä¸è´çæ¿ä»£å
-## Roadmap ### 1.0çæ¬ä¹å 1. åæå®åDiffå·¥ä½ 2.
-è½å¤æ­£å¸¸è¯»åå°æä»¶ 3.
+## Roadmap ### 1.0çæ¬ä¹å 1. è½å¤æ­£å¸¸è¯»åå°æä»¶ 2.
 æ­£å¼éå½åä¸ºKeqingï¼å·²é¢çå½åç©ºé´ï¼ ### 1.0çæ¬ä¹å 1.
 å å¿«å»ºè®¾å¤ç§è¾å¥è¾åºæµ 2. å¼å¥è¦ççæµè¯ 3.
-å¼å¥selectè¯­å¥ï¼å¯ä»¥èªå®ä¹æ¥è¯¢ï¼é¢è®¡ä½ä¸º2.0åå¸ï¼ ##
-å½åæ¥æº é¡¹ç®Leader @Jyunhou é¦ç¹ï¼ [Keqing] ---------- ## License [!
-[FOSSA Status](https://app.fossa.com/api/projects/
+å¼å¥selectè¯­å¥ï¼å¯ä»¥èªå®ä¹æ¥è¯¢ï¼é¢è®¡ä½ä¸º2.0åå¸ï¼ 4.
+åæå®åDiffå·¥ä½ ## å½åæ¥æº é¡¹ç®Leader @Jyunhou é¦ç¹ï¼ [Keqing]
+---------- ## License [![FOSSA Status](https://app.fossa.com/api/projects/
 git%2Bgithub.com%2FOSMChina%2FOSMChina-Keqing_Sword.svg?type=large)](https://
 app.fossa.com/projects/git%2Bgithub.com%2FOSMChina%2FOSMChina-
 Keqing_Sword?ref=badge_large)
```

