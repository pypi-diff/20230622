# Comparing `tmp/pyDocsis-0.3.25.tar.gz` & `tmp/pyDocsis-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDocsis-0.3.25.tar", last modified: Thu Jun 22 17:10:10 2023, max compression
+gzip compressed data, was "pyDocsis-0.3.6.tar", last modified: Mon Jun 12 16:43:39 2023, max compression
```

## Comparing `pyDocsis-0.3.25.tar` & `pyDocsis-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-22 17:10:10.320494 pyDocsis-0.3.25/
--rw-r--r--   0 tbalsley   (501) staff       (20)    11357 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/LICENSE
--rw-r--r--   0 tbalsley   (501) staff       (20)      260 2023-06-22 17:10:10.320217 pyDocsis-0.3.25/PKG-INFO
--rw-r--r--   0 tbalsley   (501) staff       (20)     1041 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/README.md
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-22 17:10:10.312500 pyDocsis-0.3.25/Scripts/
--rw-r--r--   0 tbalsley   (501) staff       (20)      322 2023-06-12 20:12:39.000000 pyDocsis-0.3.25/Scripts/cm_decode
--rw-r--r--   0 tbalsley   (501) staff       (20)    14691 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/Scripts/mib-json-builder.py
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-22 17:10:10.313434 pyDocsis-0.3.25/pyDocsis.egg-info/
--rw-r--r--   0 tbalsley   (501) staff       (20)      260 2023-06-22 17:10:10.000000 pyDocsis-0.3.25/pyDocsis.egg-info/PKG-INFO
--rw-r--r--   0 tbalsley   (501) staff       (20)      382 2023-06-22 17:10:10.000000 pyDocsis-0.3.25/pyDocsis.egg-info/SOURCES.txt
--rw-r--r--   0 tbalsley   (501) staff       (20)        1 2023-06-22 17:10:10.000000 pyDocsis-0.3.25/pyDocsis.egg-info/dependency_links.txt
--rw-r--r--   0 tbalsley   (501) staff       (20)        9 2023-06-22 17:10:10.000000 pyDocsis-0.3.25/pyDocsis.egg-info/top_level.txt
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-22 17:10:10.319757 pyDocsis-0.3.25/pydocsis/
--rw-r--r--   0 tbalsley   (501) staff       (20)     4562 2023-06-12 16:14:21.000000 pyDocsis-0.3.25/pydocsis/MTATlvs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     7842 2023-06-12 16:14:21.000000 pyDocsis-0.3.25/pydocsis/MtaConfig.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     6153 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/pydocsis/TLV.py
--rw-r--r--   0 tbalsley   (501) staff       (20)      111 2023-06-12 16:14:21.000000 pyDocsis-0.3.25/pydocsis/__init__.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     7329 2023-06-12 20:16:40.000000 pyDocsis-0.3.25/pydocsis/cmConfig.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     1698 2023-06-12 16:14:21.000000 pyDocsis-0.3.25/pydocsis/configFile.py
--rw-r--r--   0 tbalsley   (501) staff       (20)   620089 2023-06-12 16:14:21.000000 pyDocsis-0.3.25/pydocsis/docsisTlvs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)    12287 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/pydocsis/mib.py
--rw-r--r--   0 tbalsley   (501) staff       (20)    41373 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/pydocsis/mtaMibs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)       38 2023-06-22 17:10:10.320568 pyDocsis-0.3.25/setup.cfg
--rw-r--r--   0 tbalsley   (501) staff       (20)      474 2023-06-22 17:09:20.000000 pyDocsis-0.3.25/setup.py
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.789633 pyDocsis-0.3.6/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      235 2023-06-12 16:43:39.789419 pyDocsis-0.3.6/PKG-INFO
+-rw-r--r--   0 tbalsley   (501) staff       (20)      329 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/README.md
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.785669 pyDocsis-0.3.6/Scripts/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      319 2023-06-12 16:32:24.000000 pyDocsis-0.3.6/Scripts/cm_decode
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.786549 pyDocsis-0.3.6/pyDocsis.egg-info/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      235 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/PKG-INFO
+-rw-r--r--   0 tbalsley   (501) staff       (20)      346 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/SOURCES.txt
+-rw-r--r--   0 tbalsley   (501) staff       (20)        1 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/dependency_links.txt
+-rw-r--r--   0 tbalsley   (501) staff       (20)        9 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/top_level.txt
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.789135 pyDocsis-0.3.6/pydocsis/
+-rw-r--r--   0 tbalsley   (501) staff       (20)     4562 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/MTATlvs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     7842 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/MtaConfig.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     5294 2023-06-12 16:36:55.000000 pyDocsis-0.3.6/pydocsis/TLV.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)      111 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/__init__.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     6664 2023-06-12 16:40:45.000000 pyDocsis-0.3.6/pydocsis/cmConfig.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     1698 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/configFile.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)   620089 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/docsisTlvs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)    11777 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/mib.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)    15401 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/mtaMibs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)       38 2023-06-12 16:43:39.789693 pyDocsis-0.3.6/setup.cfg
+-rw-r--r--   0 tbalsley   (501) staff       (20)      431 2023-06-12 16:40:51.000000 pyDocsis-0.3.6/setup.py
```

### Comparing `pyDocsis-0.3.25/pydocsis/MTATlvs.py` & `pyDocsis-0.3.6/pydocsis/MTATlvs.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.3.25/pydocsis/MtaConfig.py` & `pyDocsis-0.3.6/pydocsis/MtaConfig.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.3.25/pydocsis/TLV.py` & `pyDocsis-0.3.6/pydocsis/TLV.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,43 +59,24 @@
             self.subTLVs = args["subTLVs"]
         else:
             self.subTLVs = []
         if "description" in args.keys():
             self.description = args["description"]
         else:
             self.description = ""
