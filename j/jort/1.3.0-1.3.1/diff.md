# Comparing `tmp/jort-1.3.0.tar.gz` & `tmp/jort-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jort-1.3.0.tar", last modified: Thu Jun 22 00:09:26 2023, max compression
+gzip compressed data, was "jort-1.3.1.tar", last modified: Thu Jun 22 05:54:06 2023, max compression
```

## Comparing `jort-1.3.0.tar` & `jort-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.353326 jort-1.3.0/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.3.0/LICENSE
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3433 2023-06-22 00:09:26.353326 jort-1.3.0/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2978 2023-06-22 00:03:27.000000 jort-1.3.0/README.md
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.345326 jort-1.3.0/jort/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      331 2023-06-21 20:57:53.000000 jort-1.3.0/jort/__init__.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1372 2023-06-20 18:11:13.000000 jort-1.3.0/jort/_config.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       21 2023-06-21 20:42:19.000000 jort-1.3.0/jort/_version.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3112 2023-05-27 04:28:06.000000 jort-1.3.0/jort/checkpoint.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1378 2023-05-27 04:28:06.000000 jort-1.3.0/jort/datetime_utils.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.3.0/jort/exceptions.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11030 2023-06-21 23:56:32.000000 jort-1.3.0/jort/jort_exe.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     9259 2023-06-21 20:57:40.000000 jort-1.3.0/jort/reporting_callbacks.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     7663 2023-06-21 23:49:04.000000 jort-1.3.0/jort/track_cli.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    10733 2023-06-21 23:39:56.000000 jort-1.3.0/jort/tracker.py
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.349326 jort-1.3.0/jort.egg-info/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3433 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      386 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/SOURCES.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/dependency_links.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       43 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/entry_points.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      153 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/requires.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/top_level.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-06-22 00:09:26.353326 jort-1.3.0/setup.cfg
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      967 2023-06-21 20:45:06.000000 jort-1.3.0/setup.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.747008 jort-1.3.1/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.3.1/LICENSE
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4280 2023-06-22 05:54:06.747008 jort-1.3.1/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3825 2023-06-22 05:52:26.000000 jort-1.3.1/README.md
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.739008 jort-1.3.1/jort/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      331 2023-06-22 00:12:17.000000 jort-1.3.1/jort/__init__.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1372 2023-06-22 00:12:17.000000 jort-1.3.1/jort/_config.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       21 2023-06-22 05:53:07.000000 jort-1.3.1/jort/_version.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3112 2023-05-27 04:28:06.000000 jort-1.3.1/jort/checkpoint.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1378 2023-05-27 04:28:06.000000 jort-1.3.1/jort/datetime_utils.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.3.1/jort/exceptions.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11030 2023-06-22 00:12:17.000000 jort-1.3.1/jort/jort_exe.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     9259 2023-06-22 00:12:17.000000 jort-1.3.1/jort/reporting_callbacks.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     7663 2023-06-22 00:12:17.000000 jort-1.3.1/jort/track_cli.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11059 2023-06-22 05:43:14.000000 jort-1.3.1/jort/tracker.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.747008 jort-1.3.1/jort.egg-info/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4280 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      386 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       43 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/entry_points.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      153 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/requires.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/top_level.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-06-22 05:54:06.747008 jort-1.3.1/setup.cfg
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      967 2023-06-22 00:12:17.000000 jort-1.3.1/setup.py
```

### Comparing `jort-1.3.0/LICENSE` & `jort-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/_config.py` & `jort-1.3.1/jort/_config.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/checkpoint.py` & `jort-1.3.1/jort/checkpoint.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/datetime_utils.py` & `jort-1.3.1/jort/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/jort_exe.py` & `jort-1.3.1/jort/jort_exe.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/reporting_callbacks.py` & `jort-1.3.1/jort/reporting_callbacks.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/track_cli.py` & `jort-1.3.1/jort/track_cli.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.0/jort/tracker.py` & `jort-1.3.1/jort/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 class Tracker(object):
     """
     A class to time sections of Python scripts by creating and closing timing
     checkpoints. 
 
     Parameters
     ----------
-    logname : str
+    log_name : str
         Filename for timing logs
     verbose : int, optional
         Options for verbosity. 0 for none, 1 for INFO, and 2 for DEBUG.
     to_db : bool, optional
-        Save all checkpoints to database
+        Save all checkpoint runtime details to database
     session_name : str, optional
         Name of job session, if saving jobs to database
 
     :ivar date_created: time of initialization
     :ivar machine: name of local machine
     :ivar checkpoints: dict of Checkpoints
     :ivar open_checkpoint_payloads: dict of job status payloads for open Checkpoints
-    :ivar logname: log filename
+    :ivar log_name: log filename
     :iver to_db: option to save all checkpoints to database
     :iver session_name: name of job session
     """
