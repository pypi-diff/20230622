# Comparing `tmp/authomize-rest-api-client-4.2.9.tar.gz` & `tmp/authomize-rest-api-client-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.2.9.tar", last modified: Sat Jun 17 06:09:34 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.0.tar", last modified: Thu Jun 22 11:36:14 2023, max compression
```

## Comparing `authomize-rest-api-client-4.2.9.tar` & `authomize-rest-api-client-4.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.795064 authomize-rest-api-client-4.2.9/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76002 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37380 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190165 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89370 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-17 06:09:15.000000 authomize-rest-api-client-4.2.9/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-17 06:09:34.000000 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-17 06:09:34.000000 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 06:09:34.000000 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-06-17 06:09:34.000000 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 06:09:34.000000 authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-17 06:09:34.799064 authomize-rest-api-client-4.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-17 06:09:18.000000 authomize-rest-api-client-4.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76002 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43982 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190165 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102274 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-22 11:36:13.000000 authomize-rest-api-client-4.3.0/setup.py
```

### Comparing `authomize-rest-api-client-4.2.9/LICENSE.txt` & `authomize-rest-api-client-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/README.md` & `authomize-rest-api-client-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-30T13:58:26+00:00
+#   timestamp: 2023-06-22T11:14:48+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -17,14 +17,28 @@
 
 
 class AccessToType(Enum):
     asset = 'asset'
     grouping = 'grouping'
 
 
+class AccountRiskScore(BaseModel):
+    blastRadiusRiskScore: Optional[int] = Field(
+        default=None,
+        description='Blast Radius Risk Score',
+        title='Blastradiusriskscore',
+    )
+    takeoverRiskScore: Optional[int] = Field(
+        default=None, description='Takeover Risk Score', title='Takeoverriskscore'
+    )
+    overallRiskScore: Optional[int] = Field(
+        default=None, description='Overall Risk Score', title='Overallriskscore'
+    )
+
+
 class AddIncidentCommentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     content: constr(max_length=1025) = Field(
         ..., description='Content of comment.', title='Content'
     )
@@ -230,28 +244,64 @@
     startDate = 'startDate'
     endDate = 'endDate'
     createdAt = 'createdAt'
     reviewerType = 'reviewerType'
     templateName = 'templateName'
 
 
+class GroupExpansion(Enum):
+    sourceApp = 'sourceApp'
+    tags = 'tags'
+
+
+class GroupMembership(BaseModel):
+    actorName: Optional[str] = Field(
+        default=None, description='Name of the member.', title='Actorname'
+    )
+    actorType: Optional[str] = Field(
+        default=None, description='Type of the member', title='Actortype'
+    )
+    actorAuthomizeId: Optional[str] = Field(
+        default=None,
+        description='Authomizer ID of the member.',
+        title='Actorauthomizeid',
+    )
+    actorOriginId: Optional[str] = Field(
+        default=None, description='Origin ID of the member~', title='Actororiginid'
+    )
+
+
 class IdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[str]] = Field(
         default=[], alias='$in', description='In', title='$In'
     )
 
 
 class IdentityExpansion(Enum):
     account = 'account'
     tags = 'tags'
 
 
+class IdentityRiskScore(BaseModel):
+    takeoverRiskScore: Optional[int] = Field(
+        default=None, description='Takeover Risk Score', title='Takeoverriskscore'
+    )
+    blastRadiusRiskScore: Optional[int] = Field(
+        default=None,
+        description='Blast Radius Risk Score',
+        title='Blastradiusriskscore',
+    )
+    summaryRiskScore: Optional[int] = Field(
+        default=None, description='Summary Risk Score', title='Summaryriskscore'
+    )
+
+
 class IncidentExpansion(Enum):
     policy = 'policy'
     assignee = 'assignee'
 
 
 class IncidentsCreatedAtFilter(BaseModel):
     class Config:
@@ -363,15 +413,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.1.3', description='**version**', title='Version'
+        default='4.3.0', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -439,14 +489,54 @@
     user = 'user'
 
 
 class SearchAssetsSortFields(Enum):
     asset_name = 'asset.name'
 
 
