# Comparing `tmp/mailbagit-0.5.1.tar.gz` & `tmp/mailbagit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailbagit-0.5.1.tar", last modified: Thu Jun 15 20:36:05 2023, max compression
+gzip compressed data, was "mailbagit-0.6.0.tar", last modified: Thu Jun 22 18:07:49 2023, max compression
```

## Comparing `mailbagit-0.5.1.tar` & `mailbagit-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.537549 mailbagit-0.5.1/
--rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     5882 2023-06-15 20:36:05.536548 mailbagit-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.463545 mailbagit-0.5.1/mailbagit/
--rw-rw-rw-   0        0        0    12594 2023-06-15 20:22:51.000000 mailbagit-0.5.1/mailbagit/__init__.py
--rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/controller.py
--rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.5.1/mailbagit/derivative.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.500548 mailbagit-0.5.1/mailbagit/derivatives/
--rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/eml.py
--rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/example.py
--rw-rw-rw-   0        0        0     2773 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/html.py
--rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/derivatives/mbox.py
--rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/pdf.py
--rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/pdf_chrome.py
--rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/txt.py
--rw-rw-rw-   0        0        0    14159 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/warc.py
--rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/email_account.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.517547 mailbagit-0.5.1/mailbagit/formats/
--rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/eml.py
--rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/example.py
--rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.5.1/mailbagit/formats/mbox.py
--rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/msg.py
--rw-rw-rw-   0        0        0    19442 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/pst.py
--rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/globals.py
--rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/guided.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.524546 mailbagit-0.5.1/mailbagit/helper/
--rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.5.1/mailbagit/helper/__init__.py
--rw-rw-rw-   0        0        0     3781 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/common.py
--rw-rw-rw-   0        0        0     4808 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/controller.py
--rw-rw-rw-   0        0        0     8257 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/derivative.py
--rw-rw-rw-   0        0        0    16736 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/helper/format.py
--rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/loggerx.py
--rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/models.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.482553 mailbagit-0.5.1/mailbagit.egg-info/
--rw-rw-rw-   0        0        0     5882 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      455 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 20:36:05.537549 mailbagit-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1640 2023-06-15 20:22:51.000000 mailbagit-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.535546 mailbagit-0.5.1/tests/
--rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.5.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.5.1/tests/test_controller.py
--rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.5.1/tests/test_formats.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.844214 mailbagit-0.6.0/
+-rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5882 2023-06-22 18:07:49.843213 mailbagit-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.760215 mailbagit-0.6.0/mailbagit/
+-rw-rw-rw-   0        0        0    12594 2023-06-22 14:02:26.000000 mailbagit-0.6.0/mailbagit/__init__.py
+-rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/controller.py
+-rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.6.0/mailbagit/derivative.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.799214 mailbagit-0.6.0/mailbagit/derivatives/
+-rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/eml.py
+-rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/example.py
+-rw-rw-rw-   0        0        0     2773 2023-06-22 15:09:33.000000 mailbagit-0.6.0/mailbagit/derivatives/html.py
+-rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/derivatives/mbox.py
+-rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/pdf.py
+-rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/pdf_chrome.py
+-rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/txt.py
+-rw-rw-rw-   0        0        0    14611 2023-06-22 14:01:35.000000 mailbagit-0.6.0/mailbagit/derivatives/warc.py
+-rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/email_account.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.813214 mailbagit-0.6.0/mailbagit/formats/
+-rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/eml.py
+-rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/example.py
+-rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.6.0/mailbagit/formats/mbox.py
+-rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/msg.py
+-rw-rw-rw-   0        0        0    20552 2023-06-22 17:36:18.000000 mailbagit-0.6.0/mailbagit/formats/pst.py
+-rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/globals.py
+-rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/guided.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.820217 mailbagit-0.6.0/mailbagit/helper/
+-rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.6.0/mailbagit/helper/__init__.py
+-rw-rw-rw-   0        0        0     3781 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/helper/common.py
+-rw-rw-rw-   0        0        0     4808 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/helper/controller.py
+-rw-rw-rw-   0        0        0     8257 2023-06-22 15:10:17.000000 mailbagit-0.6.0/mailbagit/helper/derivative.py
+-rw-rw-rw-   0        0        0    16733 2023-06-22 17:10:09.000000 mailbagit-0.6.0/mailbagit/helper/format.py
+-rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/loggerx.py
+-rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/models.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.780213 mailbagit-0.6.0/mailbagit.egg-info/
+-rw-rw-rw-   0        0        0     5882 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      455 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 18:07:49.844214 mailbagit-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2023-06-22 14:02:39.000000 mailbagit-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.841213 mailbagit-0.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.6.0/tests/test_controller.py
+-rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.6.0/tests/test_formats.py
```

### Comparing `mailbagit-0.5.1/LICENSE` & `mailbagit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/PKG-INFO` & `mailbagit-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.5.1
+Version: 0.6.0
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.5.1/README.md` & `mailbagit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/__init__.py` & `mailbagit-0.6.0/mailbagit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version of the mailbagit package
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 import os
 from pathlib import Path
 from bagit import _make_parser, Bag, BagHeaderAction, DEFAULT_CHECKSUMS
 import importlib
 from mailbagit.loggerx import setup_logging, get_logger
 from argparse import ArgumentParser, FileType
