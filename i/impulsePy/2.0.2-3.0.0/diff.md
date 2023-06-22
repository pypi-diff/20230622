# Comparing `tmp/impulsePy-2.0.2.tar.gz` & `tmp/impulsePy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impulsePy-2.0.2.tar", last modified: Tue Mar 28 15:18:07 2023, max compression
+gzip compressed data, was "dist\impulsePy-3.0.0.tar", last modified: Thu Jun 22 07:48:57 2023, max compression
```

## Comparing `impulsePy-2.0.2.tar` & `impulsePy-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 15:18:07.437704 impulsePy-2.0.2/
--rw-rw-rw-   0        0        0     1073 2021-09-22 05:22:38.000000 impulsePy-2.0.2/LICENSE
--rw-rw-rw-   0        0        0      504 2023-03-28 15:18:07.437704 impulsePy-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-28 15:11:33.000000 impulsePy-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 15:18:07.432705 impulsePy-2.0.2/impulsePy/
--rw-rw-rw-   0        0        0    19060 2023-03-28 14:56:47.000000 impulsePy-2.0.2/impulsePy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 15:18:07.436705 impulsePy-2.0.2/impulsePy.egg-info/
--rw-rw-rw-   0        0        0      504 2023-03-28 15:18:07.000000 impulsePy-2.0.2/impulsePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-03-28 15:18:07.000000 impulsePy-2.0.2/impulsePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 15:18:07.000000 impulsePy-2.0.2/impulsePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-28 15:18:07.000000 impulsePy-2.0.2/impulsePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-28 15:18:07.000000 impulsePy-2.0.2/impulsePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-28 15:18:07.438712 impulsePy-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-03-28 14:58:19.000000 impulsePy-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/
+-rw-rw-rw-   0        0        0      740 2023-06-22 07:48:57.000000 impulsePy-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-22 07:40:36.000000 impulsePy-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy/
+-rw-rw-rw-   0        0        0    21363 2023-06-22 07:37:13.000000 impulsePy-3.0.0/impulsePy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 07:48:57.000000 impulsePy-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-22 07:38:30.000000 impulsePy-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `impulsePy-2.0.2/impulsePy/__init__.py` & `impulsePy-3.0.0/impulsePy/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import logging
 import os
 from time import sleep
 
 _logger = logging.getLogger(__name__)
 
-version = "2.0.2" # Update to the latest version of the impulse API (Impule version 1.3)
+version = "3.0.0" # Added LSS controls and data
 
 controlEndpoint = "tcp://127.0.0.1:5557"
 dataEndpoint = "tcp://127.0.0.1:5556"
 
 profilesPath = os.path.expanduser('~\\Documents\\Impulse\\Profiles\\')
 profilesPath = profilesPath.replace("\\","/")
 
@@ -96,32 +96,41 @@
         self.lastSentSequence = 0
         
     def setFlag(self, flagName):
         subscriber.setFlag(flagName)
     
     def getLastData(self):
         if self.stimulus.encode() in subscriber.topics:
-            data = subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records')[0]
-            self.lastSentSequence = data["sequenceNumber"]
-            return data
+            if len(subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records'))>0:
+                data = subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records')[0]
+                self.lastSentSequence = data["sequenceNumber"]
+                return data
+            else:
+                print("No data available...")
+                return None
         else:
+            print("Topic not available...")
             return None
     
     def setPointChanged(self):
         data = subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records')[0]
         self.lastSentSequence = data["sequenceNumber"]
         
     def getNewData(self):
         if self.stimulus.encode() in subscriber.topics:
-            while subscriber.topics[self.stimulus.encode()].iloc[-1]["sequenceNumber"] == self.lastSentSequence:
-                sleep(0.001)
-            data = subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records')[0]
-            self.lastSentSequence = data["sequenceNumber"]
-            return data
+            if len(subscriber.topics[self.stimulus.encode()])>0:
+                while subscriber.topics[self.stimulus.encode()].iloc[-1]["sequenceNumber"] == self.lastSentSequence:
+                    sleep(0.001)
+                data = subscriber.topics[self.stimulus.encode()].tail(1).to_dict(orient='records')[0]
+                self.lastSentSequence = data["sequenceNumber"]
+                return data
+            else:
+                print("No data available...")
         else:
+            print("Topic not available...")
             return None
         
     def getDataFrame(self, startExpTimeOrFlag=0, endExpTimeOrFlag=None):
         if isinstance(startExpTimeOrFlag, str):
             if startExpTimeOrFlag in subscriber.flags:
                 startExpTimeOrFlag = subscriber.flags[startExpTimeOrFlag]
             else:
@@ -336,14 +345,66 @@
     def stopInitiateFlow(self):
         controlDict = {
             '$type' : 'control.gas.gplus.pressureFlow.stopInitializingFlow',
             }        
         returnMessage = sendControl(controlDict)
         return returnMessage["resultCode"]
 
+class liquid():
+    def __init__(self):
+        self.stimulus = 'liquid'
+        self.data = device(self.stimulus)
+        
+    def setHumidity(self, setPoint):
+        controlDict = {
+            '$type': 'control.liquid.v2.setHumidity',
+            'humidity': setPoint
+        }
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+
+    def setPF(self, version, outletPressure, flow):
+        controlDict = {
+            '$type': 'control.liquid.'+version+'.pressureFlow.apply',
+            'flow': flow,
+            'outletPressure': outletPressure
+        }            
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+    
+    def setPFC(self, version, outletPressure, flow, concentration):
+        controlDict = {
+            '$type': 'control.liquid.v2.pressureFlow.apply',
+            'flow': flow,
+            'concentration': concentration,
+            'outletPressure': outletPressure
+        }       
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+    
+    def setIOP(self, version, inletPressure, outletPressure):
+        controlDict = {
+            '$type': 'control.liquid.'+version+'.inletOutletPressure.apply',
+            'inletPressure1': inletPressure,
+            'outletPressure': outletPressure
+        }        
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+
+    def setI2OP(self, version, inletPressure1, inletPressure2, outletPressure):
+        controlDict = {
+            '$type': 'control.liquid.v2.inletOutletPressure.apply',
+            'inletPressure1': inletPressure1,
+            'inletPressure2': inletPressure2,
+            'outletPressure': outletPressure
+        }        
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+
+
 class apiSubscriber(threading.Thread):
     def __init__(self, endpoint):
         super().__init__()
         self.endpoint = endpoint
         self.topics = {}
         self.socket = None
         self.running = True
@@ -384,27 +445,25 @@
     
     def run(self):
         while self.running:
             try:
                 message = self.socket.recv_multipart(flags=zmq.NOBLOCK)
                 topic = message[0]
                 data = json.loads(message[1].decode('utf-8'))
-
                 if topic in self.topics:
                     df = pd.DataFrame([data], index=[0])
                     if topic != b"events":
                         if topic == b'massSpec':
                             for channel in df.iloc[0]['channels']:
                                 df[channel['name']]=channel['measuredValue']
                             df.iloc[0].drop('channels')
                         df = self.roundDataframeValues(df)
                         df["flag"]=self.currentFlag           
                         self.lastExperimentTime = df.iloc[-1]['experimentDuration']
                     self.topics[topic] = pd.concat([self.topics[topic], df], ignore_index=True)
-                
                 if topic == b"events" and data.get("newState") == "control":
                     self.updateParameters()
                     
                 if topic == b"events" and data.get("$type") == "data.event.stimulusActionFinished":
                     stimulusType = data.get("stimulusType")
                     status[stimulusType]="ready"
                     
@@ -489,11 +548,11 @@
 subscriber.start()
 subscriber.subscribe(b"events")
 
 profile = profile()
 heat = heat()
 bias = bias()
 gas = gas()
+liquid = liquid()
 
 def getParameterInfo():
-    return subscriber.parameterInfo
-
+    return subscriber.parameterInfo
```

### Comparing `impulsePy-2.0.2/setup.py` & `impulsePy-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impulsePy", # Replace with your own username
-    version="2.0.2",
+    version="3.0.0",
     author="DENSsolutions",
     author_email="merijn.pen@DENSsolutions.com",
     description="Library for controlling Impulse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