+class SearchGroupsAppIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_eq: Optional[str] = Field(
+        default=None, alias='$eq', description='Equals To', title='$Eq'
+    )
+
+
+class SearchGroupsIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class SearchGroupsOriginIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class SearchGroupsSortFields(Enum):
+    group_name = 'group.name'
+
+
+class SearchGroupsUniqueIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
 class SearchIdentitiesFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     email: Optional[EmailFilter] = Field(
         default=None,
         description='Find identities by their email address',
@@ -513,14 +603,28 @@
     order: Optional[SortOrder] = Field(
         default='ASC',
         description='Sort by ascending or descending order (ascending is the default)',
         title='Order',
     )
 
 
+class SortSchemaSearchGroupsSortFields(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    fieldName: SearchGroupsSortFields = Field(
+        ..., description='Sort the results by field name', title='FieldName'
+    )
+    order: Optional[SortOrder] = Field(
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
+    )
+
+
 class SortSchemaSearchIdentitiesSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchIdentitiesSortFields = Field(
         ..., description='Sort the results by field name', title='FieldName'
     )
@@ -553,16 +657,16 @@
         title='Name',
     )
 
 
 class TagSchema(BaseModel):
     id: str = Field(..., description='Authomize ID for the Tag', title='Id')
     name: str = Field(..., description='Name of the tag', title='Name')
-    description: str = Field(
-        ..., description='Description of the tag', title='Description'
+    description: Optional[str] = Field(
+        default=None, description='Description of the tag', title='Description'
     )
 
 
 class UniqueIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -613,20 +717,20 @@
     )
 
 
 class AssetSchema(BaseModel):
     authomizeId: str = Field(
         ..., description='Authomize ID of source application', title='Authomizeid'
     )
-    name: str = Field(
-        ...,
+    name: Optional[str] = Field(
+        default=None,
         description='Name of the asset (for example, application, virtual machine, file, etc.)',
         title='Name',
     )
-    type: str = Field(..., description='Type of asset', title='Type')
+    type: Optional[str] = Field(default=None, description='Type of asset', title='Type')
     originType: Optional[str] = Field(
         default=None,
         description='The type of asset on the source system',
         title='Origintype',
     )
     sourceApp: Optional[SourceAppSchema] = Field(
         default=None,
@@ -735,31 +839,52 @@
     values: List[Ccm402Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='ccm402', description='UniqueID', title='Id')
     name: Optional[str] = Field(
         default='CSA STAR (CCM 4.0.2)', description='Name', title='Name'
     )
 
 
-class Chainable(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    originId: Optional[OriginIdFilter] = Field(
-        default=None, description='Origin ID of the Asset.', title='Originid'
+class GroupSchema(BaseModel):
+    authomizeId: str = Field(
+        ..., description='Authomize ID of the Group.', title='Authomizeid'
     )
-    appId: Optional[AppIdFilter] = Field(
-        default=None, description='Find assets by their app ID', title='Appid'
+    name: Optional[str] = Field(
+        default=None, description='Name of the Group.', title='Name'
     )
-    uniqueId: Optional[UniqueIdFilter] = Field(
-        default=None, description='Find assets by their unique ID', title='Uniqueid'
+    type: Optional[str] = Field(
+        default=None, description='Type of the group.', title='Type'
     )
-    authomizeId: Optional[AssetIdFilter] = Field(
+    incidentsCount: Optional[int] = Field(
         default=None,
-        description='Find assets by their Authomize ID',
-        title='Authomizeid',
+        description='Number of incidents associated with the group.',
+        title='Incidentscount',
+    )
+    tags: Optional[List[TagSchema]] = Field(
+        default=None, description='List of tags associated with the group', title='Tags'
+    )
+    members: Optional[List[GroupMembership]] = Field(
+        default=[],
+        description='Entities that have direct access to the group.',
+        title='Members',
+    )
+    sourceApp: Optional[SourceAppSchema] = Field(
+        default=None, description='Authomize ID of the Group.', title='Sourceapp'
+    )
+    ownerId: Optional[str] = Field(
+        default=None, description='Authomize ID of the Group Owner.', title='Ownerid'
+    )
+    originId: Optional[str] = Field(
+        default=None,
+        description='The ID of the group on the source system',
+        title='Originid',
+    )
+    uniqueId: Optional[str] = Field(
+        default=None,
+        description='The unique ID of the group (as provided by the connector)',
+        title='Uniqueid',
     )
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
@@ -774,14 +899,17 @@
     email: Optional[str] = Field(default=None, description='Email', title='Email')
     originId: Optional[str] = Field(
         default=None, description='Origin ID', title='Originid'
     )
     originType: Optional[str] = Field(
         default=None, description='Origin Type', title='Origintype'
     )
+    riskScore: Optional[IdentityRiskScore] = Field(
+        default=None, description='Risk Scores', title='Riskscore'
+    )
 
 
 class IncidentsSeverityFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[SeverityType]] = Field(
@@ -824,14 +952,26 @@
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[CampaignSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
+class PaginatedResponseSchemaGroupSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    pagination: Optional[PaginationResponseSchema] = Field(
+        default=None, description='Pagination Metadata', title='Pagination'
+    )
+    data: List[GroupSchema] = Field(
+        ..., description='List of Actual Data', title='Data'
+    )
+
+
 class RawIdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
     name: Optional[str] = Field(
         default=None, description='Name of the identity', title='Name'
     )
     title: Optional[str] = Field(
         default=None, description='Title of the identity', title='Title'
@@ -885,24 +1025,24 @@
 
 class SearchAssetsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchAssetsSortFields]] = Field(
         default=None,
-        description='Sort the results by identity name in ascending or descending order',
+        description="Sort the results by asset's name in ascending or descending order",
         title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[AssetExpansion]] = Field(
         default=None, description='Expand fields (to show additional information)'
     )
-    filter: Optional[Chainable] = Field(
+    filter: Optional[SearchAssetsFilterBody] = Field(
         default=None,
         description='Find assets by their ID on the source system',
         title='Filter',
     )
 
 
 class SearchCampaignPermissionsRequestSchema(BaseModel):
@@ -931,19 +1071,41 @@
         default=None, description='Expand Fields'
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None,
-        description='Sort the results by identity name in ascending or descending order',
+        description='Sort the results by campaign fields in ascending or descending order',
         title='Sort',
     )
 
 
+class SearchGroupsRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    sort: Optional[List[SortSchemaSearchGroupsSortFields]] = Field(
+        default=None,
+        description="Sort the results by group's name in ascending or descending order",
+        title='Sort',
+    )
+    pagination: Optional[PaginationRequestSchema] = Field(
+        default=None, description='Pagination metadata', title='Pagination'
+    )
+    expand: Optional[List[GroupExpansion]] = Field(
+        default=None, description='Expand fields (to show additional information)'
+    )
+    filter: Optional[SearchGroupsFilterBody] = Field(
+        default=None,
+        description='Find groups by their ID on the source system',
+        title='Filter',
+    )
+
+
 class SearchIdentitiesRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchIdentitiesSortFields]] = Field(
         default=None,
         description='Sort the results by identity name in ascending or descending order',
@@ -996,15 +1158,15 @@
         default=None, description='Filter', title='Filter'
     )
     expand: Optional[List[IncidentExpansion]] = Field(
         default=None, description='Expend'
     )
     sort: Optional[List[SortSchemaSearchIncidentsSortFields]] = Field(
         default=None,
-        description='Sort the results by identity name in ascending or descending order',
+        description='Sort the results by incident fields in ascending or descending order',
         title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
 
 
@@ -1041,15 +1203,18 @@
     )
     isAdmin: Optional[bool] = Field(
         default=None,
         description='Is the account an admin account (Yes or No)',
         title='Isadmin',
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='List of tags associated with the asset', title='Tags'
+        default=None, description='Tags associated with the account.', title='Tags'
+    )
+    riskScore: Optional[AccountRiskScore] = Field(
+        default=None, description='Risk Scores for the Account.', title='Riskscore'
     )
 
 
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
@@ -1126,14 +1291,17 @@
         title='Incidentscount',
     )
     accounts: Optional[List[AccountSchema]] = Field(
         default=[],
         description='List of associated user or service accounts',
         title='Accounts',
     )
+    riskScore: Optional[IdentityRiskScore] = Field(
+        default=None, description='Risk Scores', title='Riskscore'
+    )
 
 
 class IncidentSchema(BaseModel):
     id: str = Field(..., description='Unique id', title='Id')
     createdAt: Optional[datetime] = Field(
         default=None,
         description='The date the incident was first reported.',
@@ -1229,7 +1397,47 @@
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[IncidentSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
+
+
+class SearchAssetsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    originId: Optional[OriginIdFilter] = Field(
+        default=None, description='Find assets by their origin ID', title='Originid'
+    )
+    appId: Optional[AppIdFilter] = Field(
+        default=None, description='Find assets by their app ID', title='Appid'
+    )
+    uniqueId: Optional[UniqueIdFilter] = Field(
+        default=None, description='Find assets by their unique ID', title='Uniqueid'
+    )
+    authomizeId: Optional[AssetIdFilter] = Field(
+        default=None,
+        description='Find assets by their Authomize ID',
+        title='Authomizeid',
+    )
+
+
+class SearchGroupsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
+        default=None, description='Find groups by their unique ID', title='Uniqueid'
+    )
+    originId: Optional[SearchGroupsOriginIdFilter] = Field(
+        default=None, description='Find groups by their origin ID', title='Originid'
+    )
+    appId: Optional[SearchGroupsAppIdFilter] = Field(
+        default=None, description='Find groups by their app ID', title='Appid'
+    )
+    authomizeId: Optional[SearchGroupsIdFilter] = Field(
+        default=None,
+        description='Find groups by their Authomize ID',
+        title='Authomizeid',
+    )
```

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.976013845198139%*

 * *Differences: {"'components'": "{'schemas': {'AccountSchema': {'properties': {'tags': {'description': 'Tags "*

 * *                 "associated with the account.'}, 'riskScore': OrderedDict([('title', "*

 * *                 "'Riskscore'), ('allOf', [OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/AccountRiskScore')])]), ('description', 'Risk Scores for "*

 * *                 "the Account.')])}}, 'AssetSchema': {'required': {delete: [2, 1]}}, "*

 * *                 "'IdentitySchema': {'properties': {'riskScore': OrderedDic […]*

```diff
@@ -15,14 +15,35 @@
                 "enum": [
                     "asset",
                     "grouping"
                 ],
                 "title": "AccessToType",
                 "type": "string"
             },
+            "AccountRiskScore": {
+                "properties": {
+                    "blastRadiusRiskScore": {
+                        "description": "Blast Radius Risk Score",
+                        "title": "Blastradiusriskscore",
+                        "type": "integer"
+                    },
+                    "overallRiskScore": {
+                        "description": "Overall Risk Score",
+                        "title": "Overallriskscore",
+                        "type": "integer"
+                    },
+                    "takeoverRiskScore": {
+                        "description": "Takeover Risk Score",
+                        "title": "Takeoverriskscore",
+                        "type": "integer"
+                    }
+                },
+                "title": "AccountRiskScore",
+                "type": "object"
+            },
             "AccountSchema": {
                 "properties": {
                     "authomizeId": {
                         "description": "Unique ID",
                         "title": "Authomizeid",
                         "type": "string"
                     },
@@ -61,25 +82,34 @@
                         "type": "string"
                     },
                     "originId": {
                         "description": "The identifier of the account from the source system.",
                         "title": "Originid",
                         "type": "string"
                     },
+                    "riskScore": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AccountRiskScore"
+                            }
+                        ],
+                        "description": "Risk Scores for the Account.",
+                        "title": "Riskscore"
+                    },
                     "sourceApp": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "Associated source app ",
                         "title": "Sourceapp"
                     },
                     "tags": {
-                        "description": "List of tags associated with the asset",
+                        "description": "Tags associated with the account.",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
                     "type": {
@@ -298,17 +328,15 @@
                     "uniqueId": {
                         "description": "The unique ID of the asset (as provided by the connector)",
                         "title": "Uniqueid",
                         "type": "string"
                     }
                 },
                 "required": [
-                    "authomizeId",
-                    "name",
-                    "type"
+                    "authomizeId"
                 ],
                 "title": "AssetSchema",
                 "type": "object"
             },
             "AttackTacticType": {
                 "description": "An enumeration.",
                 "enum": [
@@ -666,58 +694,14 @@
                     "AIS-03",
                     "DSP-17",
                     "DSP-01",
                     "HRS-05"
                 ],
                 "title": "Ccm402Standard"
             },
-            "Chainable": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "appId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/AppIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their app ID",
-                        "title": "Appid"
-                    },
-                    "authomizeId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/AssetIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their Authomize ID",
-                        "title": "Authomizeid"
-                    },
-                    "originId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/OriginIdFilter"
-                            }
-                        ],
-                        "description": "Origin ID of the Asset.",
-                        "title": "Originid"
-                    },
-                    "uniqueId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/UniqueIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their unique ID",
-                        "title": "Uniqueid"
-                    }
-                },
-                "title": "Chainable",
-                "type": "object"
-            },
             "CisV8Standard": {
                 "description": "An enumeration.",
                 "enum": [
                     "3.1",
                     "3.3",
                     "6.8",
                     "5.4",
@@ -821,14 +805,119 @@
                     "endDate",
                     "createdAt",
                     "reviewerType",
                     "templateName"
                 ],
                 "title": "FieldName"
             },
