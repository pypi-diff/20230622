# Comparing `tmp/pma_python-2.0.0.97.tar.gz` & `tmp/pma_python-2.0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pma_python-2.0.0.97.tar", last modified: Thu Jul 18 16:02:08 2019, max compression
+gzip compressed data, was "dist\pma_python-2.0.0.98.tar", last modified: Mon Jul 22 13:48:10 2019, max compression
```

## Comparing `pma_python-2.0.0.97.tar` & `pma_python-2.0.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2019-07-18 16:02:08.000000 pma_python-2.0.0.97/
--rw-rw-rw-   0        0        0     3225 2019-07-18 16:02:08.000000 pma_python-2.0.0.97/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2019-05-30 20:11:12.000000 pma_python-2.0.0.97/README.md
--rw-rw-rw-   0        0        0     2303 2019-05-30 20:11:12.000000 pma_python-2.0.0.97/long_desc.txt
-drwxrwxrwx   0        0        0        0 2019-07-18 16:02:08.000000 pma_python-2.0.0.97/pma_python/
--rw-rw-rw-   0        0        0      108 2019-06-24 16:26:38.000000 pma_python-2.0.0.97/pma_python/__init__.py
--rw-rw-rw-   0        0        0    15904 2019-07-18 15:57:47.000000 pma_python-2.0.0.97/pma_python/control.py
--rw-rw-rw-   0        0        0    35377 2019-07-16 13:43:15.000000 pma_python-2.0.0.97/pma_python/core.py
--rw-rw-rw-   0        0        0     4953 2019-07-16 08:50:20.000000 pma_python-2.0.0.97/pma_python/core_admin.py
--rw-rw-rw-   0        0        0    26038 2019-06-07 12:52:55.000000 pma_python-2.0.0.97/pma_python/my.py
--rw-rw-rw-   0        0        0     1202 2019-07-18 16:00:35.000000 pma_python-2.0.0.97/pma_python/pma.py
--rw-rw-rw-   0        0        0     1317 2019-07-11 09:17:59.000000 pma_python-2.0.0.97/pma_python/view.py
-drwxrwxrwx   0        0        0        0 2019-07-18 16:02:08.000000 pma_python-2.0.0.97/pma_python.egg-info/
--rw-rw-rw-   0        0        0     3225 2019-07-18 16:02:07.000000 pma_python-2.0.0.97/pma_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2019-07-18 16:02:07.000000 pma_python-2.0.0.97/pma_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-07-18 16:02:07.000000 pma_python-2.0.0.97/pma_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-06-11 14:02:39.000000 pma_python-2.0.0.97/pma_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2019-07-18 16:02:07.000000 pma_python-2.0.0.97/pma_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2019-07-18 16:02:07.000000 pma_python-2.0.0.97/pma_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-07-18 16:02:08.000000 pma_python-2.0.0.97/setup.cfg
--rw-rw-rw-   0        0        0     1008 2019-05-30 20:11:12.000000 pma_python-2.0.0.97/setup.py
+drwxrwxrwx   0        0        0        0 2019-07-22 13:48:10.000000 pma_python-2.0.0.98/
+-rw-rw-rw-   0        0        0     3225 2019-07-22 13:48:10.000000 pma_python-2.0.0.98/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2019-05-30 20:11:12.000000 pma_python-2.0.0.98/README.md
+-rw-rw-rw-   0        0        0     2303 2019-05-30 20:11:12.000000 pma_python-2.0.0.98/long_desc.txt
+drwxrwxrwx   0        0        0        0 2019-07-22 13:48:10.000000 pma_python-2.0.0.98/pma_python/
+-rw-rw-rw-   0        0        0      108 2019-06-24 16:26:38.000000 pma_python-2.0.0.98/pma_python/__init__.py
+-rw-rw-rw-   0        0        0    16588 2019-07-22 13:29:25.000000 pma_python-2.0.0.98/pma_python/control.py
+-rw-rw-rw-   0        0        0    35377 2019-07-16 13:43:15.000000 pma_python-2.0.0.98/pma_python/core.py
+-rw-rw-rw-   0        0        0     4953 2019-07-16 08:50:20.000000 pma_python-2.0.0.98/pma_python/core_admin.py
+-rw-rw-rw-   0        0        0    26038 2019-06-07 12:52:55.000000 pma_python-2.0.0.98/pma_python/my.py
+-rw-rw-rw-   0        0        0     1202 2019-07-22 13:42:53.000000 pma_python-2.0.0.98/pma_python/pma.py
+-rw-rw-rw-   0        0        0     1317 2019-07-11 09:17:59.000000 pma_python-2.0.0.98/pma_python/view.py
+drwxrwxrwx   0        0        0        0 2019-07-22 13:48:10.000000 pma_python-2.0.0.98/pma_python.egg-info/
+-rw-rw-rw-   0        0        0     3225 2019-07-22 13:48:09.000000 pma_python-2.0.0.98/pma_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2019-07-22 13:48:09.000000 pma_python-2.0.0.98/pma_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-07-22 13:48:09.000000 pma_python-2.0.0.98/pma_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-06-11 14:02:39.000000 pma_python-2.0.0.98/pma_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2019-07-22 13:48:09.000000 pma_python-2.0.0.98/pma_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2019-07-22 13:48:09.000000 pma_python-2.0.0.98/pma_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-07-22 13:48:10.000000 pma_python-2.0.0.98/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2019-05-30 20:11:12.000000 pma_python-2.0.0.98/setup.py
```

### Comparing `pma_python-2.0.0.97/PKG-INFO` & `pma_python-2.0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pma_python
-Version: 2.0.0.97
+Version: 2.0.0.98
 Summary: Universal viewing of digital microscopy, whole slide imaging and digital pathology data
 Home-page: http://github.com/pathomation/pma_python
 Author: Pathomation
 Author-email: info@pathomation.com
 License: http://free.pathomation.com/eula/
 Description: pma_python is a Python wrapper library for PMA.start (http://free.pathomation.com),
         a universal viewer by Pathomation for whole slide imaging and microscopy.
```

### Comparing `pma_python-2.0.0.97/README.md` & `pma_python-2.0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/long_desc.txt` & `pma_python-2.0.0.98/long_desc.txt`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/pma_python/control.py` & `pma_python-2.0.0.98/pma_python/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,42 +154,47 @@
 	#if is_participant_in_training_session(pmacontrolURL, participantUsername, pmacontrolSessionID, pmacoreSessionID):
 	#	raise NameError ("PMA.core user " + participantUsername + " is ALREADY registered in PMA.control training session " + str(pmacontrolSessionID))
 	url = pma._pma_join(pmacontrolURL, "api/Sessions/") + str(pmacontrolSessionID) + "/AddParticipant?SessionID=" + pmacoreSessionID
 	data = { "UserName": participantUsername, "Role": pmacontrolRole}   # default interaction mode = Locked
 	data = parse.urlencode(data).encode()
 	if (pma._pma_debug == True):
 		print("Posting to", url)
+		print("   with payload", data)
 	req =  request.Request(url=url, data=data) # this makes the method "POST"
 	resp = request.urlopen(req)
 	pma._pma_clear_url_cache()
 	return resp
 
-def register_participant_for_project(pmacontrolURL, participantUsername, pmacontrolProjectID, pmacontrolRole, pmacoreSessionID):
+def register_participant_for_project(pmacontrolURL, participantUsername, pmacontrolProjectID, pmacontrolRole, pmacoreSessionID, pmacontrolInteractionMode = pma_interaction_mode_locked):
 	"""
 	Registers a participant for all sessions in a given project, assigning a specific role
 	"""
-	registered_sessions = []
-	for session in get_training_sessions(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
-		register_participant_for_training_session(pmacontrolURL, participantUsername, session, pmacontrolRole, pmacoreSessionID)
-		registered_sessions.append(session)
+	url = pma._pma_join(pmacontrolURL, "api/Projects/") + str(pmacontrolProjectID) + "/AddParticipant?SessionID=" + pmacoreSessionID
+	data = { "UserName": participantUsername, "Role": pmacontrolRole, "InteractionMode": pmacontrolInteractionMode }   # default interaction mode = Locked
+	data = parse.urlencode(data).encode()
 	if (pma._pma_debug == True):
-		print(participantUsername, "is now registered in", registered_sessions)
-	return registered_sessions
+		print("Posting to", url)
+		print("   with payload", data)
+	req =  request.Request(url=url, data=data) # this makes the method "POST"
+	resp = request.urlopen(req)
+	pma._pma_clear_url_cache()
+	return resp
 
 def set_participant_interactionmode(pmacontrolURL, participantUsername, pmacontrolSessionID, pmacontrolCaseCollectionID, pmacontrolInteractionMode, pmacoreSessionID):
 	"""
 	Assign an interaction mode to a particpant for a given Case Collection within a trainingsession
 	"""
 	if not is_participant_in_training_session(pmacontrolURL, participantUsername, pmacontrolSessionID, pmacoreSessionID):
 		raise NameError ("PMA.core user " + participantUsername + " is NOT registered in PMA.control training session " + str(pmacontrolSessionID))
 	url = pma._pma_join(pmacontrolURL, "api/Sessions/") + str(pmacontrolSessionID) + "/InteractionMode?SessionID=" + pmacoreSessionID
 	data = { "UserName": participantUsername, "CaseCollectionId": pmacontrolCaseCollectionID, "InteractionMode": pmacontrolInteractionMode }   
 	data = parse.urlencode(data).encode()
 	if (pma._pma_debug == True):
 		print("Posting to", url)
+		print("   with payload", data)
 	req =  request.Request(url=url, data=data) # this makes the method "POST"
 	resp = request.urlopen(req)
 	pma._pma_clear_url_cache()
 	return resp
 
 def get_training_session_titles(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
 	"""
@@ -211,14 +216,28 @@
 		if pmacontrolProjectID == None:
 			dct[sess["Id"]] = sess["Title"]
 		elif pmacontrolProjectID == sess["ProjectId"]:
 			dct[sess["Id"]] = sess["Title"]
 
 	return dct
 
+def get_training_sessions(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
+	"""
+	Retrieve (training) sessions (possibly filtered by project ID), return a dictionary of session IDs and titles
+	"""
+	dct = {}
+	all = _pma_get_training_sessions(pmacontrolURL, pmacoreSessionID)
+	for sess in all:
+		if pmacontrolProjectID == None:
+			dct[sess["Id"]] = _pma_format_training_session_properly(sess)
+		elif pmacontrolProjectID == sess["ProjectId"]:
+			dct[sess["Id"]] = _pma_format_training_session_properly(sess)
+
+	return dct
+
 def get_training_session(pmacontrolURL, pmacontrolSessionID, pmacoreSessionID):
 	"""
 	Return the first (training) session with ID = pmacontrolSessionID
 	"""
 	all = _pma_get_training_sessions(pmacontrolURL, pmacoreSessionID)
 
 	for el in all:
@@ -247,29 +266,28 @@
 	(RAW JSON data; not suited for human consumption)
 	"""
 	global _pma_casecollections_json
 	
 	url = pma._pma_join(pmacontrolURL, "api/CaseCollections?sessionID=" + pma._pma_q(pmacoreSessionID))
 	try:
 		headers = {'Accept': 'application/json'}
-		# r = requests.get(url, headers=headers)
 		r = pma._pma_http_get(url, headers)
 		return r.json()
 	except Exception as e:
-		return None		
+		return None
 
 def get_case_collection_titles(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
 	"""
 	Retrieve case collections (possibly filtered by project ID), titles only
 	"""
 	try:
 		return list(get_case_collection_titles_dict(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID).values())
 	except Exception as e:
-		return None		
-	
+		return None
+
 def get_case_collection_titles_dict(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
 	"""
 	Retrieve case collections (possibly filtered by project ID), return a dictionary of case collection IDs and titles
 	"""
 	dct = {}
 	all_colls = _pma_get_case_collections(pmacontrolURL, pmacoreSessionID)
 	for coll in all_colls:
@@ -314,54 +332,53 @@
 	Helper method to convert a list of sessions with default arguments into a summarized dictionary
 	"""
 	dct = {}
 	for prj_sess in original_project_sessions:
 		dct[prj_sess["Id"]] = prj_sess["Title"]
 
 	return dct
-	
+
 def _pma_get_projects(pmacontrolURL, pmacoreSessionID):
 	"""
 	Retrieve all projects and their data in PMA.control 
 	(RAW JSON data; not suited for human consumption)
 	"""
 	global _pma_projects_json
-	
+
 	url = pma._pma_join(pmacontrolURL, "api/Projects?sessionID=" + pma._pma_q(pmacoreSessionID))
 	print (url)
 	try:
 		headers = {'Accept': 'application/json'}
-		# r = requests.get(url, headers=headers)
-		r = pma._pma_http_get(url, headers)		
+		r = pma._pma_http_get(url, headers)
 		return r.json()
 	except Exception as e:
 		return None		
 
 def get_project_titles(pmacontrolURL, pmacoreSessionID):
 	"""
 	Retrieve projects, return ONLY the titles
 	"""
 	try:
 		return list(get_project_titles_dict(pmacontrolURL, pmacoreSessionID).values())
 	except Exception as e:
-		return None		
+		return None
 
 def get_project_titles_dict(pmacontrolURL, pmacoreSessionID):
 	"""
 	Retrieve projects, return a dictionary of project-IDs and titles
 	"""
 	dct = {}
 	all_projects = _pma_get_projects(pmacontrolURL, pmacoreSessionID)
 	try:
 		for prj in all_projects:
 			dct[prj['Id']] = prj['Title']
 	except Exception as e:
 		print(e)
-		return None		
-		
+		return None
+
 	return dct
 
 def get_project(pmacontrolURL, pmacontrolProjectID, pmacoreSessionID):
 	"""
 	Retrieve project details
 	"""
 	all_projects = _pma_get_projects(pmacontrolURL, pmacoreSessionID)
@@ -388,15 +405,15 @@
 	all_colls = _pma_get_case_collections(pmacontrolURL, pmacoreSessionID)
 	for coll in all_colls:
 		for case in coll["Cases"]:
 			if case["Id"] == pmacontrolCaseID:
 				return get_project(pmacontrolURL, coll["ProjectId"], pmacoreSessionID)
 
 	return None
-	
+
 def get_project_by_case_collection_id(pmacontrolURL, pmacontrolCaseCollectionID, pmacoreSessionID):
 	"""
 	Retrieve case collection based on the case ID
 	"""
 	all_colls = _pma_get_case_collections(pmacontrolURL, pmacoreSessionID)
 	for coll in all_colls:
 		if coll["Id"] == pmacontrolCaseCollectionID:
@@ -417,11 +434,11 @@
 			
 			# now integrate case collection information
 			colls = _pma_get_case_collections(pmacontrolURL, pmacoreSessionID)
 			prj['CaseCollections'] = {}
 			for col in colls:
 				if col['ProjectId'] == prj['Id']:
 					prj['CaseCollections'][col['Id']] = col['Title']
-					
+
 			return prj
 
 	return None
```

### Comparing `pma_python-2.0.0.97/pma_python/core.py` & `pma_python-2.0.0.98/pma_python/core.py`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/pma_python/core_admin.py` & `pma_python-2.0.0.98/pma_python/core_admin.py`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/pma_python/my.py` & `pma_python-2.0.0.98/pma_python/my.py`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/pma_python/pma.py` & `pma_python-2.0.0.98/pma_python/pma.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from urllib.parse import quote
 from os.path import join
 import requests
 
-__version__ = "2.0.0.97"
+__version__ = "2.0.0.98"
 
 _pma_url_content = {}
 _pma_debug = False
 
 def _pma_join(*s):
 	joinstring = ""
 	for ss in s:
```

### Comparing `pma_python-2.0.0.97/pma_python/view.py` & `pma_python-2.0.0.98/pma_python/view.py`

 * *Files identical despite different names*

### Comparing `pma_python-2.0.0.97/pma_python.egg-info/PKG-INFO` & `pma_python-2.0.0.98/pma_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pma-python
-Version: 2.0.0.97
+Version: 2.0.0.98
 Summary: Universal viewing of digital microscopy, whole slide imaging and digital pathology data
 Home-page: http://github.com/pathomation/pma_python
 Author: Pathomation
 Author-email: info@pathomation.com
 License: http://free.pathomation.com/eula/
 Description: pma_python is a Python wrapper library for PMA.start (http://free.pathomation.com),
         a universal viewer by Pathomation for whole slide imaging and microscopy.
```

### Comparing `pma_python-2.0.0.97/setup.py` & `pma_python-2.0.0.98/setup.py`

 * *Files identical despite different names*

