# Comparing `tmp/simplenetlink-0.5-py3-none-any.whl.zip` & `tmp/simplenetlink-0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9624 bytes, number of entries: 6
--rw-r--r--  2.0 unx    15987 b- defN 21-Jan-21 11:13 simplenetlink/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 21-Jan-21 11:17 simplenetlink-0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     6408 b- defN 21-Jan-21 11:17 simplenetlink-0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jan-21 11:17 simplenetlink-0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 21-Jan-21 11:17 simplenetlink-0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      490 b- defN 21-Jan-21 11:17 simplenetlink-0.5.dist-info/RECORD
-6 files, 34348 bytes uncompressed, 8738 bytes compressed:  74.6%
+Zip file size: 9996 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    17484 b- defN 23-Jun-22 14:18 simplenetlink/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-22 14:20 simplenetlink-0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6442 b- defN 23-Jun-22 14:20 simplenetlink-0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 14:20 simplenetlink-0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 14:20 simplenetlink-0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      490 b- defN 23-Jun-22 14:20 simplenetlink-0.6.dist-info/RECORD
+6 files, 35879 bytes uncompressed, 9110 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: simplenetlink/__init__.py
 Comment: 
 
-Filename: simplenetlink-0.5.dist-info/LICENSE
+Filename: simplenetlink-0.6.dist-info/LICENSE
 Comment: 
 
-Filename: simplenetlink-0.5.dist-info/METADATA
+Filename: simplenetlink-0.6.dist-info/METADATA
 Comment: 
 
-Filename: simplenetlink-0.5.dist-info/WHEEL
+Filename: simplenetlink-0.6.dist-info/WHEEL
 Comment: 
 
-Filename: simplenetlink-0.5.dist-info/top_level.txt
+Filename: simplenetlink-0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: simplenetlink-0.5.dist-info/RECORD
+Filename: simplenetlink-0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplenetlink/__init__.py

