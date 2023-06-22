# Comparing `tmp/firebase_admin-6.1.0.tar.gz` & `tmp/firebase_admin-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firebase_admin-6.1.0.tar", last modified: Thu Feb  2 18:04:05 2023, max compression
+gzip compressed data, was "dist/firebase_admin-6.2.0.tar", last modified: Thu Jun 22 18:50:26 2023, max compression
```

## Comparing `firebase_admin-6.1.0.tar` & `firebase_admin-6.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36896 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_auth_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_gapic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32878 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_messaging_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23450 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_messaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_sseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    19442 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_token_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_user_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_user_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_user_mgt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/app_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    38016 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    37109 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/firestore_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/instance_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    18191 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/project_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/firebase_admin/tenant_mgt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/firebase_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-02 18:04:05.000000 firebase_admin-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-02-02 18:00:49.000000 firebase_admin-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36881 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_auth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_gapic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32878 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_messaging_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23450 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_messaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_sseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19442 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_token_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_user_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_user_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_user_mgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/app_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38016 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37109 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/firestore_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/instance_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/project_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/firebase_admin/tenant_mgt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/firebase_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-22 18:50:26.000000 firebase_admin-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-22 18:41:28.000000 firebase_admin-6.2.0/setup.py
```

### Comparing `firebase_admin-6.1.0/PKG-INFO` & `firebase_admin-6.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 1.2
 Name: firebase_admin
-Version: 6.1.0
+Version: 6.2.0
 Summary: Firebase Admin Python SDK
 Home-page: https://firebase.google.com/docs/admin/setup/
 Author: Firebase
 License: Apache License 2.0
+Project-URL: Release Notes, https://firebase.google.com/support/release-notes/admin/python
 Project-URL: Source, https://github.com/firebase/firebase-admin-python
 Description: The Firebase Admin Python SDK enables server-side (backend) Python developers to integrate Firebase into their services and applications.
 Keywords: firebase cloud development
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `firebase_admin-6.1.0/README.md` & `firebase_admin-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/__about__.py` & `firebase_admin-6.2.0/firebase_admin/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """About information (version, etc) for Firebase Admin SDK."""
 
-__version__ = '6.1.0'
+__version__ = '6.2.0'
 __title__ = 'firebase_admin'
 __author__ = 'Firebase'
 __license__ = 'Apache License 2.0'
 __url__ = 'https://firebase.google.com/docs/admin/setup/'
```

### Comparing `firebase_admin-6.1.0/firebase_admin/__init__.py` & `firebase_admin-6.2.0/firebase_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_auth_client.py` & `firebase_admin-6.2.0/firebase_admin/_auth_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         # If an emulator is present, check that the given value matches the expected format and set
         # endpoint URLs to use the emulator. Additionally, use a fake credential.
         emulator_host = _auth_utils.get_emulator_host()
         if emulator_host:
             base_url = 'http://{0}/identitytoolkit.googleapis.com'.format(emulator_host)
             endpoint_urls['v1'] = base_url + '/v1'
-            endpoint_urls['v2beta1'] = base_url + '/v2beta1'
+            endpoint_urls['v2'] = base_url + '/v2'
             credential = _utils.EmulatorAdminCredentials()
             self.emulated = True
         else:
             # Use credentials if provided
             credential = app.credential.get_credential()
 
         http_client = _http_client.JsonHttpClient(
@@ -63,15 +63,15 @@
         self._tenant_id = tenant_id
         self._token_generator = _token_gen.TokenGenerator(
             app, http_client, url_override=endpoint_urls.get('v1'))
         self._token_verifier = _token_gen.TokenVerifier(app)
         self._user_manager = _user_mgt.UserManager(
             http_client, app.project_id, tenant_id, url_override=endpoint_urls.get('v1'))
         self._provider_manager = _auth_providers.ProviderConfigClient(
-            http_client, app.project_id, tenant_id, url_override=endpoint_urls.get('v2beta1'))
+            http_client, app.project_id, tenant_id, url_override=endpoint_urls.get('v2'))
 
     @property
     def tenant_id(self):
         """Tenant ID associated with this client."""
         return self._tenant_id
 
     def create_custom_token(self, uid, developer_claims=None):