```

### Comparing `mailbagit-0.5.1/mailbagit/controller.py` & `mailbagit-0.6.0/mailbagit/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivative.py` & `mailbagit-0.6.0/mailbagit/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/eml.py` & `mailbagit-0.6.0/mailbagit/derivatives/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/example.py` & `mailbagit-0.6.0/mailbagit/derivatives/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/html.py` & `mailbagit-0.6.0/mailbagit/derivatives/html.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/mbox.py` & `mailbagit-0.6.0/mailbagit/derivatives/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/pdf.py` & `mailbagit-0.6.0/mailbagit/derivatives/pdf.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/pdf_chrome.py` & `mailbagit-0.6.0/mailbagit/derivatives/pdf_chrome.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/txt.py` & `mailbagit-0.6.0/mailbagit/derivatives/txt.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/derivatives/warc.py` & `mailbagit-0.6.0/mailbagit/derivatives/warc.py`

 * *Files 11% similar despite different names*

```diff
@@ -142,16 +142,23 @@
             else:
                 out_dir = os.path.join(self.format_subdirectory, message.Derivatives_Path)
                 filename = os.path.join(out_dir, str(message.Mailbag_Message_ID) + ".warc.gz")
                 errors = common.check_path_length(out_dir, errors)
                 errors = common.check_path_length(filename, errors)
                 log.debug("Writing WARC to " + str(filename))
 
-                # This is used for the WARC-Target-URI in the WARC derivatives
-                warc_uri = f"http://mailbag/{str(message.Mailbag_Message_ID)}"
+                # Try to use Message_ID for WARC-Target-URI if present, otherwise
+                if message.Message_ID is None or len(message.Message_ID) < 1:
+                    warc_uri = f"http://mailbag/{str(message.Mailbag_Message_ID)}"
+                else:
+                    # strip leading and trailing brackets and add mailto: URI scheme
+                    if message.Message_ID.startswith("<") and message.Message_ID.endswith(">"):
+                        warc_uri = "mailto:" + message.Message_ID[1:-1]
+                    else:
+                        warc_uri = "mailto:" + message.Message_ID
 
                 # Write Headers to UTF-8 JSON
                 try:
                     headers = {}
                     for key in message.Headers:
                         headers[key], errors = format.parse_header(message.Headers[key], errors)
                     headers_json = json.dumps(headers, indent=4, sort_keys=True).encode("utf-8")
```

### Comparing `mailbagit-0.5.1/mailbagit/email_account.py` & `mailbagit-0.6.0/mailbagit/email_account.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/formats/eml.py` & `mailbagit-0.6.0/mailbagit/formats/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/formats/example.py` & `mailbagit-0.6.0/mailbagit/formats/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/formats/mbox.py` & `mailbagit-0.6.0/mailbagit/formats/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/formats/msg.py` & `mailbagit-0.6.0/mailbagit/formats/msg.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/formats/pst.py` & `mailbagit-0.6.0/mailbagit/formats/pst.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import email
 from pathlib import Path
 import chardet
 from extract_msg.constants import CODE_PAGES
