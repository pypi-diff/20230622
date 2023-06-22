# Comparing `tmp/pymino-1.2.1.2.tar.gz` & `tmp/pymino-1.2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\seb\pymino\dist\.tmp-tu_mvue0\pymino-1.2.1.2.tar", last modified: Mon Jun 19 00:58:20 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-6rf3p97j\pymino-1.2.1.3.tar", last modified: Thu Jun 22 01:22:17 2023, max compression
```

## Comparing `pymino-1.2.1.2.tar` & `pymino-1.2.1.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.176039 pymino-1.2.1.2/
--rw-rw-rw-   0        0        0     1085 2023-06-18 20:03:12.000000 pymino-1.2.1.2/LICENSE
--rw-rw-rw-   0        0        0     7426 2023-06-19 00:58:20.176535 pymino-1.2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6708 2023-06-18 20:03:12.000000 pymino-1.2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.090231 pymino-1.2.1.2/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-19 00:57:26.000000 pymino-1.2.1.2/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.131895 pymino-1.2.1.2/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/account.py
--rw-rw-rw-   0        0        0   328859 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   327444 2023-06-18 20:06:03.000000 pymino-1.2.1.2/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-18 20:06:09.000000 pymino-1.2.1.2/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.159671 pymino-1.2.1.2/pymino/ext/entities/
--rw-rw-rw-   0        0        0      402 2023-06-19 00:16:35.000000 pymino-1.2.1.2/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-19 00:57:52.000000 pymino-1.2.1.2/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-19 00:56:50.000000 pymino-1.2.1.2/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-18 20:06:18.000000 pymino-1.2.1.2/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.175047 pymino-1.2.1.2/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.109575 pymino-1.2.1.2/pymino.egg-info/
--rw-rw-rw-   0        0        0     7426 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-19 00:58:20.182983 pymino-1.2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-18 20:03:12.000000 pymino-1.2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.400983 pymino-1.2.1.3/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-06-22 01:22:17.401454 pymino-1.2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.050287 pymino-1.2.1.3/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.194622 pymino-1.2.1.3/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   340242 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   338689 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.330030 pymino-1.2.1.3/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      402 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.399965 pymino-1.2.1.3/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.069629 pymino-1.2.1.3/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-22 01:22:17.403437 pymino-1.2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.3/setup.py
```

### Comparing `pymino-1.2.1.2/LICENSE` & `pymino-1.2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/PKG-INFO` & `pymino-1.2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.2
+Version: 1.2.1.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong> WARNING </strong></h3>
+    <h3 style="color: red;"><strong>WARNING</strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.2/README.md` & `pymino-1.2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong> WARNING </strong></h3>
+    <h3 style="color: red;"><strong>WARNING</strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

### Comparing `pymino-1.2.1.2/pymino/__init__.py` & `pymino-1.2.1.3/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.1.2'
+__version__ = '1.2.1.3'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.1.2/pymino/async_bot.py` & `pymino-1.2.1.3/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/bot.py` & `pymino-1.2.1.3/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/client.py` & `pymino-1.2.1.3/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/account.py` & `pymino-1.2.1.3/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/async_community.py` & `pymino-1.2.1.3/pymino/ext/async_community.py`

 * *Files 1% similar despite different names*

```diff
@@ -4848,15 +4848,15 @@
             "title": title,
             "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
             "initialMessageContent": message,
             "content": content,
             "type": 0,
             "publishToGlobal": 0,
             "timestamp": int(time() * 1000)
-            })).status
+            }))
 
 
     @community
     async def invite_chat(self, chatId: str, userIds: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
         Invites one or more users to join a chat.
 
@@ -7098,8 +7098,248 @@
                 "timestamp": int(time() * 1000),
                 "paymentContext": {
                     "discountStatus": 1 if aminoPlus else 0,
                     "discountValue": 1,
                     "isAutoRenew": autoRenew
                 }
             }