```

### Comparing `firebase_admin-6.1.0/firebase_admin/_auth_providers.py` & `firebase_admin-6.2.0/firebase_admin/_auth_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     def items(self):
         return self._current_page.provider_configs
 
 
 class ProviderConfigClient:
     """Client for managing Auth provider configurations."""
 
-    PROVIDER_CONFIG_URL = 'https://identitytoolkit.googleapis.com/v2beta1'
+    PROVIDER_CONFIG_URL = 'https://identitytoolkit.googleapis.com/v2'
 
     def __init__(self, http_client, project_id, tenant_id=None, url_override=None):
         self.http_client = http_client
         url_prefix = url_override or self.PROVIDER_CONFIG_URL
         self.base_url = '{0}/projects/{1}'.format(url_prefix, project_id)
         if tenant_id:
             self.base_url += '/tenants/{0}'.format(tenant_id)
```

### Comparing `firebase_admin-6.1.0/firebase_admin/_auth_utils.py` & `firebase_admin-6.2.0/firebase_admin/_auth_utils.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_gapic_utils.py` & `firebase_admin-6.2.0/firebase_admin/_gapic_utils.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_http_client.py` & `firebase_admin-6.2.0/firebase_admin/_http_client.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_messaging_encoder.py` & `firebase_admin-6.2.0/firebase_admin/_messaging_encoder.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_messaging_utils.py` & `firebase_admin-6.2.0/firebase_admin/_messaging_utils.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_rfc3339.py` & `firebase_admin-6.2.0/firebase_admin/_rfc3339.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_sseclient.py` & `firebase_admin-6.2.0/firebase_admin/_sseclient.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_token_gen.py` & `firebase_admin-6.2.0/firebase_admin/_token_gen.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_user_identifier.py` & `firebase_admin-6.2.0/firebase_admin/_user_identifier.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_user_import.py` & `firebase_admin-6.2.0/firebase_admin/_user_import.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_user_mgt.py` & `firebase_admin-6.2.0/firebase_admin/_user_mgt.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/_utils.py` & `firebase_admin-6.2.0/firebase_admin/_utils.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/app_check.py` & `firebase_admin-6.2.0/firebase_admin/app_check.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/auth.py` & `firebase_admin-6.2.0/firebase_admin/auth.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/credentials.py` & `firebase_admin-6.2.0/firebase_admin/credentials.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/db.py` & `firebase_admin-6.2.0/firebase_admin/db.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/exceptions.py` & `firebase_admin-6.2.0/firebase_admin/exceptions.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/firestore.py` & `firebase_admin-6.2.0/firebase_admin/firestore.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/firestore_async.py` & `firebase_admin-6.2.0/firebase_admin/firestore_async.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/instance_id.py` & `firebase_admin-6.2.0/firebase_admin/instance_id.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/messaging.py` & `firebase_admin-6.2.0/firebase_admin/messaging.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Firebase Cloud Messaging module."""
 
+import concurrent.futures
 import json
+import warnings
+import requests
 
 from googleapiclient import http
 from googleapiclient import _auth
-import requests
 
 import firebase_admin
 from firebase_admin import _http_client
 from firebase_admin import _messaging_encoder
 from firebase_admin import _messaging_utils
 from firebase_admin import _gapic_utils
 from firebase_admin import _utils
+from firebase_admin import exceptions
 
 
 _MESSAGING_ATTRIBUTE = '_messaging'
 
 
 __all__ = [
     'AndroidConfig',
@@ -111,14 +114,65 @@
 
     Raises:
         FirebaseError: If an error occurs while sending the message to the FCM service.
         ValueError: If the input arguments are invalid.
     """
     return _get_messaging_service(app).send(message, dry_run)
 