-    def toJSON(self):
-        retval = {}
-        if self.datatype == "snmp_object":
-            retval[self.tag] = {}
-            retval[self.tag]["value"] = str(self.get_value().toJSON())
-            retval[self.tag]["datatype"] = self.datatype 
-            retval[self.tag]["description"] = self.description
-            
-        elif len(self.subTLVs) == 0:
-            retval[self.tag] = {}
-            retval[self.tag]["value"] = str(self.get_value())
-            retval[self.tag]["datatype"] = self.datatype 
-            retval[self.tag]["description"] = self.description
-        else:
-            retval[self.tag] = {}
-            retval[self.tag]["description"] = self.description
-            retval[self.tag]["subTLVs"] = []
-            for st in self.subTLVs:
-                retval[self.tag]["subTLVs"].append(st.toJSON())
-        return retval
+
     def encode_for_file(self, tags=None):
         if tags is None:
             tags = {}
         if tags == {}:
             tags = DocsisTlvs
         tlv_string = ''
         htag = tags[self.tag]["hex"]
         tvalue = self.value
-        # print(tvalue)
+        print(tvalue)
         for st in self.subTLVs:
             tvalue += st.encode_for_file(tags[self.tag]["subTlvs"])
         if divmod(len(tvalue), 2)[1] == 1:
             print(htag)
             print(tvalue)
             print(divmod(len(tvalue), 2))
             raise ValueError('Invalid value length - the length must be even')
@@ -160,15 +141,15 @@
         elif self.datatype == "snmp_object":
             m = MIB()
             m.decode(value)
             if oid != "":
                 m.oid = oid
             if value != "":
                 m.value = value
-            # print(m.encode())
+            print(m.encode())
             self.value = m.encode()
 
         elif self.datatype == "strzero":
             # print(self.value)
             newval = ""
             # for ch in value:
             tmp = binascii.hexlify(value.encode("ascii")).decode()
```

### Comparing `pyDocsis-0.3.25/pydocsis/cmConfig.py` & `pyDocsis-0.3.6/pydocsis/cmConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,32 +148,15 @@
         while (len(stuff) / 2) % 4 != 0:
             stuff += "00"
         # print(stuff)
         if self.configFilePath != "":
             f = open(self.configFilePath, "wb")
             f.write(binascii.unhexlify(stuff))
             f.close()
-    def toJSON(self):
-        stuff = ''
-        retval = []
-        for tag in self.tlvs:
-            if tag.tag not in ["06", "07", "255"]:
-                if tag.tag != "00":
-                    stuff += tag.encode_for_file()
-                    retval.append(tag.toJSON())
-            elif tag.tag in ["06"]:
-                newval = hashlib.md5(binascii.unhexlify(stuff))
-                # print(newval.hexdigest())
-                if newval.hexdigest() == tag.get_value():
-                    retval.append({"MIC": "TLV6 is correct"})
-                else:
-                    retval.append({"MIC": "TLV6 is incorrect"})
-        return retval
-            
-			
+
 
 def json_this(tlvs):
     """
 I don't think I am using this for anything. It _should_ convert a cm config, or at least it's list of TLVs, into JSON
     :param tlvs: list of TLVs
     :type tlvs: [TLV]
     :return: a disct that can be easily converted to json
```

### Comparing `pyDocsis-0.3.25/pydocsis/configFile.py` & `pyDocsis-0.3.6/pydocsis/configFile.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.3.25/pydocsis/docsisTlvs.py` & `pyDocsis-0.3.6/pydocsis/docsisTlvs.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.3.25/pydocsis/mib.py` & `pyDocsis-0.3.6/pydocsis/mib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Mibs! So useful, and annoying!
 """
 # import codecs
 import binascii
