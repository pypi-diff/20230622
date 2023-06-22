# Comparing `tmp/irene_pro-0.0.65.tar.gz` & `tmp/irene_pro-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.65.tar", last modified: Wed Jun 21 10:02:32 2023, max compression
+gzip compressed data, was "irene_pro-0.0.66.tar", last modified: Thu Jun 22 07:12:00 2023, max compression
```

## Comparing `irene_pro-0.0.65.tar` & `irene_pro-0.0.66.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 10:02:32.818209 irene_pro-0.0.65/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.65/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.65/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-21 10:02:32.816214 irene_pro-0.0.65/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.65/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 10:02:32.790281 irene_pro-0.0.65/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.65/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.65/irene_pro/logic.py
--rw-rw-rw-   0        0        0    33433 2023-06-21 10:00:56.000000 irene_pro-0.0.65/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-21 10:02:32.812226 irene_pro-0.0.65/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-21 10:02:32.000000 irene_pro-0.0.65/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-21 10:02:32.000000 irene_pro-0.0.65/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 10:02:32.000000 irene_pro-0.0.65/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-21 10:02:32.000000 irene_pro-0.0.65/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 10:02:32.000000 irene_pro-0.0.65/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 10:02:32.818209 irene_pro-0.0.65/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-21 10:01:47.000000 irene_pro-0.0.65/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:12:00.440158 irene_pro-0.0.66/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.66/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.66/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-22 07:12:00.438125 irene_pro-0.0.66/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.66/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 07:12:00.407205 irene_pro-0.0.66/irene_gui_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.66/irene_gui_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.66/irene_gui_pkg/logic.py
+-rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.66/irene_gui_pkg/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:12:00.418176 irene_pro-0.0.66/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.66/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.66/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    33528 2023-06-22 07:09:35.000000 irene_pro-0.0.66/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:12:00.435131 irene_pro-0.0.66/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-22 07:12:00.000000 irene_pro-0.0.66/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-22 07:12:00.000000 irene_pro-0.0.66/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:12:00.000000 irene_pro-0.0.66/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-22 07:12:00.000000 irene_pro-0.0.66/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-22 07:12:00.000000 irene_pro-0.0.66/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:12:00.440158 irene_pro-0.0.66/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-22 07:11:05.000000 irene_pro-0.0.66/setup.py
```

### Comparing `irene_pro-0.0.65/PKG-INFO` & `irene_pro-0.0.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.65
+Version: 0.0.66
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.65/README.md` & `irene_pro-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.65/irene_pro/logic.py` & `irene_pro-0.0.66/irene_gui_pkg/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.65/irene_pro/widgets.py` & `irene_pro-0.0.66/irene_gui_pkg/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,33 +75,34 @@
             self.column(col,width = col_width, stretch=True)
             self.heading(col, text = col, anchor = CENTER)
             i += 1
 
         self.index_for_single_list_data = 0
 
         
-    def alter_rows(self):
+    def alter_rows(self, odd_color = 'gray70', even_color = 'khaki'):
         style = ttkthemes.ThemedStyle(self.master)
         style.theme_use("clam")
         style.map("Treeview", background=[('selected', 'gray40')], foreground = [('selected', 'gold')])
-        self.tag_configure('odd', background='gray70')
-        self.tag_configure('even', background='khaki')
+        self.tag_configure('odd', background=odd_color)
+        self.tag_configure('even', background=even_color)
+
 
     def insert_data(self,data, wrap_length = 70):
         def wrapping(data_list):
             """I assume that datalist is a list as the name implies"""
             all_row = []
             for item in data_list:
                 # print(f"CURRENT ITEM: {item}")
                 if type(item) == str:
                     wrapped = wrap(item, wrap_length)
                     all_row.append("\n".join(wrapped))
                 else:
                     all_row.append(item)
-                print(f"__________________{type(item)}_______{item}_________________")
+                
             return all_row
                 
         try:
             if type(data[0]) not in [list, tuple]:
                 if self.include_index:
                     tag = ('odd')
```

### Comparing `irene_pro-0.0.65/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.66/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.65
+Version: 0.0.66
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.65/setup.py` & `irene_pro-0.0.66/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3635 270d 0a44 4553 4352   '0.0.65'..DESCR
+00000100: 2027 302e 302e 3636 270d 0a44 4553 4352   '0.0.66'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

