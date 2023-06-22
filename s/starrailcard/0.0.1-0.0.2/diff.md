# Comparing `tmp/starrailcard-0.0.1.tar.gz` & `tmp/starrailcard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-0.0.1.tar", max compression
+gzip compressed data, was "starrailcard-0.0.2.tar", max compression
```

## Comparing `starrailcard-0.0.1.tar` & `starrailcard-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,44 @@
--rw-r--r--   0        0        0      506 2023-06-22 11:20:54.919557 starrailcard-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1353 2023-06-22 11:22:09.031551 starrailcard-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-17 13:06:01.306235 starrailcard-0.0.1/starrailcard/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-22 11:11:26.279283 starrailcard-0.0.1/starrailcard/honkaicard.py
--rw-r--r--   0        0        0        0 2023-06-17 13:05:17.443970 starrailcard-0.0.1/starrailcard/src/__init__.py
--rw-r--r--   0        0        0      146 2023-06-17 13:06:12.296482 starrailcard-0.0.1/starrailcard/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5623 2023-06-14 18:06:59.215231 starrailcard-0.0.1/starrailcard/src/assets/ARTIFACT.png
--rw-r--r--   0        0        0    83412 2023-06-14 17:57:00.250514 starrailcard-0.0.1/starrailcard/src/assets/bg/bg.png
--rw-r--r--   0        0        0   158031 2023-06-17 14:05:49.423459 starrailcard-0.0.1/starrailcard/src/assets/bg/bg_charters.png
--rw-r--r--   0        0        0     6705 2023-06-14 17:57:52.444545 starrailcard-0.0.1/starrailcard/src/assets/bg/frame_charters.png
--rw-r--r--   0        0        0     5628 2023-06-17 15:44:07.301010 starrailcard-0.0.1/starrailcard/src/assets/bg/maska.png
--rw-r--r--   0        0        0     7216 2023-05-24 10:00:18.675835 starrailcard-0.0.1/starrailcard/src/assets/const/Closed.png
--rw-r--r--   0        0        0     8219 2023-05-24 10:00:45.643719 starrailcard-0.0.1/starrailcard/src/assets/const/Lock.png
--rw-r--r--   0        0        0    23211 2023-05-23 20:21:03.593475 starrailcard-0.0.1/starrailcard/src/assets/const/open.png
--rw-r--r--   0        0        0  4909668 2022-09-27 23:11:24.000000 starrailcard-0.0.1/starrailcard/src/assets/font/NotoSansKR-Bold.otf
--rw-r--r--   0        0        0     8848 2023-06-14 18:09:06.500975 starrailcard-0.0.1/starrailcard/src/assets/lc/bg.png
--rw-r--r--   0        0        0     6756 2023-06-14 18:09:18.448917 starrailcard-0.0.1/starrailcard/src/assets/lc/bg_lc.png
--rw-r--r--   0        0        0     5014 2023-06-17 15:41:55.506646 starrailcard-0.0.1/starrailcard/src/assets/lc/maska.png
--rw-r--r--   0        0        0    10376 2023-06-14 18:04:44.670067 starrailcard-0.0.1/starrailcard/src/assets/LOGO.png
--rw-r--r--   0        0        0     5250 2023-06-14 18:07:34.766685 starrailcard-0.0.1/starrailcard/src/assets/Sets/bg.png
--rw-r--r--   0        0        0     4795 2023-06-14 18:07:50.587159 starrailcard-0.0.1/starrailcard/src/assets/Sets/count.png
--rw-r--r--   0        0        0     4939 2023-05-23 20:18:52.221269 starrailcard-0.0.1/starrailcard/src/assets/stars/strs_1.png
--rw-r--r--   0        0        0     5285 2023-05-23 20:18:40.906875 starrailcard-0.0.1/starrailcard/src/assets/stars/strs_2.png
--rw-r--r--   0        0        0     5270 2023-05-23 20:18:31.351225 starrailcard-0.0.1/starrailcard/src/assets/stars/strs_3.png
--rw-r--r--   0        0        0     5276 2023-05-23 20:18:20.816749 starrailcard-0.0.1/starrailcard/src/assets/stars/strs_4.png
--rw-r--r--   0        0        0     5247 2023-05-23 20:18:00.663473 starrailcard-0.0.1/starrailcard/src/assets/stars/strs_5.png
--rw-r--r--   0        0        0     5977 2023-06-14 18:06:19.159817 starrailcard-0.0.1/starrailcard/src/assets/STATS.png
--rw-r--r--   0        0        0     5536 2023-06-14 18:00:51.102004 starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg.png
--rw-r--r--   0        0        0     5767 2023-06-14 18:04:23.681149 starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg_dop.png
--rw-r--r--   0        0        0     5621 2023-06-14 18:02:14.042865 starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg_main.png
--rw-r--r--   0        0        0     3741 2023-06-14 18:01:09.230188 starrailcard-0.0.1/starrailcard/src/assets/Tallants/count.png
--rw-r--r--   0        0        0     4256 2023-06-14 18:04:05.609136 starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_0.png
--rw-r--r--   0        0        0     4834 2023-06-14 18:03:52.230355 starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_1.png
--rw-r--r--   0        0        0     4907 2023-06-14 18:03:41.048412 starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_2.png
--rw-r--r--   0        0        0     4876 2023-06-14 18:03:27.694098 starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_3.png
--rw-r--r--   0        0        0     6131 2023-06-14 18:05:43.805818 starrailcard-0.0.1/starrailcard/src/assets/UID.png
--rw-r--r--   0        0        0    13032 2023-06-22 10:13:42.022319 starrailcard-0.0.1/starrailcard/src/generators/__pycache__/one.cpython-310.pyc
--rw-r--r--   0        0        0    16523 2023-06-22 10:13:09.430221 starrailcard-0.0.1/starrailcard/src/generators/one.py
--rw-r--r--   0        0        0        0 2023-06-17 13:05:44.515063 starrailcard-0.0.1/starrailcard/src/tools/__init__.py
--rw-r--r--   0        0        0      152 2023-06-17 13:06:12.300472 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2130 2023-06-22 10:13:41.936961 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/modal.cpython-310.pyc
--rw-r--r--   0        0        0     2308 2023-06-22 10:13:41.595730 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/openFile.cpython-310.pyc
--rw-r--r--   0        0        0     3792 2023-06-22 10:13:41.554630 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/pill.cpython-310.pyc
--rw-r--r--   0        0        0     1810 2023-06-17 13:06:12.303464 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/translation.cpython-310.pyc
--rw-r--r--   0        0        0     1536 2023-06-22 10:13:42.033261 starrailcard-0.0.1/starrailcard/src/tools/__pycache__/treePaths.cpython-310.pyc
--rw-r--r--   0        0        0     1218 2023-06-22 10:12:37.123912 starrailcard-0.0.1/starrailcard/src/tools/modal.py
--rw-r--r--   0        0        0     2224 2023-06-22 10:12:18.164061 starrailcard-0.0.1/starrailcard/src/tools/openFile.py
--rw-r--r--   0        0        0     5184 2023-06-22 10:12:31.195560 starrailcard-0.0.1/starrailcard/src/tools/pill.py
--rw-r--r--   0        0        0     2191 2023-06-22 10:15:06.259650 starrailcard-0.0.1/starrailcard/src/tools/translation.py
--rw-r--r--   0        0        0     1910 2023-06-22 10:12:25.055325 starrailcard-0.0.1/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 starrailcard-0.0.1/setup.py
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 starrailcard-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-06-22 11:25:27.375318 starrailcard-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1304 2023-06-22 11:25:16.479693 starrailcard-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 13:06:01.306235 starrailcard-0.0.2/starrailcard/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-22 11:11:26.279283 starrailcard-0.0.2/starrailcard/honkaicard.py
+-rw-r--r--   0        0        0        0 2023-06-17 13:05:17.443970 starrailcard-0.0.2/starrailcard/src/__init__.py
+-rw-r--r--   0        0        0     5623 2023-06-14 18:06:59.215231 starrailcard-0.0.2/starrailcard/src/assets/ARTIFACT.png
+-rw-r--r--   0        0        0    83412 2023-06-14 17:57:00.250514 starrailcard-0.0.2/starrailcard/src/assets/bg/bg.png
+-rw-r--r--   0        0        0   158031 2023-06-17 14:05:49.423459 starrailcard-0.0.2/starrailcard/src/assets/bg/bg_charters.png
+-rw-r--r--   0        0        0     6705 2023-06-14 17:57:52.444545 starrailcard-0.0.2/starrailcard/src/assets/bg/frame_charters.png
+-rw-r--r--   0        0        0     5628 2023-06-17 15:44:07.301010 starrailcard-0.0.2/starrailcard/src/assets/bg/maska.png
+-rw-r--r--   0        0        0     7216 2023-05-24 10:00:18.675835 starrailcard-0.0.2/starrailcard/src/assets/const/Closed.png
+-rw-r--r--   0        0        0     8219 2023-05-24 10:00:45.643719 starrailcard-0.0.2/starrailcard/src/assets/const/Lock.png
+-rw-r--r--   0        0        0    23211 2023-05-23 20:21:03.593475 starrailcard-0.0.2/starrailcard/src/assets/const/open.png
+-rw-r--r--   0        0        0  4909668 2022-09-27 23:11:24.000000 starrailcard-0.0.2/starrailcard/src/assets/font/NotoSansKR-Bold.otf
+-rw-r--r--   0        0        0     8848 2023-06-14 18:09:06.500975 starrailcard-0.0.2/starrailcard/src/assets/lc/bg.png
+-rw-r--r--   0        0        0     6756 2023-06-14 18:09:18.448917 starrailcard-0.0.2/starrailcard/src/assets/lc/bg_lc.png
+-rw-r--r--   0        0        0     5014 2023-06-17 15:41:55.506646 starrailcard-0.0.2/starrailcard/src/assets/lc/maska.png
+-rw-r--r--   0        0        0    10376 2023-06-14 18:04:44.670067 starrailcard-0.0.2/starrailcard/src/assets/LOGO.png
+-rw-r--r--   0        0        0     5250 2023-06-14 18:07:34.766685 starrailcard-0.0.2/starrailcard/src/assets/Sets/bg.png
+-rw-r--r--   0        0        0     4795 2023-06-14 18:07:50.587159 starrailcard-0.0.2/starrailcard/src/assets/Sets/count.png
+-rw-r--r--   0        0        0     4939 2023-05-23 20:18:52.221269 starrailcard-0.0.2/starrailcard/src/assets/stars/strs_1.png
+-rw-r--r--   0        0        0     5285 2023-05-23 20:18:40.906875 starrailcard-0.0.2/starrailcard/src/assets/stars/strs_2.png
+-rw-r--r--   0        0        0     5270 2023-05-23 20:18:31.351225 starrailcard-0.0.2/starrailcard/src/assets/stars/strs_3.png
+-rw-r--r--   0        0        0     5276 2023-05-23 20:18:20.816749 starrailcard-0.0.2/starrailcard/src/assets/stars/strs_4.png
+-rw-r--r--   0        0        0     5247 2023-05-23 20:18:00.663473 starrailcard-0.0.2/starrailcard/src/assets/stars/strs_5.png
+-rw-r--r--   0        0        0     5977 2023-06-14 18:06:19.159817 starrailcard-0.0.2/starrailcard/src/assets/STATS.png
+-rw-r--r--   0        0        0     5536 2023-06-14 18:00:51.102004 starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg.png
+-rw-r--r--   0        0        0     5767 2023-06-14 18:04:23.681149 starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg_dop.png
+-rw-r--r--   0        0        0     5621 2023-06-14 18:02:14.042865 starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg_main.png
+-rw-r--r--   0        0        0     3741 2023-06-14 18:01:09.230188 starrailcard-0.0.2/starrailcard/src/assets/Tallants/count.png
+-rw-r--r--   0        0        0     4256 2023-06-14 18:04:05.609136 starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_0.png
+-rw-r--r--   0        0        0     4834 2023-06-14 18:03:52.230355 starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_1.png
+-rw-r--r--   0        0        0     4907 2023-06-14 18:03:41.048412 starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_2.png
+-rw-r--r--   0        0        0     4876 2023-06-14 18:03:27.694098 starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_3.png
+-rw-r--r--   0        0        0     6131 2023-06-14 18:05:43.805818 starrailcard-0.0.2/starrailcard/src/assets/UID.png
+-rw-r--r--   0        0        0    16523 2023-06-22 10:13:09.430221 starrailcard-0.0.2/starrailcard/src/generators/one.py
+-rw-r--r--   0        0        0        0 2023-06-17 13:05:44.515063 starrailcard-0.0.2/starrailcard/src/tools/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-22 10:12:37.123912 starrailcard-0.0.2/starrailcard/src/tools/modal.py
+-rw-r--r--   0        0        0     2224 2023-06-22 10:12:18.164061 starrailcard-0.0.2/starrailcard/src/tools/openFile.py
+-rw-r--r--   0        0        0     5184 2023-06-22 10:12:31.195560 starrailcard-0.0.2/starrailcard/src/tools/pill.py
+-rw-r--r--   0        0        0     2191 2023-06-22 10:15:06.259650 starrailcard-0.0.2/starrailcard/src/tools/translation.py
+-rw-r--r--   0        0        0     1910 2023-06-22 10:12:25.055325 starrailcard-0.0.2/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 starrailcard-0.0.2/setup.py
+-rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 starrailcard-0.0.2/PKG-INFO
```

### Comparing `starrailcard-0.0.1/README.md` & `starrailcard-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
- <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png?token=GHSAT0AAAAAABYNVB75OGJZE4DGVGXA3LESZEUFGZA" alt="Баннер"/>
+ <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png" alt="Баннер"/>
 </p>
 
 ____
 
 ## StarRailCard
 Module for generating Honkai Star Rail character cards
 :white_medium_square: Ability to generate with or without background.<br>
