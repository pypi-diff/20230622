# Comparing `tmp/launchpy-0.4.1.tar.gz` & `tmp/launchpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchpy-0.4.1.tar", last modified: Thu May 11 13:29:15 2023, max compression
+gzip compressed data, was "launchpy-0.4.2.tar", last modified: Thu Jun 22 12:30:36 2023, max compression
```

## Comparing `launchpy-0.4.1.tar` & `launchpy-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.256854 launchpy-0.4.1/
--rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      852 2023-05-11 13:29:15.255857 launchpy-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2022-11-09 18:49:02.000000 launchpy-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.217959 launchpy-0.4.1/launchpy/
--rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.1/launchpy/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-11 13:26:59.000000 launchpy-0.4.1/launchpy/__version__.py
--rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.1/launchpy/admin.py
--rw-rw-rw-   0        0        0      712 2021-11-08 18:47:00.000000 launchpy-0.4.1/launchpy/config.py
--rw-rw-rw-   0        0        0     6823 2022-11-08 13:20:12.000000 launchpy-0.4.1/launchpy/configs.py
--rw-rw-rw-   0        0        0    11497 2021-10-20 19:49:47.000000 launchpy-0.4.1/launchpy/connector.py
--rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.1/launchpy/launchpy.py
--rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.1/launchpy/library.py
--rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.1/launchpy/property.py
--rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.1/launchpy/synchronizer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.251868 launchpy-0.4.1/launchpy.egg-info/
--rw-rw-rw-   0        0        0      852 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 13:29:15.257851 launchpy-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.945758 launchpy-0.4.2/
+-rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2294 2023-06-22 12:30:36.944760 launchpy-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2023-06-22 12:01:59.000000 launchpy-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.855149 launchpy-0.4.2/docs/
+-rw-rw-rw-   0        0        0     3258 2022-07-13 12:52:02.000000 launchpy-0.4.2/docs/admin.md
+-rw-rw-rw-   0        0        0     3892 2021-10-20 19:49:46.000000 launchpy-0.4.2/docs/getstarted.md
+-rw-rw-rw-   0        0        0     3727 2021-10-20 19:49:46.000000 launchpy-0.4.2/docs/library.md
+-rw-rw-rw-   0        0        0     7521 2021-10-20 19:49:47.000000 launchpy-0.4.2/docs/main.md
+-rw-rw-rw-   0        0        0    16546 2023-05-10 18:11:54.000000 launchpy-0.4.2/docs/property.md
+-rw-rw-rw-   0        0        0     4657 2023-06-21 19:15:59.000000 launchpy-0.4.2/docs/releases.md
+-rw-rw-rw-   0        0        0     8286 2023-05-11 13:25:38.000000 launchpy-0.4.2/docs/synchronizer.md
+-rw-rw-rw-   0        0        0     4234 2023-05-10 18:06:32.000000 launchpy-0.4.2/docs/translator.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.908869 launchpy-0.4.2/launchpy/
+-rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.2/launchpy/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-21 19:15:00.000000 launchpy-0.4.2/launchpy/__version__.py
+-rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.2/launchpy/admin.py
+-rw-rw-rw-   0        0        0      810 2023-06-21 19:22:23.000000 launchpy-0.4.2/launchpy/config.py
+-rw-rw-rw-   0        0        0     8018 2023-06-22 10:59:40.000000 launchpy-0.4.2/launchpy/configs.py
+-rw-rw-rw-   0        0        0    13613 2023-06-22 11:00:34.000000 launchpy-0.4.2/launchpy/connector.py
+-rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.2/launchpy/launchpy.py
+-rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.2/launchpy/library.py
+-rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.2/launchpy/property.py
+-rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.2/launchpy/synchronizer.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.940774 launchpy-0.4.2/launchpy.egg-info/
+-rw-rw-rw-   0        0        0     2294 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1361 2023-06-22 12:02:18.000000 launchpy-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      101 2021-10-20 19:49:47.000000 launchpy-0.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:30:36.946756 launchpy-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.2/setup.py
```

### Comparing `launchpy-0.4.1/LICENSE` & `launchpy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/README.md` & `launchpy-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,19 @@
 - Helping functions [Core Components](./docs/main.md)
 - Admin instantiating functions [Admin Class](./docs/admin.md)
 - Managing properties [Property Class](./docs/property.md)
 - Managing Publishing Cycle [Library Class](./docs/library.md)
 - Translator functionationality [Translator Class](./docs/translator.md)
 - Synchronizer [Synchronizer Class](./docs/synchronizer.md)
 
