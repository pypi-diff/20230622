# Comparing `tmp/escp-0.0.5.tar.gz` & `tmp/escp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escp-0.0.5.tar", last modified: Sat Mar 25 10:36:12 2023, max compression
+gzip compressed data, was "escp-0.0.6.tar", last modified: Thu Jun 22 17:25:09 2023, max compression
```

## Comparing `escp-0.0.5.tar` & `escp-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.595948 escp-0.0.5/
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.581052 escp-0.0.5/.github/
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.587036 escp-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 youri      (501) staff       (20)      806 2023-03-05 12:21:43.000000 escp-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 youri      (501) staff       (20)       95 2023-03-05 09:22:23.000000 escp-0.0.5/.gitignore
--rw-r--r--   0 youri      (501) staff       (20)    35149 2023-03-05 09:22:23.000000 escp-0.0.5/LICENSE
--rw-r--r--   0 youri      (501) staff       (20)     4373 2023-03-25 10:36:12.596064 escp-0.0.5/PKG-INFO
--rw-r--r--   0 youri      (501) staff       (20)     3250 2023-03-06 18:10:29.000000 escp-0.0.5/README.md
--rw-r--r--   0 youri      (501) staff       (20)   954262 2023-03-05 12:21:43.000000 escp-0.0.5/escp.jpg
--rw-r--r--   0 youri      (501) staff       (20)       85 2023-03-05 09:22:23.000000 escp-0.0.5/pyproject.toml
--rw-r--r--   0 youri      (501) staff       (20)        5 2023-03-10 18:41:31.000000 escp-0.0.5/requirements.txt
--rw-r--r--   0 youri      (501) staff       (20)     1324 2023-03-25 10:36:12.596379 escp-0.0.5/setup.cfg
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.581225 escp-0.0.5/src/
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.588493 escp-0.0.5/src/escp/
--rw-r--r--   0 youri      (501) staff       (20)       67 2023-03-07 17:19:32.000000 escp-0.0.5/src/escp/__init__.py
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.591365 escp-0.0.5/src/escp/commands/
--rw-r--r--   0 youri      (501) staff       (20)      314 2023-03-15 16:35:51.000000 escp-0.0.5/src/escp/commands/__init__.py
--rw-r--r--   0 youri      (501) staff       (20)    14850 2023-03-25 10:33:19.000000 escp-0.0.5/src/escp/commands/commands.py
--rw-r--r--   0 youri      (501) staff       (20)     1795 2023-03-11 13:50:36.000000 escp-0.0.5/src/escp/commands/commands_24_48_pin.py
--rw-r--r--   0 youri      (501) staff       (20)     1779 2023-03-11 13:50:36.000000 escp-0.0.5/src/escp/commands/commands_9_pin.py
--rw-r--r--   0 youri      (501) staff       (20)      104 2023-03-15 16:35:51.000000 escp-0.0.5/src/escp/commands/exceptions.py
--rw-r--r--   0 youri      (501) staff       (20)      423 2023-03-05 09:22:23.000000 escp-0.0.5/src/escp/commands/lookup.py
--rw-r--r--   0 youri      (501) staff       (20)     1172 2023-03-25 10:33:19.000000 escp-0.0.5/src/escp/commands/magic_encoding.py
--rw-r--r--   0 youri      (501) staff       (20)     2354 2023-03-11 12:35:59.000000 escp-0.0.5/src/escp/commands/parameters.py
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.592954 escp-0.0.5/src/escp/demo/
--rw-r--r--   0 youri      (501) staff       (20)       23 2023-03-07 17:19:32.000000 escp-0.0.5/src/escp/demo/__init__.py
--rw-r--r--   0 youri      (501) staff       (20)      865 2023-03-15 14:45:56.000000 escp-0.0.5/src/escp/demo/char_tables.py
--rw-r--r--   0 youri      (501) staff       (20)      253 2023-03-10 19:11:01.000000 escp-0.0.5/src/escp/demo/common.py
--rw-r--r--   0 youri      (501) staff       (20)     2095 2023-03-25 10:33:19.000000 escp-0.0.5/src/escp/demo/demo.py
--rw-r--r--   0 youri      (501) staff       (20)     1251 2023-03-15 15:19:03.000000 escp-0.0.5/src/escp/demo/i18n_char_set.py
--rw-r--r--   0 youri      (501) staff       (20)     1237 2023-03-10 19:11:01.000000 escp-0.0.5/src/escp/demo/poem.py
--rw-r--r--   0 youri      (501) staff       (20)     5811 2023-03-10 19:11:01.000000 escp-0.0.5/src/escp/demo/test_page.py
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.594208 escp-0.0.5/src/escp/printer/
--rw-r--r--   0 youri      (501) staff       (20)      187 2023-03-05 09:22:23.000000 escp-0.0.5/src/escp/printer/__init__.py
--rw-r--r--   0 youri      (501) staff       (20)      381 2023-03-05 09:22:23.000000 escp-0.0.5/src/escp/printer/debug_printer.py
--rw-r--r--   0 youri      (501) staff       (20)       43 2023-03-05 09:22:23.000000 escp-0.0.5/src/escp/printer/exceptions.py
--rw-r--r--   0 youri      (501) staff       (20)      396 2023-03-05 09:22:23.000000 escp-0.0.5/src/escp/printer/output_printer.py
--rw-r--r--   0 youri      (501) staff       (20)      128 2023-03-07 06:23:57.000000 escp-0.0.5/src/escp/printer/printer.py
--rw-r--r--   0 youri      (501) staff       (20)     2376 2023-03-25 10:33:19.000000 escp-0.0.5/src/escp/printer/usb_printer.py
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.589556 escp-0.0.5/src/escp.egg-info/
--rw-r--r--   0 youri      (501) staff       (20)     4373 2023-03-25 10:36:12.000000 escp-0.0.5/src/escp.egg-info/PKG-INFO
--rw-r--r--   0 youri      (501) staff       (20)     1143 2023-03-25 10:36:12.000000 escp-0.0.5/src/escp.egg-info/SOURCES.txt
--rw-r--r--   0 youri      (501) staff       (20)        1 2023-03-25 10:36:12.000000 escp-0.0.5/src/escp.egg-info/dependency_links.txt
--rw-r--r--   0 youri      (501) staff       (20)        1 2023-03-05 09:15:42.000000 escp-0.0.5/src/escp.egg-info/not-zip-safe
--rw-r--r--   0 youri      (501) staff       (20)       24 2023-03-25 10:36:12.000000 escp-0.0.5/src/escp.egg-info/requires.txt
--rw-r--r--   0 youri      (501) staff       (20)        5 2023-03-25 10:36:12.000000 escp-0.0.5/src/escp.egg-info/top_level.txt
-drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-03-25 10:36:12.595787 escp-0.0.5/test/
--rw-r--r--   0 youri      (501) staff       (20)      283 2023-03-12 08:21:10.000000 escp-0.0.5/test/__init__.py
--rw-r--r--   0 youri      (501) staff       (20)     3940 2023-03-25 10:33:19.000000 escp-0.0.5/test/test_commands.py
--rw-r--r--   0 youri      (501) staff       (20)     1101 2023-03-11 13:53:13.000000 escp-0.0.5/test/test_commands_24_48_pins.py
--rw-r--r--   0 youri      (501) staff       (20)     1307 2023-03-11 13:52:58.000000 escp-0.0.5/test/test_commands_9_pin.py
--rw-r--r--   0 youri      (501) staff       (20)     1452 2023-03-25 10:33:19.000000 escp-0.0.5/test/test_commands_char_set.py
--rw-r--r--   0 youri      (501) staff       (20)     1452 2023-03-15 17:36:03.000000 escp-0.0.5/test/test_i18n_char_set.py
--rw-r--r--   0 youri      (501) staff       (20)     1072 2023-03-25 10:33:19.000000 escp-0.0.5/test/test_magic_text.py
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.825233 escp-0.0.6/
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.813135 escp-0.0.6/.github/
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.816944 escp-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 youri      (501) staff       (20)      806 2023-03-05 12:21:43.000000 escp-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 youri      (501) staff       (20)       95 2023-03-05 09:22:23.000000 escp-0.0.6/.gitignore
+-rw-r--r--   0 youri      (501) staff       (20)    35149 2023-03-05 09:22:23.000000 escp-0.0.6/LICENSE
+-rw-r--r--   0 youri      (501) staff       (20)     4373 2023-06-22 17:25:09.825343 escp-0.0.6/PKG-INFO
+-rw-r--r--   0 youri      (501) staff       (20)     3250 2023-03-06 18:10:29.000000 escp-0.0.6/README.md
+-rw-r--r--   0 youri      (501) staff       (20)   954262 2023-03-05 12:21:43.000000 escp-0.0.6/escp.jpg
+-rw-r--r--   0 youri      (501) staff       (20)       85 2023-03-05 09:22:23.000000 escp-0.0.6/pyproject.toml
+-rw-r--r--   0 youri      (501) staff       (20)        5 2023-03-10 18:41:31.000000 escp-0.0.6/requirements.txt
+-rw-r--r--   0 youri      (501) staff       (20)     1324 2023-06-22 17:25:09.825683 escp-0.0.6/setup.cfg
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.813329 escp-0.0.6/src/
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.817247 escp-0.0.6/src/escp/
+-rw-r--r--   0 youri      (501) staff       (20)       67 2023-03-07 17:19:32.000000 escp-0.0.6/src/escp/__init__.py
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.820105 escp-0.0.6/src/escp/commands/
+-rw-r--r--   0 youri      (501) staff       (20)      314 2023-03-15 16:35:51.000000 escp-0.0.6/src/escp/commands/__init__.py
+-rw-r--r--   0 youri      (501) staff       (20)    16441 2023-06-22 17:19:52.000000 escp-0.0.6/src/escp/commands/commands.py
+-rw-r--r--   0 youri      (501) staff       (20)     1795 2023-03-11 13:50:36.000000 escp-0.0.6/src/escp/commands/commands_24_48_pin.py
+-rw-r--r--   0 youri      (501) staff       (20)     1744 2023-03-27 15:16:21.000000 escp-0.0.6/src/escp/commands/commands_9_pin.py
+-rw-r--r--   0 youri      (501) staff       (20)      104 2023-03-15 16:35:51.000000 escp-0.0.6/src/escp/commands/exceptions.py
+-rw-r--r--   0 youri      (501) staff       (20)      423 2023-03-05 09:22:23.000000 escp-0.0.6/src/escp/commands/lookup.py
+-rw-r--r--   0 youri      (501) staff       (20)     1878 2023-06-22 17:12:11.000000 escp-0.0.6/src/escp/commands/magic_encoding.py
+-rw-r--r--   0 youri      (501) staff       (20)     2355 2023-06-20 19:15:48.000000 escp-0.0.6/src/escp/commands/parameters.py
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.821798 escp-0.0.6/src/escp/demo/
+-rw-r--r--   0 youri      (501) staff       (20)       23 2023-03-07 17:19:32.000000 escp-0.0.6/src/escp/demo/__init__.py
+-rw-r--r--   0 youri      (501) staff       (20)      865 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/char_tables.py
+-rw-r--r--   0 youri      (501) staff       (20)      253 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/common.py
+-rw-r--r--   0 youri      (501) staff       (20)     2095 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/demo.py
+-rw-r--r--   0 youri      (501) staff       (20)     1186 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/i18n_char_set.py
+-rw-r--r--   0 youri      (501) staff       (20)     1237 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/poem.py
+-rw-r--r--   0 youri      (501) staff       (20)     5811 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/demo/test_page.py
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.822924 escp-0.0.6/src/escp/printer/
+-rw-r--r--   0 youri      (501) staff       (20)      187 2023-03-05 09:22:23.000000 escp-0.0.6/src/escp/printer/__init__.py
+-rw-r--r--   0 youri      (501) staff       (20)      381 2023-03-05 09:22:23.000000 escp-0.0.6/src/escp/printer/debug_printer.py
+-rw-r--r--   0 youri      (501) staff       (20)       43 2023-03-05 09:22:23.000000 escp-0.0.6/src/escp/printer/exceptions.py
+-rw-r--r--   0 youri      (501) staff       (20)      396 2023-03-05 09:22:23.000000 escp-0.0.6/src/escp/printer/output_printer.py
+-rw-r--r--   0 youri      (501) staff       (20)      128 2023-03-07 06:23:57.000000 escp-0.0.6/src/escp/printer/printer.py
+-rw-r--r--   0 youri      (501) staff       (20)     2364 2023-06-21 18:35:37.000000 escp-0.0.6/src/escp/printer/usb_printer.py
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.818241 escp-0.0.6/src/escp.egg-info/
+-rw-r--r--   0 youri      (501) staff       (20)     4373 2023-06-22 17:25:09.000000 escp-0.0.6/src/escp.egg-info/PKG-INFO
+-rw-r--r--   0 youri      (501) staff       (20)     1165 2023-06-22 17:25:09.000000 escp-0.0.6/src/escp.egg-info/SOURCES.txt
+-rw-r--r--   0 youri      (501) staff       (20)        1 2023-06-22 17:25:09.000000 escp-0.0.6/src/escp.egg-info/dependency_links.txt
+-rw-r--r--   0 youri      (501) staff       (20)        1 2023-03-05 09:15:42.000000 escp-0.0.6/src/escp.egg-info/not-zip-safe
+-rw-r--r--   0 youri      (501) staff       (20)       24 2023-06-22 17:25:09.000000 escp-0.0.6/src/escp.egg-info/requires.txt
+-rw-r--r--   0 youri      (501) staff       (20)        5 2023-06-22 17:25:09.000000 escp-0.0.6/src/escp.egg-info/top_level.txt
+drwxr-xr-x   0 youri      (501) staff       (20)        0 2023-06-22 17:25:09.824952 escp-0.0.6/test/
+-rw-r--r--   0 youri      (501) staff       (20)      283 2023-03-12 08:21:10.000000 escp-0.0.6/test/__init__.py
+-rw-r--r--   0 youri      (501) staff       (20)      353 2023-06-20 19:32:00.000000 escp-0.0.6/test/test_accented.py
+-rw-r--r--   0 youri      (501) staff       (20)     3813 2023-06-20 19:18:57.000000 escp-0.0.6/test/test_commands.py
+-rw-r--r--   0 youri      (501) staff       (20)     1101 2023-03-11 13:53:13.000000 escp-0.0.6/test/test_commands_24_48_pins.py
+-rw-r--r--   0 youri      (501) staff       (20)     1307 2023-03-11 13:52:58.000000 escp-0.0.6/test/test_commands_9_pin.py
+-rw-r--r--   0 youri      (501) staff       (20)     1452 2023-03-25 10:33:19.000000 escp-0.0.6/test/test_commands_char_set.py
+-rw-r--r--   0 youri      (501) staff       (20)     1452 2023-03-15 17:36:03.000000 escp-0.0.6/test/test_i18n_char_set.py
+-rw-r--r--   0 youri      (501) staff       (20)     1305 2023-06-22 17:11:08.000000 escp-0.0.6/test/test_magic_text.py
```

### Comparing `escp-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `escp-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/LICENSE` & `escp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/PKG-INFO` & `escp-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library to drive ESC/P printers
 Home-page: https://github.com/yackx/python-escp
 Author: Youri Ackx
 License: GPL
 Project-URL: Bug Tracker, https://github.com/yackx/python-escp/issues
 Project-URL: Documentation, https://github.com/yackx/python-escp/blob/master/README.md
 Project-URL: Release Notes, https://github.com/yackx/python-escp/releases
```

