# Comparing `tmp/error-alerts-4.2.tar.gz` & `tmp/error-alerts-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.2.tar", last modified: Thu Jun 22 14:41:00 2023, max compression
+gzip compressed data, was "error-alerts-4.3.tar", last modified: Thu Jun 22 14:54:28 2023, max compression
```

## Comparing `error-alerts-4.2.tar` & `error-alerts-4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.627031 error-alerts-4.2/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.2/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-22 14:41:00.628030 error-alerts-4.2/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.621036 error-alerts-4.2/error_alerts/
--rw-rw-rw-   0        0        0     2426 2023-06-22 14:40:29.000000 error-alerts-4.2/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 14:41:00.626033 error-alerts-4.2/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-22 14:41:00.000000 error-alerts-4.2/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 14:41:00.628030 error-alerts-4.2/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-22 14:40:51.000000 error-alerts-4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.424728 error-alerts-4.3/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.3/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-22 14:54:28.424728 error-alerts-4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.419732 error-alerts-4.3/error_alerts/
+-rw-rw-rw-   0        0        0     2406 2023-06-22 14:54:25.000000 error-alerts-4.3/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.423729 error-alerts-4.3/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 14:54:28.425728 error-alerts-4.3/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-22 14:54:21.000000 error-alerts-4.3/setup.py
```

### Comparing `error-alerts-4.2/PKG-INFO` & `error-alerts-4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.2
+Version: 4.3
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.2/README.md` & `error-alerts-4.3/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.2/error_alerts/__init__.py` & `error-alerts-4.3/error_alerts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,34 @@
         else:
             error = str(exception)
         message = f'{title}: {error}'
         if error == self.last_error and not self.resend_repeat_errors:
             self.printer(message, level='error')
         if error != self.last_error or self.resend_repeat_errors:
             self.printer(message, level='error')
-            if self.channel:
+            if channel:
                 try:
-                    self.bot.send_message(self.channel, message[:4096])
+                    self.bot.send_message(channel, message[:4096])
                 except Exception as telegram_error:
                     self.printer('Error sending alert message to Telegram:', telegram_error, level='error')
             self.last_error = error
         if self.raise_error:
             raise Exception('Raiser') from exception
     def send_message(self, *messages, print_message=True, current_time=True, channel=None):
         if not channel:
             channel = self.channel
         final_message = ''
         for message in messages:
             final_message += message
             final_message += ' '
         if print_message:
             self.printer(final_message, current_time=current_time)
-        if self.channel:
+        if channel:
             try:
-                self.bot.send_message(self.channel, final_message[:4096])
+                self.bot.send_message(channel, final_message[:4096])
             except Exception as telegram_error:
                 self.printer('Error sending message to Telegram:', telegram_error, level='error')
     
     def printer(self, *items, level='info', current_time=True):
         if self.logger:
             if current_time:
                 self.logger.current_time(*items, level=level)
```

### Comparing `error-alerts-4.2/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.3/error_alerts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.2
+Version: 4.3
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

