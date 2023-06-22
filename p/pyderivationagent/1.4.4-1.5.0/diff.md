# Comparing `tmp/pyderivationagent-1.4.4.tar.gz` & `tmp/pyderivationagent-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyderivationagent-1.4.4.tar", last modified: Fri Mar  3 18:29:57 2023, max compression
+gzip compressed data, was "pyderivationagent-1.5.0.tar", last modified: Thu Jun 22 00:35:09 2023, max compression
```

## Comparing `pyderivationagent-1.4.4.tar` & `pyderivationagent-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1162 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/LICENSE
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/MANIFEST.in
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29879 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29436 2023-02-20 09:12:13.000000 pyderivationagent-1.4.4/README.md
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.116170 pyderivationagent-1.4.4/pyderivationagent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-03-03 18:27:43.000000 pyderivationagent-1.4.4/pyderivationagent/__init__.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.116170 pyderivationagent-1.4.4/pyderivationagent/agent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       59 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/pyderivationagent/agent/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    37413 2023-01-30 17:21:22.000000 pyderivationagent-1.4.4/pyderivationagent/agent/derivation_agent.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.116170 pyderivationagent-1.4.4/pyderivationagent/conf/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      154 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/pyderivationagent/conf/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5925 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/pyderivationagent/conf/agent_conf.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/pyderivationagent/data_model/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      113 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/data_model/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4990 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/data_model/derivation.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3073 2023-02-03 17:19:21.000000 pyderivationagent-1.4.4/pyderivationagent/data_model/iris.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2594 2022-10-20 19:07:12.000000 pyderivationagent-1.4.4/pyderivationagent/data_model/utils.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/pyderivationagent/exception/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       39 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/exception/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      336 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/exception/exception.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/pyderivationagent/kg_operations/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      126 2023-01-19 18:27:40.000000 pyderivationagent-1.4.4/pyderivationagent/kg_operations/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    15131 2023-03-03 17:23:43.000000 pyderivationagent-1.4.4/pyderivationagent/kg_operations/derivation_client.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      621 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/kg_operations/gateway.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6112 2022-11-21 12:34:31.000000 pyderivationagent-1.4.4/pyderivationagent/kg_operations/sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-03-03 18:29:57.116170 pyderivationagent-1.4.4/pyderivationagent.egg-info/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29879 2023-03-03 18:29:56.000000 pyderivationagent-1.4.4/pyderivationagent.egg-info/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      853 2023-03-03 18:29:57.000000 pyderivationagent-1.4.4/pyderivationagent.egg-info/SOURCES.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-03-03 18:29:56.000000 pyderivationagent-1.4.4/pyderivationagent.egg-info/dependency_links.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      191 2023-03-03 18:29:56.000000 pyderivationagent-1.4.4/pyderivationagent.egg-info/requires.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       18 2023-03-03 18:29:56.000000 pyderivationagent-1.4.4/pyderivationagent.egg-info/top_level.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-03-03 18:29:57.126170 pyderivationagent-1.4.4/setup.cfg
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      986 2023-03-03 18:27:43.000000 pyderivationagent-1.4.4/setup.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.986904 pyderivationagent-1.5.0/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1162 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/LICENSE
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/MANIFEST.in
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29879 2023-06-22 00:35:08.986904 pyderivationagent-1.5.0/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29436 2023-03-23 09:20:43.000000 pyderivationagent-1.5.0/README.md
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.956904 pyderivationagent-1.5.0/pyderivationagent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-06-22 00:13:07.000000 pyderivationagent-1.5.0/pyderivationagent/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.956904 pyderivationagent-1.5.0/pyderivationagent/agent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       59 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/pyderivationagent/agent/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    37986 2023-06-21 23:11:45.000000 pyderivationagent-1.5.0/pyderivationagent/agent/derivation_agent.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.966904 pyderivationagent-1.5.0/pyderivationagent/conf/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      154 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/pyderivationagent/conf/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5925 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/pyderivationagent/conf/agent_conf.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.966904 pyderivationagent-1.5.0/pyderivationagent/data_model/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      113 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/data_model/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5040 2023-06-21 21:41:34.000000 pyderivationagent-1.5.0/pyderivationagent/data_model/derivation.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3073 2023-03-23 09:20:43.000000 pyderivationagent-1.5.0/pyderivationagent/data_model/iris.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2594 2022-10-26 20:03:38.000000 pyderivationagent-1.5.0/pyderivationagent/data_model/utils.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.966904 pyderivationagent-1.5.0/pyderivationagent/exception/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       39 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/exception/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      336 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/exception/exception.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.976904 pyderivationagent-1.5.0/pyderivationagent/kg_operations/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      126 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/kg_operations/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    15482 2023-06-21 18:32:05.000000 pyderivationagent-1.5.0/pyderivationagent/kg_operations/derivation_client.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      621 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/kg_operations/gateway.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6112 2022-11-12 16:19:00.000000 pyderivationagent-1.5.0/pyderivationagent/kg_operations/sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-06-22 00:35:08.956904 pyderivationagent-1.5.0/pyderivationagent.egg-info/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    29879 2023-06-22 00:35:08.000000 pyderivationagent-1.5.0/pyderivationagent.egg-info/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      853 2023-06-22 00:35:08.000000 pyderivationagent-1.5.0/pyderivationagent.egg-info/SOURCES.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-06-22 00:35:08.000000 pyderivationagent-1.5.0/pyderivationagent.egg-info/dependency_links.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      191 2023-06-22 00:35:08.000000 pyderivationagent-1.5.0/pyderivationagent.egg-info/requires.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       18 2023-06-22 00:35:08.000000 pyderivationagent-1.5.0/pyderivationagent.egg-info/top_level.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-06-22 00:35:08.986904 pyderivationagent-1.5.0/setup.cfg
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      986 2023-06-22 00:13:07.000000 pyderivationagent-1.5.0/setup.py
```

### Comparing `pyderivationagent-1.4.4/LICENSE` & `pyderivationagent-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/PKG-INFO` & `pyderivationagent-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderivationagent
-Version: 1.4.4
+Version: 1.5.0
 Summary: pyderivationagent is a python wrapper for derivation agents as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/JPS_BASE_LIB/python_derivation_agent
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `pyderivationagent-1.4.4/README.md` & `pyderivationagent-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent/agent/derivation_agent.py` & `pyderivationagent-1.5.0/pyderivationagent/agent/derivation_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,38 +502,43 @@
                 res[self.jpsBaseLib_view.DerivationClient.AGENT_OUTPUT_KEY] = json.loads(str(outputs.getNewEntitiesJsonMap()))
                 self.logger.info("Synchronous derivation for new information generated successfully, returned response: " + str(res))
                 return json.dumps(res)
 
             # only enters below if the computation was not for new information (new instances)
             derivation = self.jpsBaseLib_view.Derivation(derivationIRI, derivationType)
             if not derivation.isDerivationAsyn() and not derivation.isDerivationWithTimeSeries():
+                # Perform the mapping between the new outputs and the downstream derivations
+                connectionMap = self.derivation_client.derivation_client.mapSyncNewOutputsToDownstream(
+                    outputs.getThisDerivation(), outputs.getNewOutputsAndRdfTypeMap())
                 # construct and fire SPARQL update given DerivationOutputs objects, if normal
                 # derivation NOTE this makes sure that the new generated instances/triples will
                 # ONLY be written to knowledge graph if the target derivation is till outdated
                 # at the point of executing SPARQL update, i.e. this solves concurrent request
                 # issue as detailed in
                 # https://github.com/cambridge-cares/TheWorldAvatar/issues/184
-                triplesChangedForSure = self.derivation_client.derivation_client.reconnectNewDerivedIRIs(
-                    outputs.getOutputTriples(), outputs.getNewEntitiesDownstreamDerivationMap(),
-                    outputs.getThisDerivation(), outputs.getRetrievedInputsAt()
+                triplesChangedForSure = self.derivation_client.derivation_client.reconnectSyncDerivation(
+                    outputs.getThisDerivation(), connectionMap,
+                    outputs.getOutputTriples(), outputs.getRetrievedInputsAt()
                 )
 
                 # for normal Derivation, we need to return both timestamp and the new derived
                 if triplesChangedForSure:
                     # if we know the triples are changed for sure, we return the triples
                     # computed by this agent
                     res[self.jpsBaseLib_view.DerivationOutputs.RETRIEVED_INPUTS_TIMESTAMP_KEY] = outputs.getRetrievedInputsAt()
                     res[self.jpsBaseLib_view.DerivationClient.AGENT_OUTPUT_KEY] = json.loads(str(outputs.getNewEntitiesJsonMap()))
+                    res[self.jpsBaseLib_view.DerivationClient.AGENT_OUTPUT_CONNECTION_KEY] = json.loads(str(self.jpsBaseLib_view.org.json.JSONObject(connectionMap)))
                     self.logger.info("Derivation update is done in the knowledge graph, returned response: " + str(res))
                 else:
                     # if we are not certain, query the knowledge graph to get the accurate
                     # information
                     updated = self.derivation_client.derivation_client.getDerivation(derivationIRI)
                     res[self.jpsBaseLib_view.DerivationOutputs.RETRIEVED_INPUTS_TIMESTAMP_KEY] = updated.getTimestamp()
                     res[self.jpsBaseLib_view.DerivationClient.AGENT_OUTPUT_KEY] = json.loads(str(updated.getBelongsToMap()))
+                    res[self.jpsBaseLib_view.DerivationClient.AGENT_OUTPUT_CONNECTION_KEY] = json.loads(str(updated.getDownstreamDerivationConnectionMap()))
                     self.logger.info("Unable to determine if the SPARQL update mutated triples, returned latest information in knowledge graph: "
                                      + str(res))
             else:
                 # for DerivationWithTimeSeries, we just need to return retrievedInputsAt
                 res[self.jpsBaseLib_view.DerivationOutputs.RETRIEVED_INPUTS_TIMESTAMP_KEY] = outputs.getRetrievedInputsAt()
                 self.logger.info(
                     "DerivationWithTimeSeries update is done, returned response: " + str(res))
```