```diff
@@ -7,17 +7,25 @@
 class SimpleNetlink(object):
     def __init__(self, namespace=None):
         self.ipr = IPRoute()
         self._log = logging.getLogger("SimpleNetlink")
         self._current_namespace = namespace
         self._previous_namespace_instance = None
         self._previous_namespace = None
-        # self._log.level = logging.DEBUG
+        self._log.level = logging.DEBUG
         self._supported_virtual_interface_types = ["ipvlan", "tagged"]
 
+
+    def reset(self):
+        self._current_namespace = None
+        self._previous_namespace_instance = None
+        self._previous_namespace = None
+        self.ipr.close()
+        self.ipr= IPRoute()
+
     def get_interface_index(self, ifname):
         res = self.ipr.link_lookup(ifname=ifname)
         if len(res) == 1:
             return res[0]
         else:
             if len(res) == 0:
                 raise ValueError(
@@ -117,15 +125,15 @@
             self._log.debug(
                 f"found interface {interface_name} in namespace {namespace} with index {idx}"
             )
         else:
             self._log.debug(f"cannot find interface {interface_name} in any namespace")
         return (namespace, idx)
 
-    def __create_tagged(self, interface_name, **kwargs):
+    def __create_tagged(self, interface_name,options={}, **kwargs):
         if kwargs.get("parent_interface"):
             (base_namespace, base_idx) = self.find_interface_in_all_namespaces(
                 kwargs.get("parent_interface")
             )
             self._log.debug(
                 f"found parent_interface {kwargs.get('parent_interface')} in namespace {base_namespace}"
             )
@@ -142,14 +150,15 @@
 
             self.ipr.link(
                 "add",
                 ifname=interface_name,
                 kind="vlan",
                 link=base_idx,
                 vlan_id=int(kwargs.get("vlan_id")),
+                **options
             )
             idx = self.get_interface_index(interface_name)
             namespace = kwargs.get("namespace")
             if namespace:
                 if kwargs.get("namespace") not in self.get_namespaces():
                     self.create_namespace(namespace)
                 self.ipr.link("set", index=idx, net_ns_fd=namespace)
@@ -159,34 +168,37 @@
                 self.ipr.link("set", index=idx, net_ns_pid=1)
             return (namespace, idx)
         else:
             raise ValueError(
                 f"parent_interface not specified for vlan interface {interface_name}"
             )
 
-    def __create_ipvlan(self, interface_name, **kwargs):
+    def __create_ipvlan(self, interface_name, options={}, **kwargs):
         ipvlan_modes = {
             "l2": 0,
             "l3": 1,
             "l3s": 2,
         }
         if kwargs.get("parent_interface"):
             (base_namespace, base_idx) = self.find_interface_in_all_namespaces(
                 kwargs.get("parent_interface")
             )
             self._log.debug(f"found parent_interface in namespace {base_namespace}")
             self.set_current_namespace(base_namespace)
+
             self.ipr.link(
                 "add",
                 ifname=interface_name,
                 kind="ipvlan",
                 link=base_idx,
                 ipvlan_mode=ipvlan_modes[
                     "l2"
                 ],  # l2 mode so arp can be handled from namespace
+                **options
+                
             )
             idx = self.get_interface_index(interface_name)
             namespace = kwargs.get("namespace")
             if namespace:
                 self.set_current_namespace(namespace)
                 self.set_current_namespace(base_namespace)
                 self.ipr.link("set", index=idx, net_ns_fd=kwargs.get("namespace"))
@@ -198,31 +210,51 @@
             return (namespace, idx)
         else:
             raise ValueError(
                 f"parent_interface not specified for ipvlan interface {interface_name}"
             )
 
     def create_interface(self, interface_name, **kwargs):
+        options={}
+        if kwargs.get("mtu"):
+            options["mtu"]=kwargs.get("mtu")
 
         f = getattr(self, f"_SimpleNetlink__create_{kwargs.get('type')}")
         if f:
-            (namespace, idx) = f(interface_name, **kwargs)
+            (namespace, idx) = f(interface_name, options, **kwargs)
             if kwargs.get("link_state", "").lower() == "down":
                 self.ipr.link("set", index=idx, state="down")
             else:
                 self._log.debug(
                     f"enabling interface {interface_name} in namespace {namespace}"
                 )
                 self.ipr.link("set", index=idx, state="up")
             return (namespace, idx)
         else:
             raise ValueError(f"type {kwargs.get('type')} not implemented")
 
-    def ensure_interface_exists(self, interface, **kwargs):
+    def _resolve_interface_type_by_index(self,idx):
+        info={}
+        from pprint import pprint
+        for attr in self.ipr.link("get", index=idx)[0]['attrs']:
+            print(attr[0])
+            if attr[0] == "IFLA_LINKINFO":
+                for inner_attr in attr[1]["attrs"]:
+                    if inner_attr[0] == "IFLA_INFO_KIND":
+                        info['type']=inner_attr[1]
+                    if info['type'] == 'vlan' and inner_attr[0] == "IFLA_INFO_DATA":
+                        for ii in inner_attr[1]['attrs']:
+                            if ii[0] == "IFLA_VLAN_ID":
+                                info['vlan_id']=ii[1]
+                break
+        return info
+
 
+    def ensure_interface_exists(self, interface, **kwargs):
+        self.reset()
         namespace, idx = self.find_interface_in_all_namespaces(interface)
         if idx:
             if kwargs.get("namespace") != namespace:
                 self._log.debug(
                     f'interface is in namespace {namespace} -> moving to {kwargs.get("namespace")}'
                 )
 
@@ -233,25 +265,32 @@
                     self.set_current_namespace(kwargs.get("namespace"))
                     self.interface_up(interface)
                 else:
                     self.set_current_namespace(namespace)
                     self.ipr.link("set", index=idx, net_ns_pid=1)
                     self.set_current_namespace(None)
                     self.interface_up(interface)
+            interface_info=self._resolve_interface_type_by_index(idx)
+            if kwargs.get('type'):
+                if interface_info.get('type') != kwargs.get('type'):
+                    self.delete_interface()
+                    raise ValueError("Cannot change interface type. please delete the interface and recreate with new configuration")
+            
+
         else:
             if kwargs.get("type") in self._supported_virtual_interface_types:
                 self._log.debug(
                     f'interface type of {interface} is virtual interface of type {kwargs.get("type")} which does not exist -> creating'
                 )
                 namespace, idx = self.create_interface(interface, **kwargs)
             else:
                 raise ValueError(
                     f"either physical interface just doesn't exist (typo?) or virtual type {kwargs.get('type')} is not supported"
                 )
-
+        
         for ipv4_config_item in kwargs.get("ipv4", []):
             self.interface_add_ipv4(interface, ipv4_config_item)
 
         return (namespace, idx)
 
     def interface_add_ipv4(self, interface_name, prefix):
         idx = self.get_interface_index(interface_name)
@@ -297,23 +336,23 @@
             else:
                 raise (e)
         self._log.debug(
             f"setting ipv4_address {prefix} on {interface_name} in namespace {self._current_namespace}"
         )
         return True
 
-    def interface_up(interface_name):
+    def interface_up(self,interface_name):
         idx = self.get_interface_index(interface_name)
         if not idx:
             raise ValueError(
                 f"interface {interface_name} not found in namespace {self._current_namespace}"
             )
         self.ipr.link("set", index=idx, state="up")
 
-    def interface_down(interface_name):
+    def interface_down(self,interface_name):
         idx = self.get_interface_index(interface_name)
         if not idx:
             raise ValueError(
                 f"interface {interface_name} not found in namespace {self._current_namespace}"
             )
         self.ipr.link("set", index=idx, state="down")
```

## Comparing `simplenetlink-0.5.dist-info/LICENSE` & `simplenetlink-0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplenetlink-0.5.dist-info/METADATA` & `simplenetlink-0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: simplenetlink
-Version: 0.5
+Version: 0.6
 Summary: Abstraction layer for for simplified usage of pyroute2
 Home-page: https://github.com/jinjamator/simplenetlink
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Requires-Dist: pyroute2
 
 Introduction
 ==================
 
 
 Simplenetlink is an abstraction layer to simplify programatic non-persistent network configuration for linux on top of pyroute2. It was written to have a simple interface for network test setups. 
@@ -176,15 +177,15 @@
     """
 
     config=yaml.safe_load(yml)
 
     # for k,v in config.items():
     #     if v.get('namespace'):
     #         ip.delete_namespace(v.get('namespace'))
-
+            
     for k,v in config.items():
         ip.ensure_interface_exists(k,**v)
 
     ip.set_current_namespace('test')
     ip.add_route('0.0.0.0/0','100.64.0.1')
     ip.set_current_namespace('test2')
     ip.add_route('0.0.0.0/0','100.64.0.1')
```

