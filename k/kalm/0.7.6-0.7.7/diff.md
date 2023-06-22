# Comparing `tmp/kalm-0.7.6.tar.gz` & `tmp/kalm-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.7.6.tar", max compression
+gzip compressed data, was "kalm-0.7.7.tar", max compression
```

## Comparing `kalm-0.7.6.tar` & `kalm-0.7.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.6/LICENSE.txt
--rw-r--r--   0        0        0     2181 2023-06-21 07:27:06.346600 kalm-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    10467 2023-06-21 07:19:26.396067 kalm-0.7.6/src/kalm/__init__.py
--rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.6/src/kalm/common.py
--rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/dns/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/dns/dns.py
--rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/gitea/__init__.py
--rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/gitea/gitea.py
--rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.6/src/kalm/inabox/__init__.py
--rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.6/src/kalm/inabox/inabox.py
--rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.6/src/kalm/jenkins/__init__.py
--rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.6/src/kalm/jenkins/jenkins.py
--rw-r--r--   0        0        0    36170 2023-06-21 07:26:55.642540 kalm-0.7.6/src/kalm/kalm.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.6/src/kalm/package_data.dat
--rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.6/src/kalm/pypi/__init__.py
--rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.6/src/kalm/pypi/pypi.py
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.6/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.7/LICENSE.txt
+-rw-r--r--   0        0        0     2181 2023-06-22 10:50:03.889157 kalm-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0    10437 2023-06-22 10:49:45.901051 kalm-0.7.7/src/kalm/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.7/src/kalm/common.py
+-rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.7/src/kalm/dns/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.7/src/kalm/dns/dns.py
+-rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.7/src/kalm/gitea/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.7/src/kalm/gitea/gitea.py
+-rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.7/src/kalm/inabox/__init__.py
+-rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.7/src/kalm/inabox/inabox.py
+-rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.7/src/kalm/jenkins/__init__.py
+-rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.7/src/kalm/jenkins/jenkins.py
+-rw-r--r--   0        0        0    35873 2023-06-22 10:49:45.901051 kalm-0.7.7/src/kalm/kalm.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.7/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.7/src/kalm/pypi/__init__.py
+-rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.7/src/kalm/pypi/pypi.py
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.7/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.7/PKG-INFO
```

### Comparing `kalm-0.7.6/LICENSE.txt` & `kalm-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/pyproject.toml` & `kalm-0.7.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.7.6"
+version = "0.7.7"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -28,15 +28,15 @@
 python-jenkins = "^1.7.0"
 urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.7.05" 
+version = "0.7.06" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.7.6/src/kalm/__init__.py` & `kalm-0.7.7/src/kalm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,14 @@
             time.sleep(60)
             
 
             
 
 
     if ready and args.action[0] == "initservice":
-        print("Init service")
         r = redis.Redis()
         r.flushdb()
         result = runme("/usr/local/bin/awx --conf.color False tokens create |jq '{'id': .id, 'token': .token }")
         parsed_json = json.loads(result["stdout"])
         runme("sudo touch /etc/kalm/kalm.service.token")
         runme("sudo touch /etc/systemd/system/kalm.service")
         runme("sudo chown knowit:knowit /etc/kalm/kalm.service.token")
```

### Comparing `kalm-0.7.6/src/kalm/dns/__init__.py` & `kalm-0.7.7/src/kalm/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/dns/dns.py` & `kalm-0.7.7/src/kalm/dns/dns.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/gitea/__init__.py` & `kalm-0.7.7/src/kalm/gitea/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/inabox/__init__.py` & `kalm-0.7.7/src/kalm/inabox/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/inabox/inabox.py` & `kalm-0.7.7/src/kalm/inabox/inabox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/jenkins/__init__.py` & `kalm-0.7.7/src/kalm/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/jenkins/jenkins.py` & `kalm-0.7.7/src/kalm/jenkins/jenkins.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/kalm.py` & `kalm-0.7.7/src/kalm/kalm.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pprint import pprint
 import json
 import requests
 import hvac
 import os
 import sys
 import datetime
+import tempfile
 import pynetbox
 import urllib3
 import datetime
 from . import common
 
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -72,14 +73,21 @@
     )
   # Method to read an existing token
   def read_secret(self, engine_name, secret):
     return self.client.secrets.kv.v2.read_secret_version(
       mount_point=engine_name,
       path=secret
     )
