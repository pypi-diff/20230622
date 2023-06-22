# Comparing `tmp/idoit_scaleup-0.0.8.tar.gz` & `tmp/idoit_scaleup-0.0.9.tar.gz`

## Comparing `idoit_scaleup-0.0.8.tar` & `idoit_scaleup-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,54 @@
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/build_and_upload_live.sh
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/build_and_upload_test.sh
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/idoit-python.code-workspace
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/test_install.sh
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/find_double_vlans.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/get_dialog.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/get_vlan.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/idoit.json.example
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/set_ip_address.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/set_logical_port.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/set_network_port.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/example/show_logical_network_ports.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/api_log.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/base.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_access.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_connector.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_cpu.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_ip.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_location.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_memory.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_network.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_network_log_port.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_networkport.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_power_consumer.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_racktables.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_storage_device.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/cat_vlan.py
--rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/category.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/conditional_read.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/consts.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/dialog.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/object.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/src/idoit_scaleup/search.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/LICENSE
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/build_and_upload_live.sh
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/build_and_upload_test.sh
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/error.log
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/idoit-python.code-workspace
+-rwxr-xr-x   0        0        0      710 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/request_20615.sh
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/test_call.sh
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/test_call.sh~
+-rwxr-xr-x   0        0        0      475 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/test_call2.sh
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/test_install.sh
+-rw-r--r--   0        0        0    37812 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/VLANS.md
+-rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/ana.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/find_double_vlans.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/find_double_vlans_in_8_dateien.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/fix_lat_lon.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/fix_pdu_name.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/get_dialog.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/get_vlan.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/idoit.json.example
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/idoit.json~
+-rw-r--r--   0        0        0    18960 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/kunden_racks.txt
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/lat_lon_1.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/set_ip_address.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/set_logical_port.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/set_network_port.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/show_logical_network_ports.py
+-rw-r--r--   0        0        0     8509 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/stromableser_cat.py
+-rw-r--r--   0        0        0    56352 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/example/whmcs.json
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/api_log.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/base.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_access.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_connector.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_cpu.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_ip.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_location.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_memory.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_network.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_network_log_port.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_networkport.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_power_consumer.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_racktables.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_storage_device.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/cat_vlan.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/category.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/conditional_read.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/consts.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/dialog.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/object.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/src/idoit_scaleup/search.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/LICENSE
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 idoit_scaleup-0.0.9/PKG-INFO
```

### Comparing `idoit_scaleup-0.0.8/build_and_upload_test.sh` & `idoit_scaleup-0.0.9/build_and_upload_test.sh`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/example/find_double_vlans.py` & `idoit_scaleup-0.0.9/example/find_double_vlans.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/example/set_ip_address.py` & `idoit_scaleup-0.0.9/example/set_ip_address.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/example/set_logical_port.py` & `idoit_scaleup-0.0.9/example/set_logical_port.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,41 +2,32 @@
 
 from idoit_scaleup import createApiCalls, consts
 
 import json
 
 config_file = 'idoit.json'
 
-OBJ_ID = 4005
+OBJ_ID = 3115
 
 f = open(config_file)
 cfg = json.load(f)
 f.close()
 idoit_apis = createApiCalls(cfg)
 api = idoit_apis[consts.C__CATG__NETWORK_LOG_PORT]
 api.set_debug_mode()
 data = {
-    'title': 'bond1',
-    'mac': 'C8:1F:66:CA:29:52',
-    'id': 6,
+    'title': 'mgm0',
+    'id': 114,
+    'active': 1,
     'port_type': 1,
-    'ports': [7490, 9188],
-    'addresses': [11],
+    'ports': [],
+    'addresses': [256],
 }
 cats = api.update_category(OBJ_ID, data)
 
-data = {
-    'title': 'mgm0',
-    'id': 7,
-    'parent': 6,
-    'net': [12619],
-    'addresses': [7],
-}
-cats = api.update_category(OBJ_ID, data)
 
 print(json.dumps(cats))
 print('----------------')
 api.set_debug_mode(False)
 cats = api.read_categories(OBJ_ID)
 for cat in cats:
-    # if cat['id']==6:
     print(json.dumps(cat))
```

