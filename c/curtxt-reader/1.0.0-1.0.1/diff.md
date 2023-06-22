# Comparing `tmp/curtxt-reader-1.0.0.tar.gz` & `tmp/curtxt-reader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtxt-reader-1.0.0.tar", last modified: Thu Jun 22 10:35:40 2023, max compression
+gzip compressed data, was "curtxt-reader-1.0.1.tar", last modified: Thu Jun 22 14:00:37 2023, max compression
```

## Comparing `curtxt-reader-1.0.0.tar` & `curtxt-reader-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 10:35:40.832652 curtxt-reader-1.0.0/
--rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.0.0/LICENSE
--rw-r--r--   0 iris      (1000) iris      (1000)    21247 2023-06-22 10:35:40.832652 curtxt-reader-1.0.0/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      793 2023-06-22 10:25:33.000000 curtxt-reader-1.0.0/README.md
--rwxr-xr-x   0 iris      (1000) iris      (1000)     5667 2023-06-21 20:40:32.000000 curtxt-reader-1.0.0/curtxt.py
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 10:35:40.829319 curtxt-reader-1.0.0/curtxt_reader.egg-info/
--rw-r--r--   0 iris      (1000) iris      (1000)    21247 2023-06-22 10:35:40.000000 curtxt-reader-1.0.0/curtxt_reader.egg-info/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-06-22 10:35:40.000000 curtxt-reader-1.0.0/curtxt_reader.egg-info/SOURCES.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-06-22 10:35:40.000000 curtxt-reader-1.0.0/curtxt_reader.egg-info/dependency_links.txt
--rw-r--r--   0 iris      (1000) iris      (1000)       48 2023-06-22 10:35:40.000000 curtxt-reader-1.0.0/curtxt_reader.egg-info/entry_points.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-06-22 10:35:40.000000 curtxt-reader-1.0.0/curtxt_reader.egg-info/top_level.txt
--rw-r--r--   0 iris      (1000) iris      (1000)      906 2023-06-22 10:34:04.000000 curtxt-reader-1.0.0/pyproject.toml
--rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-06-22 10:35:40.832652 curtxt-reader-1.0.0/setup.cfg
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/
+-rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.0.1/LICENSE
+-rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      895 2023-06-22 10:38:24.000000 curtxt-reader-1.0.1/README.md
+-rwxr-xr-x   0 iris      (1000) iris      (1000)     5953 2023-06-22 13:58:57.000000 curtxt-reader-1.0.1/curtxt.py
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/curtxt_reader.egg-info/
+-rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)       48 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/entry_points.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/top_level.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)      906 2023-06-22 14:00:20.000000 curtxt-reader-1.0.1/pyproject.toml
+-rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-06-22 14:00:37.756132 curtxt-reader-1.0.1/setup.cfg
```

### Comparing `curtxt-reader-1.0.0/LICENSE` & `curtxt-reader-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.0.0/PKG-INFO` & `curtxt-reader-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple ncurses-based plain text reader written
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -388,14 +388,15 @@
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Curses txt reader
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
+[![PyPI version](https://badge.fury.io/py/curtxt-reader.svg)](https://badge.fury.io/py/curtxt-reader)
 ## About
 A simple ncurses-based plain text reader written in python.  
 ## Instalation
 From PyPI:  
 	
     $ pip install curtxt-reader
```

### Comparing `curtxt-reader-1.0.0/README.md` & `curtxt-reader-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Curses txt reader
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
+[![PyPI version](https://badge.fury.io/py/curtxt-reader.svg)](https://badge.fury.io/py/curtxt-reader)
 ## About
 A simple ncurses-based plain text reader written in python.  
 ## Instalation
 From PyPI:  
 	
     $ pip install curtxt-reader
```

### Comparing `curtxt-reader-1.0.0/curtxt.py` & `curtxt-reader-1.0.1/curtxt.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,63 +3,68 @@
 from fileinput import input as f_input
 from sys import argv
 import os
 import curses
 
 
 class main_window:
-    MARGIN_X = 4
-    MARGIN_Y = 8
+    # SUMS of both left and right margins
+    MARGINS_X = 4
+    MARGINS_Y = 8
 
     def __init__(self):
-        self.height = curses.LINES - main_window.MARGIN_Y
+        self.height = curses.LINES - main_window.MARGINS_Y
         self.output_raw = self.__get_raw_output()
-        self.longes_line_len = len(max(self.output_raw, key=len)) or 80
+        self.longest_line_len = len(max(self.output_raw, key=len)) or 80
         self.page_count = self.__get_page_count()
-        self.width = (self.longes_line_len + 1) * self.page_count + 3
-        self.start_x = trunc((curses.COLS - self.longes_line_len * self.page_count) / 2)
-        self.start_y = trunc(main_window.MARGIN_Y / 2)
+        self.width = (self.longest_line_len + 1) * self.page_count + 3
+        self.start_x = trunc((curses.COLS - self.longest_line_len * self.page_count - 4) / 2)
+        self.start_y = trunc(main_window.MARGINS_Y / 2)
         self.pages = self.__fill_pages()
         self.current_page = 0
+        with open("win.log", "a") as log:
+            print(f'{curses.COLS}, {self.longest_line_len}, {self.width}, {self.start_x}', file=log, flush=True)
         self.__create_window()
 
     def __fill_pages(self):
         pages = list()
         page_len_rows = self.height - 2
         text_pages_count = ceil(len(self.output_raw) / (self.height - 2))
         for i in range(0, text_pages_count):
             pages.append(self.output_raw[i * page_len_rows: i * page_len_rows + page_len_rows])
         return pages
 
     def __get_raw_output(self):
         raw_data = list()
-        max_len_available = curses.COLS - self.MARGIN_X * 2 - 2
+        max_len_available = curses.COLS - main_window.MARGINS_X - 4
         try:
             for line in f_input():
                 line_st = line.rstrip()
                 if (len(line_st) > max_len_available):
-                    raw_data.append(line_st[0:max_len_available])
-                    raw_data.append(line_st[max_len_available + 1: len(line_st)])
+                    for i in range(0, len(line_st) - 1, max_len_available):
+                        raw_data.append(line_st[i:i + max_len_available])
                     continue
                 raw_data.append(line_st)
         except FileNotFoundError:
             curses.endwin()
             print(f'File {argv[1]} not found')
             exit()
         if (len(raw_data) == 0):
             exit()
         return raw_data
 
     def __get_page_count(self):
         try:
             term_pages_count = trunc(
-                (curses.COLS - main_window.MARGIN_X / 2) / self.longes_line_len)
+                (curses.COLS - main_window.MARGINS_X / 2) / self.longest_line_len)
         except ZeroDivisionError:
             term_pages_count = 1
         text_pages_count = ceil(len(self.output_raw) / (self.height - 2))  # 2 - borders
+        if (term_pages_count <= 0):
+            term_pages_count = 1
         if (text_pages_count > term_pages_count):
             return term_pages_count
         return text_pages_count
 
     def __create_window(self):
         self.window = curses.newwin(self.height, self.width, self.start_y, self.start_x)
         self.window.bkgd(" ", curses.color_pair(2))
@@ -70,15 +75,15 @@
         self.window.border()
         cursor_y = 1
         cursor_x = 2
         for page in self.pages[self.current_page: self.current_page + self.page_count]:
             for line in page:
                 self.window.addstr(cursor_y, cursor_x, line)
                 cursor_y += 1
-            cursor_x += self.longes_line_len + 1
+            cursor_x += self.longest_line_len + 1
             cursor_y = 1
         self.window.refresh()
 
     def page_up(self):
         if (self.current_page == 0):
             return
         self.current_page -= self.page_count
```

### Comparing `curtxt-reader-1.0.0/curtxt_reader.egg-info/PKG-INFO` & `curtxt-reader-1.0.1/curtxt_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple ncurses-based plain text reader written
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -388,14 +388,15 @@
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Curses txt reader
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
+[![PyPI version](https://badge.fury.io/py/curtxt-reader.svg)](https://badge.fury.io/py/curtxt-reader)
 ## About
 A simple ncurses-based plain text reader written in python.  
 ## Instalation
 From PyPI:  
 	
     $ pip install curtxt-reader
```

### Comparing `curtxt-reader-1.0.0/pyproject.toml` & `curtxt-reader-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curtxt-reader"
-version = "1.0.0"
+version = "1.0.1"
 description = "A simple ncurses-based plain text reader written"
 readme = "README.md"
 authors = [{ name = "1256-bits" , email = "128bit@eclipso.eu" }]
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