### Comparing `escp-0.0.5/README.md` & `escp-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/escp.jpg` & `escp-0.0.6/escp.jpg`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/setup.cfg` & `escp-0.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = escp
-version = 0.0.5
+version = 0.0.6
 url = https://github.com/yackx/python-escp
 description = A library to drive ESC/P printers
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 license = GPL
 license_file = LICENSE
 author = Youri Ackx
```

### Comparing `escp-0.0.5/src/escp/commands/commands.py` & `escp-0.0.6/src/escp/commands/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TypeVar
 from abc import ABC, abstractmethod
 
 from .exceptions import InvalidEncodingError
 from .parameters import Margin, PageLengthUnit, Typeface, Justification, CharacterSetVariant, CharacterTable
-from .magic_encoding import magic_encoding
+from .magic_encoding import default_plain_char_substitutions, default_char_set_substitutions
 
 
 def int_to_bytes(value: int) -> bytes:
     return int.to_bytes(value, length=1, byteorder='big', signed=False)
 
 
 T = TypeVar('T', bound='Commands')
@@ -129,19 +129,24 @@
         return self._append_cmd('character_set', int_to_bytes(cs.value))
 
     def text(self, content: bytes | str | int, *, encoding=None) -> T:
         """Add text to the buffer.
 
         Make sure the string or bytes you send are compatible with the printer encoding.
 
+        This method does not attempt to alter the content to fit the printer capabilities.
+        See `magic_text` if you need support for characters that cannot be printed directly.
+
+        This method's exact behavior depends on the content type:
+        - If it is a string, it will be byte encoded using the given encoding.
+        - If it is an integer, it will be converted to a single byte: 42 -> b'\x2a'.
+        - If it is bytes, it will be added as is.
+
         :param content:
         Text to add. Can be a string, bytes or integer.
-        If it is a string, it will be encoded using the given encoding.
-        If it is an integer, it will be converted to a single byte: 42 -> b'\x2a'.
-        If it is bytes, it will be added as is.
 
         :param encoding:
         Encoding to use when converting a string to bytes.
         The natural encoding for ESC/P is `cp437`, but you can use any compatible encoding.
         Note that the ESC/P2 manual refers to 'PC437' encoding.
         """
         if encoding and not isinstance(encoding, str):