-## Get Stated
+## Get Started
 
 A [get started guide](./docs/getstarted.md) has been created to explain the different functionality.
 You can find a more detail description functionalities at [datanalyst.info](https://datanalyst.info).
 
-~~A Jupyter notebook is also available in the github for demo.~~ To be updated.
-
 ## Main documentation
 
 Most of the documentation has been imported from the datanalyst website [here](./docs/main.md).
 
 ## Release information
 
 You can find release information [here](./docs/releases.md).
```

### Comparing `launchpy-0.4.1/launchpy/admin.py` & `launchpy-0.4.2/launchpy/admin.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/launchpy/config.py` & `launchpy-0.4.2/launchpy/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 
 token = ""
 config_object = {
     "org_id": "",
     "api_key": "",
     "pathToKey": "",
     "secret": "",
-    "tokenEndpoint" : "https://ims-na1.adobelogin.com/ims/exchange/jwt",
+    "jwtTokenEndpoint" : "https://ims-na1.adobelogin.com/ims/exchange/jwt",
+    "oauthTokenEndpointV2" : "https://ims-na1.adobelogin.com/ims/token/v2",
     "date_limit" : 0,
     "scope_admin" : "https://ims-na1.adobelogin.com/s/ent_reactor_admin_sdk",
     "scope_dev" : "https://ims-na1.adobelogin.com/s/ent_reactor_sdk",
-    "official_scope" :  ""
+    "official_scope" :  "",
+    "scopes":""
 }
 
 header = {"Accept": "application/vnd.api+json;revision=1",
           "Content-Type": "application/vnd.api+json",
           "Authorization": "Bearer " + token,
           "x-gw-ims-org-id": config_object['org_id']
           }
```

### Comparing `launchpy-0.4.1/launchpy/configs.py` & `launchpy-0.4.2/launchpy/configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,50 +18,56 @@
         return Path('.' + path)
     elif path.startswith('\\') and Path('.' + path).exists():
         return Path('.' + path)
     else:
         return None
 
 
-def createConfigFile(scope: str = "https://ims-na1.adobelogin.com/s/ent_reactor_admin_sdk", verbose: object = False)->None:
+def createConfigFile(scope: str = "https://ims-na1.adobelogin.com/s/ent_reactor_admin_sdk",auth_type: str = "oauthV2", verbose: object = False)->None:
     """
     This function will create a 'config_launch_admin.json' file where you can store your access data. 
     Arguments:
         scope: OPTIONAL : if you have problem with scope during API connection, you may need to update this.
             scope="https://ims-na1.adobelogin.com/s/ent_reactor_admin_sdk"
             or 
             scope="https://ims-na1.adobelogin.com/s/ent_reactor_sdk"
+        auth_type : OPTIONAL : The type of Oauth type you want to use for your config file. Possible value: "jwt" or "oauthV2"
     """
     json_data = {
         'org_id': '<orgID>',
         'client_id': "<client_id>",
-        'tech_id': "<something>@techacct.adobe.com",
         'secret': "<YourSecret>",
-        'pathToKey': '<path/to/your/privatekey.key>',
         'scope': scope
     }
+    if auth_type == 'oauthV2':
+        json_data['scopes'] = "<scopes>"
+    elif auth_type == 'jwt':
+        json_data["tech_id"] = "<something>@techacct.adobe.com"
+        json_data["pathToKey"] = "<path/to/your/privatekey.key>"
     with open('config_launch_admin.json', 'w') as cf:
         cf.write(json.dumps(json_data, indent=4))
     if verbose:
         print(
             f" file created at this location : {os.getcwd()}{os.sep}config_launch_admin.json")
 
-def importConfigFile(path: str) -> None:
+def importConfigFile(path: str = None,auth_type:str=None) -> None:
     """Reads the file denoted by the supplied `path` and retrieves the configuration information
     from it.
 
     Arguments:
         path: REQUIRED : path to the configuration file. Can be either a fully-qualified or relative.
-
+        auth_type : OPTIONAL : The type of Auth to be used by default. Detected if none is passed, OauthV2 takes precedence.
+                        Possible values: "jwt" or "oauthV2"
     Example of path value.
     "config.json"
     "./config.json"
     "/my-folder/config.json"
     """
-
+    if path is None:
+        raise ValueError("a path must be provided")
     config_file_path: Optional[Path] = find_path(path)
     if config_file_path is None:
         raise FileNotFoundError(
             f"Unable to find the configuration file under path `{path}`."
         )
     with open(config_file_path, 'r') as file:
         provided_config = json.load(file)
@@ -69,22 +75,31 @@
         if 'api_key' in provided_keys:
             ## old naming for client_id
             client_id = provided_config['api_key']
         elif 'client_id' in provided_keys:
             client_id = provided_config['client_id']
         else:
             raise RuntimeError(f"Either an `api_key` or a `client_id` should be provided.")
-        configure(
-            org_id=provided_config['org_id'],
-            tech_id=provided_config['tech_id'],
-            secret=provided_config['secret'],
-            path_to_key=provided_config['pathToKey'],
-            client_id=client_id
-
-        )
+        if auth_type is None:
+            if 'scopes' in provided_keys:
+                auth_type = 'oauthV2'
+            elif 'tech_id' in provided_keys and "pathToKey" in provided_keys:
+                auth_type = 'jwt'
+        args = {
+            "org_id" : provided_config['org_id'],
+            "secret" : provided_config['secret'],
+            "client_id" : client_id,
+            "scope" : provided_config['scope']
+        }
+        if auth_type == 'oauthV2':
+            args["scopes"] = provided_config["scopes"].replace(' ','')
+        if auth_type == 'jwt':
+            args["tech_id"] = provided_config["tech_id"]
+            args["path_to_key"] = provided_config["pathToKey"]
+        configure(**args)
 
 
 def saveFile(data:str,filename:str=None,type:str='txt',encoding:str='utf-8')->None:
     """
     Save file to your system.
     Arguments:
         data : REQUIRED : data to be saved
@@ -110,14 +125,15 @@
 
 def configure(org_id: str = None,
               tech_id: str = None,
               secret: str = None,
               client_id: str = None,
               path_to_key: str=None,
               private_key: str = None,
+              scopes : str= None,
               scope: str="https://ims-na1.adobelogin.com/s/ent_reactor_admin_sdk",
               ):
     """Performs programmatic configuration of the API using provided values.
     Arguments:
         org_id : REQUIRED : Organization ID
         tech_id : REQUIRED : Technical Account ID
         secret : REQUIRED : secret generated for your connection
@@ -127,29 +143,30 @@
         scope : OPTIONAL : Scope that is needed for JWT auth.
             Possible scope: https://www.adobe.io/authentication/auth-methods.html#!AdobeDocs/adobeio-auth/master/JWT/Scopes.md
     """
     if not org_id:
         raise ValueError("`org_id` must be specified in the configuration.")
     if not client_id:
         raise ValueError("`client_id` must be specified in the configuration.")
-    if not tech_id:
+    if not tech_id and not scopes:
         raise ValueError("`tech_id` must be specified in the configuration.")
     if not secret:
         raise ValueError("`secret` must be specified in the configuration.")
-    if not path_to_key and not private_key:
-        raise ValueError("`pathToKey` or `private_key` must be specified in the configuration.")
+    if not path_to_key and not private_key and not scopes:
+        raise ValueError("`scopes` must be specified if Oauth setup.\n `pathToKey` or `private_key` must be specified in the configuration if JWT setup.")
     config_object["org_id"] = org_id
     header["x-gw-ims-org-id"] = org_id
     config_object["client_id"] = client_id
     header["x-api-key"] = client_id
     config_object["tech_id"] = tech_id
     config_object["secret"] = secret
     config_object["pathToKey"] = path_to_key
     config_object["private_key"] = private_key
     config_object["official_scope"] = scope
+    config_object["scopes"] = scopes
     # ensure the reset of the state by overwriting possible values from previous import.
     config_object["date_limit"] = 0
     config_object["token"] = ""
 
 
 def get_private_key_from_config(config: dict) -> str:
     """
```

### Comparing `launchpy-0.4.1/launchpy/connector.py` & `launchpy-0.4.2/launchpy/connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 import time
 from typing import Dict, Union
-
+from copy import deepcopy
 # Non standard libraries
 import jwt
 import requests
 from launchpy import config, configs
 
 class AdobeRequest:
     """
@@ -26,29 +26,32 @@
             header : OPTIONAL : header of the config modules
             verbose : OPTIONAL : display comment on the request.
             retry : OPTIONAL : If you wish to retry failed GET requests
         """
         if config_object['org_id'] == '':
             raise Exception(
                 'You have to upload the configuration file with importConfigFile method.')
-        self.config = config_object
+        self.config = deepcopy(config_object)
         self.header = header
         self.retry = retry
         if self.config['token'] == '' or time.time() > self.config['date_limit']:
-            token_and_expiry = self.get_token_and_expiry_for_config(config=self.config, verbose=verbose)
+            if 'scopes' in self.config.keys() and self.config.get('scopes',None) is not None:
+                self.connectionType = 'oauthV2'
+                token_and_expiry = self.get_oauth_token_and_expiry_for_config(config=self.config, verbose=verbose)
+            elif self.config.get("private_key",None) is not None or self.config.get("pathToKey",None) is not None:
+                self.connectionType = 'jwt'
+                token_and_expiry = self.get_jwt_token_and_expiry_for_config(config=self.config, verbose=verbose)
             token = token_and_expiry['token']
             expiry = token_and_expiry['expiry']
             self.token = token
             self.config['token'] = token
-            self.config['date_limit'] = time.time() + expiry / 1000 - 500
+            self.config['date_limit'] = time.time() + expiry - 500
             self.header.update({'Authorization': f'Bearer {token}'})
 
-    
-
-    def get_token_and_expiry_for_config(self,config: dict, verbose: bool = False, save: bool = False, *args, **kwargs) -> Dict[str, str]:
+    def get_jwt_token_and_expiry_for_config(self,config: dict, verbose: bool = False, save: bool = False, *args, **kwargs) -> Dict[str, str]:
         """
         Retrieve the token by using the information provided by the user during the import importConfigFile function.
         Arguments :
             config : REQUIRED : config object to passs for information
             verbose : OPTIONAL : Default False. If set to True, print information.
             save : OPTIONAL : Default False. If set to True, save the toke in the .
         """
@@ -82,37 +85,69 @@
             'jwt_token': encoded_jwt_admin
         }
         payload_dev = {
             'client_id': config['client_id'],
             'client_secret': config['secret'],
             'jwt_token': encoded_jwt_dev
         }
