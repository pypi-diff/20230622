# Comparing `tmp/action-graph-1.2.8.tar.gz` & `tmp/action-graph-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.2.8.tar", last modified: Fri Jun 16 14:47:09 2023, max compression
+gzip compressed data, was "action-graph-1.2.9.tar", last modified: Wed Jun 21 20:48:10 2023, max compression
```

## Comparing `action-graph-1.2.8.tar` & `action-graph-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.8/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.8/README.md
--rw-r--r--   0        0        0      684 2023-06-16 14:46:27.786532 action-graph-1.2.8/action_graph/__init__.py
--rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.2.8/action_graph/action.py
--rw-r--r--   0        0        0     9491 2023-06-16 02:52:33.411377 action-graph-1.2.8/action_graph/agent.py
--rw-r--r--   0        0        0     4689 2023-06-16 03:39:34.857713 action-graph-1.2.8/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-16 14:46:33.286410 action-graph-1.2.8/pyproject.toml
--rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.2.8/tests/01-redundant_precon_test.py
--rwxr-xr-x   0        0        0     1096 2023-06-16 14:35:32.753006 action-graph-1.2.8/tests/02-multi_feasible_test.py
--rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.2.8/tests/03-references_test.py
--rwxr-xr-x   0        0        0      917 2023-06-16 14:31:44.398052 action-graph-1.2.8/tests/04-loop_test.py
--rw-r--r--   0        0        0        0 2023-06-16 14:40:25.834530 action-graph-1.2.8/tests/__init__.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.9/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.9/README.md
+-rw-r--r--   0        0        0      684 2023-06-21 20:46:34.412529 action-graph-1.2.9/action_graph/__init__.py
+-rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.2.9/action_graph/action.py
+-rw-r--r--   0        0        0     9491 2023-06-16 02:52:33.411377 action-graph-1.2.9/action_graph/agent.py
+-rw-r--r--   0        0        0     4691 2023-06-21 20:44:45.869031 action-graph-1.2.9/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-21 20:46:26.104567 action-graph-1.2.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.2.9/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1096 2023-06-16 14:35:32.753006 action-graph-1.2.9/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.2.9/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      917 2023-06-16 14:31:44.398052 action-graph-1.2.9/tests/04-loop_test.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:40:25.834530 action-graph-1.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.9/PKG-INFO
```

### Comparing `action-graph-1.2.8/LICENSE` & `action-graph-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/README.md` & `action-graph-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/action_graph/__init__.py` & `action-graph-1.2.9/action_graph/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.2.8/action_graph/action.py` & `action-graph-1.2.9/action_graph/action.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/action_graph/agent.py` & `action-graph-1.2.9/action_graph/agent.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/action_graph/planner.py` & `action-graph-1.2.9/action_graph/planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,14 @@
         action_lookup: Dict[Tuple[Any, Any], List[Action]] = defaultdict(list)
         for action in actions:
             for k, v in action.effects.items():
                 action_lookup[(k, v)].append(action)
         return action_lookup
 
     def __parse_references(self, ref: Any, state: State) -> Any:
-        if ref[1:] in state:
-            return state[ref[1:]]
+        while ref[1:] in state:
+            ref = state[ref[1:]]
         return ref
 
     def __make_unique(self, path):
         unique = set()
         return [x for x in path if x not in unique and not unique.add(x)]
```

### Comparing `action-graph-1.2.8/pyproject.toml` & `action-graph-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.2.8"
+version = "1.2.9"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.2.8/tests/01-redundant_precon_test.py` & `action-graph-1.2.9/tests/01-redundant_precon_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/tests/02-multi_feasible_test.py` & `action-graph-1.2.9/tests/02-multi_feasible_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/tests/03-references_test.py` & `action-graph-1.2.9/tests/03-references_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/tests/04-loop_test.py` & `action-graph-1.2.9/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.8/PKG-INFO` & `action-graph-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.2.8
+Version: 1.2.9
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