+            "GroupExpansion": {
+                "description": "An enumeration.",
+                "enum": [
+                    "sourceApp",
+                    "tags"
+                ],
+                "title": "GroupExpansion",
+                "type": "string"
+            },
+            "GroupMembership": {
+                "properties": {
+                    "actorAuthomizeId": {
+                        "description": "Authomizer ID of the member.",
+                        "title": "Actorauthomizeid",
+                        "type": "string"
+                    },
+                    "actorName": {
+                        "description": "Name of the member.",
+                        "title": "Actorname",
+                        "type": "string"
+                    },
+                    "actorOriginId": {
+                        "description": "Origin ID of the member~",
+                        "title": "Actororiginid",
+                        "type": "string"
+                    },
+                    "actorType": {
+                        "description": "Type of the member",
+                        "title": "Actortype",
+                        "type": "string"
+                    }
+                },
+                "title": "GroupMembership",
+                "type": "object"
+            },
+            "GroupSchema": {
+                "properties": {
+                    "authomizeId": {
+                        "description": "Authomize ID of the Group.",
+                        "title": "Authomizeid",
+                        "type": "string"
+                    },
+                    "incidentsCount": {
+                        "description": "Number of incidents associated with the group.",
+                        "title": "Incidentscount",
+                        "type": "integer"
+                    },
+                    "members": {
+                        "default": [],
+                        "description": "Entities that have direct access to the group.",
+                        "items": {
+                            "$ref": "#/components/schemas/GroupMembership"
+                        },
+                        "title": "Members",
+                        "type": "array"
+                    },
+                    "name": {
+                        "description": "Name of the Group.",
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "originId": {
+                        "description": "The ID of the group on the source system",
+                        "title": "Originid",
+                        "type": "string"
+                    },
+                    "ownerId": {
+                        "description": "Authomize ID of the Group Owner.",
+                        "title": "Ownerid",
+                        "type": "string"
+                    },
+                    "sourceApp": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SourceAppSchema"
+                            }
+                        ],
+                        "description": "Authomize ID of the Group.",
+                        "title": "Sourceapp"
+                    },
+                    "tags": {
+                        "description": "List of tags associated with the group",
+                        "items": {
+                            "$ref": "#/components/schemas/TagSchema"
+                        },
+                        "title": "Tags",
+                        "type": "array"
+                    },
+                    "type": {
+                        "description": "Type of the group.",
+                        "title": "Type",
+                        "type": "string"
+                    },
+                    "uniqueId": {
+                        "description": "The unique ID of the group (as provided by the connector)",
+                        "title": "Uniqueid",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "authomizeId"
+                ],
+                "title": "GroupSchema",
+                "type": "object"
+            },
             "HTTPValidationError": {
                 "properties": {
                     "detail": {
                         "items": {
                             "$ref": "#/components/schemas/ValidationError"
                         },
                         "title": "Detail",
@@ -859,14 +948,35 @@
                 "enum": [
                     "account",
                     "tags"
                 ],
                 "title": "IdentityExpansion",
                 "type": "string"
             },
+            "IdentityRiskScore": {
+                "properties": {
+                    "blastRadiusRiskScore": {
+                        "description": "Blast Radius Risk Score",
+                        "title": "Blastradiusriskscore",
+                        "type": "integer"
+                    },
+                    "summaryRiskScore": {
+                        "description": "Summary Risk Score",
+                        "title": "Summaryriskscore",
+                        "type": "integer"
+                    },
+                    "takeoverRiskScore": {
+                        "description": "Takeover Risk Score",
+                        "title": "Takeoverriskscore",
+                        "type": "integer"
+                    }
+                },
+                "title": "IdentityRiskScore",
+                "type": "object"
+            },
             "IdentitySchema": {
                 "properties": {
                     "accountIds": {
                         "default": [],
                         "description": "The account IDs associated with the identity",
                         "items": {
                             "type": "string"
@@ -909,14 +1019,23 @@
                         "type": "integer"
                     },
                     "name": {
                         "description": "Name of the identity",
                         "title": "Name",
                         "type": "string"
                     },
+                    "riskScore": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/IdentityRiskScore"
+                            }
+                        ],
+                        "description": "Risk Scores",
+                        "title": "Riskscore"
+                    },
                     "tags": {
                         "description": "The tags provided for the identity",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
@@ -972,14 +1091,23 @@
                         "title": "Originid",
                         "type": "string"
                     },
                     "originType": {
                         "description": "Origin Type",
                         "title": "Origintype",
                         "type": "string"
+                    },
+                    "riskScore": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/IdentityRiskScore"
+                            }
+                        ],
+                        "description": "Risk Scores",
+                        "title": "Riskscore"
                     }
                 },
                 "required": [
                     "id",
                     "object"
                 ],
                 "title": "IncidentEntitiesSchema",
