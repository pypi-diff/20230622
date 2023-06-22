# Comparing `tmp/breeze_strategies-6.0.4.tar.gz` & `tmp/breeze_strategies-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.4.tar", last modified: Thu Jun 22 07:36:04 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.5.tar", last modified: Thu Jun 22 08:54:09 2023, max compression
```

## Comparing `breeze_strategies-6.0.4.tar` & `breeze_strategies-6.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.987253 breeze_strategies-6.0.4/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.4/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-22 07:36:04.984253 breeze_strategies-6.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-22 07:28:15.000000 breeze_strategies-6.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.831358 breeze_strategies-6.0.4/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.4/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20409 2023-06-22 07:33:12.000000 breeze_strategies-6.0.4/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.979261 breeze_strategies-6.0.4/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:36:04.987253 breeze_strategies-6.0.4/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-22 07:28:24.000000 breeze_strategies-6.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:09.478360 breeze_strategies-6.0.5/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-22 08:54:09.477364 breeze_strategies-6.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-22 08:53:40.000000 breeze_strategies-6.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:09.432182 breeze_strategies-6.0.5/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.5/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20417 2023-06-22 08:54:01.000000 breeze_strategies-6.0.5/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:09.470811 breeze_strategies-6.0.5/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-22 08:54:09.000000 breeze_strategies-6.0.5/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-22 08:54:09.000000 breeze_strategies-6.0.5/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:54:09.000000 breeze_strategies-6.0.5/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 08:54:09.000000 breeze_strategies-6.0.5/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-22 08:54:09.000000 breeze_strategies-6.0.5/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:54:09.479358 breeze_strategies-6.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-22 08:53:32.000000 breeze_strategies-6.0.5/setup.py
```

### Comparing `breeze_strategies-6.0.4/LICENSE` & `breeze_strategies-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.4/PKG-INFO` & `breeze_strategies-6.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.4
+Version: 6.0.5
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.4
+pip install breeze_strategies==6.0.5
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.4/README.md` & `breeze_strategies-6.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.4
+pip install breeze_strategies==6.0.5
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.4/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.5/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,19 +332,19 @@
                     sqcall_price = record["average_price"]
                     break
             for record in putrecords["Success"]:
                 if(record['status'] == "Executed"):
                     sqput_price = record["average_price"]
                     break
             
-            plcall = round((float(sqcall_price) - int(self.callexecution))*int(self.quantity),2)
-            plput = round((float(sqput_price) - int(self.putexecution))*int(self.quantity),2)
+            plcall = round((float(sqcall_price) - float(self.callexecution))*int(self.quantity),2)
+            plput = round((float(sqput_price) - float(self.putexecution))*int(self.quantity),2)
 
-            self.currentcall = (float(sqcall_price) - int(self.callexecution))
-            self.currentput = (float(sqput_price) - int(self.putexecution))
+            self.currentcall = (float(sqcall_price) - float(self.callexecution))
+            self.currentput = (float(sqput_price) - float(self.putexecution))
 
             print("-------------------------------------------------------")
             print("Profit and Loss Report........")
             print(f"P&L (CALL) : {plcall}/- Rs")
             print(f"P&L (PUT) : {plput}/- Rs")
             print(f"P&L (NET) : {plput + plcall}/- Rs")
             print("-------------------------------------------------------")
```

### Comparing `breeze_strategies-6.0.4/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.5/breeze_strategies.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.4
+Version: 6.0.5
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.4
+pip install breeze_strategies==6.0.5
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.4/setup.py` & `breeze_strategies-6.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.4",
+    version="6.0.5",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