### Comparing `idoit_scaleup-0.0.8/example/set_network_port.py` & `idoit_scaleup-0.0.9/example/set_network_port.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/__init__.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/__init__.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/api_log.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/api_log.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/base.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/base.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_connector.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_connector.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_location.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_location.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_network_log_port.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_network_log_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         raise Exception(
             'Funktioniert nur wenn es nur eine Kategorie gibt, ' +
             'muss mit ID spezifiziert werden')
 
     def fix_obj(self, cdata):
         if ('interface' in cdata.keys()) and (cdata['interface'] is not None):
             cdata['interface'] = "%d_C__CATG__NETWORK_INTERFACE" % cdata['interface']
-
         if ('addresses' in cdata.keys()) and (cdata['addresses'] is not None):
             rtn = []
             for ele in cdata['addresses']:
-                rtn.append("%d_C__CATG__IP" % ele)
+                rtn.append(str(ele))
             cdata['addresses'] = rtn
+
         if ('ports' in cdata.keys()) and (cdata['ports'] is not None):
             rtn = []
             for ele in cdata['ports']:
                 rtn.append("%d_%s" % (ele, C__CATG__NETWORK_PORT))
             cdata['ports'] = rtn
 
     def save_category(self, objId, data):
```

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_networkport.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_networkport.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_racktables.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_racktables.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/cat_vlan.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/cat_vlan.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/category.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/category.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/conditional_read.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/conditional_read.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/consts.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/consts.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/dialog.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/dialog.py`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/src/idoit_scaleup/object.py` & `idoit_scaleup-0.0.9/src/idoit_scaleup/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 from .base import IDoitApiBase
 
 
 class IDoitObject(IDoitApiBase):
     def __init__(self, cfg, obj_type: str):
         super().__init__(cfg)
         self.obj_type = obj_type
+
     def get_by_title(self, title: str, categories: List = []):
         params = {
             'filter': {
                 'type': self.obj_type,
                 'title': title,
             },
-            'categories': categories
         }
+        if len(categories) > 0:
+            params['categories'] = categories
         rtn = self.xml_rpc_call('cmdb.objects', params)
         if len(rtn['result']) == 0:
             return None
         else:
             return rtn['result'][0]
 
     def get_all(self, categories: List = []):
         params = {
             'filter': {
                 'type': self.obj_type
             },
-            'categories': categories
         }
+        if len(categories) > 0:
+            params['categories'] = categories
         rtn = self.xml_rpc_call('cmdb.objects', params)
         return rtn['result']
 
     def create_object_with_title(self, title: str):
         params = {
             'title': title,
             'type': self.obj_type
@@ -50,8 +53,8 @@
         return objId
 
     def update_object(self, obj_id: str, title: str):
         params = {
             'id': obj_id,
             'title': title,
         }
-        return self.xml_rpc_call('cmdb.object.update', params)
+        return self.xml_rpc_call('cmdb.object.update', params)
```

### Comparing `idoit_scaleup-0.0.8/LICENSE` & `idoit_scaleup-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idoit_scaleup-0.0.8/pyproject.toml` & `idoit_scaleup-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "idoit_scaleup"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sven Anders", email="sanders@scaleuptech.com" },
   { name="Freerk-Ole Zakfeld", email="fzakfeld@scaleuptech.com" }
 ]
 description = "i-doit pythonapi"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `idoit_scaleup-0.0.8/PKG-INFO` & `idoit_scaleup-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoit_scaleup
-Version: 0.0.8
+Version: 0.0.9
 Summary: i-doit pythonapi
 Project-URL: Homepage, https://github.com/ScaleUp-Technologies/i-doit-python
 Project-URL: Bug Tracker, https://github.com/ScaleUp-Technologies/i-doit-python/issues
 Author-email: Sven Anders <sanders@scaleuptech.com>, Freerk-Ole Zakfeld <fzakfeld@scaleuptech.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

