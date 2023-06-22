# Comparing `tmp/citros-23.23.5.tar.gz` & `tmp/citros-23.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.23.5.tar", last modified: Thu Jun  8 17:27:49 2023, max compression
+gzip compressed data, was "citros-23.25.1.tar", last modified: Thu Jun 22 19:45:47 2023, max compression
```

## Comparing `citros-23.23.5.tar` & `citros-23.25.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.062560 citros-23.23.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 17:27:34.000000 citros-23.23.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 17:27:49.062560 citros-23.23.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 17:27:34.000000 citros-23.23.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.058560 citros-23.23.5/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-08 17:27:34.000000 citros-23.23.5/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.058560 citros-23.23.5/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 17:27:34.000000 citros-23.23.5/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 17:27:34.000000 citros-23.23.5/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.058560 citros-23.23.5/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 17:27:34.000000 citros-23.23.5/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-06-08 17:27:34.000000 citros-23.23.5/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.062560 citros-23.23.5/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 17:27:34.000000 citros-23.23.5/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 17:27:34.000000 citros-23.23.5/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 17:27:34.000000 citros-23.23.5/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.062560 citros-23.23.5/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 17:27:34.000000 citros-23.23.5/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 17:27:34.000000 citros-23.23.5/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 17:27:34.000000 citros-23.23.5/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.062560 citros-23.23.5/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 17:27:34.000000 citros-23.23.5/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 17:27:34.000000 citros-23.23.5/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 17:27:34.000000 citros-23.23.5/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 17:27:34.000000 citros-23.23.5/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.058560 citros-23.23.5/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 17:27:49.000000 citros-23.23.5/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 17:27:49.000000 citros-23.23.5/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:27:49.000000 citros-23.23.5/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 17:27:49.000000 citros-23.23.5/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 17:27:49.000000 citros-23.23.5/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 17:27:34.000000 citros-23.23.5/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 17:27:49.062560 citros-23.23.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 17:27:34.000000 citros-23.23.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:27:49.062560 citros-23.23.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 17:27:34.000000 citros-23.23.5/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 17:27:34.000000 citros-23.23.5/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 17:27:34.000000 citros-23.23.5/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 19:45:30.000000 citros-23.25.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 19:45:47.279244 citros-23.25.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 19:45:30.000000 citros-23.25.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.271244 citros-23.25.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-22 19:45:30.000000 citros-23.25.1/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 19:45:30.000000 citros-23.25.1/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 19:45:30.000000 citros-23.25.1/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 19:45:30.000000 citros-23.25.1/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-22 19:45:30.000000 citros-23.25.1/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 19:45:30.000000 citros-23.25.1/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-22 19:45:30.000000 citros-23.25.1/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-22 19:45:30.000000 citros-23.25.1/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.275244 citros-23.25.1/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 19:45:47.000000 citros-23.25.1/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 19:45:30.000000 citros-23.25.1/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:45:47.279244 citros-23.25.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 19:45:30.000000 citros-23.25.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:45:47.279244 citros-23.25.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 19:45:30.000000 citros-23.25.1/tests/test_parse_xml.py
```

### Comparing `citros-23.23.5/LICENSE` & `citros-23.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/PKG-INFO` & `citros-23.25.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.5
+Version: 23.25.1
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.5/README.md` & `citros-23.25.1/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/bin/citros` & `citros-23.25.1/bin/citros`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from decouple import config
 
 from InquirerPy import prompt
 from prompt_toolkit.validation import Validator, ValidationError
 
 from citros.launches import generate_launch_description  
 
-# in seconds
-DEFAULT_SIMULATION_TIMEOUT = 10*60
+
+DEFAULT_SIMULATION_TIMEOUT = 10*60  # in seconds
 
 
 class NumberValidator(Validator):
     """
     small helper class for validating user input during an interactive session.
     """
     def validate(self, document):
@@ -27,15 +27,15 @@
         except ValueError:
             raise ValidationError(message="Please enter a number",
                                   cursor_position=len(document.text))
 
 
 
 def print_citros():
-    print ("""
+    print (f"""
 ==============================================
  ██████╗██╗████████╗██████╗  ██████╗ ███████╗
 ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
 ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
 ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
 ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝
@@ -136,14 +136,17 @@
     :param args.key:
     :param args.completions:
     """
     print_citros()       
 
     sim_id, batch_id, run_id = args.simulation_id, args.batch_id, args.run_id
     remote, timeout, key, completions = args.remote, args.timeout, args.key, args.completions
+    
+    global DEBUG
+    DEBUG = args.debug
 
     with Citros() as citros:
         if key:
             loggedin = citros.authenticate_with_key(key)
             if not loggedin:
                 sys.exit("run.authenticate_with_key: please log in first!") 
         
@@ -214,32 +217,34 @@
             print (e)
             traceback.print_exc()
             print("------------------------")
             continue
     print(f" - Finished [{batch_run_id}] batch.")    
 
 
-def single_simulation_run(batch_id, sid, timeout):   
+def single_simulation_run(batch_id, run_id, timeout):   
     # running inside ROS workspace context.  
     from launch import LaunchService 
 
-    print(f" + + running simulation [{sid}]")  
+    print(f" + + running simulation [{run_id}]")  
     
     # create a new instance of citros so that a new logger will be created 
-    # and mapped according to batch_id, simulation_run_id. Very inelegant.
+    # and mapped according to batch_id and run_id. Very inelegant.
     # TODO: find a simple way to map the loggers without instantiating Citros. 
-    with Citros(batch_id, sid) as citros:
+    with Citros(batch_id, run_id) as citros:
         launch_description = generate_launch_description(citros, str(timeout))
+
         if launch_description is None:
-            sys.exit(f'Couldn\'t run sid:[{sid}]. Something went wrong, probably with connection to CITROS. ')    
-        #launch_service = LaunchService(debug=True)
-        launch_service = LaunchService()
+            sys.exit(f'Couldn\'t run run_id:[{run_id}]. Something went wrong,\
+                      probably with connection to CITROS. ')
+
+        launch_service = LaunchService(debug=DEBUG)
         launch_service.include_launch_description(launch_description)
         ret = launch_service.run()    
-        print(f" - - Finished simulation sid = [{sid}] with return code [{ret}].")    
+        print(f" - - Finished simulation run_id = [{run_id}] with return code [{ret}].")    
     
 
 def run_simulation_by_batch(citros : Citros, batch_id, run_id, timeout):
     # k8s indexed batch job is passing the index with JOB_COMPLETION_INDEX env variable.
     if run_id == "JOB_COMPLETION_INDEX":
         run_id = config("JOB_COMPLETION_INDEX", "bad-value-from-k8s")
         print(f"got JOB_COMPLETION_INDEX={run_id} from k8s.")
@@ -334,15 +339,15 @@
 \t Powered by Lulav Space
 
         ''',
         formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-V', "--version",
                         action="version",
-                        version="%(prog)s " + citros_version)
+                        version="CITROS " + citros_version)
     
     subparsers = parser.add_subparsers(title="commands", help="citros commands", dest='command', required=True)
 
     # -----------------------------------------
     build_parser = subparsers.add_parser("login", help="log in to citros")
     build_parser.add_argument("-username", default=None, help="username")
     build_parser.add_argument("-password", default=None, help="password")
@@ -381,14 +386,15 @@
     build_parser.add_argument("-s", "--simulation_id", nargs='?', default=None, help="Simulation id")
     build_parser.add_argument("-b", "--batch_id", nargs='?', default=None, help="Batch id")
     build_parser.add_argument("-i", "--run_id", nargs='?', default='', help="run id")
     build_parser.add_argument("-c", "--completions", nargs='?', default=1, help="number of times to run the simulation")
     build_parser.add_argument("-t", "--timeout", nargs='?', default=DEFAULT_SIMULATION_TIMEOUT, help="simulation timeout")
     build_parser.add_argument("-k", "--key", nargs='?', default=None, help="jwt key of the user")
     build_parser.add_argument("-r", "--remote", action='store_true', help="simulation timeout")
+    build_parser.add_argument("-d", "--debug", action='store_true', help="simulation timeout")
     build_parser.set_defaults(func=run)
      
     # experimental
     # -----------------------------------------
     build_parser = subparsers.add_parser("upload_bag", help="upload bag to citros")
     build_parser.add_argument("bag", help="bag file")
     build_parser.add_argument("batch_run_id", help="Batch run id")
```

