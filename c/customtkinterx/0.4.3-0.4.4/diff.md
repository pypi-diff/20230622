# Comparing `tmp/customtkinterx-0.4.3.tar.gz` & `tmp/customtkinterx-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.4.3.tar", max compression
+gzip compressed data, was "customtkinterx-0.4.4.tar", max compression
```

## Comparing `customtkinterx-0.4.3.tar` & `customtkinterx-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,55 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.3/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1323 2023-06-22 01:38:37.719610 customtkinterx-0.4.3/customtkinterx/__init__.py
--rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.3/customtkinterx/__main__.py
--rw-r--r--   0        0        0    10207 2023-06-22 01:09:11.417087 customtkinterx-0.4.3/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6744 2023-06-19 11:05:29.722427 customtkinterx-0.4.3/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.3/customtkinterx/CTkGhostSharkTheme.py
--rw-r--r--   0        0        0     8803 2023-06-20 12:13:02.421335 customtkinterx-0.4.3/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     4566 2023-06-20 09:30:34.136863 customtkinterx-0.4.3/customtkinterx/CTkKanban.py
--rw-r--r--   0        0        0     1279 2023-06-20 10:15:40.135212 customtkinterx-0.4.3/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     7667 2023-06-20 11:05:15.033164 customtkinterx-0.4.3/customtkinterx/CTkMaterialTheme.py
--rw-r--r--   0        0        0     2637 2023-06-22 01:46:19.472328 customtkinterx-0.4.3/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.3/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     7659 2023-06-20 11:03:56.651312 customtkinterx-0.4.3/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.3/customtkinterx/CTkOffice2019Theme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0     2971 2023-06-20 10:09:30.744234 customtkinterx-0.4.3/customtkinterx/CTkSnackBar.py
--rw-r--r--   0        0        0      768 2023-06-22 01:54:42.088680 customtkinterx-0.4.3/customtkinterx/CTkStack.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.3/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.3/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.3/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.3/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.3/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.3/customtkinterx/fluent_android/__init__.py
--rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
--rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAppBar.py
--rw-r--r--   0        0        0     5680 2023-06-20 12:13:36.856108 customtkinterx-0.4.3/customtkinterx/fluent_android/FluentAndroid.json
--rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.3/customtkinterx/GhostShark.json
--rw-r--r--   0        0        0    10021 2023-06-20 08:42:06.949292 customtkinterx-0.4.3/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     6706 2023-06-20 12:01:51.720398 customtkinterx-0.4.3/customtkinterx/Material.json
--rw-r--r--   0        0        0     6706 2023-06-20 10:59:12.383731 customtkinterx-0.4.3/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.3/customtkinterx/Musix-Dark.png
--rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.3/customtkinterx/Musix.png
--rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.3/customtkinterx/Office2019.json
--rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.3/customtkinterx/PublicSans-Regular.ttf
--rw-r--r--   0        0        0    11524 2023-06-20 12:12:10.818717 customtkinterx-0.4.3/customtkinterx/test.py
--rw-r--r--   0        0        0      345 2023-06-22 03:21:52.727275 customtkinterx-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3698 2023-06-20 08:20:21.780955 customtkinterx-0.4.3/README.md
--rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 customtkinterx-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.4/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1383 2023-06-22 09:16:54.227454 customtkinterx-0.4.4/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.4/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     7725 2023-06-22 09:05:07.756811 customtkinterx-0.4.4/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     2837 2023-06-22 09:04:29.630248 customtkinterx-0.4.4/customtkinterx/CTkCustomBorder.py
+-rw-r--r--   0        0        0     6744 2023-06-19 11:05:29.722427 customtkinterx-0.4.4/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.4/customtkinterx/CTkGhostSharkTheme.py
+-rw-r--r--   0        0        0     8803 2023-06-20 12:13:02.421335 customtkinterx-0.4.4/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     4566 2023-06-20 09:30:34.136863 customtkinterx-0.4.4/customtkinterx/CTkKanban.py
+-rw-r--r--   0        0        0     1279 2023-06-20 10:15:40.135212 customtkinterx-0.4.4/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     7667 2023-06-20 11:05:15.033164 customtkinterx-0.4.4/customtkinterx/CTkMaterialTheme.py
+-rw-r--r--   0        0        0     2637 2023-06-22 01:46:19.472328 customtkinterx-0.4.4/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-22 09:00:51.757273 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-22 09:00:51.777319 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-22 09:00:51.765283 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-22 09:00:51.770803 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.4/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     7659 2023-06-20 11:03:56.651312 customtkinterx-0.4.4/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.4/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.4/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-22 09:00:51.791860 customtkinterx-0.4.4/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-22 09:00:51.796366 customtkinterx-0.4.4/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0     2971 2023-06-20 10:09:30.744234 customtkinterx-0.4.4/customtkinterx/CTkSnackBar.py
+-rw-r--r--   0        0        0      768 2023-06-22 01:54:42.088680 customtkinterx-0.4.4/customtkinterx/CTkStack.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.4/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-22 09:00:51.833466 customtkinterx-0.4.4/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-22 09:00:51.841990 customtkinterx-0.4.4/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.4/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.4/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-22 09:00:51.801383 customtkinterx-0.4.4/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-22 09:00:51.806378 customtkinterx-0.4.4/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.4/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.4/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.4/customtkinterx/fluent_android/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-22 09:00:51.725687 customtkinterx-0.4.4/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7135 2023-06-22 09:00:51.729709 customtkinterx-0.4.4/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
+-rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.4/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
+-rw-r--r--   0        0        0     1796 2023-06-22 09:23:54.491541 customtkinterx-0.4.4/customtkinterx/fluent_android/CTkFluentAppBar.py
+-rw-r--r--   0        0        0     5680 2023-06-20 12:13:36.856108 customtkinterx-0.4.4/customtkinterx/fluent_android/FluentAndroid.json
+-rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.4/customtkinterx/GhostShark.json
+-rw-r--r--   0        0        0    10021 2023-06-20 08:42:06.949292 customtkinterx-0.4.4/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     6706 2023-06-20 12:01:51.720398 customtkinterx-0.4.4/customtkinterx/Material.json
+-rw-r--r--   0        0        0     6706 2023-06-20 10:59:12.383731 customtkinterx-0.4.4/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.4/customtkinterx/Musix-Dark.png
+-rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.4/customtkinterx/Musix.png
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.4/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.4/customtkinterx/PublicSans-Regular.ttf
+-rw-r--r--   0        0        0    11524 2023-06-20 12:12:10.818717 customtkinterx-0.4.4/customtkinterx/test.py
+-rw-r--r--   0        0        0      345 2023-06-22 09:29:23.151915 customtkinterx-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3698 2023-06-20 08:20:21.780955 customtkinterx-0.4.4/README.md
+-rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 customtkinterx-0.4.4/PKG-INFO
```

### Comparing `customtkinterx-0.4.3/customtkinterx/__init__.py` & `customtkinterx-0.4.4/customtkinterx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from customtkinterx.CTkCustomBorder import CTkCustomBorder
 from customtkinterx.CTkCustom import CTkCustom, bind_move as bind_root_move
