# Comparing `tmp/odoo14_addons_oca_queue-14.0.20230316.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_queue-14.0.20230621.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1383 bytes, number of entries: 4
--rw-r--r--  2.0 unx      807 b- defN 23-Mar-17 07:16 odoo14_addons_oca_queue-14.0.20230316.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-17 07:16 odoo14_addons_oca_queue-14.0.20230316.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-17 07:16 odoo14_addons_oca_queue-14.0.20230316.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      400 b- defN 23-Mar-17 07:16 odoo14_addons_oca_queue-14.0.20230316.0.dist-info/RECORD
-4 files, 1300 bytes uncompressed, 593 bytes compressed:  54.4%
+Zip file size: 1395 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      857 b- defN 23-Jun-22 04:50 odoo14_addons_oca_queue-14.0.20230621.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 04:50 odoo14_addons_oca_queue-14.0.20230621.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-22 04:50 odoo14_addons_oca_queue-14.0.20230621.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      400 b- defN 23-Jun-22 04:50 odoo14_addons_oca_queue-14.0.20230621.0.dist-info/RECORD
+4 files, 1350 bytes uncompressed, 605 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_queue-14.0.20230316.0.dist-info/METADATA
+Filename: odoo14_addons_oca_queue-14.0.20230621.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_queue-14.0.20230316.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_queue-14.0.20230621.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_queue-14.0.20230316.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_queue-14.0.20230621.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_queue-14.0.20230316.0.dist-info/RECORD
+Filename: odoo14_addons_oca_queue-14.0.20230621.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_queue-14.0.20230316.0.dist-info/METADATA` & `odoo14_addons_oca_queue-14.0.20230621.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-queue
-Version: 14.0.20230316.0
+Version: 14.0.20230621.0
 Summary: Meta package for oca-queue Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Dist: odoo14-addon-base-export-async
 Requires-Dist: odoo14-addon-base-import-async
+Requires-Dist: odoo14-addon-export-async-schedule
 Requires-Dist: odoo14-addon-queue-job
 Requires-Dist: odoo14-addon-queue-job-batch
 Requires-Dist: odoo14-addon-queue-job-context
 Requires-Dist: odoo14-addon-queue-job-cron
 Requires-Dist: odoo14-addon-queue-job-cron-jobrunner
 Requires-Dist: odoo14-addon-queue-job-subscribe
 Requires-Dist: odoo14-addon-test-base-import-async
```

