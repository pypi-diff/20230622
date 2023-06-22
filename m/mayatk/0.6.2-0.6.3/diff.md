# Comparing `tmp/mayatk-0.6.2.tar.gz` & `tmp/mayatk-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.6.2.tar", last modified: Thu Jun 22 16:15:03 2023, max compression
+gzip compressed data, was "mayatk-0.6.3.tar", last modified: Wed Mar 29 13:02:37 2023, max compression
```

## Comparing `mayatk-0.6.2.tar` & `mayatk-0.6.3.tar`

### file list

```diff
@@ -1,50 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.252503 mayatk-0.6.2/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.2/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1466 2023-06-22 16:15:03.251503 mayatk-0.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.127504 mayatk-0.6.2/mayatk/
--rw-rw-rw-   0        0        0     5702 2023-06-22 16:14:59.000000 mayatk-0.6.2/mayatk/__init__.py
--rw-rw-rw-   0        0        0     8075 2023-06-05 16:23:13.000000 mayatk-0.6.2/mayatk/cam_utils.py
--rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.2/mayatk/cam_utils.py.bak
--rw-rw-rw-   0        0        0    65402 2023-06-14 17:05:48.000000 mayatk-0.6.2/mayatk/cmpt_utils.py
--rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.2/mayatk/cmpt_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.168504 mayatk-0.6.2/mayatk/display_utils/
--rw-rw-rw-   0        0        0      428 2023-04-16 16:33:47.000000 mayatk-0.6.2/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     7433 2023-06-13 02:25:19.000000 mayatk-0.6.2/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0    30776 2023-05-30 18:39:58.000000 mayatk-0.6.2/mayatk/edit_utils.py
--rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.2/mayatk/macro_utils.py
--rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.2/mayatk/mash_utils.py
--rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.2/mayatk/mash_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.188502 mayatk-0.6.2/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      367 2023-04-16 16:33:48.000000 mayatk-0.6.2/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0     9122 2023-06-12 14:32:54.000000 mayatk-0.6.2/mayatk/mat_utils/mat_utils.py
--rw-rw-rw-   0        0        0    19177 2023-06-20 19:06:12.000000 mayatk-0.6.2/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    15233 2023-06-17 12:48:05.000000 mayatk-0.6.2/mayatk/misc_utils.py
--rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.2/mayatk/misc_utils.py.bak
--rw-rw-rw-   0        0        0    29580 2023-06-22 00:27:45.000000 mayatk-0.6.2/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    13413 2023-06-16 01:20:55.000000 mayatk-0.6.2/mayatk/project_utils.py
--rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.2/mayatk/project_utils.py.bak
--rw-rw-rw-   0        0        0    20346 2023-06-06 18:19:16.000000 mayatk-0.6.2/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.2/mayatk/rig_utils.py.bak
--rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.2/mayatk/script_utils.py
--rw-rw-rw-   0        0        0    32313 2023-06-06 18:19:16.000000 mayatk-0.6.2/mayatk/xform_utils.py
--rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.2/mayatk/xform_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.156534 mayatk-0.6.2/mayatk.egg-info/
--rw-rw-rw-   0        0        0     1466 2023-06-22 16:15:02.000000 mayatk-0.6.2/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.2/mayatk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1016 2023-06-22 16:15:02.000000 mayatk-0.6.2/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.2/mayatk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-22 16:15:02.000000 mayatk-0.6.2/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 16:15:02.000000 mayatk-0.6.2/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 16:15:03.252503 mayatk-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-06 18:19:16.000000 mayatk-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:15:03.250504 mayatk-0.6.2/test/
--rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.2/test/__init__.py
--rw-rw-rw-   0        0        0    26011 2023-06-14 17:56:40.000000 mayatk-0.6.2/test/cmpt_utils_test.py
--rw-rw-rw-   0        0        0     7670 2023-05-20 15:49:30.000000 mayatk-0.6.2/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     4485 2023-06-11 12:52:05.000000 mayatk-0.6.2/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     7863 2023-06-17 12:29:32.000000 mayatk-0.6.2/test/misc_utils_test.py
--rw-rw-rw-   0        0        0     8241 2023-06-14 16:56:33.000000 mayatk-0.6.2/test/node_utils_test.py
--rw-rw-rw-   0        0        0     5080 2023-05-20 16:17:57.000000 mayatk-0.6.2/test/rig_utils_test.py
--rw-rw-rw-   0        0        0     3406 2023-06-14 17:14:08.000000 mayatk-0.6.2/test/run_tests.py
--rw-rw-rw-   0        0        0     7292 2023-05-20 17:08:16.000000 mayatk-0.6.2/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-03-29 13:02:37.777938 mayatk-0.6.3/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1156 2023-03-29 13:02:37.776938 mayatk-0.6.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-29 13:02:37.703619 mayatk-0.6.3/mayatk/
+-rw-rw-rw-   0        0        0    36893 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Cmpt.py
+-rw-rw-rw-   0        0        0    16375 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Core.py
+-rw-rw-rw-   0        0        0    24525 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Edit.py
+-rw-rw-rw-   0        0        0    20518 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Macro.py
+-rw-rw-rw-   0        0        0    11798 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Mash.py
+-rw-rw-rw-   0        0        0    18112 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Node.py
+-rw-rw-rw-   0        0        0    16410 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Rig.py
+-rw-rw-rw-   0        0        0     7721 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Script.py
+-rw-rw-rw-   0        0        0    26279 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/Xform.py
+-rw-rw-rw-   0        0        0     1730 2023-03-29 13:02:32.000000 mayatk-0.6.3/mayatk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 13:02:37.729610 mayatk-0.6.3/mayatk/shadertk/
+-rw-rw-rw-   0        0        0      697 2023-03-28 23:39:14.000000 mayatk-0.6.3/mayatk/shadertk/__init__.py
+-rw-rw-rw-   0        0        0    15042 2023-03-28 23:39:16.000000 mayatk-0.6.3/mayatk/shadertk/stingray_arnold_shader.py
+drwxrwxrwx   0        0        0        0 2023-03-29 13:02:37.719610 mayatk-0.6.3/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-03-29 13:02:37.000000 mayatk-0.6.3/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.3/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-29 13:02:37.000000 mayatk-0.6.3/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-03-29 13:02:37.000000 mayatk-0.6.3/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-29 13:02:37.777938 mayatk-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2131 2023-03-28 23:39:16.000000 mayatk-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-29 13:02:37.775918 mayatk-0.6.3/test/
+-rw-rw-rw-   0        0        0     5655 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/Node_test.py
+-rw-rw-rw-   0        0        0      989 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/__init__.py
+-rw-rw-rw-   0        0        0     9786 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/cmpt_test.py
+-rw-rw-rw-   0        0        0     6162 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/core_test.py
+-rw-rw-rw-   0        0        0     4697 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/edit_test.py
+-rw-rw-rw-   0        0        0     3109 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/rig_test.py
+-rw-rw-rw-   0        0        0     3072 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/run_tests.py
+-rw-rw-rw-   0        0        0     4641 2023-03-28 23:39:16.000000 mayatk-0.6.3/test/xform_test.py
```

### Comparing `mayatk-0.6.2/LICENSE` & `mayatk-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.2/mayatk.egg-info/PKG-INFO.bak` & `mayatk-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 ```
 
 ### Example use-case:
 ###### Import the class `Node` from the package.
 ###### As the name suggests, the class `Node` holds the package's node related functions.
 ```python
 from mayatk import Node