@@ -155,42 +160,65 @@
                 raise InvalidEncodingError(f'length of content encoded to {encoding} mismatches original length')
         elif isinstance(content, int):
             c = int_to_bytes(content)
         elif isinstance(content, bytes):
             c = content
         return self._append(c)
 
-    def magic_text(self, content: str) -> T:
-        """Print UTF-8 text using the magic encoding.
+    def magic_text(
+            self,
+            content: str,
+            *,
+            character_set_substitution: dict[str, tuple[CharacterSetVariant, bytes]] = None,
+            plain_text_substitution: dict[str, bytes] = None,
+    ) -> T:
+        """Print UTF-8 text using character substitutions and character set switching.
 
         This method will attempt to issue character set commands in order to print
         the given UTF-8 string.
 
-        For instance, if the string contains an accented character 'é', it will switch to French
-        character set (`CharacterSetVariant.FRANCE` i.e. ESC R \x01), print the character,
-        and switch back to the original character set (USA is assumed).
+        It will also perform character substitutions for characters that have
+        UTF-8 equivalents in the printer character set.
+
+        For instance, if the string contains an accented character 'é',
+        it will switch to French character set (`CharacterSetVariant.FRANCE` i.e. ESC R \x01),
+        print the character, and switch back to the original character set.
 
