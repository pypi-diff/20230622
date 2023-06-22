# Comparing `tmp/napalm-slx-os-0.1.1.tar.gz` & `tmp/napalm-slx-os-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-slx-os-0.1.1.tar", last modified: Mon May  8 15:00:09 2023, max compression
+gzip compressed data, was "napalm-slx-os-0.2.0.tar", last modified: Thu Jun 22 11:30:41 2023, max compression
```

## Comparing `napalm-slx-os-0.1.1.tar` & `napalm-slx-os-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/
--rw-r--r--   0 jens      (1000) jens      (1000)    11357 2020-08-24 14:43:55.000000 napalm-slx-os-0.1.1/LICENSE
--rw-r--r--   0 jens      (1000) jens      (1000)      114 2023-04-05 12:27:42.000000 napalm-slx-os-0.1.1/MANIFEST.in
--rw-r--r--   0 jens      (1000) jens      (1000)      575 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      127 2023-05-08 13:59:45.000000 napalm-slx-os-0.1.1/README.md
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/napalm_slx_os/
--rw-r--r--   0 jens      (1000) jens      (1000)      735 2023-04-05 12:36:34.000000 napalm-slx-os-0.1.1/napalm_slx_os/__init__.py
--rw-r--r--   0 jens      (1000) jens      (1000)    15070 2023-05-08 14:58:53.000000 napalm-slx-os-0.1.1/napalm_slx_os/slx_os.py
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/napalm_slx_os/utils/
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/
--rw-r--r--   0 jens      (1000) jens      (1000)      110 2023-04-05 14:20:56.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_inventory_chassis.tpl
--rw-r--r--   0 jens      (1000) jens      (1000)     1419 2023-05-05 12:49:27.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_neighbors.tpl
--rw-r--r--   0 jens      (1000) jens      (1000)      429 2023-05-05 12:04:57.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_summary.tpl
--rw-r--r--   0 jens      (1000) jens      (1000)     1434 2023-05-08 13:47:23.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_neighbors.tpl
--rw-r--r--   0 jens      (1000) jens      (1000)      573 2023-05-08 13:47:29.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_summary.tpl
--rw-r--r--   0 jens      (1000) jens      (1000)      165 2023-04-05 13:10:21.000000 napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_version.tpl
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/
--rw-r--r--   0 jens      (1000) jens      (1000)      575 2023-05-08 15:00:09.000000 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      664 2023-05-08 15:00:09.000000 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/SOURCES.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        1 2023-05-08 15:00:09.000000 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/dependency_links.txt
--rw-r--r--   0 jens      (1000) jens      (1000)      149 2023-05-08 15:00:09.000000 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/requires.txt
--rw-r--r--   0 jens      (1000) jens      (1000)       14 2023-05-08 15:00:09.000000 napalm-slx-os-0.1.1/napalm_slx_os.egg-info/top_level.txt
--rw-r--r--   0 jens      (1000) jens      (1000)      861 2023-05-08 14:59:07.000000 napalm-slx-os-0.1.1/pyproject.toml
--rw-r--r--   0 jens      (1000) jens      (1000)      521 2023-05-08 15:00:09.144736 napalm-slx-os-0.1.1/setup.cfg
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/
+-rw-r--r--   0 jens      (1000) jens      (1000)    11357 2020-08-24 14:43:55.000000 napalm-slx-os-0.2.0/LICENSE
+-rw-r--r--   0 jens      (1000) jens      (1000)      114 2023-04-05 12:27:42.000000 napalm-slx-os-0.2.0/MANIFEST.in
+-rw-r--r--   0 jens      (1000) jens      (1000)     2495 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/PKG-INFO
+-rw-r--r--   0 jens      (1000) jens      (1000)     2047 2023-06-17 16:12:11.000000 napalm-slx-os-0.2.0/README.md
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/napalm_slx_os/
+-rw-r--r--   0 jens      (1000) jens      (1000)      735 2023-04-05 12:36:34.000000 napalm-slx-os-0.2.0/napalm_slx_os/__init__.py
+-rw-r--r--   0 jens      (1000) jens      (1000)    18549 2023-06-17 15:50:57.000000 napalm-slx-os-0.2.0/napalm_slx_os/slx_os.py
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/napalm_slx_os/utils/
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/
+-rw-r--r--   0 jens      (1000) jens      (1000)      309 2023-06-17 15:30:53.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_arp.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)      110 2023-04-05 14:20:56.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_inventory_chassis.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)     1419 2023-05-05 12:49:27.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_neighbors.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)      429 2023-05-05 12:04:57.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_summary.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)     1434 2023-05-08 13:47:23.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_neighbors.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)      573 2023-05-08 13:47:29.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_summary.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)      165 2023-04-05 13:10:21.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_version.tpl
+-rw-r--r--   0 jens      (1000) jens      (1000)      197 2023-06-17 15:37:49.000000 napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_vrf.tpl
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/
+-rw-r--r--   0 jens      (1000) jens      (1000)     2495 2023-06-22 11:30:41.000000 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/PKG-INFO
+-rw-r--r--   0 jens      (1000) jens      (1000)      766 2023-06-22 11:30:41.000000 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/SOURCES.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)        1 2023-06-22 11:30:41.000000 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/dependency_links.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)      149 2023-06-22 11:30:41.000000 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/requires.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)       14 2023-06-22 11:30:41.000000 napalm-slx-os-0.2.0/napalm_slx_os.egg-info/top_level.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)      861 2023-06-22 11:27:38.000000 napalm-slx-os-0.2.0/pyproject.toml
+-rw-r--r--   0 jens      (1000) jens      (1000)      521 2023-06-22 11:30:41.147436 napalm-slx-os-0.2.0/setup.cfg
```

### Comparing `napalm-slx-os-0.1.1/LICENSE` & `napalm-slx-os-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os/__init__.py` & `napalm-slx-os-0.2.0/napalm_slx_os/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os/slx_os.py` & `napalm-slx-os-0.2.0/napalm_slx_os/slx_os.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 from napalm.base.exceptions import ConnectionClosedException
 from napalm.base.helpers import textfsm_extractor
 from napalm.base.netmiko_helpers import netmiko_args
 from netmiko import BaseConnection
 
 
 @dataclasses.dataclass
