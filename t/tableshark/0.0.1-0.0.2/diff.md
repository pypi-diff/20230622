# Comparing `tmp/tableshark-0.0.1.tar.gz` & `tmp/tableshark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableshark-0.0.1.tar", last modified: Thu Jun 22 09:43:47 2023, max compression
+gzip compressed data, was "tableshark-0.0.2.tar", last modified: Thu Jun 22 10:03:47 2023, max compression
```

## Comparing `tableshark-0.0.1.tar` & `tableshark-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:47.472184 tableshark-0.0.1/
--rw-rw-rw-   0        0        0     1075 2023-06-22 09:43:46.000000 tableshark-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    20423 2023-06-22 09:43:47.472184 tableshark-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    20172 2023-06-22 09:28:35.000000 tableshark-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 09:43:47.472184 tableshark-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      524 2023-06-22 09:36:47.000000 tableshark-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:47.460421 tableshark-0.0.1/tableshark/
--rw-rw-rw-   0        0        0      146 2023-06-22 08:28:50.000000 tableshark-0.0.1/tableshark/__init__.py
--rw-rw-rw-   0        0        0    37273 2023-06-22 06:27:30.000000 tableshark-0.0.1/tableshark/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:47.462420 tableshark-0.0.1/tableshark.egg-info/
--rw-rw-rw-   0        0        0    20423 2023-06-22 09:43:47.000000 tableshark-0.0.1/tableshark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-22 09:43:47.000000 tableshark-0.0.1/tableshark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 09:43:47.000000 tableshark-0.0.1/tableshark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-22 09:43:47.000000 tableshark-0.0.1/tableshark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 09:43:47.000000 tableshark-0.0.1/tableshark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 10:03:47.499298 tableshark-0.0.2/
+-rw-rw-rw-   0        0        0     1075 2023-06-22 09:43:46.000000 tableshark-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    21486 2023-06-22 10:03:47.499298 tableshark-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    21235 2023-06-22 09:48:06.000000 tableshark-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 10:03:47.500297 tableshark-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      524 2023-06-22 09:49:54.000000 tableshark-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:03:47.497298 tableshark-0.0.2/tableshark/
+-rw-rw-rw-   0        0        0      146 2023-06-22 08:28:50.000000 tableshark-0.0.2/tableshark/__init__.py
+-rw-rw-rw-   0        0        0    37273 2023-06-22 06:27:30.000000 tableshark-0.0.2/tableshark/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:03:47.498298 tableshark-0.0.2/tableshark.egg-info/
+-rw-rw-rw-   0        0        0    21486 2023-06-22 10:03:47.000000 tableshark-0.0.2/tableshark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-06-22 10:03:47.000000 tableshark-0.0.2/tableshark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:03:47.000000 tableshark-0.0.2/tableshark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-22 10:03:47.000000 tableshark-0.0.2/tableshark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 10:03:47.000000 tableshark-0.0.2/tableshark.egg-info/top_level.txt
```

### Comparing `tableshark-0.0.1/LICENSE` & `tableshark-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tableshark-0.0.1/PKG-INFO` & `tableshark-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 Metadata-Version: 2.1
 Name: tableshark
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple table management tool
 Author: vladimirkirdan
 Author-email: vladimir.kirdan@bk.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# TableShark
+TableShark is a Python library for working with tables. It provides functionality for parsing, storing, and manipulating
+tables in various formats. It also provides a convenient way to handle table headers and cells.
+
+## Installation
+You can install TableShark using `pip`:
+```shell
+pip install tableshark
+```
+TableShark is a lightweight Python library that simplifies working with tabular data. It provides intuitive classes 
+and functions for creating, manipulating, and analyzing tables. With TableLib, you can easily import tables 
+from various data sources such as lists, pandas DataFrames, Excel files, CSV files, JSON files, and SQL databases.
+You can perform common table operations like adding rows and columns, merging tables, filtering data, and sorting.
+The library also offers seamless conversion between tables and popular formats like pandas DataFrames, Excel files,
+and CSV files. TableShark's user-friendly API and comprehensive documentation make it a valuable tool for anyone working
+with tabular data in Python.
+
 ## TableError
 `TableError` is a custom exception class defined in this Python library. It is derived from the built-in Exception
 class, allowing you to raise and handle specific errors related to table operations.
 
 ### Usage
 You can use `TableError` to handle exceptional scenarios that may occur during table processing or manipulation.
 It provides a straightforward way to identify and handle errors specific to table operations within your codebase.