-        The switch occurs only if necessary, i.e. if the character is not available in the current character set.
+        The switch occurs only if necessary, i.e. if the character is not available
+        in the current character set.
 
-        See `magic_encoding` for the mapping. Note that the mapping is far from complete.
+        If an upward arrow '↑' is encountered, it will be replaced by b'\x18'.
 
         :param content: UTF-8 string to print.
+        :param character_set_substitution: Character set substitutions to use.
+        :param plain_text_substitution: Plain text substitutions to use.
         """
+        if not character_set_substitution:
+            character_set_substitution = default_char_set_substitutions
+        if not plain_text_substitution:
+            plain_text_substitution = default_plain_char_substitutions
+
         initial_character_set = self.current_character_set
         for c in content:
             try:
-                cs, code = magic_encoding[c]
-                if self.current_character_set.value != cs.value:
-                    self.character_set(cs)
-                self.text(code)
+                # attempt to use a character substitution, e.g. '↑' becomes b'\x18'
+                substitute = plain_text_substitution[c]
+                self._append(substitute)
             except KeyError:
-                # no magic encoding needed
-                if self.current_character_set.value != initial_character_set.value:
-                    self.character_set(initial_character_set)
-                self.text(c)
+                try:
+                    # attempt to use a magic character set
+                    character_set, code = character_set_substitution[c]
+                    if self.current_character_set.value != character_set.value:
+                        self.character_set(character_set)
+                    self.text(code)
+                except KeyError:
+                    # treat as a regular character
+                    if self.current_character_set.value != initial_character_set.value:
+                        self.character_set(initial_character_set)
+                    self.text(c)
 
         if self.current_character_set != initial_character_set:
             self.character_set(initial_character_set)
 
         return self
 
     def cr_lf(self, how_many=1) -> T:
@@ -255,14 +283,17 @@
 
     def typeface(self, tf: Typeface) -> T:
         return self._append_cmd('typeface', int_to_bytes(tf.value))
 
     def margin(self, margin: Margin, value: int) -> T:
         """Set a margin.
 
