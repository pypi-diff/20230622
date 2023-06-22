# Comparing `tmp/chilitools-0.1.9.tar.gz` & `tmp/chilitools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chilitools-0.1.9.tar", max compression
+gzip compressed data, was "chilitools-0.2.0.tar", max compression
```

## Comparing `chilitools-0.1.9.tar` & `chilitools-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0     2304 2022-04-19 09:34:55.875899 chilitools-0.1.9/chilitools/__init__.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.1.9/chilitools/api/__init__.py
--rw-r--r--   0        0        0     5517 2022-04-15 23:50:24.374182 chilitools-0.1.9/chilitools/api/connector.py
--rw-r--r--   0        0        0     9603 2022-04-15 23:49:00.607323 chilitools-0.1.9/chilitools/api/endpoints.py
--rw-r--r--   0        0        0     2545 2022-04-15 23:49:27.095259 chilitools-0.1.9/chilitools/api/mycp.py
--rw-r--r--   0        0        0     2879 2022-04-18 07:00:29.267954 chilitools-0.1.9/chilitools/api/response.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.1.9/chilitools/settings/__init__.py
--rw-r--r--   0        0        0      206 2022-04-18 11:17:55.948277 chilitools-0.1.9/chilitools/settings/apiKeys.txt
--rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.1.9/chilitools/settings/config.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.1.9/chilitools/utilities/__init__.py
--rw-r--r--   0        0        0     2008 2022-04-15 01:52:44.257856 chilitools-0.1.9/chilitools/utilities/backoffice.py
--rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.1.9/chilitools/utilities/defaults.py
--rw-r--r--   0        0        0      844 2022-04-15 01:52:44.258048 chilitools-0.1.9/chilitools/utilities/errors.py
--rw-r--r--   0        0        0     3685 2022-04-18 11:04:47.374932 chilitools-0.1.9/chilitools/utilities/file.py
--rw-r--r--   0        0        0      571 2022-04-15 01:52:44.258259 chilitools-0.1.9/chilitools/utilities/logger.py
--rw-r--r--   0        0        0     1846 2022-04-15 01:52:44.258365 chilitools-0.1.9/chilitools/utilities/menu.py
--rw-r--r--   0        0        0      600 2022-04-15 01:52:44.258461 chilitools-0.1.9/chilitools/utilities/pdf.py
--rw-r--r--   0        0        0      123 2022-04-15 01:52:44.258556 chilitools-0.1.9/chilitools/utilities/strings.py
--rw-r--r--   0        0        0     1266 2022-04-15 01:52:44.258650 chilitools-0.1.9/chilitools/utilities/xml.py
--rw-r--r--   0        0        0      492 2022-04-19 09:36:06.872394 chilitools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      864 2022-04-19 09:39:48.398573 chilitools-0.1.9/setup.py
--rw-r--r--   0        0        0      565 2022-04-19 09:39:48.398740 chilitools-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3655 2023-06-22 03:49:54.710379 chilitools-0.2.0/chilitools/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.0/chilitools/api/__init__.py
+-rw-r--r--   0        0        0     7160 2023-03-20 16:14:22.242821 chilitools-0.2.0/chilitools/api/connector.py
+-rw-r--r--   0        0        0    20888 2023-06-22 02:56:00.106030 chilitools-0.2.0/chilitools/api/endpoints.py
+-rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.0/chilitools/api/mycp.py
+-rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.0/chilitools/api/response.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.0/chilitools/grafx/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.0/chilitools/grafx/api/__init__.py
+-rw-r--r--   0        0        0     1517 2023-06-22 03:37:59.463934 chilitools-0.2.0/chilitools/grafx/api/environment.py
+-rw-r--r--   0        0        0     2232 2023-06-20 04:20:59.710105 chilitools-0.2.0/chilitools/grafx/auth.py
+-rw-r--r--   0        0        0     1796 2023-06-22 02:21:13.595697 chilitools-0.2.0/chilitools/grafx/connector.py
+-rw-r--r--   0        0        0      940 2023-06-22 03:35:09.815597 chilitools-0.2.0/chilitools/grafx/document.py
+-rw-r--r--   0        0        0      661 2023-06-20 20:56:54.535362 chilitools-0.2.0/chilitools/grafx/environment.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.0/chilitools/settings/__init__.py
+-rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.0/chilitools/settings/config.py
+-rw-r--r--   0        0        0    12468 2022-09-27 16:58:06.159255 chilitools-0.2.0/chilitools/utilities/ServerMigration.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.0/chilitools/utilities/__init__.py
+-rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.0/chilitools/utilities/backoffice.py
+-rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.0/chilitools/utilities/defaults.py
+-rw-r--r--   0        0        0     2069 2023-06-13 15:46:56.759605 chilitools-0.2.0/chilitools/utilities/document.py
+-rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.0/chilitools/utilities/errors.py
+-rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.0/chilitools/utilities/file.py
+-rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.0/chilitools/utilities/logger.py
+-rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.0/chilitools/utilities/strings.py
+-rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.0/chilitools/utilities/xmltools.py
+-rw-r--r--   0        0        0      505 2023-06-22 03:49:15.793073 chilitools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.0/PKG-INFO
```

### Comparing `chilitools-0.1.9/chilitools/api/mycp.py` & `chilitools-0.2.0/chilitools/api/mycp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,56 @@
+from operator import truediv
 import requests