+def send_each(messages, dry_run=False, app=None):
+    """Sends each message in the given list via Firebase Cloud Messaging.
+
+    If the ``dry_run`` mode is enabled, the message will not be actually delivered to the
+    recipients. Instead FCM performs all the usual validations, and emulates the send operation.
+
+    Args:
+        messages: A list of ``messaging.Message`` instances.
+        dry_run: A boolean indicating whether to run the operation in dry run mode (optional).
+        app: An App instance (optional).
+
+    Returns:
+        BatchResponse: A ``messaging.BatchResponse`` instance.
+
+    Raises:
+        FirebaseError: If an error occurs while sending the message to the FCM service.
+        ValueError: If the input arguments are invalid.
+    """
+    return _get_messaging_service(app).send_each(messages, dry_run)
+
+def send_each_for_multicast(multicast_message, dry_run=False, app=None):
+    """Sends the given mutlicast message to each token via Firebase Cloud Messaging (FCM).
+
+    If the ``dry_run`` mode is enabled, the message will not be actually delivered to the
+    recipients. Instead FCM performs all the usual validations, and emulates the send operation.
+
+    Args:
+        multicast_message: An instance of ``messaging.MulticastMessage``.
+        dry_run: A boolean indicating whether to run the operation in dry run mode (optional).
+        app: An App instance (optional).
+
+    Returns:
+        BatchResponse: A ``messaging.BatchResponse`` instance.
+
+    Raises:
+        FirebaseError: If an error occurs while sending the message to the FCM service.
+        ValueError: If the input arguments are invalid.
+    """
+    if not isinstance(multicast_message, MulticastMessage):
+        raise ValueError('Message must be an instance of messaging.MulticastMessage class.')
+    messages = [Message(
+        data=multicast_message.data,
+        notification=multicast_message.notification,
+        android=multicast_message.android,
+        webpush=multicast_message.webpush,
+        apns=multicast_message.apns,
+        fcm_options=multicast_message.fcm_options,
+        token=token
+    ) for token in multicast_message.tokens]
+    return _get_messaging_service(app).send_each(messages, dry_run)
+
 def send_all(messages, dry_run=False, app=None):
     """Sends the given list of messages via Firebase Cloud Messaging as a single batch.
 
     If the ``dry_run`` mode is enabled, the message will not be actually delivered to the
     recipients. Instead FCM performs all the usual validations, and emulates the send operation.
 
     Args:
@@ -128,15 +182,18 @@
 
     Returns:
         BatchResponse: A ``messaging.BatchResponse`` instance.
 
     Raises:
         FirebaseError: If an error occurs while sending the message to the FCM service.
         ValueError: If the input arguments are invalid.
+
+    send_all() is deprecated. Use send_each() instead.
     """
+    warnings.warn('send_all() is deprecated. Use send_each() instead.', DeprecationWarning)
     return _get_messaging_service(app).send_all(messages, dry_run)
 
 def send_multicast(multicast_message, dry_run=False, app=None):
     """Sends the given mutlicast message to all tokens via Firebase Cloud Messaging (FCM).
 
     If the ``dry_run`` mode is enabled, the message will not be actually delivered to the
     recipients. Instead FCM performs all the usual validations, and emulates the send operation.
@@ -148,15 +205,19 @@
 
     Returns:
         BatchResponse: A ``messaging.BatchResponse`` instance.
 
     Raises:
         FirebaseError: If an error occurs while sending the message to the FCM service.
         ValueError: If the input arguments are invalid.
+
+    send_multicast() is deprecated. Use send_each_for_multicast() instead.
     """