-Node.is_locator(<obj>)
+Node.isLocator(<obj>)
 ```
 ###### You can also import a function directly.
 ```python
 from mayatk.Node import isGroup
 isGroup(<obj>)
 ```
```

### Comparing `mayatk-0.6.2/mayatk.egg-info/SOURCES.txt.bak` & `mayatk-0.6.3/mayatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.2/test/__init__.py` & `mayatk-0.6.3/test/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,42 +2,40 @@
 # coding=utf-8
 import os, sys
 import unittest
 import inspect
 
 
 class Main(unittest.TestCase):
-    """ """
+	'''
+	'''
+	def perform_test(self, case):
+		'''
+		'''
+		for expression, expected_result in case.items():
+			m = str(expression).split('(')[0] #ie. 'self.setCase' from "self.setCase('xxx', 'upper')"
+
+			try:
+				path = os.path.abspath(inspect.getfile(eval(m)))
+			except TypeError as error:
+				path = ''
+
+			result = eval(expression)
+			self.assertEqual(
+				result, 
+				expected_result, 
+				"\n\nError: {}\n  Call:     {}\n  Expected: {} {}\n  Returned: {} {}".format(path, expression.replace('self.', '', 1), type(expected_result), expected_result, type(result), result)
+			)
+
+# -----------------------------------------------------------------------------
+
+
+
+
 
-    def perform_test(self, case):
-        """ """
-        for expression, expected_result in case.items():
-            m = str(expression).split("(")[
-                0
-            ]  # ie. 'self.set_case' from "self.set_case('xxx', 'upper')"
-
-            try:
-                path = os.path.abspath(inspect.getfile(eval(m)))
-            except TypeError as error:
-                path = ""
-
-            result = eval(expression)
-            self.assertEqual(
-                result,
-                expected_result,
-                "\n\nError: {}\n  Call:     {}\n  Expected: {} {}\n  Returned: {} {}".format(
-                    path,
-                    expression.replace("self.", "", 1),
-                    type(expected_result),
-                    expected_result,
-                    type(result),
-                    result,
-                ),
-            )
 
 
-# -----------------------------------------------------------------------------
 
 
 # -----------------------------------------------------------------------------
 # Notes