+class _VRF:
+    name: str
+    id: int
+
+
+@dataclasses.dataclass
 class _BGPNeighborDetail:
     ip_address: str
     asn: int
     description: str
     bgp_type: str
     router_id: str
     vrf: str
@@ -165,26 +171,29 @@
         self.timeout = timeout
 
         if optional_args is None:
             optional_args = {}
 
         self.netmiko_optional_args = netmiko_args(optional_args)
 
+        self._candidate_config: Optional[str] = None
+        self._config_is_merge: bool = False
+
     def open(self):
         """Open connection to device"""
         self.device = self._netmiko_open(
             device_type='extreme_slx',
             netmiko_optional_args=self.netmiko_optional_args
         )
 
     def close(self):
         """Close connection to device"""
         self._netmiko_close()
 
-    def _send_command(self, command):
+    def _send_command(self, command: str) -> str:
         """Wrapper for self.device.send.command().
         If command is a list will iterate through commands until valid command.
         """
         try:
             output = self.device.send_command(command)
             return self._send_command_postprocess(output)
         except (socket.error, EOFError) as e:
@@ -365,15 +374,22 @@
             }
 
             bgp_detail[neighbor.vrf_name][neighbor.asn].append(details)
 
         # Make clean copy of all values to avoid pickling issues
         bgp_detail = json.loads(json.dumps(bgp_detail))
 
-        return bgp_detail
+        # Convert asn keys to int
+        result_bgp_detail = {}
+        for vrf_name, vrf_data in bgp_detail.items():
+            result_bgp_detail[vrf_name] = {}
+            for asn, asn_data in vrf_data.items():
+                result_bgp_detail[vrf_name][int(asn)] = asn_data
+
+        return result_bgp_detail
 
     def get_bgp_neighbors(self) -> Dict[str, models.BGPStateNeighborsPerVRFDict]:
         bgp_data = self._get_bgp_data()
 
         output = defaultdict(lambda: {"peers": {}})
 
         # TODO: Fix multi-vrf setup
@@ -406,7 +422,88 @@
                 }
             }
 
         # Make clean copy of all values to avoid pickling issues
         output = json.loads(json.dumps(output))
 
         return output