-        response = requests.post(config['tokenEndpoint'], headers=header_jwt, data=payload_admin)
+        response = requests.post(config['jwtTokenEndpoint'], headers=header_jwt, data=payload_admin)
         json_response = response.json()
         if 'error' in json_response.keys():
             if json_response['error'] == "invalid_scope":
                 try:
-                    response = requests.post(config['tokenEndpoint'], headers=header_jwt, data=payload_dev)
+                    response = requests.post(config['jwtTokenEndpoint'], headers=header_jwt, data=payload_dev)
                     json_response = response.json()
                 except Exception as e:
                     print(json.dumps(json_response, indent=4))
                     raise Exception(e)
         try:
             token = json_response['access_token']
         except KeyError:
             print('Issue retrieving token')
             print(json_response)
-        expiry = json_response['expires_in']
+        expiry = json_response['expires_in'] / 1000
         if save:
             with open('token.txt', 'w') as f:
                 f.write(token)
             print(f'token has been saved here: {os.getcwd()}{os.sep}token.txt')
         if verbose:
             print('token valid till : ' + time.ctime(time.time() + expiry / 1000))
         return {'token': token, 'expiry': expiry}
+    
+    def get_oauth_token_and_expiry_for_config(self,config:dict,verbose:bool=False,save:bool=False)->Dict[str,str]:
+        """
+        Retrieve the access token by using the OAuth information provided by the user
+        during the import importConfigFile function.
+        Arguments :
+            config : REQUIRED : Configuration object.
+            verbose : OPTIONAL : Default False. If set to True, print information.
+            save : OPTIONAL : Default False. If set to True, save the toke in the .
+        """
+        if config is None:
+            raise ValueError("config dictionary is required")
+        oauth_payload = {
+            "grant_type": "client_credentials",
+            "client_id": config["client_id"],
+            "client_secret": config["secret"],
+            "scope": config["scopes"]
+        }
+        response = requests.post(
+            config["oauthTokenEndpointV2"], data=oauth_payload)
+        json_response = response.json()
+        if 'access_token' in json_response.keys():
+            token = json_response['access_token']
+            expiry = json_response["expires_in"]
+        else:
+            return json.dumps(json_response,indent=2)
+        if save:
+            with open('token.txt', 'w') as f:
+                f.write(token)
+        if verbose:
+            print('token valid till : ' + time.ctime(time.time() + expiry))
+        return {'token': token, 'expiry': expiry}
 
 
     def _get_jwt(self,payload: dict, private_key: str) -> str:
         """
         Ensure that jwt enconding return the same type (str) as versions < 2.0.0 returned bytes and >2.0.0 return strings. 
         """
         token: Union[str, bytes] = jwt.encode(payload, private_key, algorithm='RS256')