```

### Comparing `starrailcard-0.0.1/starrailcard/honkaicard.py` & `starrailcard-0.0.2/starrailcard/honkaicard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/ARTIFACT.png` & `starrailcard-0.0.2/starrailcard/src/assets/ARTIFACT.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/bg/bg.png` & `starrailcard-0.0.2/starrailcard/src/assets/bg/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/bg/bg_charters.png` & `starrailcard-0.0.2/starrailcard/src/assets/bg/bg_charters.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/bg/frame_charters.png` & `starrailcard-0.0.2/starrailcard/src/assets/bg/frame_charters.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/bg/maska.png` & `starrailcard-0.0.2/starrailcard/src/assets/bg/maska.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/const/Closed.png` & `starrailcard-0.0.2/starrailcard/src/assets/const/Closed.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/const/Lock.png` & `starrailcard-0.0.2/starrailcard/src/assets/const/Lock.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/const/open.png` & `starrailcard-0.0.2/starrailcard/src/assets/const/open.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/font/NotoSansKR-Bold.otf` & `starrailcard-0.0.2/starrailcard/src/assets/font/NotoSansKR-Bold.otf`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/lc/bg.png` & `starrailcard-0.0.2/starrailcard/src/assets/lc/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/lc/bg_lc.png` & `starrailcard-0.0.2/starrailcard/src/assets/lc/bg_lc.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/lc/maska.png` & `starrailcard-0.0.2/starrailcard/src/assets/lc/maska.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/LOGO.png` & `starrailcard-0.0.2/starrailcard/src/assets/LOGO.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Sets/bg.png` & `starrailcard-0.0.2/starrailcard/src/assets/Sets/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Sets/count.png` & `starrailcard-0.0.2/starrailcard/src/assets/Sets/count.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/stars/strs_1.png` & `starrailcard-0.0.2/starrailcard/src/assets/stars/strs_1.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/stars/strs_2.png` & `starrailcard-0.0.2/starrailcard/src/assets/stars/strs_2.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/stars/strs_3.png` & `starrailcard-0.0.2/starrailcard/src/assets/stars/strs_3.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/stars/strs_4.png` & `starrailcard-0.0.2/starrailcard/src/assets/stars/strs_4.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/stars/strs_5.png` & `starrailcard-0.0.2/starrailcard/src/assets/stars/strs_5.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/STATS.png` & `starrailcard-0.0.2/starrailcard/src/assets/STATS.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg_dop.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg_dop.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/bg_main.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/bg_main.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/count.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/count.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_0.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_0.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_1.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_1.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_2.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_2.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/Tallants/dop_3.png` & `starrailcard-0.0.2/starrailcard/src/assets/Tallants/dop_3.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/assets/UID.png` & `starrailcard-0.0.2/starrailcard/src/assets/UID.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/generators/one.py` & `starrailcard-0.0.2/starrailcard/src/generators/one.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/tools/modal.py` & `starrailcard-0.0.2/starrailcard/src/tools/modal.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/tools/openFile.py` & `starrailcard-0.0.2/starrailcard/src/tools/openFile.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/tools/pill.py` & `starrailcard-0.0.2/starrailcard/src/tools/pill.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/tools/translation.py` & `starrailcard-0.0.2/starrailcard/src/tools/translation.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/starrailcard/src/tools/treePaths.py` & `starrailcard-0.0.2/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.1/setup.py` & `starrailcard-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
                       'assets/stars/*']}
 
 install_requires = \
 ['Pillow>=9.4.0,<10.0.0', 'honkairail>=1.0.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'starrailcard',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Module for generating Honkai Star Rail character cards',
-    'long_description': '<p align="center">\n <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png?token=GHSAT0AAAAAABYNVB75OGJZE4DGVGXA3LESZEUFGZA" alt="Баннер"/>\n</p>\n\n____\n\n## StarRailCard\nModule for generating Honkai Star Rail character cards\n:white_medium_square: Ability to generate with or without background.<br>\n:white_medium_square: Ability to set a custom image.<br>\n:white_medium_square: Flexible map settings.\n\n## Installation:\n```\npip install starrailcard\n```\n\n## Launch:\n``` python\nfrom starrailcard import honkaicard \nimport asyncio\n\nasync def mains():\n    while True:\n        async with honkaicard.MiHoMoCard() as hmhm:\n            r = await hmhm.creat(700649319)\n            print(r)\n\nasyncio.run(mains())\n```\n\n## Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cht  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n|  Khaenri\'ah  |     kh  | Khaenri\'ah |',
+    'long_description': '<p align="center">\n <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png" alt="Баннер"/>\n</p>\n\n____\n\n## StarRailCard\nModule for generating Honkai Star Rail character cards\n:white_medium_square: Ability to generate with or without background.<br>\n:white_medium_square: Ability to set a custom image.<br>\n:white_medium_square: Flexible map settings.\n\n## Installation:\n```\npip install starrailcard\n```\n\n## Launch:\n``` python\nfrom starrailcard import honkaicard \nimport asyncio\n\nasync def mains():\n    while True:\n        async with honkaicard.MiHoMoCard() as hmhm:\n            r = await hmhm.creat(700649319)\n            print(r)\n\nasyncio.run(mains())\n```\n\n## Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cht  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n|  Khaenri\'ah  |     kh  | Khaenri\'ah |',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/StarRailCard',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `starrailcard-0.0.1/PKG-INFO` & `starrailcard-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module for generating Honkai Star Rail character cards
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: None
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.4.0,<10.0.0)
 Requires-Dist: honkairail (>=1.0.9,<2.0.0)
 Project-URL: Repository, https://github.com/DEViantUA/StarRailCard
 Description-Content-Type: text/markdown
 
 <p align="center">
- <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png?token=GHSAT0AAAAAABYNVB75OGJZE4DGVGXA3LESZEUFGZA" alt="Баннер"/>
+ <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png" alt="Баннер"/>
 </p>
 
 ____
 
 ## StarRailCard
 Module for generating Honkai Star Rail character cards
 :white_medium_square: Ability to generate with or without background.<br>
```

