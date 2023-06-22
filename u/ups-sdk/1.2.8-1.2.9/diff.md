# Comparing `tmp/ups_sdk-1.2.8.tar.gz` & `tmp/ups_sdk-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ups_sdk-1.2.8.tar", last modified: Sat Feb 18 08:44:00 2023, max compression
+gzip compressed data, was "ups_sdk-1.2.9.tar", last modified: Thu Jun 22 14:53:40 2023, max compression
```

## Comparing `ups_sdk-1.2.8.tar` & `ups_sdk-1.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 08:44:00.138431 ups_sdk-1.2.8/
--rw-rw-rw-   0        0        0     1089 2022-11-25 12:45:05.000000 ups_sdk-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      288 2023-02-18 08:44:00.138431 ups_sdk-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      785 2023-01-03 08:26:58.000000 ups_sdk-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-18 08:44:00.075939 ups_sdk-1.2.8/UPS_SDK/
--rw-rw-rw-   0        0        0       22 2023-02-18 08:43:49.000000 ups_sdk-1.2.8/UPS_SDK/__init__.py
--rw-rw-rw-   0        0        0     1601 2023-01-19 08:01:48.000000 ups_sdk-1.2.8/UPS_SDK/main.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:44:00.122807 ups_sdk-1.2.8/UPS_SDK/models/
--rw-rw-rw-   0        0        0      489 2022-11-19 11:48:55.000000 ups_sdk-1.2.8/UPS_SDK/models/AccessRequest.py
--rw-rw-rw-   0        0        0     1015 2022-11-25 14:40:12.000000 ups_sdk-1.2.8/UPS_SDK/models/ActivityItem.py
--rw-rw-rw-   0        0        0      227 2022-11-25 14:40:18.000000 ups_sdk-1.2.8/UPS_SDK/models/ActivityLocation.py
--rw-rw-rw-   0        0        0      318 2023-02-02 10:37:30.000000 ups_sdk-1.2.8/UPS_SDK/models/Address.py
--rw-rw-rw-   0        0        0      130 2022-07-22 09:00:38.000000 ups_sdk-1.2.8/UPS_SDK/models/Message.py
--rw-rw-rw-   0        0        0     1138 2022-11-25 14:40:35.000000 ups_sdk-1.2.8/UPS_SDK/models/Package.py
--rw-rw-rw-   0        0        0      208 2022-11-25 14:40:41.000000 ups_sdk-1.2.8/UPS_SDK/models/PackageWeight.py
--rw-rw-rw-   0        0        0      171 2023-02-18 08:43:30.000000 ups_sdk-1.2.8/UPS_SDK/models/ReferenceNumber.py
--rw-rw-rw-   0        0        0      136 2022-07-22 08:59:52.000000 ups_sdk-1.2.8/UPS_SDK/models/ReferenceNumberItem.py
--rw-rw-rw-   0        0        0      265 2022-11-25 14:40:50.000000 ups_sdk-1.2.8/UPS_SDK/models/Response.py
--rw-rw-rw-   0        0        0      130 2022-07-22 08:59:48.000000 ups_sdk-1.2.8/UPS_SDK/models/Service.py
--rw-rw-rw-   0        0        0      144 2022-11-25 14:41:25.000000 ups_sdk-1.2.8/UPS_SDK/models/ShipTo.py
--rw-rw-rw-   0        0        0     1472 2022-11-25 14:41:10.000000 ups_sdk-1.2.8/UPS_SDK/models/Shipment.py
--rw-rw-rw-   0        0        0      211 2022-11-25 14:41:16.000000 ups_sdk-1.2.8/UPS_SDK/models/ShipmentWeight.py
--rw-rw-rw-   0        0        0      210 2023-01-19 08:05:19.000000 ups_sdk-1.2.8/UPS_SDK/models/Shipper.py
--rw-rw-rw-   0        0        0      220 2022-11-25 14:41:32.000000 ups_sdk-1.2.8/UPS_SDK/models/Status.py
--rw-rw-rw-   0        0        0      111 2022-07-22 09:00:10.000000 ups_sdk-1.2.8/UPS_SDK/models/StatusCode.py
--rw-rw-rw-   0        0        0      133 2022-07-22 09:00:06.000000 ups_sdk-1.2.8/UPS_SDK/models/StatusType.py
--rw-rw-rw-   0        0        0      525 2022-08-01 17:17:58.000000 ups_sdk-1.2.8/UPS_SDK/models/TrackError.py
--rw-rw-rw-   0        0        0     1300 2022-11-23 15:20:45.000000 ups_sdk-1.2.8/UPS_SDK/models/TrackRequest.py
--rw-rw-rw-   0        0        0     1131 2022-12-27 09:18:28.000000 ups_sdk-1.2.8/UPS_SDK/models/TrackResponse.py
--rw-rw-rw-   0        0        0      149 2022-11-19 11:52:25.000000 ups_sdk-1.2.8/UPS_SDK/models/TrackType.py
--rw-rw-rw-   0        0        0      156 2022-08-01 17:20:10.000000 ups_sdk-1.2.8/UPS_SDK/models/TransactionReference.py
--rw-rw-rw-   0        0        0      118 2022-08-26 14:38:07.000000 ups_sdk-1.2.8/UPS_SDK/models/UnitOfMeasurement.py
--rw-rw-rw-   0        0        0      832 2022-08-26 14:38:57.000000 ups_sdk-1.2.8/UPS_SDK/models/__init__.py
--rw-rw-rw-   0        0        0     1355 2023-02-18 08:43:39.000000 ups_sdk-1.2.8/UPS_SDK/test.py
--rw-rw-rw-   0        0        0       42 2023-02-18 08:44:00.138431 ups_sdk-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      587 2023-01-19 08:02:23.000000 ups_sdk-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:44:00.138431 ups_sdk-1.2.8/ups_sdk.egg-info/
--rw-rw-rw-   0        0        0      288 2023-02-18 08:43:59.000000 ups_sdk-1.2.8/ups_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-02-18 08:43:59.000000 ups_sdk-1.2.8/ups_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 08:43:59.000000 ups_sdk-1.2.8/ups_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-18 08:43:59.000000 ups_sdk-1.2.8/ups_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 14:53:40.435288 ups_sdk-1.2.9/
+-rw-rw-rw-   0        0        0     1089 2022-11-25 12:45:05.000000 ups_sdk-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-06-22 14:53:40.435288 ups_sdk-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2023-01-03 08:26:58.000000 ups_sdk-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 14:53:40.162744 ups_sdk-1.2.9/UPS_SDK/
+-rw-rw-rw-   0        0        0       22 2023-06-22 14:53:32.000000 ups_sdk-1.2.9/UPS_SDK/__init__.py
+-rw-rw-rw-   0        0        0     1601 2023-01-19 08:01:48.000000 ups_sdk-1.2.9/UPS_SDK/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:53:40.406673 ups_sdk-1.2.9/UPS_SDK/models/
+-rw-rw-rw-   0        0        0      489 2022-11-19 11:48:55.000000 ups_sdk-1.2.9/UPS_SDK/models/AccessRequest.py
+-rw-rw-rw-   0        0        0     1015 2022-11-25 14:40:12.000000 ups_sdk-1.2.9/UPS_SDK/models/ActivityItem.py
+-rw-rw-rw-   0        0        0      227 2022-11-25 14:40:18.000000 ups_sdk-1.2.9/UPS_SDK/models/ActivityLocation.py
+-rw-rw-rw-   0        0        0      318 2023-02-02 10:37:30.000000 ups_sdk-1.2.9/UPS_SDK/models/Address.py
+-rw-rw-rw-   0        0        0      130 2022-07-22 09:00:38.000000 ups_sdk-1.2.9/UPS_SDK/models/Message.py
+-rw-rw-rw-   0        0        0     1138 2022-11-25 14:40:35.000000 ups_sdk-1.2.9/UPS_SDK/models/Package.py
+-rw-rw-rw-   0        0        0      208 2022-11-25 14:40:41.000000 ups_sdk-1.2.9/UPS_SDK/models/PackageWeight.py
+-rw-rw-rw-   0        0        0      171 2023-02-18 08:43:30.000000 ups_sdk-1.2.9/UPS_SDK/models/ReferenceNumber.py
+-rw-rw-rw-   0        0        0      136 2022-07-22 08:59:52.000000 ups_sdk-1.2.9/UPS_SDK/models/ReferenceNumberItem.py
+-rw-rw-rw-   0        0        0      265 2022-11-25 14:40:50.000000 ups_sdk-1.2.9/UPS_SDK/models/Response.py
+-rw-rw-rw-   0        0        0      130 2022-07-22 08:59:48.000000 ups_sdk-1.2.9/UPS_SDK/models/Service.py
+-rw-rw-rw-   0        0        0      144 2022-11-25 14:41:25.000000 ups_sdk-1.2.9/UPS_SDK/models/ShipTo.py
+-rw-rw-rw-   0        0        0     1472 2022-11-25 14:41:10.000000 ups_sdk-1.2.9/UPS_SDK/models/Shipment.py
+-rw-rw-rw-   0        0        0      211 2022-11-25 14:41:16.000000 ups_sdk-1.2.9/UPS_SDK/models/ShipmentWeight.py
+-rw-rw-rw-   0        0        0      210 2023-01-19 08:05:19.000000 ups_sdk-1.2.9/UPS_SDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      220 2022-11-25 14:41:32.000000 ups_sdk-1.2.9/UPS_SDK/models/Status.py
+-rw-rw-rw-   0        0        0      111 2022-07-22 09:00:10.000000 ups_sdk-1.2.9/UPS_SDK/models/StatusCode.py
+-rw-rw-rw-   0        0        0      133 2022-07-22 09:00:06.000000 ups_sdk-1.2.9/UPS_SDK/models/StatusType.py
+-rw-rw-rw-   0        0        0      525 2022-08-01 17:17:58.000000 ups_sdk-1.2.9/UPS_SDK/models/TrackError.py
+-rw-rw-rw-   0        0        0     1300 2022-11-23 15:20:45.000000 ups_sdk-1.2.9/UPS_SDK/models/TrackRequest.py
+-rw-rw-rw-   0        0        0     1279 2023-06-22 14:53:25.000000 ups_sdk-1.2.9/UPS_SDK/models/TrackResponse.py
+-rw-rw-rw-   0        0        0      149 2022-11-19 11:52:25.000000 ups_sdk-1.2.9/UPS_SDK/models/TrackType.py
+-rw-rw-rw-   0        0        0      156 2022-08-01 17:20:10.000000 ups_sdk-1.2.9/UPS_SDK/models/TransactionReference.py
+-rw-rw-rw-   0        0        0      118 2022-08-26 14:38:07.000000 ups_sdk-1.2.9/UPS_SDK/models/UnitOfMeasurement.py
+-rw-rw-rw-   0        0        0      832 2022-08-26 14:38:57.000000 ups_sdk-1.2.9/UPS_SDK/models/__init__.py
+-rw-rw-rw-   0        0        0     1355 2023-02-18 08:43:39.000000 ups_sdk-1.2.9/UPS_SDK/test.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 14:53:40.436285 ups_sdk-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      587 2023-01-19 08:02:23.000000 ups_sdk-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:53:40.428314 ups_sdk-1.2.9/ups_sdk.egg-info/
+-rw-rw-rw-   0        0        0      288 2023-06-22 14:53:39.000000 ups_sdk-1.2.9/ups_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-06-22 14:53:40.000000 ups_sdk-1.2.9/ups_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:53:39.000000 ups_sdk-1.2.9/ups_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 14:53:39.000000 ups_sdk-1.2.9/ups_sdk.egg-info/top_level.txt
```

### Comparing `ups_sdk-1.2.8/LICENSE` & `ups_sdk-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/README.md` & `ups_sdk-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/main.py` & `ups_sdk-1.2.9/UPS_SDK/main.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/ActivityItem.py` & `ups_sdk-1.2.9/UPS_SDK/models/ActivityItem.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/Package.py` & `ups_sdk-1.2.9/UPS_SDK/models/Package.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/Shipment.py` & `ups_sdk-1.2.9/UPS_SDK/models/Shipment.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/TrackError.py` & `ups_sdk-1.2.9/UPS_SDK/models/TrackError.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/TrackRequest.py` & `ups_sdk-1.2.9/UPS_SDK/models/TrackRequest.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/TrackResponse.py` & `ups_sdk-1.2.9/UPS_SDK/models/TrackResponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,11 @@
                 shipment["Package"]["Activity"] = [shipment["Package"]["Activity"]]
             
             redirect_or_alternate_tracking_number = package.get("Redirect") or package.get("AlternateTrackingNumber")
             if redirect_or_alternate_tracking_number is None:
                 
                 if isinstance(shipment["ReferenceNumber"], dict):
                     shipment["ReferenceNumber"] = [shipment["ReferenceNumber"]]
-            
+                    
+            if isinstance(shipment["ReferenceNumber"], dict):
+                shipment["ReferenceNumber"] = [shipment["ReferenceNumber"]]
         super().__init__(**data)
```

### Comparing `ups_sdk-1.2.8/UPS_SDK/models/__init__.py` & `ups_sdk-1.2.9/UPS_SDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/UPS_SDK/test.py` & `ups_sdk-1.2.9/UPS_SDK/test.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/setup.py` & `ups_sdk-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ups_sdk-1.2.8/ups_sdk.egg-info/SOURCES.txt` & `ups_sdk-1.2.9/ups_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