@@ -122,18 +157,21 @@
 
     def _checkingDate(self) -> None:
         """
         Checking if the token is still valid
         """
         now = time.time()
         if now > self.config['date_limit']:
-            token_with_expiry = self.get_token_and_expiry_for_config(config=self.config)
-            token = token_with_expiry['token']
+            if self.connectionType =='oauthV2':
+                token_and_expiry = self.get_oauth_token_and_expiry_for_config(config=self.config)
+            elif self.connectionType == 'jwt':
+                token_and_expiry = self.get_jwt_token_and_expiry_for_config(config=self.config)
+            token = token_and_expiry['token']
             self.config['token'] = token
-            self.config['date_limit'] = time.time() + token_with_expiry['expiry'] / 1000 - 500
+            self.config['date_limit'] = time.time() + token_and_expiry['expiry'] - 500
             self.header.update({'Authorization': f'Bearer {token}'})
 
     def getData(self, endpoint: str, params: dict = None, data: dict = None, headers: dict = None, *args, **kwargs):
         """
         Abstraction for getting data
         """
         internRetry = self.retry - kwargs.get("retry", 0)
```

### Comparing `launchpy-0.4.1/launchpy/launchpy.py` & `launchpy-0.4.2/launchpy/launchpy.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/launchpy/library.py` & `launchpy-0.4.2/launchpy/library.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/launchpy/property.py` & `launchpy-0.4.2/launchpy/property.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/launchpy/synchronizer.py` & `launchpy-0.4.2/launchpy/synchronizer.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.1/setup.py` & `launchpy-0.4.2/setup.py`

 * *Files identical despite different names*