@@ -1372,15 +1500,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.1.3",
+                        "default": "4.3.0",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1558,14 +1686,41 @@
                 },
                 "required": [
                     "data"
                 ],
                 "title": "PaginatedResponseSchema[CampaignsPermissionSchema]",
                 "type": "object"
             },
+            "PaginatedResponseSchema_GroupSchema_": {
+                "additionalProperties": false,
+                "properties": {
+                    "data": {
+                        "description": "List of Actual Data",
+                        "items": {
+                            "$ref": "#/components/schemas/GroupSchema"
+                        },
+                        "title": "Data",
+                        "type": "array"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationResponseSchema"
+                            }
+                        ],
+                        "description": "Pagination Metadata",
+                        "title": "Pagination"
+                    }
+                },
+                "required": [
+                    "data"
+                ],
+                "title": "PaginatedResponseSchema[GroupSchema]",
+                "type": "object"
+            },
             "PaginatedResponseSchema_IdentitySchema_": {
                 "additionalProperties": false,
                 "properties": {
                     "data": {
                         "description": "List of Actual Data",
                         "items": {
                             "$ref": "#/components/schemas/IdentitySchema"
@@ -1848,15 +2003,15 @@
                             "$ref": "#/components/schemas/AssetExpansion"
                         },
                         "type": "array"
                     },
                     "filter": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/Chainable"
+                                "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody__"
                             }
                         ],
                         "description": "Find assets by their ID on the source system",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