+        For left and right margins, the value equals the number of characters
+        from the left-most mechanically printable position, in the current character pitch.
+
         The right margin value starts from the left margin.
         Example:
             left margin = 10 (1 inch left margin)
             right margin = 75 (1 inch right margin)
 
         Top margin is only available on ESC/P2 printers.
```

### Comparing `escp-0.0.5/src/escp/commands/commands_24_48_pin.py` & `escp-0.0.6/src/escp/commands/commands_24_48_pin.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/src/escp/commands/commands_9_pin.py` & `escp-0.0.6/src/escp/commands/commands_9_pin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Self
 
-from escp.commands.commands import T
-
-from .commands import Commands, int_to_bytes, CharacterTable
+from .commands import T, Commands, int_to_bytes, CharacterTable
 
 
 class Commands_9_Pin(Commands):
 
     specific_cmds = {
         'line_spacing_n_216': b'\x1b3',
     }
```

### Comparing `escp-0.0.5/src/escp/commands/parameters.py` & `escp-0.0.6/src/escp/commands/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.d2 = d2
         self.d3 = d3
 
     def __str__(self):
         return f'{self.name} (d2={self.d2}, d3={self.d3})'
 
     # int value is d2 and d3 parameters in the manual
-    # d1 to be setseparately
+    # d1 to be set separately
     # [C-75]
 
     ITALIC = 0, 0
     PC437_US = 1, 0
     PC437_GREEK = 1, 16
     PC932_JAPANESE = 2, 0
     PC850_MULTILINGUAL = 3, 0