+from os import getenv, remove
+from os.path import exists
 from chilitools.settings.config import LOGIN_FILE
 from chilitools.utilities.defaults import STAFF_TYPE, USER_TYPE
 from chilitools.utilities.file import checkForFile, readFile, writeFile
 
 
 def getCredentials() -> dict:
-  if checkForFile(fileName=LOGIN_FILE):
+  if getenv('CHILI_PUBLISH_USERNAME') is not None and getenv('CHILI_PUBLISH_PASSWORD') is not None:
+    login = {'type':STAFF_TYPE, 'credentials': { 'Username': getenv('CHILI_PUBLISH_USERNAME'), 'Password': getenv('CHILI_PUBLISH_PASSWORD') }}
+  elif checkForFile(fileName=LOGIN_FILE):
+    # Login was found in file, lets load it
     login = readFile(fileName=LOGIN_FILE, isJSON=True)
   else:
+    # Login not created yet, let's create one
     login = inputCredentials()
   return login
 
+def formatLogin(username: str, password: str, login_type: str = USER_TYPE) -> str:
+  return {'type':login_type, 'credentials': { 'Username': username, 'Password': password }}
+
+def writeLoginFile(login_info: dict) -> bool:
+  try:
+    writeFile(fileName=LOGIN_FILE, data=login_info, isJSON=True)
+    return True
+  except Exception as e:
+    print("There was an issue writing the login file")
+    return False
+
+def deleteLoginFile() -> bool:
+  try:
+    if exists(LOGIN_FILE):
+      remove(LOGIN_FILE)
+    return True
+  except Exception as e:
+    print(f"There was an issue deleting the login file: {e}")
+    return False
+
 def inputCredentials() -> dict:
   print("Please enter your CHILI username")
   username = input().strip()
   print("Please enter your CHILI password")
   password = input().strip()
-  login = {'type':USER_TYPE, 'credentials': { 'Username': username, 'Password': password }}
-  writeFile(fileName=LOGIN_FILE, data=login, isJSON=True)
+  login_type = STAFF_TYPE if "@" in username else USER_TYPE
+  if login_type == STAFF_TYPE: print("Staff account detected, configuring login details for staff login syntax")
+  login = formatLogin(username=username, password=password, login_type=login_type)
+  writeLoginFile(login_info=login)
   return login
 
 def setUserType(userType: str) -> bool:
   if checkForFile(fileName=LOGIN_FILE):
     login = readFile(fileName=LOGIN_FILE, isJSON=True)
     login['type'] = userType
   writeFile(fileName=LOGIN_FILE, data=login, isJSON=True)