### Comparing `citros-23.23.5/citros/__init__.py` & `citros-23.25.1/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros.py` & `citros-23.25.1/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_bag.py` & `citros-23.25.1/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_batch.py` & `citros-23.25.1/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_events.py` & `citros-23.25.1/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_integration.py` & `citros-23.25.1/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_params.py` & `citros-23.25.1/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/citros_utils.py` & `citros-23.25.1/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/launches/__init__.py` & `citros-23.25.1/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/launches/launch.py` & `citros-23.25.1/citros/launches/launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             PythonLaunchDescriptionSource([
                 os.path.join(get_package_share_directory(package["name"]), 'launch'), 
                 f"/{launch['name']}"
             ]),
             launch_arguments={}.items(),
         )
 
-        citros.log.info("Starting clients launch")
+        citros.log.info(f"Starting clients launch package:{package['name']} launch:{launch['name']}")
         citros.events.running(batch_run_id=batch_run_id, sid=simulation_run_id, tag="LAUNCH", message="Starting clients launch", metadata=None)
 
         return [
             client_launch
         ]
 
         # second option. add actions for nodes.
```

### Comparing `citros-23.23.5/citros/logger/__init__.py` & `citros-23.25.1/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/logger/logger.py` & `citros-23.25.1/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/logger/logger_pg_handler.py` & `citros-23.25.1/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/parsers/__init__.py` & `citros-23.25.1/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/parsers/parser_ros2.py` & `citros-23.25.1/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/rosbag/__init__.py` & `citros-23.25.1/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/rosbag/reader_base.py` & `citros-23.25.1/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/rosbag/reader_mcap.py` & `citros-23.25.1/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/citros/rosbag/reader_sqlite.py` & `citros-23.25.1/citros/rosbag/reader_sqlite.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 import sqlite3
 import json
 import os
 
 
 CHUNK_SIZE = 50 * 1024 * 1024
 
