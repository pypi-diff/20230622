# Comparing `tmp/curtxt-reader-1.0.1.tar.gz` & `tmp/curtxt-reader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtxt-reader-1.0.1.tar", last modified: Thu Jun 22 14:00:37 2023, max compression
+gzip compressed data, was "curtxt-reader-1.0.2.tar", last modified: Thu Jun 22 14:20:13 2023, max compression
```

## Comparing `curtxt-reader-1.0.1.tar` & `curtxt-reader-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/
--rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.0.1/LICENSE
--rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      895 2023-06-22 10:38:24.000000 curtxt-reader-1.0.1/README.md
--rwxr-xr-x   0 iris      (1000) iris      (1000)     5953 2023-06-22 13:58:57.000000 curtxt-reader-1.0.1/curtxt.py
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:00:37.752799 curtxt-reader-1.0.1/curtxt_reader.egg-info/
--rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/SOURCES.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/dependency_links.txt
--rw-r--r--   0 iris      (1000) iris      (1000)       48 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/entry_points.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-06-22 14:00:37.000000 curtxt-reader-1.0.1/curtxt_reader.egg-info/top_level.txt
--rw-r--r--   0 iris      (1000) iris      (1000)      906 2023-06-22 14:00:20.000000 curtxt-reader-1.0.1/pyproject.toml
--rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-06-22 14:00:37.756132 curtxt-reader-1.0.1/setup.cfg
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:20:13.132813 curtxt-reader-1.0.2/
+-rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.0.2/LICENSE
+-rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:20:13.129480 curtxt-reader-1.0.2/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      895 2023-06-22 10:38:24.000000 curtxt-reader-1.0.2/README.md
+-rwxr-xr-x   0 iris      (1000) iris      (1000)     5794 2023-06-22 14:18:10.000000 curtxt-reader-1.0.2/curtxt.py
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-06-22 14:20:13.129480 curtxt-reader-1.0.2/curtxt_reader.egg-info/
+-rw-r--r--   0 iris      (1000) iris      (1000)    21349 2023-06-22 14:20:13.000000 curtxt-reader-1.0.2/curtxt_reader.egg-info/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-06-22 14:20:13.000000 curtxt-reader-1.0.2/curtxt_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-06-22 14:20:13.000000 curtxt-reader-1.0.2/curtxt_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)       48 2023-06-22 14:20:13.000000 curtxt-reader-1.0.2/curtxt_reader.egg-info/entry_points.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-06-22 14:20:13.000000 curtxt-reader-1.0.2/curtxt_reader.egg-info/top_level.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)      906 2023-06-22 14:19:35.000000 curtxt-reader-1.0.2/pyproject.toml
+-rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-06-22 14:20:13.132813 curtxt-reader-1.0.2/setup.cfg
```

### Comparing `curtxt-reader-1.0.1/LICENSE` & `curtxt-reader-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.0.1/PKG-INFO` & `curtxt-reader-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple ncurses-based plain text reader written
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `curtxt-reader-1.0.1/README.md` & `curtxt-reader-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.0.1/curtxt.py` & `curtxt-reader-1.0.2/curtxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
         self.longest_line_len = len(max(self.output_raw, key=len)) or 80
         self.page_count = self.__get_page_count()
         self.width = (self.longest_line_len + 1) * self.page_count + 3
         self.start_x = trunc((curses.COLS - self.longest_line_len * self.page_count - 4) / 2)
         self.start_y = trunc(main_window.MARGINS_Y / 2)
         self.pages = self.__fill_pages()
         self.current_page = 0
-        with open("win.log", "a") as log:
-            print(f'{curses.COLS}, {self.longest_line_len}, {self.width}, {self.start_x}', file=log, flush=True)
         self.__create_window()
 
     def __fill_pages(self):
         pages = list()
         page_len_rows = self.height - 2
         text_pages_count = ceil(len(self.output_raw) / (self.height - 2))
         for i in range(0, text_pages_count):
@@ -116,17 +114,17 @@
 
     def __create_window(self):
         self.window = curses.newwin(self.height, self.width, self.start_y, self.start_x)
         self.window.bkgd(" ", curses.color_pair(2))
         self.__draw_window_content()
 
     def __draw_window_content(self):
+        self.window.deleteln()
         if (not self.bar_visible):
             self.window.bkgd(" ", curses.color_pair(1))
-            self.window.deleteln()
             self.window.refresh()
             return
         progress_str = f'{ceil(self.current_page / self.page_count * 100)}% [{self.current_page}/{self.page_count}]'
         self.window.bkgd(" ", curses.color_pair(2))
         self.window.addstr(0, 1, self.filename)
         self.window.addstr(0, self.width - len(progress_str) - 1, progress_str)
         self.window.refresh()
```

### Comparing `curtxt-reader-1.0.1/curtxt_reader.egg-info/PKG-INFO` & `curtxt-reader-1.0.2/curtxt_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple ncurses-based plain text reader written
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `curtxt-reader-1.0.1/pyproject.toml` & `curtxt-reader-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curtxt-reader"
-version = "1.0.1"
+version = "1.0.2"
 description = "A simple ncurses-based plain text reader written"
 readme = "README.md"
 authors = [{ name = "1256-bits" , email = "128bit@eclipso.eu" }]
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