+
 from customtkinterx.CTkFluentTheme import use_fluent_theme as CTkFluentTheme
 from customtkinterx.CTkMinimalTheme import use_minimal_theme as CTkMinimalTheme
 from customtkinterx.CTkMaterialTheme import use_material_theme as CTkMaterialTheme
 from customtkinterx.CTkOffice2019Theme import use_office2019_theme as CTkOffice2019Theme
 from customtkinterx.CTkGhostSharkTheme import use_ghost_shark_theme as CTkGhostSharkTheme
 
 from customtkinterx.CTkStack import CTkStack
 from customtkinterx.CTkInfoBar import CTkInfoBar, NORMAL, SUCCESS, CAUTION, CRITICAL
 from customtkinterx.CTkMegaMenuBar import CTkMegaMenuBar, CTkMegaMenu
 from customtkinterx.CTkSnackBar import CTkSnackBar
 from customtkinterx.CTkKanban import CTkKanbanCard, CTkKanban
-
 from customtkinterx.fluent_android import *
 
 # From https://github.com/Akascape/CTkMenuBar
 from customtkinterx.CTkMenuBar import CTkMenuBar, CTkTitleMenu, CustomDropdownMenu as CTkCustomDropdownMenu
 
 # From https://github.com/Akascape/CTkPDFViewer
 from customtkinterx.CTkPDFViewer import CTkPDFViewer
