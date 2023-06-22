# Comparing `tmp/jort-1.2.0.tar.gz` & `tmp/jort-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jort-1.2.0.tar", last modified: Tue May 23 23:50:08 2023, max compression
+gzip compressed data, was "jort-1.3.0.tar", last modified: Thu Jun 22 00:09:26 2023, max compression
```

## Comparing `jort-1.2.0.tar` & `jort-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.263861 jort-1.2.0/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.2.0/LICENSE
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-23 23:50:08.263861 jort-1.2.0/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1862 2023-05-22 22:30:52.000000 jort-1.2.0/README.md
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.255861 jort-1.2.0/jort/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      294 2023-05-23 01:49:41.000000 jort-1.2.0/jort/__init__.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1872 2023-05-19 21:26:18.000000 jort-1.2.0/jort/checkpoint.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      476 2023-05-23 23:19:43.000000 jort-1.2.0/jort/config.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1330 2023-05-19 22:08:52.000000 jort-1.2.0/jort/datetime_utils.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.2.0/jort/exceptions.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4846 2023-05-23 23:32:29.000000 jort-1.2.0/jort/jort_exe.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     8013 2023-05-23 23:35:49.000000 jort-1.2.0/jort/reporting_callbacks.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5019 2023-05-23 23:44:05.000000 jort-1.2.0/jort/track_cli.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5228 2023-05-23 23:22:34.000000 jort-1.2.0/jort/tracker.py
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.259861 jort-1.2.0/jort.egg-info/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      368 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/SOURCES.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/dependency_links.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       44 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/entry_points.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       98 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/requires.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/top_level.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-05-23 23:50:08.263861 jort-1.2.0/setup.cfg
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      953 2023-05-23 22:59:53.000000 jort-1.2.0/setup.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.353326 jort-1.3.0/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.3.0/LICENSE
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3433 2023-06-22 00:09:26.353326 jort-1.3.0/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2978 2023-06-22 00:03:27.000000 jort-1.3.0/README.md
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.345326 jort-1.3.0/jort/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      331 2023-06-21 20:57:53.000000 jort-1.3.0/jort/__init__.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1372 2023-06-20 18:11:13.000000 jort-1.3.0/jort/_config.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       21 2023-06-21 20:42:19.000000 jort-1.3.0/jort/_version.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3112 2023-05-27 04:28:06.000000 jort-1.3.0/jort/checkpoint.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1378 2023-05-27 04:28:06.000000 jort-1.3.0/jort/datetime_utils.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.3.0/jort/exceptions.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11030 2023-06-21 23:56:32.000000 jort-1.3.0/jort/jort_exe.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     9259 2023-06-21 20:57:40.000000 jort-1.3.0/jort/reporting_callbacks.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     7663 2023-06-21 23:49:04.000000 jort-1.3.0/jort/track_cli.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    10733 2023-06-21 23:39:56.000000 jort-1.3.0/jort/tracker.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 00:09:26.349326 jort-1.3.0/jort.egg-info/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3433 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      386 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       43 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/entry_points.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      153 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/requires.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-06-22 00:09:25.000000 jort-1.3.0/jort.egg-info/top_level.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-06-22 00:09:26.353326 jort-1.3.0/setup.cfg
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      967 2023-06-21 20:45:06.000000 jort-1.3.0/setup.py
```

### Comparing `jort-1.2.0/LICENSE` & `jort-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jort-1.2.0/jort/reporting_callbacks.py` & `jort-1.3.0/jort/reporting_callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,87 @@
+from abc import ABC, abstractmethod
 import os
 import json
 import smtplib
 import ssl
 import email
 from email import encoders
 from email.mime.base import MIMEBase
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.mime.application import MIMEApplication
 import twilio.rest
 import humanfriendly
-from . import config
+from . import _config
 from . import exceptions
 
 
-class Callback(object):
+class Callback(ABC):
+    """
+    Abstract base class for notification callbacks.
+    """
     def __init__(self):
         pass
 
+    @abstractmethod
     def format_message(self, payload):
+        """
+        Format notification message as a string.
+        """
         pass
 
+    @abstractmethod
     def execute(self, payload):
+        """
+        Send notification given job status payload.
+        """
         pass
     
     
 class PrintReport(Callback):
-    def __init__(self):
-        pass
-
-    def format_message(self, payload):
-        return (
-            f'\n'
-            f'The job \'{payload["name"]}\' finished running '
-            f'in {humanfriendly.format_timespan(payload["runtime"])}'
-        )
-
-    def execute(self, payload):
-        print(self.format_message(payload))
-
-
-class SMSNotification(Callback):
     """
-    Send SMS notifications to and from numbers managed by your Twilio account.
+    Print job runtime on completion.
     """
