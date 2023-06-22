# Comparing `tmp/orthanc_tools-0.8.8.tar.gz` & `tmp/orthanc_tools-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_tools-0.8.8.tar", last modified: Mon May 22 08:38:07 2023, max compression
+gzip compressed data, was "orthanc_tools-0.8.9.tar", last modified: Thu Jun 22 11:07:01 2023, max compression
```

## Comparing `orthanc_tools-0.8.8.tar` & `orthanc_tools-0.8.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.545486 orthanc_tools-0.8.8/orthanc_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/orthanc_tools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/old_files_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/time_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_cloner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_folder_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_test_db_populator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/pacs_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.545486 orthanc_tools-0.8.8/orthanc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/tests/test_3_orthancs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/tests/test_old_files_deleter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.366539 orthanc_tools-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 11:07:01.366539 orthanc_tools-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.362539 orthanc_tools-0.8.9/orthanc_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.362539 orthanc_tools-0.8.9/orthanc_tools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/helpers/old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/helpers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/helpers/time_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.366539 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_message_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_report_series_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_worklist_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_cloner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_folder_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/orthanc_test_db_populator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/orthanc_tools/pacs_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.362539 orthanc_tools-0.8.9/orthanc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 11:07:01.000000 orthanc_tools-0.8.9/orthanc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-22 11:07:01.000000 orthanc_tools-0.8.9/orthanc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:07:01.000000 orthanc_tools-0.8.9/orthanc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 11:07:01.000000 orthanc_tools-0.8.9/orthanc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 11:07:01.000000 orthanc_tools-0.8.9/orthanc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 11:07:01.366539 orthanc_tools-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:07:01.366539 orthanc_tools-0.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/tests/test_3_orthancs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-22 11:04:10.000000 orthanc_tools-0.8.9/tests/test_old_files_deleter.py
```

### Comparing `orthanc_tools-0.8.8/LICENSE.txt` & `orthanc_tools-0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/PKG-INFO` & `orthanc_tools-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc_tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.8/README.md` & `orthanc_tools-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/__init__.py` & `orthanc_tools-0.8.9/orthanc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/helpers/old_files_deleter.py` & `orthanc_tools-0.8.9/orthanc_tools/helpers/old_files_deleter.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/helpers/scheduler.py` & `orthanc_tools-0.8.9/orthanc_tools/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/helpers/time_out.py` & `orthanc_tools-0.8.9/orthanc_tools/helpers/time_out.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/helpers/timer.py` & `orthanc_tools-0.8.9/orthanc_tools/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/__init__.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_client.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_error.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_error.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_parser.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_message_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_validator.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_message_validator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_parser.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_report_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_report_series_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_server.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_server.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py` & `orthanc_tools-0.8.9/orthanc_tools/hl7Lib/hl7_worklist_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_cloner.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_cloner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_comparator.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_comparator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_folder_importer.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_folder_importer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_forwarder.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_forwarder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_monitor.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_monitor.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools/orthanc_test_db_populator.py` & `orthanc_tools-0.8.9/orthanc_tools/orthanc_test_db_populator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     'Lyman', 'MacDonald', 'Mackay', 'Mackenzie', 'MacLeod', 'Manning', 'Marshall', 'Martin', 'Mathis', 'May', 'McDonald', 'McLean', 'McGrath', 'Metcalfe', 'Miller', 'Mills', 'Mitchell',
     'Morgan', 'Morrison', 'Murray', 'Nash', 'Newman', 'Nolan', 'North', 'Ogden', 'Oliver', 'Paige', 'Parr', 'Parsons', 'Paterson', 'Payne', 'Peake', 'Peters', 'Piper', 'Poole', 'Powell',
     'Pullman', 'Quinn', 'Rampling', 'Randall', 'Rees', 'Reid', 'Roberts', 'Robertson', 'Ross', 'Russell', 'Rutherford', 'Sanderson', 'Scott', 'Sharp', 'Short', 'Simpson', 'Skinner',
     'Slater', 'Smith', 'Springer', 'Stewart', 'Sutherland', 'Taylor', 'Terry', 'Thomson', 'Tucker', 'Turner', 'Underwood', 'Vance', 'Vaughan', 'Walker', 'Wallace', 'Walsh', 'Watson',
     'Welch', 'White', 'Wilkins', 'Wilson', 'Wright', 'Young']
 
 
+labels = ['Label1', "Label2", "Label3", "Label4", "Label5", "Label6", "Label7", "Label8", "Label9"]
+
 class OrthancTestDbPopulator:
     """
     Populates an Orthanc with a test DB
     """
 
     def __init__(self,
                  api_client: OrthancApiClient,
@@ -119,14 +121,15 @@
 
             logger.info(f"-created study {tags['StudyDescription']}")
 
             if self._series_count is not None:
                 series_count = self._series_count
             else:
                 series_count = random.randint(1, 6)
+
             for series_counter in range(0, series_count):
                 tags = self.generate_series_tags(tags, series_counter, study_counter)
 
                 if tags["Modality"] in ["MR", "CT"]:
                     if self._instances_count is not None:
                         instances_count = self._instances_count
                     else:
@@ -136,16 +139,20 @@
 
                 logger.info(f"--created series {tags['Modality']} with {instances_count} instances")
 
                 for instance_counter in range(0, instances_count):
                     tags = self.generate_instance_tags(tags, instance_counter, series_counter, study_counter)
 
                     dicom = helpers.generate_test_dicom_file(width=2, height=2, tags=tags)
-                    self._api_client.upload(buffer=dicom)
+                    instance_id = self._api_client.upload(buffer=dicom)[0]
 
+            study_id = self._api_client.instances.get_parent_study_id(instance_id)
+            for labels_count in range(0, random.randint(0, 3)):
+                label = labels[random.randint(0, len(labels) - 1)]
+                self._api_client.studies.add_label(study_id, label)
 
 # examples:
 # python orthanc_tools/orthanc_test_db_populator.py --url=http://192.168.0.10:8042 --user=user --password=pwd --studies=50 --seed=42
 
 if __name__ == '__main__':
     level = logging.INFO
```

### Comparing `orthanc_tools-0.8.8/orthanc_tools/pacs_migrator.py` & `orthanc_tools-0.8.9/orthanc_tools/pacs_migrator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/orthanc_tools.egg-info/PKG-INFO` & `orthanc_tools-0.8.9/orthanc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.8/orthanc_tools.egg-info/SOURCES.txt` & `orthanc_tools-0.8.9/orthanc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/release-notes.md` & `orthanc_tools-0.8.9/release-notes.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v 0.8.9
+=======
+- `OrthancTestDbPopulator`: now labelling studies
+
 v 0.8.8
 =======
 
 - `OrthancMonitor`: fixed monitor
 
 v 0.8.7
 =======
```

### Comparing `orthanc_tools-0.8.8/setup.py` & `orthanc_tools-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.8.8',  # Required
+    version='0.8.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc Tools',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -126,15 +126,15 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
         'requests',
-        'orthanc-api-client>=0.12.2',
+        'orthanc-api-client>=0.13.1',
         'pydicom>=2.3.1',
         'hl7==0.4.2',
         'six'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `orthanc_tools-0.8.8/tests/test_3_orthancs.py` & `orthanc_tools-0.8.9/tests/test_3_orthancs.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.8/tests/test_old_files_deleter.py` & `orthanc_tools-0.8.9/tests/test_old_files_deleter.py`

 * *Files identical despite different names*

