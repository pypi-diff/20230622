# Comparing `tmp/ICICONSOLE-0.0.8.tar.gz` & `tmp/ICICONSOLE-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.8.tar", last modified: Thu Jun  8 22:15:23 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.9.tar", last modified: Fri Jun  9 00:57:34 2023, max compression
```

## Comparing `ICICONSOLE-0.0.8.tar` & `ICICONSOLE-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.324452 ICICONSOLE-0.0.8/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.323231 ICICONSOLE-0.0.8/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9689 2023-06-08 22:11:12.000000 ICICONSOLE-0.0.8/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.324085 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.8/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-08 22:15:23.324317 ICICONSOLE-0.0.8/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.8/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1021 2023-06-08 22:13:43.000000 ICICONSOLE-0.0.8/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-08 22:15:23.324485 ICICONSOLE-0.0.8/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.432371 ICICONSOLE-0.0.9/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.431097 ICICONSOLE-0.0.9/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-09 00:56:38.000000 ICICONSOLE-0.0.9/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    10098 2023-06-09 00:56:32.000000 ICICONSOLE-0.0.9/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.431999 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.9/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-09 00:57:34.432229 ICICONSOLE-0.0.9/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.9/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1021 2023-06-09 00:57:25.000000 ICICONSOLE-0.0.9/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-09 00:57:34.432405 ICICONSOLE-0.0.9/setup.cfg
```

### Comparing `ICICONSOLE-0.0.8/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.9/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.8/ICICONSOLE/__main__.py` & `ICICONSOLE-0.0.9/ICICONSOLE/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 
     # Loop so that the console keeps prompting the user for commands, until the user exits
     while(True):
         # This is reading the actual input from the user; the input message shows the username and the pod id
         query = str(input("[" + user + "@" + pod_id + "] "))
 
         executeCypher = True
+        node = False
+        listedProps = False
 
         # This is a switch statement that allows for the user to type in a command, and the console will execute the command.
         match query:
             case "exit":
                 os._exit(0)
                 executeCypher = False
             # The command to pick a new pod to connect to. Calls the choosePod function, defined below.
@@ -111,42 +113,50 @@
                 try:
                     helpCypher()
                     executeCypher = False
                 except:
                     pass
             case "all":
                 query = bcc.getAll()
+                node = True
             case "allNames":
                 query = bcc.getAllNames()
             case "oneByName":
                 query = bcc.getOneByName()
+                node = True
             case "allProperty":
                 query = bcc.allProperty()
             case "allProperties":
                 query = bcc.allProperties()
             case "allPropertiesForNode":
                 query = bcc.allPropertiesForNode()
+                listedProps = True
             case _:
                 pass
 
         if (executeCypher):
             # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
             try: 
                 result = graph.run(query)
                 
-                try:
+                if node:
                     data = []
                     for record in result:
                         node = record[0]
                         properties = dict(node)
                         data.append(properties)
                     df = pd.DataFrame(data)
                     with pd.option_context('display.max_rows', None, 'display.max_columns', None):
                         scroll(df)
-                except:
+                elif listedProps:
+                    data = result.data()[0]['keys(n)']
+                    df = pd.DataFrame(data)
+                    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
+                        scroll(df)
+                else:
                     df = graph.run(query).to_data_frame()
                     with pd.option_context('expand_frame_repr', False, 'display.max_rows', None): 
                         print(df)
 
 
 
             # Error catching, if the Cypher was not executed properly
```

### Comparing `ICICONSOLE-0.0.8/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.9/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.8
+Version: 0.0.9
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.8/LICENSE` & `ICICONSOLE-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.8/PKG-INFO` & `ICICONSOLE-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.8
+Version: 0.0.9
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.8/README.md` & `ICICONSOLE-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.8/pyproject.toml` & `ICICONSOLE-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.8"
+version = "0.0.9"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