```

### Comparing `tableshark-0.0.1/README.md` & `tableshark-0.0.2/tableshark.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: tableshark
+Version: 0.0.2
+Summary: A simple table management tool
+Author: vladimirkirdan
+Author-email: vladimir.kirdan@bk.ru
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# TableShark
+TableShark is a Python library for working with tables. It provides functionality for parsing, storing, and manipulating
+tables in various formats. It also provides a convenient way to handle table headers and cells.
+
+## Installation
+You can install TableShark using `pip`:
+```shell
+pip install tableshark
+```
+TableShark is a lightweight Python library that simplifies working with tabular data. It provides intuitive classes 
+and functions for creating, manipulating, and analyzing tables. With TableLib, you can easily import tables 
+from various data sources such as lists, pandas DataFrames, Excel files, CSV files, JSON files, and SQL databases.
+You can perform common table operations like adding rows and columns, merging tables, filtering data, and sorting.
+The library also offers seamless conversion between tables and popular formats like pandas DataFrames, Excel files,
+and CSV files. TableShark's user-friendly API and comprehensive documentation make it a valuable tool for anyone working
+with tabular data in Python.
+
 ## TableError
 `TableError` is a custom exception class defined in this Python library. It is derived from the built-in Exception
 class, allowing you to raise and handle specific errors related to table operations.
 
 ### Usage
 You can use `TableError` to handle exceptional scenarios that may occur during table processing or manipulation.
 It provides a straightforward way to identify and handle errors specific to table operations within your codebase.
@@ -498,8 +525,8 @@
 
 * `__str__()`: Returns a string representation of the schema.
 * `__repr__()`: Returns a string representation that can be used to recreate the schema.
 ### Conclusion
 The `Schema` class allows you to organize and work with a collection of tables. It provides methods to create a 
 schema from various sources such as Excel files, CSV files, SQL databases, and JSON files. You can iterate over
 the tables, add new tables, and access specific tables within the schema. Use the `Schema` class to manage and 
-manipulate multiple tables efficiently in your projects.
+manipulate multiple tables efficiently in your projects.
```

### Comparing `tableshark-0.0.1/setup.py` & `tableshark-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='tableshark',
-      version='0.0.1',
+      version='0.0.2',
       description='A simple table management tool',
       long_description=readme(),
       long_description_content_type='text/markdown',
       author_email='vladimir.kirdan@bk.ru',
       author='vladimirkirdan',
       install_requires=['pandas>=2.0.2', 'openpyxl>=3.0.7'],
       packages=find_packages(),
```

### Comparing `tableshark-0.0.1/tableshark/main.py` & `tableshark-0.0.2/tableshark/main.py`

 * *Files identical despite different names*

### Comparing `tableshark-0.0.1/tableshark.egg-info/PKG-INFO` & `tableshark-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-Metadata-Version: 2.1
-Name: tableshark
-Version: 0.0.1
-Summary: A simple table management tool
-Author: vladimirkirdan
-Author-email: vladimir.kirdan@bk.ru
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# TableShark
+TableShark is a Python library for working with tables. It provides functionality for parsing, storing, and manipulating
+tables in various formats. It also provides a convenient way to handle table headers and cells.
+
+## Installation
+You can install TableShark using `pip`:
+```shell
+pip install tableshark
+```
+TableShark is a lightweight Python library that simplifies working with tabular data. It provides intuitive classes 
+and functions for creating, manipulating, and analyzing tables. With TableLib, you can easily import tables 
+from various data sources such as lists, pandas DataFrames, Excel files, CSV files, JSON files, and SQL databases.
+You can perform common table operations like adding rows and columns, merging tables, filtering data, and sorting.
+The library also offers seamless conversion between tables and popular formats like pandas DataFrames, Excel files,
+and CSV files. TableShark's user-friendly API and comprehensive documentation make it a valuable tool for anyone working
+with tabular data in Python.
 
 ## TableError
 `TableError` is a custom exception class defined in this Python library. It is derived from the built-in Exception
 class, allowing you to raise and handle specific errors related to table operations.
 
 ### Usage
 You can use `TableError` to handle exceptional scenarios that may occur during table processing or manipulation.
@@ -508,8 +515,8 @@
 
 * `__str__()`: Returns a string representation of the schema.
 * `__repr__()`: Returns a string representation that can be used to recreate the schema.
 ### Conclusion
 The `Schema` class allows you to organize and work with a collection of tables. It provides methods to create a 
 schema from various sources such as Excel files, CSV files, SQL databases, and JSON files. You can iterate over
 the tables, add new tables, and access specific tables within the schema. Use the `Schema` class to manage and 
-manipulate multiple tables efficiently in your projects.
+manipulate multiple tables efficiently in your projects.
```