```

### Comparing `customtkinterx-0.4.3/customtkinterx/__main__.py` & `customtkinterx-0.4.4/customtkinterx/__main__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkCustom.py` & `customtkinterx-0.4.4/customtkinterx/CTkCustom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from customtkinter import CTk, CTkToplevel, CTkFrame, CTkLabel, CTkButton, ThemeManager, get_appearance_mode
+from customtkinterx.CTkCustomBorder import CTkCustomBorder
 from tkinter import ttk
 
 
 def bind_move(widget, root):
     def _click(event):
         global x, y
         x, y = event.x, event.y
@@ -13,76 +14,21 @@
         s = f"+{new_x}+{new_y}"
         root.geometry(s)
 
     widget.bind("<Button-1>", _click, add="+")
     widget.bind("<B1-Motion>", _move, add="+")
 
 
-class CTkCustom(CTk):
+class CTkCustom(CTkCustomBorder):
     def __init__(self, title: str = "", advanced: bool = True, titlebar: bool = True,
                  client_edge: bool = False, window_edge: bool = False, titlebar_layout: str = "pack", **kwargs):
         try:
             super().__init__(**kwargs)
         except:
             pass
-        from sys import platform
-        if advanced:
-            if platform == "win32":
-                if "CTkCustom" in ThemeManager.theme:
-                    self.__transparent_color = ThemeManager.theme["CTkCustom"]["transparent_color"]
-                else:
-                    self.__transparent_color = "#101010"
-                self.attributes("-transparentcolor", self.__transparent_color)
-                self.configure(fg_color=self.__transparent_color)
-            elif platform == "darwin":
-                self.__transparent_color = 'systemTransparent'
-                self.attributes("-transparent", True)
-                self.configure(fg_color=self.__transparent_color)
-            else:
-                self.__transparent_color = '#000001'
-
-        self.wm_overrideredirect(True)
-
-        if advanced:
-            if platform == "win32":
-                from ctypes import windll
-                windll.uxtheme
-                GWL_EXSTYLE = -20
-                WS_EX_APPWINDOW = 0x00040000
-                WS_EX_TOOLWINDOW = 0x00000080
-                WS_EX_CLIENTEDGE = 0x00000200
-                WS_EX_WINDOWEDGE = 0x00000100
-                hwnd = windll.user32.GetParent(self.winfo_id())
-                style = windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
-                style = style & ~WS_EX_TOOLWINDOW
-                style = style | WS_EX_APPWINDOW
-                if client_edge:
-                    style = style | WS_EX_CLIENTEDGE
-                if window_edge:
-                    style = style | WS_EX_WINDOWEDGE
-                res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
-                self.style32 = style
-            else:
-                try:
-                    self.wm_attributes("-topmost", True)
-                except:
-                    pass
-
-        self.minsize(150, 180)
-
-        self.__frame_border = CTkFrame(self, border_width=1,
-                                       background_corner_colors=(
-                                           self.__transparent_color,
-                                           self.__transparent_color,
-                                           self.__transparent_color,
-                                           self.__transparent_color
-                                       )
-                                       )
-        self.__frame_border.pack(fill="both", expand=True, padx=0, pady=0)
-
         if titlebar:
             self.create_titlebar(title)
 
     def minimize(self):
         try:
             from ctypes import windll
             hwnd = windll.user32.GetParent(self.winfo_id())
@@ -128,29 +74,29 @@
         if custom:
             self.sizegrip = CTkButton(self.__frame_border, width=32, height=32, text="⚪")
             self.sizegrip.configure(cursor="sizing")
 
             self.sizegrip.bind("<Button-1>", self._sizegrip_click)
             self.sizegrip.bind("<B1-Motion>", self._sizegrip_move)
             self.sizegrip._text_color = ThemeManager.theme["CTkLabel"]["text_color"]
