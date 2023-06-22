# Comparing `tmp/error-alerts-4.1.tar.gz` & `tmp/error-alerts-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.1.tar", last modified: Thu Jun 15 14:36:34 2023, max compression
+gzip compressed data, was "error-alerts-4.2.tar", last modified: Thu Jun 22 14:41:00 2023, max compression
```

## Comparing `error-alerts-4.1.tar` & `error-alerts-4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.771242 error-alerts-4.1/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.1/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-15 14:36:34.771242 error-alerts-4.1/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.765246 error-alerts-4.1/error_alerts/
--rw-rw-rw-   0        0        0     2280 2023-04-12 16:43:51.000000 error-alerts-4.1/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.770243 error-alerts-4.1/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 14:36:34.771242 error-alerts-4.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-15 14:34:49.000000 error-alerts-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.627031 error-alerts-4.2/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.2/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-22 14:41:00.628030 error-alerts-4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.621036 error-alerts-4.2/error_alerts/
+-rw-rw-rw-   0        0        0     2426 2023-06-22 14:40:29.000000 error-alerts-4.2/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.626033 error-alerts-4.2/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 14:41:00.628030 error-alerts-4.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-22 14:40:51.000000 error-alerts-4.2/setup.py
```

### Comparing `error-alerts-4.1/PKG-INFO` & `error-alerts-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.1
+Version: 4.2
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.1/README.md` & `error-alerts-4.2/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.1/error_alerts/__init__.py` & `error-alerts-4.2/error_alerts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,17 @@
             self.bot = Bot(token=token)
         self.channel = channel
         self.logger = logger
         self.full_error = full_error
         self.raise_error = raise_error
         self.resend_repeat_errors = resend_repeat_errors
         self.last_error = None
-    def send(self, title='Error', exception=None):
+    def send(self, title='Error', exception=None, channel=None):
+        if not channel:
+            channel = self.channel
         if self.full_error:
             error = traceback.format_exc()
         else:
             error = str(exception)
         message = f'{title}: {error}'
         if error == self.last_error and not self.resend_repeat_errors:
             self.printer(message, level='error')
@@ -25,15 +27,17 @@
                 try:
                     self.bot.send_message(self.channel, message[:4096])
                 except Exception as telegram_error:
                     self.printer('Error sending alert message to Telegram:', telegram_error, level='error')
             self.last_error = error
         if self.raise_error:
             raise Exception('Raiser') from exception
-    def send_message(self, *messages, print_message=True, current_time=True):
+    def send_message(self, *messages, print_message=True, current_time=True, channel=None):
+        if not channel:
+            channel = self.channel
         final_message = ''
         for message in messages:
             final_message += message
             final_message += ' '
         if print_message:
             self.printer(final_message, current_time=current_time)
         if self.channel:
```

### Comparing `error-alerts-4.1/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.2/error_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.1
+Version: 4.2
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