-        ))
+        ))
+    
+    @community
+    async def fetch_store_bubbles(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> BubbleList:
+        """
+        Fetches a list of chat bubbles from the store.
+
+        :param start: The starting index of the bubbles to fetch. (Default: 0)
+        :type start: int, optional
+        :param size: The number of bubbles to fetch. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch the bubbles from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `BubbleList` object containing the fetched chat bubbles.
+        :rtype: BubbleList
+
+        This function sends a GET request to the API to fetch a list of chat bubbles from the store.
+
+        `BubbleList` represents a list of chat bubbles.
+
+        **Example usage:**
+
+        >>> bubbles = client.community.fetch_store_bubbles(start=0, size=10)
+        ... for bubble in bubbles.name:
+        ...     print(bubble)
+        """
+        return Bubble(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}"
+        ))
+
+    @community
+    async def fetch_store_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> StickerList:
+        """
+        Fetches a list of stickers from the community store.
+
+        :param start: The index of the first sticker to retrieve. (Default: 0)
+        :type start: int, optional
+        :param size: The number of stickers to retrieve. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch stickers from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `StickerList` object containing the fetched stickers.
+        :rtype: StickerList
+
+        This function sends a GET request to the API to fetch a list of stickers from the community store.
+
+        `StickerList` represents a list of stickers in the community store.
+
+        **Example usage:**
+
+        >>> stickers = client.community.fetch_store_stickers(start=0, size=10)
+        ... for sticker in stickers.name:
+        ...     print(sticker)
+        """
+        return StickerList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=sticker&start={start}&size={size}"
+        ))
+    
+    @community
+    async def fetch_community_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CommunityStickerList:
+        """
+        Fetches a list of community stickers.
+
+        :param start: The starting index of the sticker list to fetch. (Default: 0)
+        :type start: int, optional
+        :param size: The number of stickers to fetch. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch stickers from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityStickerList` object containing the fetched community stickers.
+        :rtype: CommunityStickerList
+
+        This function sends a GET request to the API to fetch a list of community stickers. The fetched stickers are returned
+        as a `CommunityStickerList` object.
+
+        `CommunityStickerList` represents a list of community stickers.
+
+        **Example usage:**
+
+        >>> stickers = client.community.fetch_community_stickers(start=0, size=10)
+        ... for sticker in stickers.name:
+        ...     print(sticker)
+        """
+        return CommunityStickerList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/sticker-collection?type=community-shared"
+        ))
+    
+    @community
+    async def reorder_featured_users(self, userIds: list[str], comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Reorders the featured users in the community.
+
+        :param userIds: A list of user IDs representing the desired order of the featured users.
+        :type userIds: list[str]
+        :param comId: The ID of the community to reorder the featured users in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the result of the reorder operation.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to reorder the featured users in the specified community.
+
+        `ApiResponse` represents the response received from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.reorder_featured_users(["user1", "user2", "user3"])
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/user-profile/featured/reorder",
+            data = {
+                "uidList": userIds,
+                "timestamp": int(time() * 1000)
+            }
+        ))
+    
+    @community
+    async def add_to_favorites(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Adds a user to yout favorite users list in the community.
+
+        :param userId: The ID of the user to add to the favorites list.
+        :type userId: str
+        :param comId: The ID of the community to add the user to the favorites list in.
+                    If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the response of the API request.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to add a user to your favorite users in the community.
+
+        `ApiResponse` represents the response from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.add_to_favorites("123456789")
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/user-group/quick-access/{userId}"
+        ))
+    
+    @community
+    async def fetch_admin_log(self,
+                  userId: str = None,
+                  blogId: str = None,
+                  wikiId: str = None,
+                  quizId: str = None,
+                  fileId: str = None,
+                  pageToken: str = None,
+                  size: int = 25,
+                  comId: Union[str, int] = None):
+        """
+        Fetches the admin log entries for the specified parameters.
+
+        :param userId: The ID of the user to filter the admin log by. (Optional)
+        :type userId: str, optional
+        :param blogId: The ID of the blog to filter the admin log by. (Optional)
+        :type blogId: str, optional
+        :param wikiId: The ID of the wiki to filter the admin log by. (Optional)
+        :type wikiId: str, optional
+        :param quizId: The ID of the quiz to filter the admin log by. (Optional)
+        :type quizId: str, optional
+        :param fileId: The ID of the file to filter the admin log by. (Optional)
+        :type fileId: str, optional
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
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
+        >>> admin_log = client.community.fetch_admin_log(userId="12345")
+        ... for entry in admin_log:
+        ...     print(entry.action)
+        ...     print(entry.timestamp)
+        """
+        if pageToken is None:
+            if userId: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}"
+            )
+            elif blogId: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}"
+            )
+            elif wikiId: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}"
+            )
+            elif quizId: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}"
+            )
+            elif fileId: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}"
+            )
+            else: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}"
+            )
+        elif userId: return await self.session.handler(
+                method = "GET",
+                url =  f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}&pageToken={pageToken}"
+            )
+        elif blogId: return await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif wikiId: return await self.session.hadler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif quizId: return await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif fileId: return await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        else: return await self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}&pageToken={pageToken}"
+            )
```

### Comparing `pymino-1.2.1.2/pymino/ext/async_context.py` & `pymino-1.2.1.3/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/async_event_handler.py` & `pymino-1.2.1.3/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/async_socket.py` & `pymino-1.2.1.3/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/community.py` & `pymino-1.2.1.3/pymino/ext/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -4769,15 +4769,15 @@
             "title": title,
             "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
             "initialMessageContent": message,
             "content": content,
             "type": 0,
             "publishToGlobal": 0,
             "timestamp": int(time() * 1000)