```

### Comparing `escp-0.0.5/src/escp/demo/char_tables.py` & `escp-0.0.6/src/escp/demo/char_tables.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/src/escp/demo/demo.py` & `escp-0.0.6/src/escp/demo/demo.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/src/escp/demo/i18n_char_set.py` & `escp-0.0.6/src/escp/demo/i18n_char_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from escp import CharacterSetVariant
-
-from ..commands import Commands, Justification, PageLengthUnit, CharacterTable
-from ..printer import Printer
 from .common import print_and_reset
-
+from ..commands import CharacterSetVariant, Commands
+from ..printer import Printer
 
 PAGE_LENGTH_INCHES = 12
 
 
 def print_i18n_char_set(printers: [Printer], cmd: Commands):
     def _print_and_reset():
         print_and_reset(printers, cmd)
```

### Comparing `escp-0.0.5/src/escp/demo/poem.py` & `escp-0.0.6/src/escp/demo/poem.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/src/escp/demo/test_page.py` & `escp-0.0.6/src/escp/demo/test_page.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/src/escp/printer/usb_printer.py` & `escp-0.0.6/src/escp/printer/usb_printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import sys
 import typing
 
 import usb.core
 import usb.util
 
-from .printer import Printer
 from .exceptions import PrinterNotFound