### Comparing `pyderivationagent-1.4.4/pyderivationagent/conf/agent_conf.py` & `pyderivationagent-1.5.0/pyderivationagent/conf/agent_conf.py`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent/data_model/derivation.py` & `pyderivationagent-1.5.0/pyderivationagent/data_model/derivation.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
     def getDerivationIRI(self):
         return self.derivation_inputs.getDerivationIRI()
 
     def getInputs(self):
         return ast.literal_eval(str(self.derivation_inputs.getInputs()))
 
     def getIris(self, rdfType):
-        return list(self.derivation_inputs.getIris(rdfType))
+        iris = self.derivation_inputs.getIris(rdfType)
+        return list(iris) if iris is not None else None
 
 
 class DerivationOutputs():
     """This is a warpper class for uk.ac.cam.cares.jps.base.derivation.DerivationOutputs.java.
     All methods provided here are wrapped around the relevant methods in the java class,
     as references for developers to handle derivations within python derivation agents."""
```

### Comparing `pyderivationagent-1.4.4/pyderivationagent/data_model/iris.py` & `pyderivationagent-1.5.0/pyderivationagent/data_model/iris.py`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent/data_model/utils.py` & `pyderivationagent-1.5.0/pyderivationagent/data_model/utils.py`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent/kg_operations/derivation_client.py` & `pyderivationagent-1.5.0/pyderivationagent/kg_operations/derivation_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,26 @@
         """
         self.derivation_client.dropTimestampsOf(entities)
 
 
     ##############################################
     ## Methods for requesting update derivation ##
     ##############################################
+    def getDerivations(self, agentIRI: str) -> list:
+        """Get the derivations of the given agent.
+
+        Args:
+            agentIRI (str): IRI of the agent
+
+        Returns:
+            list: List of IRIs of the derivations that isDerivedUsing the given agent
+        """
+        return list(self.derivation_client.getDerivations(agentIRI))
+
+
     def getDerivationsOf(self, entities: List[str]) -> Dict[str, str]:
         """Get the derivations of the given entities.
 
         Args:
             entities (List[str]): List of entities
 
         Returns:
```

### Comparing `pyderivationagent-1.4.4/pyderivationagent/kg_operations/gateway.py` & `pyderivationagent-1.5.0/pyderivationagent/kg_operations/gateway.py`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent/kg_operations/sparql_client.py` & `pyderivationagent-1.5.0/pyderivationagent/kg_operations/sparql_client.py`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/pyderivationagent.egg-info/PKG-INFO` & `pyderivationagent-1.5.0/pyderivationagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderivationagent
-Version: 1.4.4
+Version: 1.5.0
 Summary: pyderivationagent is a python wrapper for derivation agents as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/JPS_BASE_LIB/python_derivation_agent
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `pyderivationagent-1.4.4/pyderivationagent.egg-info/SOURCES.txt` & `pyderivationagent-1.5.0/pyderivationagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyderivationagent-1.4.4/setup.py` & `pyderivationagent-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='pyderivationagent',
-    version='1.4.4',
+    version='1.5.0',
     author='Jiaru Bai',
     author_email='jb2197@cam.ac.uk',
     license='MIT',
     python_requires='>=3.5',
     description="pyderivationagent is a python wrapper for derivation agents as part of The World Avatar project.",
     url="https://github.com/cambridge-cares/TheWorldAvatar/tree/main/JPS_BASE_LIB/python_derivation_agent",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(exclude=['tests','tests.*']),
-    install_requires=['py4jps>=1.0.34', 'flask==2.1.0', 'gunicorn==20.0.4', 'Flask-APScheduler', 'rdflib', 'python-dotenv', 'yagmail'],
+    install_requires=['py4jps>=1.0.35', 'flask==2.1.0', 'gunicorn==20.0.4', 'Flask-APScheduler', 'rdflib', 'python-dotenv', 'yagmail'],
     extras_require={
         "dev": [
             "testcontainers>=3.4.2",
             "pytest>=6.2.3",
             "pytest-docker-compose>=3.2.1",
             "pytest-rerunfailures>=10.2"
         ],
```