+    warnings.warn('send_multicast() is deprecated. Use send_each_for_multicast() instead.',
+                  DeprecationWarning)
     if not isinstance(multicast_message, MulticastMessage):
         raise ValueError('Message must be an instance of messaging.MulticastMessage class.')
     messages = [Message(
         data=multicast_message.data,
         notification=multicast_message.notification,
         android=multicast_message.android,
         webpush=multicast_message.webpush,
@@ -352,14 +413,43 @@
                 json=data
             )
         except requests.exceptions.RequestException as error:
             raise self._handle_fcm_error(error)
         else:
             return resp['name']
 
+    def send_each(self, messages, dry_run=False):
+        """Sends the given messages to FCM via the FCM v1 API."""
+        if not isinstance(messages, list):
+            raise ValueError('messages must be a list of messaging.Message instances.')
+        if len(messages) > 500:
+            raise ValueError('messages must not contain more than 500 elements.')
+
+        def send_data(data):
+            try:
+                resp = self._client.body(
+                    'post',
+                    url=self._fcm_url,
+                    headers=self._fcm_headers,
+                    json=data)
+            except requests.exceptions.RequestException as exception:
+                return SendResponse(resp=None, exception=self._handle_fcm_error(exception))
+            else:
+                return SendResponse(resp, exception=None)
+
+        message_data = [self._message_data(message, dry_run) for message in messages]
+        try:
+            with concurrent.futures.ThreadPoolExecutor(max_workers=len(message_data)) as executor:
+                responses = [resp for resp in executor.map(send_data, message_data)]
+                return BatchResponse(responses)
+        except Exception as error:
+            raise exceptions.UnknownError(
+                message='Unknown error while making remote service calls: {0}'.format(error),
+                cause=error)
+
     def send_all(self, messages, dry_run=False):
         """Sends the given messages to FCM via the batch API."""
         if not isinstance(messages, list):
             raise ValueError('messages must be a list of messaging.Message instances.')
         if len(messages) > 500:
             raise ValueError('messages must not contain more than 500 elements.')
```

### Comparing `firebase_admin-6.1.0/firebase_admin/ml.py` & `firebase_admin-6.2.0/firebase_admin/ml.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/project_management.py` & `firebase_admin-6.2.0/firebase_admin/project_management.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/storage.py` & `firebase_admin-6.2.0/firebase_admin/storage.py`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/firebase_admin/tenant_mgt.py` & `firebase_admin-6.2.0/firebase_admin/tenant_mgt.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def enable_email_link_sign_in(self):
         return self._data.get('enableEmailLinkSignin', False)
 
 
 class _TenantManagementService:
     """Firebase tenant management service."""
 
-    TENANT_MGT_URL = 'https://identitytoolkit.googleapis.com/v2beta1'
+    TENANT_MGT_URL = 'https://identitytoolkit.googleapis.com/v2'
 
     def __init__(self, app):
         credential = app.credential.get_credential()
         version_header = 'Python/Admin/{0}'.format(firebase_admin.__version__)
         base_url = '{0}/projects/{1}'.format(self.TENANT_MGT_URL, app.project_id)
         self.app = app
         self.client = _http_client.JsonHttpClient(
```

### Comparing `firebase_admin-6.1.0/firebase_admin.egg-info/PKG-INFO` & `firebase_admin-6.2.0/firebase_admin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 1.2
 Name: firebase-admin
-Version: 6.1.0
+Version: 6.2.0
 Summary: Firebase Admin Python SDK
 Home-page: https://firebase.google.com/docs/admin/setup/
 Author: Firebase
 License: Apache License 2.0
+Project-URL: Release Notes, https://firebase.google.com/support/release-notes/admin/python
 Project-URL: Source, https://github.com/firebase/firebase-admin-python
 Description: The Firebase Admin Python SDK enables server-side (backend) Python developers to integrate Firebase into their services and applications.
 Keywords: firebase cloud development
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `firebase_admin-6.1.0/firebase_admin.egg-info/SOURCES.txt` & `firebase_admin-6.2.0/firebase_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebase_admin-6.1.0/setup.py` & `firebase_admin-6.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 setup(
     name=about['__title__'],
     version=about['__version__'],
     description='Firebase Admin Python SDK',
     long_description=long_description,
     url=about['__url__'],
     project_urls={
+        'Release Notes': 'https://firebase.google.com/support/release-notes/admin/python',
         'Source': 'https://github.com/firebase/firebase-admin-python',
     },
     author=about['__author__'],
     license=about['__license__'],
     keywords='firebase cloud development',
     install_requires=install_requires,
     packages=['firebase_admin'],
```