+# Issue with Postgrers, json object doesnt support infinity, -infinity or nan
+def remove_inf(o):
+    if o is None:
+        return "nan"
+    if isinstance(o, float): 
+        print(o, " ", type(o))
+        if o == float('inf'):
+            return "inf"
+        if o == -float('inf'):
+            return "-inf"
+        if o == float('nan'):
+            return "nan"
+        return o
+    
+    if isinstance(o, dict): 
+        return {
+            k: remove_inf(v) for k, v in o.items()
+        }
+        
+    if isinstance(o, (list, tuple)): 
+        return [remove_inf(x) for x in o]
+    
+    return o
+                
 ###############
 ##### PG ######
 ############### 
 class BagReaderSQL():
     def read_messages(self, input_bag, simulation_run_id):
         from rosidl_runtime_py.convert import get_message_slot_types, message_to_yaml, message_to_csv, message_to_ordereddict
         from rosidl_runtime_py.utilities import get_message
@@ -29,15 +53,19 @@
             if topic_name in ["/rosout", "/client_count", "/connected_clients"]:
                 continue
             rows = self.cursor.execute(f"select id, timestamp, data from messages where topic_id = {self.topics[topic_name]['id']}").fetchall()            
             rid = 0
             for id, timestamp, data in rows:
                 d_data = deserialize_message(data, self.topics[topic_name]["message"])
                 msg_dict = message_to_ordereddict(d_data)
-                json_data = json.dumps(msg_dict)
+                
+                # after = json.dumps(dict1, allow_nan=False) 
+                # will raise an arrer of json contains Infinity or Nan
+                json_data = json.dumps(remove_inf(msg_dict), allow_nan=False) 
+                # json_data = json.dumps(msg_dict)
                 
                 row = chr(0x1E).join([f"{simulation_run_id}", f"{rid}", f"{timestamp}", f"{topic_name}", f"{self.topics[topic_name]['type']}", json_data])
                 rid = rid + 1
                 bytes_wrote = buffer.write(row + '\n')
                 size = size + bytes_wrote
                 # 10MB chunks max
                 if size >= CHUNK_SIZE:
```

### Comparing `citros-23.23.5/citros.egg-info/PKG-INFO` & `citros-23.25.1/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.5
+Version: 23.25.1
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.5/citros.egg-info/SOURCES.txt` & `citros-23.25.1/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/setup.py` & `citros-23.25.1/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/tests/test_parse_makefile.py` & `citros-23.25.1/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/tests/test_parse_setup_py.py` & `citros-23.25.1/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.5/tests/test_parse_xml.py` & `citros-23.25.1/tests/test_parse_xml.py`

 * *Files identical despite different names*