@@ -1864,15 +2019,15 @@
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
                         "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort the results by identity name in ascending or descending order",
+                        "description": "Sort the results by asset's name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchAssetsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -1946,25 +2101,134 @@
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
                         "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort the results by identity name in ascending or descending order",
+                        "description": "Sort the results by campaign fields in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_FieldName_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
                 "title": "SearchCampaignsRequestSchema",
                 "type": "object"
             },
+            "SearchGroupsAppIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$eq": {
+                        "description": "Equals To",
+                        "title": "$Eq",
+                        "type": "string"
+                    }
+                },
+                "title": "SearchGroupsAppIdFilter",
+                "type": "object"
+            },
+            "SearchGroupsIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchGroupsIdFilter",
+                "type": "object"
+            },
+            "SearchGroupsOriginIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchGroupsOriginIdFilter",
+                "type": "object"
+            },
+            "SearchGroupsRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "expand": {
+                        "description": "Expand fields (to show additional information)",
+                        "items": {
+                            "$ref": "#/components/schemas/GroupExpansion"
+                        },
+                        "type": "array"
+                    },
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody__"
+                            }
+                        ],
+                        "description": "Find groups by their ID on the source system",
+                        "title": "Filter"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationRequestSchema"
+                            }
+                        ],
+                        "description": "Pagination metadata",
+                        "title": "Pagination"
+                    },
+                    "sort": {
+                        "description": "Sort the results by group's name in ascending or descending order",
+                        "items": {
+                            "$ref": "#/components/schemas/SortSchema_SearchGroupsSortFields_"
+                        },
+                        "title": "Sort",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchGroupsRequestSchema",
+                "type": "object"
+            },
+            "SearchGroupsSortFields": {
+                "description": "An enumeration.",
+                "enum": [
+                    "group.name"
+                ],
+                "title": "SearchGroupsSortFields",
+                "type": "string"
+            },
+            "SearchGroupsUniqueIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchGroupsUniqueIdFilter",
+                "type": "object"
+            },
             "SearchIdentitiesFilterBody": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "authomizeId": {
                         "allOf": [
                             {
@@ -2133,15 +2397,15 @@
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
                         "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort the results by identity name in ascending or descending order",
+                        "description": "Sort the results by incident fields in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchIncidentsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -2242,14 +2506,43 @@
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[SearchAssetsSortFields]",
                 "type": "object"
             },
+            "SortSchema_SearchGroupsSortFields_": {
+                "additionalProperties": false,
+                "properties": {
+                    "fieldName": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsSortFields"
+                            }
+                        ],
+                        "description": "Sort the results by field name",
+                        "title": "FieldName"
+                    },
+                    "order": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SortOrder"
+                            }
+                        ],
+                        "default": "ASC",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
+                        "title": "Order"
+                    }
+                },
+                "required": [
+                    "fieldName"
+                ],
+                "title": "SortSchema[SearchGroupsSortFields]",
+                "type": "object"
+            },
             "SortSchema_SearchIdentitiesSortFields_": {
                 "additionalProperties": false,
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchIdentitiesSortFields"
@@ -2340,16 +2633,15 @@
                         "description": "Name of the tag",
                         "title": "Name",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
-                    "name",
-                    "description"
+                    "name"
                 ],
                 "title": "TagSchema",
                 "type": "object"
             },
             "UniqueIdFilter": {
                 "additionalProperties": false,
                 "properties": {
@@ -2448,28 +2740,116 @@
                 "required": [
                     "loc",
                     "msg",
                     "type"
                 ],
                 "title": "ValidationError",
                 "type": "object"
+            },
+            "_class__authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody__": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "appId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AppIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their app ID",
+                        "title": "Appid"
+                    },
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AssetIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their Authomize ID",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/OriginIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their origin ID",
+                        "title": "Originid"
+                    },
+                    "uniqueId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/UniqueIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their unique ID",
+                        "title": "Uniqueid"
+                    }
+                },
+                "title": "<class 'authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody'>",
+                "type": "object"
+            },
+            "_class__authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody__": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "appId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsAppIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their app ID",
+                        "title": "Appid"
+                    },
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their Authomize ID",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsOriginIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their origin ID",
+                        "title": "Originid"
+                    },
+                    "uniqueId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsUniqueIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their unique ID",
+                        "title": "Uniqueid"
+                    }
+                },
+                "title": "<class 'authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody'>",
+                "type": "object"
             }
         },
         "securitySchemes": {
             "APIKeyHeader": {
                 "in": "header",
                 "name": "Authorization",
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.3",
+        "version": "4.3.0",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -3075,14 +3455,61 @@
                 ],
                 "summary": "Search Assets",
                 "tags": [
                     "Inventory"
                 ]
             }
         },
+        "/v2/inventory/groups/search": {
+            "post": {
+                "description": "Find specific groups on Authomize and get related data (as found on the group\u2019s Single Entity page)",
+                "operationId": "search_groups_v2_inventory_groups_search_post",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/SearchGroupsRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/PaginatedResponseSchema_GroupSchema_"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Search Groups",
+                "tags": [
+                    "Inventory"
+                ]
+            }
+        },
         "/v2/inventory/identities/search": {
             "post": {
                 "description": "Find specific identities on Authomize and get related data (as found on Identity Single Entity page). Search by email address or AuthomizeID.",
                 "operationId": "search_identities_v2_inventory_identities_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
```

### Comparing `authomize-rest-api-client-4.2.9/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.9/setup.py` & `authomize-rest-api-client-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.2.9',
+        version='4.3.0',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

