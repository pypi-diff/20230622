# Comparing `tmp/brunospackage-0.0.8.tar.gz` & `tmp/brunospackage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunospackage-0.0.8.tar", last modified: Fri Jun  2 08:19:43 2023, max compression
+gzip compressed data, was "brunospackage-0.0.9.tar", last modified: Thu Jun 22 02:53:30 2023, max compression
```

## Comparing `brunospackage-0.0.8.tar` & `brunospackage-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.443461 brunospackage-0.0.8/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 08:19:43.443338 brunospackage-0.0.8/PKG-INFO
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.442274 brunospackage-0.0.8/brunospackage/
--rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.8/brunospackage/__init__.py
--rw-r--r--   0 bdtacchi   (501) staff       (20)    16297 2023-06-02 08:18:13.000000 brunospackage-0.0.8/brunospackage/functions.py
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.443144 brunospackage-0.0.8/brunospackage.egg-info/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/PKG-INFO
--rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/SOURCES.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/dependency_links.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/requires.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/top_level.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 08:19:43.443511 brunospackage-0.0.8/setup.cfg
--rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-02 08:19:34.000000 brunospackage-0.0.8/setup.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-22 02:53:30.944971 brunospackage-0.0.9/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-22 02:53:30.944836 brunospackage-0.0.9/PKG-INFO
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-22 02:53:30.943412 brunospackage-0.0.9/brunospackage/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.9/brunospackage/__init__.py
+-rw-r--r--   0 bdtacchi   (501) staff       (20)    16535 2023-06-22 02:44:53.000000 brunospackage-0.0.9/brunospackage/functions.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-22 02:53:30.944623 brunospackage-0.0.9/brunospackage.egg-info/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-22 02:53:30.000000 brunospackage-0.0.9/brunospackage.egg-info/PKG-INFO
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-22 02:53:30.000000 brunospackage-0.0.9/brunospackage.egg-info/SOURCES.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-22 02:53:30.000000 brunospackage-0.0.9/brunospackage.egg-info/dependency_links.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-22 02:53:30.000000 brunospackage-0.0.9/brunospackage.egg-info/requires.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-22 02:53:30.000000 brunospackage-0.0.9/brunospackage.egg-info/top_level.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-22 02:53:30.945015 brunospackage-0.0.9/setup.cfg
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-22 02:47:53.000000 brunospackage-0.0.9/setup.py
```

### Comparing `brunospackage-0.0.8/PKG-INFO` & `brunospackage-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.8/brunospackage/functions.py` & `brunospackage-0.0.9/brunospackage/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
         # Check if df is not a list:
         self.isList = False
         self.has_changed_x = False
         if not isinstance(df, list):
             self.df1 = df
             self.time_column1 = time_column
             self.unit_pattern1 = self.UNIT_PATTERNS.get(unit_format, self.UNIT_PATTERNS['hyphen'])
-            self.columns1 = [col for col in df.columns if col != time_column]  # exclude time_column from columns to plot
+            self.columns1 = [col for col in df.columns if col != time_column]  
+            # exclude time_column from columns to plot
+            # Sort columns alphabetically
+            self.columns1.sort()
             self.current_column_index1 = 0
         else:
             self.isList = True
             # If list contains more than two dataframes, raise error
             if len(df) > 2:
                 raise ValueError("List of dataframes can only contain 2 dataframes")
             self.df1 = df[0]
@@ -44,15 +47,19 @@
                 self.unit_format2 = unit_format[1]
             else:
                 self.unit_format1 = unit_format
                 self.unit_format2 = unit_format
             self.unit_pattern1 = self.UNIT_PATTERNS.get(self.unit_format1, self.UNIT_PATTERNS['hyphen'])
             self.unit_pattern2 = self.UNIT_PATTERNS.get(self.unit_format2, self.UNIT_PATTERNS['hyphen'])
             self.columns1 = [col for col in self.df1.columns if col != self.time_column1]  # exclude time_column from columns to plot
+            # Sort columns alphabetically
+            self.columns1.sort()
             self.columns2 = [col for col in self.df2.columns if col != self.time_column2]  # exclude time_column from columns to plot
+            # Sort columns alphabetically
+            self.columns2.sort()
             self.current_column_index1 = 0
             self.current_column_index2 = 0
 
 
         self.root = tk.Tk()
         self.window_width = 900
         self.window_height = 800
```

### Comparing `brunospackage-0.0.8/brunospackage.egg-info/PKG-INFO` & `brunospackage-0.0.9/brunospackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.8/setup.py` & `brunospackage-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'Helper functions that I use often'
 LONG_DESCRIPTION = '''A package that allows me to import functions that I use often.'''
 # DataFramePlotter - given a dataframe with multiple variables, plots each variable against time in a tkinter window. Requires pandas, matplotlib, tkinter, and re. The usage is: 
 #     import brunospackage as bp
 #     plotter = bp.DataFramePlotter(df, nameOfTimeColumn, unit_format)
 #     plotter.run()'''
```