-            })).status
+            }))
 
 
     @community
     def invite_chat(self, chatId: str, userIds: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
         Invites one or more users to join a chat.
 
@@ -7015,8 +7015,248 @@
                 "timestamp": int(time() * 1000),
                 "paymentContext": {
                     "discountStatus": 1 if aminoPlus else 0,
                     "discountValue": 1,
                     "isAutoRenew": autoRenew
                 }
             }
-        ))
+        ))
+    
+    @community
+    def fetch_store_bubbles(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> BubbleList:
+        """
+        Fetches a list of chat bubbles from the store.
+
+        :param start: The starting index of the bubbles to fetch. (Default: 0)
+        :type start: int, optional
+        :param size: The number of bubbles to fetch. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch the bubbles from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `BubbleList` object containing the fetched chat bubbles.
+        :rtype: BubbleList
+
+        This function sends a GET request to the API to fetch a list of chat bubbles from the store.
+
+        `BubbleList` represents a list of chat bubbles.
+
+        **Example usage:**
+
+        >>> bubbles = client.community.fetch_store_bubbles(start=0, size=10)
+        ... for bubble in bubbles.name:
+        ...     print(bubble)
+        """
+        return Bubble(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}"
+        ))
+
+    @community
+    def fetch_store_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> StickerList:
+        """
+        Fetches a list of stickers from the community store.
+
+        :param start: The index of the first sticker to retrieve. (Default: 0)
+        :type start: int, optional
+        :param size: The number of stickers to retrieve. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch stickers from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `StickerList` object containing the fetched stickers.
+        :rtype: StickerList
+
+        This function sends a GET request to the API to fetch a list of stickers from the community store.
+
+        `StickerList` represents a list of stickers in the community store.
+
+        **Example usage:**
+
+        >>> stickers = client.community.fetch_store_stickers(start=0, size=10)
+        ... for sticker in stickers.name:
+        ...     print(sticker)
+        """
+        return StickerList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=sticker&start={start}&size={size}"
+        ))
+    
+    @community
+    def fetch_community_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CommunityStickerList:
+        """
+        Fetches a list of community stickers.
+
+        :param start: The starting index of the sticker list to fetch. (Default: 0)
+        :type start: int, optional
+        :param size: The number of stickers to fetch. (Default: 25)
+        :type size: int, optional
+        :param comId: The ID of the community to fetch stickers from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityStickerList` object containing the fetched community stickers.
+        :rtype: CommunityStickerList
+
+        This function sends a GET request to the API to fetch a list of community stickers. The fetched stickers are returned
+        as a `CommunityStickerList` object.
+
+        `CommunityStickerList` represents a list of community stickers.
+
+        **Example usage:**
+
+        >>> stickers = client.community.fetch_community_stickers(start=0, size=10)
+        ... for sticker in stickers.name:
+        ...     print(sticker)
+        """
+        return CommunityStickerList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/sticker-collection?type=community-shared"
+        ))
+    
+    @community
+    def reorder_featured_users(self, userIds: list[str], comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Reorders the featured users in the community.
+
+        :param userIds: A list of user IDs representing the desired order of the featured users.
+        :type userIds: list[str]
+        :param comId: The ID of the community to reorder the featured users in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the result of the reorder operation.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to reorder the featured users in the specified community.
+
+        `ApiResponse` represents the response received from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.reorder_featured_users(["user1", "user2", "user3"])
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/user-profile/featured/reorder",
+            data = {
+                "uidList": userIds,
+                "timestamp": int(time() * 1000)
+            }
+        ))
+    
+    @community
+    def add_to_favorites(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Adds a user to yout favorite users list in the community.
+
+        :param userId: The ID of the user to add to the favorites list.
+        :type userId: str
+        :param comId: The ID of the community to add the user to the favorites list in.
+                    If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the response of the API request.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to add a user to your favorite users in the community.
+
+        `ApiResponse` represents the response from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.add_to_favorites("123456789")
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/user-group/quick-access/{userId}"
+        ))
+    
+    @community
+    def fetch_admin_log(self,
+                  userId: str = None,
+                  blogId: str = None,
+                  wikiId: str = None,
+                  quizId: str = None,
+                  fileId: str = None,
+                  pageToken: str = None,
+                  size: int = 25,
+                  comId: Union[str, int] = None):
+        """
+        Fetches the admin log entries for the specified parameters.
+
+        :param userId: The ID of the user to filter the admin log by. (Optional)
+        :type userId: str, optional
+        :param blogId: The ID of the blog to filter the admin log by. (Optional)
+        :type blogId: str, optional
+        :param wikiId: The ID of the wiki to filter the admin log by. (Optional)
+        :type wikiId: str, optional
+        :param quizId: The ID of the quiz to filter the admin log by. (Optional)
+        :type quizId: str, optional
+        :param fileId: The ID of the file to filter the admin log by. (Optional)
+        :type fileId: str, optional
+        :param pageToken: The token for pagination. (Optional)
+        :type pageToken: str, optional
+        :param size: The number of log entries to fetch per page. (Default: 25)
+        :type size: int, optional
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
+        >>> admin_log = client.community.fetch_admin_log(userId="12345")
+        ... for entry in admin_log:
+        ...     print(entry.action)
+        ...     print(entry.timestamp)
+        """
+        if pageToken is None:
+            if userId: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}"
+            )
+            elif blogId: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}"
+            )
+            elif wikiId: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}"
+            )
+            elif quizId: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}"
+            )
+            elif fileId: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}"
+            )
+            else: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}"
+            )
+        elif userId: return self.session.handler(
+                method = "GET",
+                url =  f"/x{comId or self.community_id}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}&pageToken={pageToken}"
+            )
+        elif blogId: return self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif wikiId: return self.session.hadler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif quizId: return self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        elif fileId: return self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}&pageToken={pageToken}"
+        )
+        else: return self.session.handler(
+                method = "GET",
+                url = f"/x{comId or self.community_id}/s/admin/operation?pagingType=t&size={size}&pageToken={pageToken}"
+            )
```

### Comparing `pymino-1.2.1.2/pymino/ext/console.py` & `pymino-1.2.1.3/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/context.py` & `pymino-1.2.1.3/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/dispatcher.py` & `pymino-1.2.1.3/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/acm.py` & `pymino-1.2.1.3/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/api_response.py` & `pymino-1.2.1.3/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/bubble.py` & `pymino-1.2.1.3/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.3/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/comments.py` & `pymino-1.2.1.3/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/enums.py` & `pymino-1.2.1.3/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.3/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/general.py` & `pymino-1.2.1.3/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/handlers.py` & `pymino-1.2.1.3/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/link_info.py` & `pymino-1.2.1.3/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/member.py` & `pymino-1.2.1.3/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/messages.py` & `pymino-1.2.1.3/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/notification.py` & `pymino-1.2.1.3/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/sticker.py` & `pymino-1.2.1.3/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/threads.py` & `pymino-1.2.1.3/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.3/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.3/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/handle_queue.py` & `pymino-1.2.1.3/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/socket.py` & `pymino-1.2.1.3/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.3/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.3/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/commands.py` & `pymino-1.2.1.3/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.3/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/generate.py` & `pymino-1.2.1.3/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/menu.py` & `pymino-1.2.1.3/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.3/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.3/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.3/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.2
+Version: 1.2.1.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong> WARNING </strong></h3>
+    <h3 style="color: red;"><strong>WARNING</strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.2/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.3/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.2/setup.cfg` & `pymino-1.2.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e32 0d0a 6175  on = 1.2.1.2..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e33 0d0a 6175  on = 1.2.1.3..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.2/setup.py` & `pymino-1.2.1.3/setup.py`

 * *Files identical despite different names*