+from .printer import Printer
 
 
 class UsbPrinter(Printer):
     # Reference printer Epson LX-300+II
     # ID_VENDOR = 0x04b8
     # ID_PRODUCT = 0x0005
 
@@ -30,15 +29,15 @@
         devices = usb.core.show_devices()
         self.log(devices)
 
         self.device: usb.core.Device = usb.core.find(idVendor=self.id_vendor, idProduct=self.id_product)
         if not self.device:
             hex_value = lambda x: f'0x{x:04x}'
             raise PrinterNotFound(f'USB id_vendor={hex_value(id_vendor)} id_product={hex_value(id_product)}')
-        self.log(self.device)
+        self.log(str(self.device))
         # TODO Check is printer
 
         self.detach_kernel_driver()
 
         self.log("Reset device")
         self.device.reset()
 
@@ -47,31 +46,32 @@
         self.log(f"Module: ${module}")
         if module.endswith('libusb1'):
             # TODO Explicit check for errno 13 (permission denied)
             check_driver = None
             try:
                 check_driver = self.device.is_kernel_driver_active(interface=0)
             except usb.core.USBError as e:
-                self.log(f"Failed to check kernel driver activation: ${e}", file=sys.stderr)
+                self.log(f"Failed to check kernel driver activation: ${e}")
 
             if check_driver is None or check_driver:
                 try:
                     self.device.detach_kernel_driver(0)
                 except usb.core.USBError as e:
-                    self.log(f"Failed to detach kernel driver: ${e}", file=sys.stderr)
+                    self.log(f"Failed to detach kernel driver: ${e}")
 
     def send(self, sequence: bytes):
         self.device.write(self.endpoint_out, sequence, 5)
 
     def close(self):
         self.log('Releasing USB')
         if self.device:
             usb.util.dispose_resources(self.device)
         self.device = None
-        self.log_io.flush()
+        if self.log_io:
+            self.log_io.flush()
 
     def log(self, message: str):
         if self.log_io:
             self.log_io.write(message)
 
     def __del__(self):
         self.close()
```

### Comparing `escp-0.0.5/src/escp.egg-info/PKG-INFO` & `escp-0.0.6/src/escp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library to drive ESC/P printers
 Home-page: https://github.com/yackx/python-escp
 Author: Youri Ackx
 License: GPL
 Project-URL: Bug Tracker, https://github.com/yackx/python-escp/issues
 Project-URL: Documentation, https://github.com/yackx/python-escp/blob/master/README.md
 Project-URL: Release Notes, https://github.com/yackx/python-escp/releases