-    def __init__(self, receive_number=None):
-        config_data = config.get_config_data()
-        self.receive_number = config_data.get("twilio_receive_number")
-        self.send_number = config_data.get("twilio_send_number")
-        self.twilio_account_sid = config_data.get("twilio_account_sid")
-        self.twilio_auth_token = config_data.get("twilio_auth_token")
-        if receive_number is not None:
-            self.receive_number = receive_number
-
-        if self.twilio_account_sid is None or self.twilio_auth_token is None:
-            raise exceptions.JortCredentialException("Missing Twilio credentials, add with `jort -i` command")
-        if self.send_number is None:
-            raise exceptions.JortException("Missing Twilio sending number, add with `jort -i` command")
-        if self.receive_number is None:
-            raise exceptions.JortException("Missing receiving number")
+    def __init__(self):
+        pass
 
     def format_message(self, payload):
         if payload["status"] == "success":
             return (
-                f'Your job \'{payload["name"]}\' successfully completed '
+                f'\n'
+                f'Your job `{payload["name"]}` successfully completed '
                 f'in {humanfriendly.format_timespan(payload["runtime"])}'
             )
         elif payload["status"] == "error":
             error_text = payload["error_message"].split(":")[0]
             return (
-                f'Your job \'{payload["name"]}\' exited in error ({error_text}) '
+                f'\n'
+                f'Your job `{payload["name"]}` exited in error ({error_text}) '
                 f'after {humanfriendly.format_timespan(payload["runtime"])}'
             )
         elif payload["status"] == "finished":
             return (
-                f'Your job \'{payload["name"]}\' finished running '
+                f'\n'
+                f'Your job `{payload["name"]}` finished running '
                 f'in {humanfriendly.format_timespan(payload["runtime"])}'
             )
         else:
             raise exceptions.JortException(f'Invalid status: {payload["status"]}')
-    
+
     def execute(self, payload):
-        client = twilio.rest.Client(self.twilio_account_sid,
-                                    self.twilio_auth_token)
-        message = client.messages.create(body=self.format_message(payload),
-                                         from_=self.send_number,
-                                         to=self.receive_number)
+        print(self.format_message(payload))
 
 
 class EmailNotification(Callback):
     """
-    Send email notifications to and from your email account.
+    Send email notifications to and from your email account. Requires login 
+    credentials, which can be entered at the command line via :code:`jort -i`.
     """
     def __init__(self, email=None):
-        config_data = config.get_config_data()
+        config_data = _config.get_config_data()
         self.email = config_data.get("email")
         self.smtp_server = config_data.get("smtp_server")
         self.email_password = config_data.get("email_password")
         if email is not None:
             self.email = email
 
         if self.email_password is None:
@@ -183,15 +167,15 @@
         email_data = self.format_message(payload)
 
         message = MIMEMultipart("alternative")
         message.attach(MIMEText(email_data["body"], "plain"))
         message.attach(MIMEText(email_data["html_body"], "html"))
 
         if payload["stdout_fn"] is not None:
-            stdout_path = f'{config.JORT_DIR}/{payload["stdout_fn"]}'
+            stdout_path = f'{_config.JORT_DIR}/{payload["stdout_fn"]}'
             with open(stdout_path, "r") as f:
                 attachment = MIMEApplication(f.read(), _subtype="txt")
             attachment.add_header("Content-Disposition", "attachment", filename="output.txt")
 
             message_mix = MIMEMultipart("mixed")
             message_mix.attach(message)
             message_mix.attach(attachment)
@@ -203,12 +187,57 @@
 
         # Secure connection
         context = ssl.create_default_context()
         with smtplib.SMTP_SSL(self.smtp_server, port=465, context=context) as server:
             server.login(self.email, self.email_password)
             server.sendmail(message["From"], message["To"], message.as_string())
 
-            
 
+class TextNotification(Callback):
+    """
+    Send SMS notifications to and from numbers managed by your Twilio account. Requires 
+    Twilio credentials, which can be entered at the command line via :code:`jort -i`.
+    """
+    def __init__(self, receive_number=None):
+        config_data = _config.get_config_data()
+        self.receive_number = config_data.get("twilio_receive_number")
+        self.send_number = config_data.get("twilio_send_number")
+        self.twilio_account_sid = config_data.get("twilio_account_sid")
+        self.twilio_auth_token = config_data.get("twilio_auth_token")
+        if receive_number is not None:
+            self.receive_number = receive_number
 
+        if self.twilio_account_sid is None or self.twilio_auth_token is None:
+            raise exceptions.JortCredentialException("Missing Twilio credentials, add with `jort -i` command")
+        if self.send_number is None:
+            raise exceptions.JortException("Missing Twilio sending number, add with `jort -i` command")
+        if self.receive_number is None:
+            raise exceptions.JortException("Missing receiving number")
+
+    def format_message(self, payload):
+        if payload["status"] == "success":
+            return (
+                f'Your job `{payload["name"]}` successfully completed '
+                f'in {humanfriendly.format_timespan(payload["runtime"])}'
+            )
+        elif payload["status"] == "error":
+            error_text = payload["error_message"].split(":")[0]
+            return (
+                f'Your job `{payload["name"]}` exited in error ({error_text}) '
+                f'after {humanfriendly.format_timespan(payload["runtime"])}'
+            )
+        elif payload["status"] == "finished":
+            return (
+                f'Your job `{payload["name"]}` finished running '
+                f'in {humanfriendly.format_timespan(payload["runtime"])}'
+            )
+        else:
+            raise exceptions.JortException(f'Invalid status: {payload["status"]}')
+    
+    def execute(self, payload):
+        client = twilio.rest.Client(self.twilio_account_sid,
+                                    self.twilio_auth_token)
+        message = client.messages.create(body=self.format_message(payload),
+                                         from_=self.send_number,
+                                         to=self.receive_number)
```

### Comparing `jort-1.2.0/setup.py` & `jort-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
-__version__ = '1.2.0'
-
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 entry_points = {
     'console_scripts': [
-        'jort = jort.jort_exe:main'
+        'jort = jort.jort_exe:cli'
     ]
 }
 
 with open("requirements.txt", "r") as f:
     install_requires = f.readlines()
 
+exec(open('jort/_version.py').read())
 setuptools.setup(
     name='jort',
     version=__version__,
     author='Bryan Brzycki',
     author_email='bbrzycki@berkeley.edu',
     description='Script profiler with checkpoints',
     long_description=long_description,
```