-    def __init__(self, logname="tracker.log", verbose=0, to_db=False, session_name=None):
+    def __init__(self, log_name="tracker.log", verbose=0, to_db=False, session_name=None):
         self.date_created = datetime_utils.get_iso_date()
         self.machine = _config.get_config_data().get("machine")
         self.checkpoints = {}
         self.open_checkpoint_payloads = {}
 
         # Manage session name, id; if session name is provided, get the id from db
         self.to_db = to_db
@@ -60,22 +60,22 @@
                 if self.to_db:
                     sql = (
                         "INSERT INTO sessions VALUES(?, ?)"
                     )
                     cur.execute(sql, (self.session_id, self.session_name))
                     con.commit()
 
-        self.logname = logname
+        self.log_name = log_name
         if verbose != 0:
             print(f"Starting session `{self.session_name}`")
             # if verbose == 1:
             #     level = logging.INFO
             # else:
             #     level = logging.DEBUG
-            # file_handler = logging.FileHandler(filename=self.logname, mode="w")
+            # file_handler = logging.FileHandler(filename=self.log_name, mode="w")
             # stdout_handler = logging.StreamHandler(sys.stdout)
             # handlers = [file_handler, stdout_handler]
 
             # logging.basicConfig(level=level,
             #                     format="%(asctime)s %(name)-15s %(levelname)-8s %(message)s",
             #                     handlers=handlers, 
             #                     force=True)
@@ -134,14 +134,16 @@
 
         Parameters
         ----------
         name : str, optional
             Checkpoint name
         callbacks : list, optional
             List of optional notification callbacks
+        to_db : bool, optional
+            Save checkpoint runtime details to database
         """
         if name is None:
             name = list(self.open_checkpoint_payloads.keys())[-1]
         elif name not in self.open_checkpoint_payloads:
             raise KeyError(f"No open checkpoint named {name}")
 
         payload = self.open_checkpoint_payloads.pop(name)
@@ -217,29 +219,31 @@
         """
         name = list(self.open_checkpoint_payloads.keys())[0]
         payload = self.open_checkpoint_payloads[name]
         payload["status"] = "error"
         payload["error_message"] = traceback.format_exc().strip().split('\n')[-1]
         raise
 
-    def track(self, f=None, callbacks=[], report=False):
+    def track(self, f=None, callbacks=[], to_db=False, report=False):
         """
         Function wrapper for tracker, to be used as a decorator. Creates a checkpoint
         with the input function's name. 
 
         Without parameters / evaluation, the decorator simply creates the checkpoint 
         and times the input function. With parameters, this method can execute 
         callbacks and print a report. 
 
         Parameters
         ----------
         f : func, optional
             Function to decorate
         callbacks : list, optional
             List of optional notification callbacks
+        to_db : bool, optional
+            Save checkpoint runtime details to database
         report : bool, optional
             Option to print tracker report at function completion
         """
         assert callable(f) or f is None
         def decorator(func):
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
@@ -248,15 +252,15 @@
                     result = func(*args, **kwargs)
                 except Exception as e:
                     payload = self.open_checkpoint_payloads[func.__qualname__]
                     payload["status"] = "error"
                     payload["error_message"] = traceback.format_exc().strip().split('\n')[-1]
                     raise
                 finally:
-                    self.stop(name=func.__qualname__, callbacks=callbacks)
+                    self.stop(name=func.__qualname__, callbacks=callbacks, to_db=to_db)
                     if report:
                         self.report()
                 return result
             return wrapper
         return decorator(f) if f else decorator
         
     def report(self, dec=1):
@@ -269,26 +273,28 @@
             Decimal precision
         """
         for name in self.checkpoints:
             ckpt = self.checkpoints[name]
             print(ckpt.report(dec=dec))
             
             
-def track(f=None, callbacks=[], report=True):
+def track(f=None, callbacks=[], to_db=False, report=True):
     """
     Independent function wrapper, to be used as a decorator, that creates a one-off
     tracker.
     
     Without parameters / evaluation, the decorator simply times the input function
     and prints a report by default. With parameters, this method can execute notification
     callbacks and control whether or not to print a report. 
 
     Parameters
     ----------
     f : func, optional
         Function to decorate
     callbacks : list, optional
         List of optional notification callbacks
+    to_db : bool, optional
+        Save checkpoint runtime details to database
     report : bool, optional
         Option to print tracker report at function completion
     """
-    return Tracker(verbose=0).track(f=f, callbacks=callbacks, report=report)
+    return Tracker(verbose=0).track(f=f, callbacks=callbacks, to_db=to_db, report=report)
```

### Comparing `jort-1.3.0/setup.py` & `jort-1.3.1/setup.py`

 * *Files identical despite different names*