@@ -32,39 +61,38 @@
 
     requestURL = "https://my.chili-publish.com/api/v1/auth/login"
 
     requestHeaders = {
         "Content-Type":"application/json",
         "accept": "*/*"
     }
-
     response = requests.post(url=requestURL, headers=requestHeaders, json=login['credentials'])
 
     if response.status_code != 200:
       return f"There was an error generating an OAuth Bearer Token. Status Code: {response.status_code}. Text: {response.text}"
     else:
       return response.json()['token']
   return "This method uses Azure AD OAuth login and is reserved for CHILI Staff"
 
 def generateLoginTokenForURL(backofficeURL: str) -> str:
   login = getCredentials()
   if login['type'] == STAFF_TYPE:
     requestURL = "https://my.chili-publish.com/api/v1/backoffice/generate"
 
     requestHeaders = {
-        "Content-Type":"application/json",
-        "accept": "application/json",
-        "Authorization": "Bearer " + generateOAuthTokenFromCredentials(login=login)
+      "content-type":"application/json",
+      "accept": "*/*",
+      "authorization": "Bearer " + generateOAuthTokenFromCredentials(login=login)
     }
 
     requestJSON = {
-        "Url":backofficeURL
+      "Url":backofficeURL
     }
 
     response = requests.post(url=requestURL, headers=requestHeaders, json=requestJSON)
 
     if response.status_code != 200:
-        return f"There was an error generating an login token. Status Code: {response.status_code}. Text: {response.text}"
+      return f"There was an error generating an login token. Status Code: {response.status_code}. Text: {response.text}"
     else:
-        return response.json()['token']
+      return response.json()['token']
   return "This method uses Azure AD OAuth login and is reserved for CHILI Staff"
```

### Comparing `chilitools-0.1.9/chilitools/api/response.py` & `chilitools-0.2.0/chilitools/api/response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import xmltodict
 import json
 
-from chilitools.utilities.defaults import statusCodes
+from typing import OrderedDict
 from requests import Response
+from chilitools.utilities.defaults import statusCodes
 
 class ChiliResponse:
 
     def __init__(self, response: Response):
         self.response = response
         self.statusCode = response.status_code
         self.success = False
@@ -47,30 +48,35 @@
 
     def contentAsDict(self) -> dict:
         return self.data
 
     def didSucceed(self) -> bool:
         return self.success
 
+    def getURL(self) -> str:
+        if 'urlInfo' in self.data:
+            return self.data['urlInfo']['@url']
+        return "There is no URL node found in the result that can be processed"
+
     def __repr__(self) -> str:
          return f'ChiliResponse(success={self.success}, statusCode={self.response.status_code}, statusDescription={self.statusDescription}, data={self.data}, contentType={self.type}, responseText={self.response.text})'
 
     def __str__(self) -> str:
         return f'ChiliResponse(success={self.success}, statusCode={self.response.status_code}, statusDescription={self.statusDescription}, data={self.data}, contentType={self.type}, responseText={self.response.text})'
 
     def __iter__(self):
         yield from self.data
 
     @property
     def text(self) -> str:
         return self.response.text
 
     @property
-    def content(self) -> bytes:
-        return self.response.content
+    def content(self) -> OrderedDict:
+        return self.contentAsDict()
 
     @property
     def json(self) -> str:
         return json.dumps(self.data)
 
     @property
     def status(self) -> dict:
```

### Comparing `chilitools-0.1.9/chilitools/utilities/defaults.py` & `chilitools-0.2.0/chilitools/utilities/defaults.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.1.9/chilitools/utilities/errors.py` & `chilitools-0.2.0/chilitools/utilities/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class ErrorHandler:
     def __init__(self):
          self.errors = {
             "FILENOTFOUND":"File not found",
-            "GENAPIKEY":"There was an issue generating an API key",
+            "GENAPIKEY":"There was an issue generating an API key, please make sure your login credentials are correct",
             "GENLOGINFORURL":"TODO",
             "GENOAUTH":"There was an error generating an OAuth token using the credentials files. Please ensure your username and password are correct.",
             "INVALIDBACKOFFICEURL": "The CHILI BackOffice URL entered can not be proceessed, please try again. The URL should end with interface.aspx",
             "TASKNOTSUCCEEDED": "The task did not succeed"
         }
 
     def getError(self, errorName):
```

### Comparing `chilitools-0.1.9/chilitools/utilities/file.py` & `chilitools-0.2.0/chilitools/utilities/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,134 @@
 from __future__ import annotations
 import requests
 import json
+from base64 import b64encode
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from chilitools.api.connector import ChiliConnector
 
-from os.path import isfile, dirname, realpath
+from os.path import isfile, dirname, realpath, sep, getsize
 from os import makedirs
 from chilitools.utilities.errors import ErrorHandler
-from chilitools.utilities.xml import getTaskResultURL
+from chilitools.utilities.strings import convertFileSize
+from chilitools.utilities.xmltools import getTaskResultURL, removeTimelineTags
 from chilitools.utilities.defaults import DEFAULT_TASKPRIORITY
 
-def currentPath() -> str:
-  return dirname(realpath(__file__))
+def currentPath(file: str) -> str:
+  return dirname(realpath(file))
 
-def readFile(fileName: str, isJSON: bool = False) -> dict:
+def getBase64String(filePath: str = None, fileBytes: bytes = None) -> str:
+  """Returns a string of the base64 encoded file bytes.
+  You can pass fileBytes directly or a file path to the file you would like to encode
+
+  :type filePath: str
+  :type fileBytes: bytes
+  """
+  if fileBytes and filePath is None:
+    return 'You must provide a file path or file bytes for this function'
+  if filePath is not None:
+    with open(filePath, 'rb') as file:
+      fileBytes = file.read()
+  fileData = b64encode(fileBytes)
+  return fileData.decode('utf-8')
+
+def readFile(fileName: str, isJSON: bool = False, encoding: str = None):
   if checkForFile(fileName=fileName):
-    with open(fileName, 'r') as file:
+    with open(fileName, 'r', encoding=encoding) as file:
       if isJSON:
         return json.loads(file.read())
       else:
         return file.read()
   else:
     return ErrorHandler().getError(errorName="FILENOTFOUND")
 
-def writeFile(fileName: str, data, isJSON: bool = False) -> None:
+def writeFile(fileName: str, data, isJSON: bool = False, encoding: str = None) -> None:
   makedirs(dirname(fileName), exist_ok=True)
-  with open(fileName, 'w') as file:
+  with open(fileName, 'w', encoding=encoding) as file:
     if isJSON:
       file.write(json.dumps(data))
     else:
       file.write(data)
 
 def checkForFile(fileName: str) -> bool:
   if isfile(fileName):
     return True
   return False
 
-def downloadFile(url: str, fullFileName: str) -> bool:
+def removeTimelineFromDocFile(fileName: str, outputFolder: str, verbose: bool = False) -> str:
+  # try:
+    print(f"File size before stripping tags: {convertFileSize(getsize(fileName), 'kb')}")
+    with open(file=fileName, mode='r') as file:
+      docXML = file.read()
+    docXML = removeTimelineTags(docXML=docXML, verbose=verbose)
+    # sep = os.path.sep
+    path = fileName.split(sep)
+    fileName = path.pop().split('.xml')[0]
+    outputFile = sep.join(path) + sep + outputFolder + fileName + '.xml'
+    makedirs(dirname(outputFile), exist_ok=True)
+    with open(file=outputFile, mode='w', encoding='utf-8') as file:
+      file.write(docXML)
+    print(f"File size after stripping tags: {convertFileSize(getsize(outputFile), 'kb')}")
+    return 'Successfully stripped timeline tags from document XML'
+  # except Exception as e:
+  #   return f'There was an issue removing the timeline docs: {e}'
+
+def downloadFile(url: str, fullFileName: str, queryParams: dict = None) -> bool:
+  if queryParams is None: queryParams = {}
   try:
-    download = requests.get(url=url, allow_redirects=True)
+    download = requests.get(url=url, allow_redirects=True, params=queryParams)
     open(fullFileName, 'wb').write(download.content)
     return True
   except Exception as e:
     print(e)
     return False
 
-def generateAndDownloadPDF(connector: ChiliConnector, fullFileName: str, documentID: str = None, documentXML: str = None, settingsXML: str = None, settingsID: str = None, taskPriority: int = DEFAULT_TASKPRIORITY, verbose: bool = False) -> str:
+def generateAndDownloadPDF(connector: ChiliConnector, fullFileName: str, documentID: str = None, documentXML: str = None, settingsXML: str = None, settingsID: str = None, taskPriority: int = DEFAULT_TASKPRIORITY, verbose: bool = False, downloadXML: bool = False) -> str:
+
   if documentID is None and documentXML is None:
     return 'You need to provide a document ID or document XML parameter'
+
   if settingsID is None and settingsXML is None:
     return "You need to provide a PDF Export Settings Item ID or PDF Export Settings XML"
+  
+  if downloadXML is True and documentID is not None:
+    if verbose: print("Downloading XML for document")
+    resp = connector.resources.ResourceItemGetXML(
+      resourceType="documents",
+      itemID=documentID
+    )
+    if not resp.didSucceed:
+      return "There was a problem getting the XML for the document"
+    documentXML = resp.text
+    documentID = None
+
   if settingsID is not None:
     print(f"Getting PDF Export Settings XML for {settingsID}")
     settingsXML = connector.resources.getPDFSettingsXML(settingsID=settingsID).text
+
   if documentID is not None:
     resp = connector.makeRequest(
       method='post',
       endpoint=f"/resources/documents/{documentID}/representations/pdf",
       queryParams={'taskPriority':taskPriority},
       json={'settingsXML':settingsXML}
     )
   elif documentXML is not None:
     resp = connector.documents.createTempPDF(documentXML=documentXML, settingsXML=settingsXML)
   if verbose: print(resp.text)
   if resp.didSucceed():
+    with open("C:\\Users\\Austin\\Desktop\\python_request.txt", "w") as file:
+      file.write(resp.response.request.body.decode('utf-8'))
     taskID = resp.contentAsDict()['task']['@id']
     task = connector.system.waitForTask(taskID=taskID, debug=verbose)
-    if task == ErrorHandler().getError("TASKNOTSUCCEEDED"):
-      return ErrorHandler().getError("TASKNOTSUCCEEDED")
-    success = downloadFile(url=getTaskResultURL(task=task), fullFileName=fullFileName)
+    resultURL = getTaskResultURL(task=task)
+    if resultURL == ErrorHandler().getError(errorName="TASKNOTSUCCEEDED"):
+      return False
+    success = downloadFile(url=resultURL, fullFileName=fullFileName)
     print(f"URL: {getTaskResultURL(task=task)}")
     if success:
       return (f"The file successfully downloaded to {fullFileName}")
     return "The file download process failed."
 
 def createAndDownloadImages(connector: ChiliConnector, documentID: str, imageConversionProfileID: str, settingsXML: str, taskPriority: int = DEFAULT_TASKPRIORITY):
   resp = connector.makeRequest(
@@ -83,8 +137,8 @@
     queryParams={'imageConversionProfileID':imageConversionProfileID, 'taskPriority':taskPriority},
     json={'settingsXML':settingsXML}
   )
   if resp.didSucceed():
     taskID = resp.contentAsDict()['task']['@id']
     task = connector.system.waitForTask(taskID=taskID)
     return task
-  return f"Request to make images failed: {resp.text}"
+  return f"Request to make images failed: {resp.text}"
```