-import json
-import os
+from pydocsis.mtaMibs import mibs
+
 # import hashlib
 
 # import asn1
 
 
 oidDataTypes = {"103": "HexString", "66": "UInt32", "64": "IPAddress", "6": "objectIdentifier", "5": "Null",
                 "4": "HexString", "3": "BitString", "2": "Integer32", "1": "Boolean"}
@@ -54,30 +54,24 @@
     def __init__(self):
         # storing these as strings
         self.oid = ""
         self.index = ""
         self.value = ""
         self.dataType = ""
         self.isHashed = False
-        self.description = ""
-    
-    def toJSON(self):
-        return {"oid": self.oid, "value": self.value, "datatype": self.dataType, "description": self.description}
-        
 
     def decode(self, hex_junk):
         """
         based on panda_inline4's comment at
         https://stackoverflow.com/questions/49653398/converting-oid-of-public-key-etc-in-hex-data-to-the-dot-format
 
         """
         # decodes the mib stuff from the config file.
-        mibs = json.load(open(os.path.expanduser('~/.mibs.json')))
         hex_list = []
-        OID_str = '.'
+        OID_str = ''
         for char in range(0, len(hex_junk), 2):
             hex_list.append(hex_junk[char] + hex_junk[char + 1])
 
         for element in range(len(hex_list)):
             hex_list[element] = int(hex_list[element], 16)
         # decoder = asn1.Decoder()
         # decoder.start(hex_list)
@@ -121,27 +115,23 @@
         while len(hex_list) > 0:
             oidlength -= 1
             val = ((val << 7) | ((hex_list[0] & 0x7F)))
             if in_index == False:
                 if (hex_list[0] & 0x80) != 0x80:
                     OID_str += "." + str(val)
                     val = 0
-                # if len([x for x in mibs.keys() if x.startswith(OID_str)]) == 1:
-                #     in_index = True
-                #     self.description = mibs[OID_str]["name"]
+                if OID_str in mibs.keys():
+                    in_index = True
             else:
                 # print(binascii.unhexlify(str(hex(hex_list[0])).replace('0x', '')))
                 try:
                     self.index += str(binascii.unhexlify(str(hex(hex_list[0])).replace('0x', '')).decode())
                 except:
-                    self.index += str(hex_list[0])
+                    self.index += "X" + str(hex_list[0])
             self.oid = OID_str
-            if len([x for x in mibs.keys() if x.startswith(OID_str)]) == 1:
-                    # in_index = True
-                    self.description = mibs[OID_str]["name"]
             # print(self.oid)
             if oidlength == 0:
                 del hex_list[0]
                 datatype = hex_list[0]
                 del hex_list[0]
                 datalength = int(str(hex_list[0]), 16)
                 del hex_list[0]
@@ -155,15 +145,15 @@
                         if oidDataTypes[str(datatype)] == "IPAddress":
                             snmpdata += str(hex_list[0])
                             if len(hex_list) > 1:
                                 snmpdata += "."
                         elif oidDataTypes[str(datatype)] == "HexString":
                             working = ""
                             while len(hex_list) > 1:
-                                if self.oid == ".1.3.6.1.2.1.140.1.2.11" or self.oid == ".1.3.6.1.4.1.4115.11.1.52":
+                                if self.oid == "1.3.6.1.2.1.140.1.2.11" or self.oid == "1.3.6.1.4.1.4115.11.1.52":
                                     snmpdata += str(hex(hex_list[0])).replace('0x', '')
                                 else:
                                     # print(binascii.unhexlify(str(hex(hex_list[0])).replace('0x', '')))
                                     try:
                                         snmpdata += binascii.unhexlify(str(hex(hex_list[0])).replace('0x', '')).decode()
                                     except:
                                         if hex_list[0] == 13:
```