+from RTFDE.deencapsulate import DeEncapsulator
 from mailbagit.loggerx import get_logger
 from mailbagit.email_account import EmailAccount
 from mailbagit.models import Email, Attachment
 import mailbagit.helper.format as format
 import mailbagit.helper.common as common
 import uuid
 
@@ -110,14 +111,26 @@
                                             value = entry.get_data_as_integer()
                                             # Use the extract_msg code page in constants.py
                                             encodings[2] = {"name": CODE_PAGES[value], "label": "PidTagMessageCodepage"}
                             # messageObj.html_body sometimes fails. This seems to often be the case for email in "Deleted Items"
                             try:
                                 if messageObj.html_body:
                                     html_body, html_encoding, errors = format.safely_decode("HTML", messageObj.html_body, encodings, errors)
+                                elif messageObj.rtf_body:
+                                    # Try to pull the HTML out of the RTF body
+                                    # HT to extract_msg for this https://github.com/TeamMsgExtractor/msg-extractor/blob/3cffc2e0d82a0301cfaca2b05c5ef35bfc96a8cb/extract_msg/message_base.py#L958
+                                    rtf_body = messageObj.rtf_body
+                                    # I dunno why this needs a len of 125 ¯\_(ツ)_/¯
+                                    while rtf_body and rtf_body[-1] != 125:
+                                        rtf_body = rtf_body[:-1]
+                                    # decode it before using DeEncapsulator
+                                    rtf_string, html_encoding, errors = format.safely_decode("HTML", rtf_body, encodings, errors)
+                                    deencapsulated_body = DeEncapsulator(rtf_string)
+                                    deencapsulated_body.deencapsulate()
+                                    html_body = deencapsulated_body.html
                             except:
                                 pass
                             if messageObj.plain_text_body:
                                 encodings[len(encodings.keys()) + 1] = {
                                     "name": "utf-8",
                                     "label": "manual",
                                 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mailbagit-0.5.1/mailbagit/guided.py` & `mailbagit-0.6.0/mailbagit/guided.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/helper/common.py` & `mailbagit-0.6.0/mailbagit/helper/common.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/helper/controller.py` & `mailbagit-0.6.0/mailbagit/helper/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/helper/derivative.py` & `mailbagit-0.6.0/mailbagit/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/helper/format.py` & `mailbagit-0.6.0/mailbagit/helper/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if encodings[priority]["name"]:
             try:
                 valid_encoding = codecs.lookup(encodings[priority]["name"]).name.lower()
                 valid.append(valid_encoding)
                 text = binary_text.decode(valid_encoding)
                 used = encodings[priority]["name"]
                 success = True
-                continue
+                break
             except Exception as e:
                 errorObj = e
                 failed.append(encodings[priority]["name"])
 
     if success == False:
         try:
             detected = chardet.detect(binary_text)["encoding"]
```

### Comparing `mailbagit-0.5.1/mailbagit/loggerx.py` & `mailbagit-0.6.0/mailbagit/loggerx.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit/models.py` & `mailbagit-0.6.0/mailbagit/models.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/mailbagit.egg-info/PKG-INFO` & `mailbagit-0.6.0/mailbagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.5.1
+Version: 0.6.0
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.5.1/mailbagit.egg-info/SOURCES.txt` & `mailbagit-0.6.0/mailbagit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/setup.py` & `mailbagit-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mailbagit",
-    version="0.5.1",
+    version="0.6.0",
     author="Gregory Wiedeman",
     author_email="gwiedeman@albany.edu",
     description="A tool for preserving email with multiple masters.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UAlbanyArchives/mailbag",
     packages=setuptools.find_namespace_packages(exclude=("tests")),
```

### Comparing `mailbagit-0.5.1/tests/test_controller.py` & `mailbagit-0.6.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.1/tests/test_formats.py` & `mailbagit-0.6.0/tests/test_formats.py`

 * *Files identical despite different names*

