# Comparing `tmp/lest-0.3.0.tar.gz` & `tmp/lest-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lest-0.3.0.tar", last modified: Wed Apr 12 07:24:13 2023, max compression
+gzip compressed data, was "lest-0.4.0.tar", last modified: Thu Jun 22 08:56:12 2023, max compression
```

## Comparing `lest-0.3.0.tar` & `lest-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.557674 lest-0.3.0/
--rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1143 2023-04-12 07:24:13.556673 lest-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      640 2023-04-12 06:56:59.000000 lest-0.3.0/README.md
--rw-rw-rw-   0        0        0      493 2023-04-12 07:20:31.000000 lest-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:24:13.557674 lest-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.521158 lest-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.548670 lest-0.3.0/src/lest/
--rw-rw-rw-   0        0        0      371 2023-04-12 06:57:45.000000 lest-0.3.0/src/lest/__init__.py
--rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.3.0/src/lest/assertions.py
--rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.3.0/src/lest/registerer.py
--rw-rw-rw-   0        0        0     2128 2023-04-11 08:52:17.000000 lest-0.3.0/src/lest/runner.py
--rw-rw-rw-   0        0        0      184 2023-04-11 08:52:17.000000 lest-0.3.0/src/lest/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.554673 lest-0.3.0/src/lest.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.390659 lest-0.4.0/
+-rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1198 2023-06-22 08:56:12.389657 lest-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-06-22 08:48:11.000000 lest-0.4.0/README.md
+-rw-rw-rw-   0        0        0      493 2023-06-22 08:54:20.000000 lest-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:56:12.390659 lest-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.300639 lest-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.367655 lest-0.4.0/src/lest/
+-rw-rw-rw-   0        0        0      446 2023-06-22 08:44:53.000000 lest-0.4.0/src/lest/__init__.py
+-rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.4.0/src/lest/assertions.py
+-rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.4.0/src/lest/registerer.py
+-rw-rw-rw-   0        0        0     2160 2023-06-22 08:50:50.000000 lest-0.4.0/src/lest/runner.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 08:40:08.000000 lest-0.4.0/src/lest/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.384658 lest-0.4.0/src/lest.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/top_level.txt
```

### Comparing `lest-0.3.0/LICENSE` & `lest-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lest-0.3.0/PKG-INFO` & `lest-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.3.0
+Version: 0.4.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -56,8 +56,8 @@
 
 
 run()
 ```
 
 Output (to visible the highlighting, it's a print-screen):
 
-![](result.png)
+![](https://raw.githubusercontent.com/wchistow/lest/master/result.png)
```

### Comparing `lest-0.3.0/README.md` & `lest-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 
 run()
 ```
 
 Output (to visible the highlighting, it's a print-screen):
 
-![](result.png)
+![](https://raw.githubusercontent.com/wchistow/lest/master/result.png)
```

### Comparing `lest-0.3.0/src/lest/assertions.py` & `lest-0.4.0/src/lest/assertions.py`

 * *Files identical despite different names*

### Comparing `lest-0.3.0/src/lest/runner.py` & `lest-0.4.0/src/lest/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.elapsed = 0
         self.errors = 0
 
     def run(self, funcs: list[Callable], setup: Callable | None = None) -> None:
         if setup is None:
             setup = lambda: ...  # Empty function.
         for func in funcs:
-            print(f'Running [{func.__name__}]... ', end='')
+            print(f'Running [{func.__module__}.{func.__name__}]... ', end='')
             start = perf_counter()
             setup()
             try:
                 func()
             except AssertionError:
                 self.elapsed += perf_counter() - start
                 self.console.print('[red]FAILED:[/red]')
@@ -45,14 +45,14 @@
 
         result_table.add_column('Total tests', style='blue')
         result_table.add_column('Successful', style='green')
         result_table.add_column('Failed', style='red')
         result_table.add_column('Errors', style='red')
         result_table.add_column('Time elapsed', style='white')
 
-        result_table.add_row(str(self.successful + self.failed),
+        result_table.add_row(str(self.successful + self.failed + self.errors),
                              str(self.successful),
                              str(self.failed),
                              str(self.errors),
                              '{:5.3f}'.format(self.elapsed))
 
         self.console.print(result_table)
```

### Comparing `lest-0.3.0/src/lest.egg-info/PKG-INFO` & `lest-0.4.0/src/lest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.3.0
+Version: 0.4.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -56,8 +56,8 @@
 
 
 run()
 ```
 
 Output (to visible the highlighting, it's a print-screen):
 
-![](result.png)
+![](https://raw.githubusercontent.com/wchistow/lest/master/result.png)
```

