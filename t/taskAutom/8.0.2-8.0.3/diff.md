# Comparing `tmp/taskAutom-8.0.2.tar.gz` & `tmp/taskAutom-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-8.0.2.tar", last modified: Fri Jun  2 18:41:30 2023, max compression
+gzip compressed data, was "taskAutom-8.0.3.tar", last modified: Fri Jun  2 19:43:09 2023, max compression
```

## Comparing `taskAutom-8.0.2.tar` & `taskAutom-8.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.2/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 18:41:30.814967 taskAutom-8.0.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.2/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-02 18:41:30.814967 taskAutom-8.0.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-02 18:41:22.000000 taskAutom-8.0.2/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-02 18:41:16.000000 taskAutom-8.0.2/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66936 2023-06-02 18:38:17.000000 taskAutom-8.0.2/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.755346 taskAutom-8.0.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.3/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 19:43:09.755346 taskAutom-8.0.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.3/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-02 19:43:09.755346 taskAutom-8.0.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-02 19:33:06.000000 taskAutom-8.0.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.751346 taskAutom-8.0.3/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.751346 taskAutom-8.0.3/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-02 19:32:38.000000 taskAutom-8.0.3/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    67035 2023-06-02 19:36:03.000000 taskAutom-8.0.3/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.755346 taskAutom-8.0.3/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-8.0.2/LICENSE` & `taskAutom-8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.2/PKG-INFO` & `taskAutom-8.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.2
+Version: 8.0.3
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-8.0.2/README.md` & `taskAutom-8.0.3/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.2/setup.py` & `taskAutom-8.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='8.0.2',
+    version='8.0.3',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-8.0.2/src/taskAutom/taskAutom.py` & `taskAutom-8.0.3/src/taskAutom/taskAutom.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-LATEST_VERSION = '8.0.2'
+LATEST_VERSION = '8.0.3'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -936,15 +936,15 @@
 
 		# We update the outputjob relevant information...
 		if self.outputJob == 2:
 			self.connInfo['pluginScript'] = DICT_VENDOR[self.connInfo['deviceType']]['START_SCRIPT'] + \
 											DICT_VENDOR[self.connInfo['deviceType']]['FIRST_LINE'] + \
 											routerInfo['pluginScript'][-1] + \
 											DICT_VENDOR[self.connInfo['deviceType']]['LAST_LINE'] + \
-											DICT_VENDOR[self.connInfo['deviceType']]['FIN_SCRIPT']	
+											DICT_VENDOR[self.connInfo['deviceType']]['FIN_SCRIPT']				
 		elif self.outputJob == 3:
 			self.connInfo['ftpFiles'] = routerInfo['ftpFiles']
 			self.connInfo['ftpTotalTxFiles'] = 0
 
 		# Do we you use jumpHosts?
 		if self.connInfo['useSSHTunnel'] is True or dictParam['inventoryFile'] != None:
 			self.connInfo['jumpHost'] = [x for i,x in enumerate(self.connInfo['jumpHosts']) if self.connInfo['num'] % len(self.connInfo['jumpHosts']) == i][0]
@@ -1034,16 +1034,15 @@
 		outputJson = {}
 
 		mdDevice           = re.match('^md_',deviceType)
 		mdShow             = DICT_VENDOR[connInfo['deviceType']]['SHOW']
 
 
 		# ### Writes to a connection. 
-
-		if type(inText) == type([]):
+		if isinstance(inText,list):
 
 			if pluginType == 'config':
 
 				try:
 					outputTxt    = conn2rtr.send_config_set(config_commands=inText, enter_config_mode=False, cmd_verify=cmdVerify, read_timeout=readTimeOut)
 					aluLogReason = ""
 					runStatus    = 1
@@ -1071,15 +1070,15 @@
 					runStatus    = 1
 
 				except Exception as e:
 					outputTxt = outputTxt + '\n' + cmd + '\n' + rx
 					aluLogReason = str(e).replace('\n',' ')
 					runStatus    = -1
 
-		elif type(inText) == type(''):
+		elif isinstance(inText,str):
 			
 			try:
 				outputTxt    = conn2rtr.send_command(inText, expect_string=expectString, cmd_verify=cmdVerify, read_timeout=readTimeOut)
 				aluLogReason = ""
 				runStatus    = 1					
 			except Exception as e:
 				outputTxt    = ''
@@ -1430,25 +1429,28 @@
 
 		tEnd  = time.time()
 		tDiff = tEnd - tStart
 
 		## Analizing output only if writing to connection was successfull
 		if aluLogReason == "":
 			
+			# we verify correctness of execution ...
 			if any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in major_error_list]):
 				aluLogReason = "MajorFailed"
-			elif any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in minor_error_list]):				
+			elif any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in minor_error_list]):
 				aluLogReason = "MinorFailed"
 			elif any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in info_error_list]):
 				aluLogReason = "InfoFailed"
-			elif not any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in fin_script]):
-				aluLogReason = 'Incomplete'
 			else:
 				aluLogReason = "SendSuccess"
 
+			# we verify completeness of execution ...
+			if not any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in fin_script]):
+				aluLogReason = aluLogReason + ':Incomplete'
+
 		fncPrintConsole(connInfo['strConn'] + "Time: " + fncFormatTime(tDiff) + ". Result: " + aluLogReason, show=1)
 
 		connInfo['aluLogReason'] = aluLogReason
 		connInfo['runStatus']    = runStatus
 		connInfo['tDiff']        = tDiff
 		connInfo['outRx']        = outRx
 		connInfo['outRxJson']    = outRxJson
```

### Comparing `taskAutom-8.0.2/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.3/taskAutom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.2
+Version: 8.0.3
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