+def checkout_git_repo(url, branch, path):
+  #create a temporary directory
+  tmpdir = tempfile.mkdtemp()
+  #clone the repo
+  command = "cd %s && git clone -b %s %s %s" % (tmpdir, branch, url, path)
+  os.system(command)
+
 
 def getawxdata(item, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/" + item
   intheloop = "first"
   while ( intheloop == "first" or intheloop != "out" ):
     try:
@@ -193,15 +201,14 @@
   
   
 
 
   if os.path.exists("/etc/kalm/kalm.d/%s.json" % subproject):
     with open("/etc/kalm.d/subproject.json") as f:
       data = json.load(f)
-      print(data)
 
   else:
       open("/etc/kalm/kalm.d/%s.json" % subproject, 'w').close()
       with open("/etc/kalm/kalm.d/%s.json" % subproject, 'w') as f:
         json.dump(data, f)
 
     
@@ -238,15 +245,14 @@
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     url = os.getenv("TOWER_HOST") + "/api/v2/inventories/"
     resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     prettyllog("manage", "inventories", name, organization, resp.status_code, response)
     loop = True
     while ( loop ):
-        print("looop")
         getawxdata("inventories", mytoken, r)
         try:
             invid = (awx_get_id("inventories", name, r))
         except:
             print("Unexpected error")
         if (invid != "" ):
           loop = False
@@ -303,19 +309,14 @@
   return fileval
 
 
 ############################################################################################################################
 # update ansible vault
 ############################################################################################################################
 def awx_update_vault(ansiblevault, organization, mytoken, r):
-  print("------------------------------------------------------------------")
-  print(ansiblevault)
-  print(organization)
-  print("------------------------------------------------------------------")
-
   for vault in ansiblevault[organization]['vault']:
     credential = { 
       "name": vault['name'], 
       "description": vault['description'], 
       "type": "Vault", 
       "vault_id": vault['vault_id'], 
       "vault_password": vault['vault_password'], 
@@ -485,16 +486,14 @@
   credid = (awx_get_id("credentials", credential, r))
   print('associatecommand = "awx job_template associate %s --credential %s >/dev/null 2>/dev/null " % ( tmplid, credid)')
   print("We should not use any awx cli commands, but the API is not consisten and sometimes fails to set the credentials")
   if VERIFY_SSL == False:
     associatecommand = "/usr/local/bin/awx job_template associate %s --credential %s -k >/dev/null 2>/dev/null " % ( tmplid, credid)  
   else:
     associatecommand = "/usr/local/bin/awx job_template associate %s --credential %s >/dev/null 2>/dev/null " % ( tmplid, credid)
-    
-  print(associatecommand)
   os.system(associatecommand)
   ############################################################################### end of create job template ##########################################
 
 
 ######################################
 # function:  Create Team
 ######################################
@@ -721,16 +720,14 @@
   ########################################################################################################################
   # Load and set ansible secrets in ansible vault
   ########################################################################################################################
   prettyllog("init", "runtime", "config", "init", "001", "loadning secrets")
   ansiblevaultfile = "/etc/kalm/secret.json"
   f = open(ansiblevaultfile)
   ansiblevault = json.loads(f.read())
-  print(ansiblevault)
-
   f.close
 
 
   ########################################################################################################################
   # Load  and set ansible automation org
   ########################################################################################################################
   cfgfile = "/etc/kalm/kalm.json"
@@ -836,15 +833,14 @@
     try: 
       inventories = org['inventories']
     except:
       prettyllog("config", "initialize", "inventories", orgname, "000",  "No inventories found")
 
     for inventory in inventories:
       valid=True
-      print(inventory)
       try:
         inventoryname = inventory['name']
       except:
         inventoryname = "Missing"
         valid = False
       try: 
         inventorydesc = inventory['description']
@@ -854,15 +850,14 @@
         inventorytype = inventory['type']
       except:
         inventorytype = "static"
       try:
         inventoryvariables = inventory['variables']
       except:
         inventoryvariables = {}
-      print(inventoryvariables)
       if valid:
         awx_create_inventory(inventoryname, inventorydesc, orgname, inventorytype, inventoryvariables, mytoken, r)
       else:
         prettyllog("config", "initialize", "inventories", inventory, "000",  "Inventory is invalid")
 
 
 
@@ -898,31 +893,28 @@
         awx_create_label(labelname, orgname, mytoken, r)
     except:
       prettyllog("config", "initialize", "labels", orgname, "000",  "No labels found")
 
     ######################################
     # Templates
     ######################################
-    print("Templates")
-    print("============================DEBUG==============================YY")
     try:
       templates = org['templates']
       for template in templates:
         templatename = template['name']
         templatedescription = template['description']
         templatejob_type = template['job_type']
         templateinventory =  template['inventory']
         templateproject = template['project']
         templateEE = template['EE']
         templatecredential = template['credentials']  
         templateplaybook = template['playbook']
         awx_create_template(templatename, templatedescription, templatejob_type, templateinventory, templateproject, templateEE, templatecredential, templateplaybook, orgname, mytoken, r)
     except:
       prettyllog("config", "initialize", "templates", orgname, "000",  "No templates found")
-    print("============================DEBUG==============================YY")
 
     ######################################
     # Schedules
     ######################################
     try:
       schedules = org['schedules']
       for schedule in schedules:
```

### Comparing `kalm-0.7.6/src/kalm/pypi/__init__.py` & `kalm-0.7.7/src/kalm/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/src/kalm/pypi/pypi.py` & `kalm-0.7.7/src/kalm/pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.6/PKG-INFO` & `kalm-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.7.6
+Version: 0.7.7
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