```

### Comparing `escp-0.0.5/src/escp.egg-info/SOURCES.txt` & `escp-0.0.6/src/escp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,13 +31,14 @@
 src/escp/printer/__init__.py
 src/escp/printer/debug_printer.py
 src/escp/printer/exceptions.py
 src/escp/printer/output_printer.py
 src/escp/printer/printer.py
 src/escp/printer/usb_printer.py
 test/__init__.py
+test/test_accented.py
 test/test_commands.py
 test/test_commands_24_48_pins.py
 test/test_commands_9_pin.py
 test/test_commands_char_set.py
 test/test_i18n_char_set.py
 test/test_magic_text.py
```

### Comparing `escp-0.0.5/test/test_commands.py` & `escp-0.0.6/test/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,18 +137,14 @@
         commands.line_spacing(1, 1)
 
 
 def test_page_length_in_lines(commands):
     assert commands.page_length(20, PageLengthUnit.LINES).buffer == b'\x1b\x43\x14'
 
 
-def test_page_length_in_lines(commands):
-    assert commands.page_length(20, PageLengthUnit.LINES).buffer == b'\x1b\x43\x14'
-
-
 def test_page_length_in_inch(commands):
     assert commands.page_length(20, PageLengthUnit.INCHES).buffer == b'\x1bC\x00\x14'
 
 
 def test_clear(commands):
     commands.text("Hello world")
     assert commands.clear().buffer == b''
```

### Comparing `escp-0.0.5/test/test_commands_24_48_pins.py` & `escp-0.0.6/test/test_commands_24_48_pins.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/test/test_commands_9_pin.py` & `escp-0.0.6/test/test_commands_9_pin.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/test/test_commands_char_set.py` & `escp-0.0.6/test/test_commands_char_set.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/test/test_i18n_char_set.py` & `escp-0.0.6/test/test_i18n_char_set.py`

 * *Files identical despite different names*

### Comparing `escp-0.0.5/test/test_magic_text.py` & `escp-0.0.6/test/test_magic_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import pytest
-from escp import CharacterSetVariant
-
+from src.escp import CharacterSetVariant
 from test import CommandsDefault
 
 
 @pytest.fixture
 def commands():
     return CommandsDefault()
 
 
-def test_magic_text_no_magic_needed(commands):
+def test_magic_needed(commands):
     assert commands.magic_text("Hello world").buffer == b'Hello world'
 
 
-def test_magic_text_no_magic_needed_special_char(commands):
+def test_no_magic_needed_special_char(commands):
     assert commands.magic_text("Hello $").buffer == b'Hello $'
 
 
-def test_magic_text_switch_once(commands):
+def test_char_set_switch_once(commands):
     assert commands.magic_text("Salut à toi").buffer == b'Salut \x1bR\x01\x40\x1bR\x00 toi'
 
 
-def test_magic_text_switch_once_for_multiple_characters(commands):
+def test_switch_char_set_for_multiple_characters(commands):
     assert commands.magic_text("Salut ààà toi").buffer == b'Salut \x1bR\x01\x40\x40\x40\x1bR\x00 toi'
 
 
-def test_magic_text_switch_twice(commands):
+def test_switch_char_switch_twice(commands):
     assert commands.magic_text("Salut à toi©").buffer == b'Salut \x1bR\x01\x40\x1bR\x00 toi\x1bR\x40\x7b\x1bR\x00'
 
 
-def test_magic_text_no_switch_already_good_char_set(commands):
+def test_no_switch_already_good_char_set(commands):
     commands.character_set(CharacterSetVariant.FRANCE)
     assert commands.magic_text("Salut à toi").buffer == b'\x1bR\x01Salut \x40 toi'
+
+
+def test_character_substitution(commands):
+    assert commands.magic_text("a → b").buffer == b'a \x1a b'
+
+
+def test_char_set_switch_once_plus_one_substitution(commands):
+    assert commands.magic_text("→Salut à toi").buffer == b'\x1aSalut \x1bR\x01\x40\x1bR\x00 toi'
```

