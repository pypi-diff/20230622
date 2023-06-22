# Comparing `tmp/customtkinterx-0.4.2.tar.gz` & `tmp/customtkinterx-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.4.2.tar", max compression
+gzip compressed data, was "customtkinterx-0.4.3.tar", max compression
```

## Comparing `customtkinterx-0.4.2.tar` & `customtkinterx-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.2/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1323 2023-06-22 01:38:37.719610 customtkinterx-0.4.2/customtkinterx/__init__.py
--rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.2/customtkinterx/__main__.py
--rw-r--r--   0        0        0    10207 2023-06-22 01:09:11.417087 customtkinterx-0.4.2/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6744 2023-06-19 11:05:29.722427 customtkinterx-0.4.2/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.2/customtkinterx/CTkGhostSharkTheme.py
--rw-r--r--   0        0        0     8803 2023-06-20 12:13:02.421335 customtkinterx-0.4.2/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     4566 2023-06-20 09:30:34.136863 customtkinterx-0.4.2/customtkinterx/CTkKanban.py
--rw-r--r--   0        0        0     1279 2023-06-20 10:15:40.135212 customtkinterx-0.4.2/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     7667 2023-06-20 11:05:15.033164 customtkinterx-0.4.2/customtkinterx/CTkMaterialTheme.py
--rw-r--r--   0        0        0     2637 2023-06-22 01:46:19.472328 customtkinterx-0.4.2/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.2/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.2/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.2/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.2/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     7659 2023-06-20 11:03:56.651312 customtkinterx-0.4.2/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.2/customtkinterx/CTkOffice2019Theme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.2/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0     2971 2023-06-20 10:09:30.744234 customtkinterx-0.4.2/customtkinterx/CTkSnackBar.py
--rw-r--r--   0        0        0      768 2023-06-22 01:54:42.088680 customtkinterx-0.4.2/customtkinterx/CTkStack.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.2/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.2/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.2/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.2/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.2/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.2/customtkinterx/fluent_android/__init__.py
--rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.2/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
--rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.2/customtkinterx/fluent_android/CTkFluentAppBar.py
--rw-r--r--   0        0        0     5680 2023-06-20 12:13:36.856108 customtkinterx-0.4.2/customtkinterx/fluent_android/FluentAndroid.json
--rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.2/customtkinterx/GhostShark.json
--rw-r--r--   0        0        0    10021 2023-06-20 08:42:06.949292 customtkinterx-0.4.2/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     6706 2023-06-20 12:01:51.720398 customtkinterx-0.4.2/customtkinterx/Material.json
--rw-r--r--   0        0        0     6706 2023-06-20 10:59:12.383731 customtkinterx-0.4.2/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.2/customtkinterx/Musix-Dark.png
--rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.2/customtkinterx/Musix.png
--rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.2/customtkinterx/Office2019.json
--rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.2/customtkinterx/PublicSans-Regular.ttf
--rw-r--r--   0        0        0    11524 2023-06-20 12:12:10.818717 customtkinterx-0.4.2/customtkinterx/test.py
--rw-r--r--   0        0        0      368 2023-06-22 03:20:22.779838 customtkinterx-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3698 2023-06-20 08:20:21.780955 customtkinterx-0.4.2/README.md
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 customtkinterx-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.3/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1323 2023-06-22 01:38:37.719610 customtkinterx-0.4.3/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.3/customtkinterx/__main__.py
+-rw-r--r--   0        0        0    10207 2023-06-22 01:09:11.417087 customtkinterx-0.4.3/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6744 2023-06-19 11:05:29.722427 customtkinterx-0.4.3/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.3/customtkinterx/CTkGhostSharkTheme.py
+-rw-r--r--   0        0        0     8803 2023-06-20 12:13:02.421335 customtkinterx-0.4.3/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     4566 2023-06-20 09:30:34.136863 customtkinterx-0.4.3/customtkinterx/CTkKanban.py
+-rw-r--r--   0        0        0     1279 2023-06-20 10:15:40.135212 customtkinterx-0.4.3/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     7667 2023-06-20 11:05:15.033164 customtkinterx-0.4.3/customtkinterx/CTkMaterialTheme.py
+-rw-r--r--   0        0        0     2637 2023-06-22 01:46:19.472328 customtkinterx-0.4.3/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     7659 2023-06-20 11:03:56.651312 customtkinterx-0.4.3/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.3/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0     2971 2023-06-20 10:09:30.744234 customtkinterx-0.4.3/customtkinterx/CTkSnackBar.py
+-rw-r--r--   0        0        0      768 2023-06-22 01:54:42.088680 customtkinterx-0.4.3/customtkinterx/CTkStack.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.3/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.3/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.3/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.3/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.3/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.3/customtkinterx/fluent_android/__init__.py
+-rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
+-rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAppBar.py
+-rw-r--r--   0        0        0     5680 2023-06-20 12:13:36.856108 customtkinterx-0.4.3/customtkinterx/fluent_android/FluentAndroid.json
+-rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.3/customtkinterx/GhostShark.json
+-rw-r--r--   0        0        0    10021 2023-06-20 08:42:06.949292 customtkinterx-0.4.3/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     6706 2023-06-20 12:01:51.720398 customtkinterx-0.4.3/customtkinterx/Material.json
+-rw-r--r--   0        0        0     6706 2023-06-20 10:59:12.383731 customtkinterx-0.4.3/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.3/customtkinterx/Musix-Dark.png
+-rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.3/customtkinterx/Musix.png
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.3/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.3/customtkinterx/PublicSans-Regular.ttf
+-rw-r--r--   0        0        0    11524 2023-06-20 12:12:10.818717 customtkinterx-0.4.3/customtkinterx/test.py
+-rw-r--r--   0        0        0      345 2023-06-22 03:21:52.727275 customtkinterx-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3698 2023-06-20 08:20:21.780955 customtkinterx-0.4.3/README.md
+-rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 customtkinterx-0.4.3/PKG-INFO
```

### Comparing `customtkinterx-0.4.2/customtkinterx/__init__.py` & `customtkinterx-0.4.3/customtkinterx/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/__main__.py` & `customtkinterx-0.4.3/customtkinterx/__main__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkCustom.py` & `customtkinterx-0.4.3/customtkinterx/CTkCustom.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.4.3/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkGhostSharkTheme.py` & `customtkinterx-0.4.3/customtkinterx/CTkGhostSharkTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.4.3/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkKanban.py` & `customtkinterx-0.4.3/customtkinterx/CTkKanban.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkListBox.py` & `customtkinterx-0.4.3/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMaterialTheme.py` & `customtkinterx-0.4.3/customtkinterx/CTkMaterialTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.4.3/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.4.3/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkOffice2019Theme.py` & `customtkinterx-0.4.3/customtkinterx/CTkOffice2019Theme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkSnackBar.py` & `customtkinterx-0.4.3/customtkinterx/CTkSnackBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkStack.py` & `customtkinterx-0.4.3/customtkinterx/CTkStack.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.4.3/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.4.3/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Fluent.json` & `customtkinterx-0.4.3/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/fluent_android/CTkFluentAndroidTheme.py` & `customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAndroidTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/fluent_android/CTkFluentAppBar.py` & `customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAppBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/fluent_android/FluentAndroid.json` & `customtkinterx-0.4.3/customtkinterx/fluent_android/FluentAndroid.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/GhostShark.json` & `customtkinterx-0.4.3/customtkinterx/GhostShark.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/LaunchMusix.py` & `customtkinterx-0.4.3/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Material.json` & `customtkinterx-0.4.3/customtkinterx/Material.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Minimal.json` & `customtkinterx-0.4.3/customtkinterx/Minimal.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Musix-Dark.png` & `customtkinterx-0.4.3/customtkinterx/Musix-Dark.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Musix.png` & `customtkinterx-0.4.3/customtkinterx/Musix.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/Office2019.json` & `customtkinterx-0.4.3/customtkinterx/Office2019.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/PublicSans-Regular.ttf` & `customtkinterx-0.4.3/customtkinterx/PublicSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/customtkinterx/test.py` & `customtkinterx-0.4.3/customtkinterx/test.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/README.md` & `customtkinterx-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.2/PKG-INFO` & `customtkinterx-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.4.2
+Version: 0.4.3
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: customtkinter (>=5.1.3,<6.0.0)
-Requires-Dist: pyautogui (>=0.9.54,<0.10.0)
 Description-Content-Type: text/markdown
 
 # CustomTkinterX
 > 解释器需Python3.7及以上
 
 `customtkinter`的扩展组件功能库，同时也采集了其他开发者制作的组件，并进行仅类型提示上的修改（源代码`__main__.py`上有标注）
```