-# -----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
```

### Comparing `mayatk-0.6.2/test/run_tests.py` & `mayatk-0.6.3/test/run_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 # !/usr/bin/python
 # coding=utf-8
 import importlib
 
 
 def run_test_cases(test_module):
-    """Runs all test cases within a test module.
+	"""Runs all test cases within a test module.
 
-    Parameters:
-            test_module (str)(module): A module object or a string representing the module name.
+	Parameters:
+		test_module (str)(module): A module object or a string representing the module name.
 
-    """
-    if isinstance(test_module, str):
-        test_module = importlib.import_module(test_module)
-
-    for _, obj in test_module.__dict__.items():
-        if isinstance(obj, type) and obj.__module__ == test_module.__name__:
-            obj = obj()
-            for method_name in dir(obj):
-                if method_name.startswith("test_"):
-                    test_case = getattr(obj, method_name)
-                    test_case()
+	"""
+	if isinstance(test_module, str):
+		test_module = importlib.import_module(test_module)
+		
+	for name, obj in test_module.__dict__.items():
+		if isinstance(obj, type) and obj.__module__ == test_module.__name__:
+			obj = obj()
+			for method_name in dir(obj):
+				if method_name.startswith("test_"):
+					test_case = getattr(obj, method_name)
+					test_case()
 
 
 def run_tests(module_names):
-    """Reloads the non-test and test modules and runs the test cases within the test modules.
+	"""Reloads the non-test and test modules and runs the test cases within the test modules.
 
-    Parameters:
-            module_names (list): A list of strings representing the names of the non-test modules.
-
-    """
-    for module_name in module_names:
-        module = __import__(f"mayatk.{module_name}", fromlist=[module_name])
-        test_module = __import__(
-            f"test.{module_name}_test", fromlist=[f"{module_name}_test"]
-        )
-        importlib.reload(module)
-        importlib.reload(test_module)
-        msg_start = f"-> Starting tests for {module_name} .."
-        print(f"{'-'*len(msg_start)}\n{msg_start}")
-        run_test_cases(test_module)
-        print(f"<- {module_name} tests completed.\n{'-'*len(msg_start)}")
+	Parameters:
+		module_names (list): A list of strings representing the names of the non-test modules.
 
+	"""
+	for module_name in module_names:
+		module = __import__(f"mayatk.{module_name}", fromlist=[module_name])
+		test_module = __import__(f"test.{module_name}_test", fromlist=[f"{module_name}_test"])
+		importlib.reload(module)
+		importlib.reload(test_module)
+		msg_start = f'-> Starting tests for {module_name} ..'
+		print (f"{'-'*len(msg_start)}\n{msg_start}")
+		run_test_cases(test_module)
+		print (f"<- {module_name} tests completed.\n{'-'*len(msg_start)}")
 
 # --------------------------------------------------------------------------------------------
 
-if __name__ == "__main__":
-    run_tests(
-        [
-            "misc_utils",
-            "node_utils",
-            "cmpt_utils",
-            "edit_utils",
-            "xform_utils",
-            "rig_utils",
-            "mat_utils",
-        ]
-    )
+if __name__=='__main__':
+
+	run_tests([
+		'Core',
+		'Node',
+		'Cmpt',
+		'Edit',
+		'Xform',
+		'Rig',
+	])
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 
+
 # --------------------------------------------------------------------------------------------
 # deprecated:
 # --------------------------------------------------------------------------------------------
 
-# from mayatk import Misc; from test import core_test; importlib.reload(Misc); importlib.reload(core_test); run_tests(core_test)
+# from mayatk import Core; from test import core_test; importlib.reload(Core); importlib.reload(core_test); run_tests(core_test)
 # from mayatk import Node; from test import node_test; importlib.reload(Node); importlib.reload(node_test); run_tests(node_test)
 # from mayatk import Cmpt; from test import cmpt_test; importlib.reload(Cmpt); importlib.reload(cmpt_test); run_tests(cmpt_test)
 # from mayatk import Edit; from test import edit_test; importlib.reload(Edit); importlib.reload(edit_test); run_tests(edit_test)
 # from mayatk import Xform; from test import xform_test; importlib.reload(Xform); importlib.reload(xform_test); run_tests(xform_test)
 # from mayatk import Rig; from test import rig_test; importlib.reload(Rig); importlib.reload(rig_test); run_tests(rig_test)
 
 # from test import core_test;  core_test.unittest.main(exit=False)
 # from test import edit_test;  edit_test.unittest.main(exit=False)
 # from test import cmpt_test;  cmpt_test.unittest.main(exit=False)
 # from test import rig_test;   rig_test.unittest.main(exit=False)
-# from test import xform_test; xform_test.unittest.main(exit=False)
+# from test import xform_test; xform_test.unittest.main(exit=False)
```