-            self.sizegrip._fg_color = self.sizegrip._hover_color = self.__frame_border._fg_color
+            self.sizegrip._fg_color = self.sizegrip._hover_color = self.mainframe._fg_color
             self.sizegrip._draw()
             self.sizegrip.pack(side="bottom", anchor="se", padx=3, pady=3)
         else:
             if get_appearance_mode() == "Dark":
                 ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][1])
             else:
                 ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][0])
-            self.sizegrip = ttk.Sizegrip(self.__frame_border, style="CTkCustom.TSizegrip")
+            self.sizegrip = ttk.Sizegrip(self.mainframe, style="CTkCustom.TSizegrip")
             self.sizegrip.pack(side="bottom", anchor="se", padx=5, pady=5, ipady=2)
         return self.sizegrip
 
     def create_titlebar(self, title: str, titlebar_layout: str = "pack"):
 
-        self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=ThemeManager.theme["CTkFrame"]["corner_radius"]/2+2)
+        self.__frame_title = CTkFrame(self.mainframe, border_width=0, corner_radius=ThemeManager.theme["CTkFrame"]["corner_radius"]/2+2)
         self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
         self.bind_move(self.__frame_title)
 
         self.title(title)
 
         self.maximized = False
 
@@ -216,18 +162,14 @@
     def titlebar_closebutton(self):
         return self.__button_close
 
     @property
     def titlebar_minimizebutton(self):
         return self.__button_minimize
 
-    @property
-    def mainframe(self):
-        return self.__frame_border
-
     def _click(self, event):
         import warnings
 
         warnings.warn(
             '请不要使用此方法'
             '请使用bind_move',
             DeprecationWarning,
```

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.4.4/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkGhostSharkTheme.py` & `customtkinterx-0.4.4/customtkinterx/CTkGhostSharkTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.4.4/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkKanban.py` & `customtkinterx-0.4.4/customtkinterx/CTkKanban.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkListBox.py` & `customtkinterx-0.4.4/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMaterialTheme.py` & `customtkinterx-0.4.4/customtkinterx/CTkMaterialTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.4.4/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.4.4/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.4.4/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.4.4/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.4.4/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkOffice2019Theme.py` & `customtkinterx-0.4.4/customtkinterx/CTkOffice2019Theme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.4.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkSnackBar.py` & `customtkinterx-0.4.4/customtkinterx/CTkSnackBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkStack.py` & `customtkinterx-0.4.4/customtkinterx/CTkStack.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.4.4/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.4.4/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Fluent.json` & `customtkinterx-0.4.4/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAndroidTheme.py` & `customtkinterx-0.4.4/customtkinterx/fluent_android/CTkFluentAndroidTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/fluent_android/CTkFluentAppBar.py` & `customtkinterx-0.4.4/customtkinterx/fluent_android/CTkFluentAppBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return self.__subtitle
 
     def show(self):
         self.pack(fill="x", side="top")
 
 
 if __name__ == '__main__':
-    from customtkinterx import CTkCustom
+    from customtkinterx import CTkCustom, CTkMinimalTheme
     from customtkinter import CTk, set_appearance_mode, set_widget_scaling
 
     set_appearance_mode("dark")
 
     CTkFluentAndroidTheme()
 
     root = CTkCustom()
```

### Comparing `customtkinterx-0.4.3/customtkinterx/fluent_android/FluentAndroid.json` & `customtkinterx-0.4.4/customtkinterx/fluent_android/FluentAndroid.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/GhostShark.json` & `customtkinterx-0.4.4/customtkinterx/GhostShark.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/LaunchMusix.py` & `customtkinterx-0.4.4/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Material.json` & `customtkinterx-0.4.4/customtkinterx/Material.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Minimal.json` & `customtkinterx-0.4.4/customtkinterx/Minimal.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Musix-Dark.png` & `customtkinterx-0.4.4/customtkinterx/Musix-Dark.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Musix.png` & `customtkinterx-0.4.4/customtkinterx/Musix.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/Office2019.json` & `customtkinterx-0.4.4/customtkinterx/Office2019.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/PublicSans-Regular.ttf` & `customtkinterx-0.4.4/customtkinterx/PublicSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/customtkinterx/test.py` & `customtkinterx-0.4.4/customtkinterx/test.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/README.md` & `customtkinterx-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.3/PKG-INFO` & `customtkinterx-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.4.3
+Version: 0.4.4
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

