# Comparing `tmp/pymino-1.2.1.6.tar.gz` & `tmp/pymino-1.2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-afeabpsf\pymino-1.2.1.6.tar", last modified: Thu Jun 22 01:49:34 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-a_jwzy15\pymino-1.2.1.7.tar", last modified: Thu Jun 22 04:18:58 2023, max compression
```

## Comparing `pymino-1.2.1.6.tar` & `pymino-1.2.1.7.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.989063 pymino-1.2.1.6/
--rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.6/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-06-22 01:49:34.989559 pymino-1.2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.890855 pymino-1.2.1.6/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-22 01:48:35.000000 pymino-1.2.1.6/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.927558 pymino-1.2.1.6/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/account.py
--rw-rw-rw-   0        0        0   340339 2023-06-22 01:48:27.000000 pymino-1.2.1.6/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   338874 2023-06-22 01:49:07.000000 pymino-1.2.1.6/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.969719 pymino-1.2.1.6/pymino/ext/entities/
--rw-rw-rw-   0        0        0      402 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.987575 pymino-1.2.1.6/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.6/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:49:34.902263 pymino-1.2.1.6/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-06-22 01:49:34.000000 pymino-1.2.1.6/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-06-22 01:49:34.000000 pymino-1.2.1.6/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 01:49:34.000000 pymino-1.2.1.6/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-22 01:49:34.000000 pymino-1.2.1.6/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 01:49:34.000000 pymino-1.2.1.6/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-22 01:49:34.992039 pymino-1.2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.698957 pymino-1.2.1.7/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.7/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-06-22 04:18:58.699453 pymino-1.2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.637454 pymino-1.2.1.7/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-22 04:17:43.000000 pymino-1.2.1.7/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.663742 pymino-1.2.1.7/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   343858 2023-06-22 04:17:24.000000 pymino-1.2.1.7/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   342341 2023-06-22 04:17:35.000000 pymino-1.2.1.7/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.687550 pymino-1.2.1.7/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-06-22 03:04:45.000000 pymino-1.2.1.7/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-06-22 04:13:53.000000 pymino-1.2.1.7/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.697965 pymino-1.2.1.7/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.646408 pymino-1.2.1.7/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-22 04:18:58.705406 pymino-1.2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.7/setup.py
```

### Comparing `pymino-1.2.1.6/LICENSE` & `pymino-1.2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/PKG-INFO` & `pymino-1.2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.6
+Version: 1.2.1.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.6/README.md` & `pymino-1.2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/__init__.py` & `pymino-1.2.1.7/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.1.6'
+__version__ = '1.2.1.7'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.1.6/pymino/async_bot.py` & `pymino-1.2.1.7/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/bot.py` & `pymino-1.2.1.7/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/client.py` & `pymino-1.2.1.7/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/account.py` & `pymino-1.2.1.7/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/async_community.py` & `pymino-1.2.1.7/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -7274,15 +7274,16 @@
                   userId: str = None,
                   blogId: str = None,
                   wikiId: str = None,
                   quizId: str = None,
                   fileId: str = None,
                   pageToken: str = None,
                   size: int = 25,
-                  comId: Union[str, int] = None):
+                  comId: Union[str, int] = None
+                  ) -> AdminLogList:
         """
         Fetches the admin log entries for the specified parameters.
 
         :param userId: The ID of the user to filter the admin log by. (Optional)
         :type userId: str, optional
         :param blogId: The ID of the blog to filter the admin log by. (Optional)
         :type blogId: str, optional
@@ -7309,55 +7310,133 @@
 
         >>> admin_log = client.community.fetch_admin_log(userId="12345")
         ... for entry in admin_log:
         ...     print(entry.action)
         ...     print(entry.timestamp)
         """
         if pageToken is None:
-            if userId: return await self.session.handler(
+            if userId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}"
-            )
-            elif blogId: return await self.session.handler(
+            ))
+            elif blogId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}"
-            )
-            elif wikiId: return await self.session.handler(
+            ))
+            elif wikiId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}"
-            )
-            elif quizId: return await self.session.handler(
+            ))
+            elif quizId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}"
-            )
-            elif fileId: return await self.session.handler(
+            ))
+            elif fileId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}"
-            )
-            else: return await self.session.handler(
+            ))
+            else: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}"
-            )
-        elif userId: return await self.session.handler(
+            ))
+        elif userId: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url =  f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}&pageToken={pageToken}"
-            )
-        elif blogId: return await self.session.handler(
+            ))
+        elif blogId: return AdminLogList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif wikiId: return await self.session.hadler(
+        ))
+        elif wikiId: return AdminLogList(await self.session.hadler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif quizId: return await self.session.handler(
+        ))
+        elif quizId: return AdminLogList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif fileId: return await self.session.handler(
+        ))
+        elif fileId: return AdminLogList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        else: return await self.session.handler(
+        ))
+        else: return AdminLogList(await self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}&pageToken={pageToken}"
-            )
+            ))
+        
+
+    @community
+    async def fetch_user_moderation_history(
+        self,
+        userId: str,
+        pageToken: str = None,
+        size: int = 25,
+        comId: Union[str, int] = None
+    ) -> AdminLogList:
+        """
+        Fetches the moderation history for the specified user.
+
+        :param userId: The ID of the user to fetch the moderation history for.
+        :type userId: str
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch the moderation history from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The moderation history for the specified user.
+        :rtype: response object
+
+        This function fetches the moderation history for the specified user in the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> moderation_history = client.community.fetch_user_moderation_history("12345")
+        ... for entry in moderation_history:
+        ...     print(entry.action)
+        ...     print(entry.timestamp)
+        """
+        return await self.fetch_admin_log(userId=userId, pageToken=pageToken, size=size, comId=comId)
+
+
+    @community
+    async def fetch_leader_log(
+        self,
+        userId: str,
+        size: int = 25,
+        pageToken: str = None,
+        comId: Union[str, int] = None
+    ) -> AdminLogList:
+        """
+        Fetches the admin log entries for the specified parameters.
+
+        :param userId: The ID of the user to filter the admin log by.
+        :type userId: str
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param comId: The ID of the community to fetch the admin log from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The admin log entries matching the specified parameters.
+        :rtype: response object
+
+        This function fetches the admin log entries for the specified parameters in the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> admin_log = client.community.fetch_admin_log(userId=client.userId)
+        ... for penalty_type, ban_reason, userId in zip(adminLog.operation_name, adminLog.ext_data.note, adminLog.objectId):
+        ...     print(f"{penalty_type} - {ban_reason} - {userId}")
+        """
+        if pageToken: return AdminLogList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pageToken={pageToken}&pagingType=t"
+        ))
+        else: return AdminLogList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pagingType=t"
+        ))
```

### Comparing `pymino-1.2.1.6/pymino/ext/async_context.py` & `pymino-1.2.1.7/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/async_event_handler.py` & `pymino-1.2.1.7/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/async_socket.py` & `pymino-1.2.1.7/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/community.py` & `pymino-1.2.1.7/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -7192,15 +7192,16 @@
                   userId: str = None,
                   blogId: str = None,
                   wikiId: str = None,
                   quizId: str = None,
                   fileId: str = None,
                   pageToken: str = None,
                   size: int = 25,
-                  comId: Union[str, int] = None):
+                  comId: Union[str, int] = None
+    ) -> AdminLogList:
         """
         Fetches the admin log entries for the specified parameters.
 
         :param userId: The ID of the user to filter the admin log by. (Optional)
         :type userId: str, optional
         :param blogId: The ID of the blog to filter the admin log by. (Optional)
         :type blogId: str, optional
@@ -7227,55 +7228,133 @@
 
         >>> admin_log = client.community.fetch_admin_log(userId="12345")
         ... for entry in admin_log:
         ...     print(entry.action)
         ...     print(entry.timestamp)
         """
         if pageToken is None:
-            if userId: return self.session.handler(
+            if userId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}"
-            )
-            elif blogId: return self.session.handler(
+            ))
+            elif blogId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}"
-            )
-            elif wikiId: return self.session.handler(
+            ))
+            elif wikiId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}"
-            )
-            elif quizId: return self.session.handler(
+            ))
+            elif quizId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}"
-            )
-            elif fileId: return self.session.handler(
+            ))
+            elif fileId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}"
-            )
-            else: return self.session.handler(
+            ))
+            else: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}"
-            )
-        elif userId: return self.session.handler(
+            ))
+        elif userId: return AdminLogList(self.session.handler(
                 method = "GET",
                 url =  f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}&pageToken={pageToken}"
-            )
-        elif blogId: return self.session.handler(
+            ))
+        elif blogId: return AdminLogList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif wikiId: return self.session.hadler(
+        ))
+        elif wikiId: return AdminLogList(self.session.hadler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif quizId: return self.session.handler(
+        ))
+        elif quizId: return AdminLogList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        elif fileId: return self.session.handler(
+        ))
+        elif fileId: return AdminLogList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}&pageToken={pageToken}"
-        )
-        else: return self.session.handler(
+        ))
+        else: return AdminLogList(self.session.handler(
                 method = "GET",
                 url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}&pageToken={pageToken}"
-            )
+            ))
+
+
+    @community
+    def fetch_user_moderation_history(
+        self,
+        userId: str,
+        pageToken: str = None,
+        size: int = 25,
+        comId: Union[str, int] = None
+    ) -> AdminLogList:
+        """
+        Fetches the moderation history for the specified user.
+
+        :param userId: The ID of the user to fetch the moderation history for.
+        :type userId: str
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch the moderation history from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The moderation history for the specified user.
+        :rtype: response object
+
+        This function fetches the moderation history for the specified user in the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> moderation_history = client.community.fetch_user_moderation_history("12345")
+        ... for entry in moderation_history:
+        ...     print(entry.action)
+        ...     print(entry.timestamp)
+        """
+        return self.fetch_admin_log(userId=userId, pageToken=pageToken, size=size, comId=comId)
+
+
+    @community
+    def fetch_leader_log(
+        self,
+        userId: str,
+        size: int = 25,
+        pageToken: str = None,
+        comId: Union[str, int] = None
+    ) -> AdminLogList:
+        """
+        Fetches the admin log entries for the specified parameters.
+
+        :param userId: The ID of the user to filter the admin log by.
+        :type userId: str
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param comId: The ID of the community to fetch the admin log from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The admin log entries matching the specified parameters.
+        :rtype: response object
+
+        This function fetches the admin log entries for the specified parameters in the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> admin_log = client.community.fetch_admin_log(userId=client.userId)
+        ... for penalty_type, ban_reason, userId in zip(adminLog.operation_name, adminLog.ext_data.note, adminLog.objectId):
+        ...     print(f"{penalty_type} - {ban_reason} - {userId}")
+        """
+        if pageToken: return AdminLogList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pageToken={pageToken}&pagingType=t"
+        ))
+        else: return AdminLogList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pagingType=t"
+        ))
```

### Comparing `pymino-1.2.1.6/pymino/ext/console.py` & `pymino-1.2.1.7/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/context.py` & `pymino-1.2.1.7/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/dispatcher.py` & `pymino-1.2.1.7/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/acm.py` & `pymino-1.2.1.7/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/api_response.py` & `pymino-1.2.1.7/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/bubble.py` & `pymino-1.2.1.7/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.7/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/comments.py` & `pymino-1.2.1.7/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/enums.py` & `pymino-1.2.1.7/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.7/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/general.py` & `pymino-1.2.1.7/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/handlers.py` & `pymino-1.2.1.7/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/link_info.py` & `pymino-1.2.1.7/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/member.py` & `pymino-1.2.1.7/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/messages.py` & `pymino-1.2.1.7/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/notification.py` & `pymino-1.2.1.7/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/sticker.py` & `pymino-1.2.1.7/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/threads.py` & `pymino-1.2.1.7/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.7/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.7/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/handle_queue.py` & `pymino-1.2.1.7/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/socket.py` & `pymino-1.2.1.7/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.7/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.7/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/commands.py` & `pymino-1.2.1.7/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.7/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/generate.py` & `pymino-1.2.1.7/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/menu.py` & `pymino-1.2.1.7/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.7/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.7/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.6/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.7/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.6
+Version: 1.2.1.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.6/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.7/pymino.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pymino/ext/console.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
 pymino/ext/entities/acm.py
+pymino/ext/entities/admin_log.py
 pymino/ext/entities/api_response.py
 pymino/ext/entities/bubble.py
 pymino/ext/entities/chat_threads.py
 pymino/ext/entities/comments.py
 pymino/ext/entities/enums.py
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
```

### Comparing `pymino-1.2.1.6/setup.cfg` & `pymino-1.2.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e36 0d0a 6175  on = 1.2.1.6..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e37 0d0a 6175  on = 1.2.1.7..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.6/setup.py` & `pymino-1.2.1.7/setup.py`

 * *Files identical despite different names*