+
+    def load_merge_candidate(self, filename: Optional[str] = None, config: Optional[str] = None) -> None:
+        if filename is not None:
+            with open(filename, 'r') as f:
+                config_str = f.read()
+        elif config is not None:
+            config_str = config
+        else:
+            raise ValueError("filename or config must be provided")
+
+        self._candidate_config = config_str
+        self._config_is_merge = True
+
+    def discard_config(self) -> None:
+        self._candidate_config = None
+
+    def compare_config(self) -> str:
+        return 'no good mechanism exists to compare the config'
+
+    def commit_config(self, message: str = "", revert_in: Optional[int] = None) -> None:
+        if self._candidate_config is None:
+            raise ValueError("No config to commit")
+
+        if not self._config_is_merge:
+            raise ValueError("Only merge configs are supported")
+
+        self.device.send_config_set(config_commands=self._candidate_config.splitlines())
+        self._candidate_config = None
+
+    def get_config(
+            self, retrieve: str = "all", full: bool = False, sanitized: bool = False
+    ) -> models.ConfigDict:
+        # Caveat: sanitized is not supported
+
+        config_data = {
+            'running': '',
+            'startup': '',
+            'candidate': '',
+        }
+
+        all_suffix = " all" if full else ""
+
+        if retrieve in ("all", "running"):
+            config_data["running"] = self._send_command(f"show running-config{all_suffix}")
+        if retrieve in ("all", "startup"):
+            config_data["startup"] = self._send_command(f"show startup-config{all_suffix}")
+
+        return config_data
+
+    def slx_get_vrfs(self) -> List[_VRF]:
+        vrfs = []
+        vrf_data = self._send_and_parse_command("show vrf", 'show_vrf')
+        for vrf_entry in vrf_data:
+            vrfs.append(_VRF(name=vrf_entry['vrfname'], id=int(vrf_entry['vrfid'])))
+        return vrfs
+
+    def get_arp_table(self, vrf: str = "") -> List[models.ARPTableDict]:
+        if vrf == '':
+            vrfs_to_check = [vrf.name for vrf in self.slx_get_vrfs()]
+        else:
+            vrfs_to_check = [vrf]
+
+        arp_table: List[models.ARPTableDict] = []
+        for vrf_name in vrfs_to_check:
+            arp_data = self._send_and_parse_command(f"show arp vrf {vrf_name}", 'show_arp')
+            for arp_entry in arp_data:
+                # convert age from hh:mm:ss to seconds
+                age = arp_entry['age']
+                age_parts = age.split(':')
+                age_seconds = int(age_parts[0]) * 3600 + int(age_parts[1]) * 60 + int(age_parts[2])
+
+                interface = arp_entry['l2interface'].replace(' ', '') + '|' + arp_entry['l3interface'].replace(' ', '')
+
+                arp_table.append({
+                    'interface': interface,
+                    'mac': arp_entry['macaddress'],
+                    'ip': arp_entry['address'],
+                    'age': age_seconds,
+                })
+
+        return arp_table
```

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_neighbors.tpl` & `napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ip_bgp_neighbors.tpl`

 * *Files identical despite different names*

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_neighbors.tpl` & `napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_neighbors.tpl`

 * *Files identical despite different names*

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_summary.tpl` & `napalm-slx-os-0.2.0/napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_summary.tpl`

 * *Files identical despite different names*

### Comparing `napalm-slx-os-0.1.1/napalm_slx_os.egg-info/SOURCES.txt` & `napalm-slx-os-0.2.0/napalm_slx_os.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,13 +6,15 @@
 napalm_slx_os/__init__.py
 napalm_slx_os/slx_os.py
 napalm_slx_os.egg-info/PKG-INFO
 napalm_slx_os.egg-info/SOURCES.txt
 napalm_slx_os.egg-info/dependency_links.txt
 napalm_slx_os.egg-info/requires.txt
 napalm_slx_os.egg-info/top_level.txt
+napalm_slx_os/utils/textfsm_templates/show_arp.tpl
 napalm_slx_os/utils/textfsm_templates/show_inventory_chassis.tpl
 napalm_slx_os/utils/textfsm_templates/show_ip_bgp_neighbors.tpl
 napalm_slx_os/utils/textfsm_templates/show_ip_bgp_summary.tpl
 napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_neighbors.tpl
 napalm_slx_os/utils/textfsm_templates/show_ipv6_bgp_summary.tpl
-napalm_slx_os/utils/textfsm_templates/show_version.tpl
+napalm_slx_os/utils/textfsm_templates/show_version.tpl
+napalm_slx_os/utils/textfsm_templates/show_vrf.tpl
```

### Comparing `napalm-slx-os-0.1.1/pyproject.toml` & `napalm-slx-os-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "napalm-slx-os"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name = "Jens Vogler", email = "vogler@init7.net" }
 ]
 description = "SLX-OS Driver for NAPALM"
 readme = "README.md"
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `napalm-slx-os-0.1.1/setup.cfg` & `napalm-slx-os-0.2.0/setup.cfg`

 * *Files identical despite different names*

