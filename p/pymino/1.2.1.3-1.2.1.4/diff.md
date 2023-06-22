# Comparing `tmp/pymino-1.2.1.3.tar.gz` & `tmp/pymino-1.2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-6rf3p97j\pymino-1.2.1.3.tar", last modified: Thu Jun 22 01:22:17 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-zt51ab7a\pymino-1.2.1.4.tar", last modified: Thu Jun 22 01:28:41 2023, max compression
```

## Comparing `pymino-1.2.1.3.tar` & `pymino-1.2.1.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.400983 pymino-1.2.1.3/
--rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.3/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-06-22 01:22:17.401454 pymino-1.2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.050287 pymino-1.2.1.3/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.194622 pymino-1.2.1.3/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/account.py
--rw-rw-rw-   0        0        0   340242 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   338689 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.330030 pymino-1.2.1.3/pymino/ext/entities/
--rw-rw-rw-   0        0        0      402 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.399965 pymino-1.2.1.3/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.3/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:22:17.069629 pymino-1.2.1.3/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 01:22:16.000000 pymino-1.2.1.3/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-22 01:22:17.403437 pymino-1.2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.701355 pymino-1.2.1.4/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-06-22 01:28:41.701850 pymino-1.2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.633401 pymino-1.2.1.4/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.663658 pymino-1.2.1.4/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   340220 2023-06-22 01:27:59.000000 pymino-1.2.1.4/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   338709 2023-06-22 01:27:12.000000 pymino-1.2.1.4/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.686971 pymino-1.2.1.4/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      402 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.700362 pymino-1.2.1.4/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.4/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-22 01:28:41.645305 pymino-1.2.1.4/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-06-22 01:28:41.000000 pymino-1.2.1.4/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2023-06-22 01:28:41.000000 pymino-1.2.1.4/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 01:28:41.000000 pymino-1.2.1.4/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-22 01:28:41.000000 pymino-1.2.1.4/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 01:28:41.000000 pymino-1.2.1.4/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-22 01:28:41.703833 pymino-1.2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.4/setup.py
```

### Comparing `pymino-1.2.1.3/LICENSE` & `pymino-1.2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/PKG-INFO` & `pymino-1.2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.3
+Version: 1.2.1.4
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
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.3/README.md` & `pymino-1.2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/__init__.py` & `pymino-1.2.1.4/pymino/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/async_bot.py` & `pymino-1.2.1.4/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/bot.py` & `pymino-1.2.1.4/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/client.py` & `pymino-1.2.1.4/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/account.py` & `pymino-1.2.1.4/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/async_community.py` & `pymino-1.2.1.4/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -6671,15 +6671,16 @@
         ... print(community.total_members)
         """
         return CommunityStats(
             await self.session.handler(
                 method = "GET",
                 url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
         ))
-    
+
+
     @community
     async def edit_blog(self, blogId: str,
                   title: str = None,
                   content: str = None,
                   imageList: list = None,
                   categoriesList: list = None,
                   backgroundColor: str = None,
@@ -6750,15 +6751,16 @@
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
         
         return CBlog(await self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/blog/{blogId}",
             data = data
         ))
-    
+
+
     @community
     async def delete_notification(self, notificationId: str, comId: str = None) -> ApiResponse:
         """
         Deletes a notification.
 
         :param notificationId: The ID of the notification to delete.
         :type notificationId: str
@@ -6784,15 +6786,16 @@
         ... except:
         ...     print("Failed to delete notification.")
         """
         return ApiResponse(await self.session.handler(
             method = "DELETE",
             url = f"/x{comId or self.community_id}/s/notification/{notificationId}"
         ))
-    
+
+
     @community
     async def flag(self,
              reason: str,
              flagType: int,
              userId: str = None,
              blogId: str = None,
              wikiId: str = None,
@@ -6863,15 +6866,16 @@
         flagMethod = "g-flag" if asGuest else "flag"
 
         return ApiResponse(await self.session.handler(
             method = "POST",
             url = f"/x{comId}/s/{flagMethod}",
             data = data
         ))
-    
+
+
     @community
     async def promotion(self, noticeId: str, type: str = "accept", comId: str = None) -> ApiResponse:
         """
         Promotes or performs an action on a community notice.
 
         :param noticeId: The ID of the community notice to promote or perform an action on.
         :type noticeId: str
@@ -6899,15 +6903,16 @@
         ... else:
         ...     print("Failed to accept notice promotion.")
         """
         return ApiResponse(await self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/notice/{noticeId}/{type}"
         ))
-    
+
+
     @community
     async def change_vc_permission(self, chatId: str, permission: int, comId: Union[str, int]) -> ApiResponse:
         """
         Changes the voice chat permission for a chat in the community.
 
         :param chatId: The ID of the chat for which the voice chat permission will be changed.
         :type chatId: str
@@ -6943,15 +6948,16 @@
                 data = {
                     "vvChatJoinType": permission,
                     "timestamp": int(time() * 1000)
                 }
             ))
         else:
             raise ValueError("Incorrect permission type.")
-        
+
+
     @community
     async def fetch_blocked_users(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Fetches a list of blocked users in the community.
 
         :param start: The starting index of the blocked users to fetch (pagination). Default is 0.
         :type start: int, optional
@@ -6974,15 +6980,16 @@
         >>> for user in blocked_users:
         ...     print(user.username)
         """
         return UserProfileList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/block?start={start}&size={size}"
         ))
-    
+
+
     @community
     async def search_users(self, nickname: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Searches for users based on their nickname.
 
         :param nickname: The nickname to search for.
         :type nickname: str
@@ -7011,14 +7018,15 @@
         ...     print(profile.nickname)
         """
         return UserProfileList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/user-profile?type=name&q={nickname}&start={start}&size={size}"
         ))
 
+
     @community
     async def fetch_message(self, chatId: str, messageId: str, comId: Union[str, int] = None) -> Message:
         """
         Fetches a specific message from a chat thread.
 
         :param chatId: The ID of the chat thread where the message is located.
         :type chatId: str
@@ -7043,14 +7051,15 @@
         >>> print(message.text)
         """
         return Message(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/message/{messageId}"
         ))
 
+
     @community
     async def purchase(self,
                  objectId: str,
                  objectType: int,
                  aminoPlus: bool = True,
                  autoRenew: bool = False,
                  comId: Union[str, int] = None) -> ApiResponse:
@@ -7099,15 +7108,16 @@
                 "paymentContext": {
                     "discountStatus": 1 if aminoPlus else 0,
                     "discountValue": 1,
                     "isAutoRenew": autoRenew
                 }
             }
         ))
-    
+
+
     @community
     async def fetch_store_bubbles(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> BubbleList:
         """
         Fetches a list of chat bubbles from the store.
 
         :param start: The starting index of the bubbles to fetch. (Default: 0)
         :type start: int, optional
@@ -7129,14 +7139,15 @@
         ...     print(bubble)
         """
         return Bubble(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}"
         ))
 
+
     @community
     async def fetch_store_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> StickerList:
         """
         Fetches a list of stickers from the community store.
 
         :param start: The index of the first sticker to retrieve. (Default: 0)
         :type start: int, optional
@@ -7157,15 +7168,16 @@
         ... for sticker in stickers.name:
         ...     print(sticker)
         """
         return StickerList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=sticker&start={start}&size={size}"
         ))
-    
+
+
     @community
     async def fetch_community_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CommunityStickerList:
         """
         Fetches a list of community stickers.
 
         :param start: The starting index of the sticker list to fetch. (Default: 0)
         :type start: int, optional
@@ -7187,17 +7199,18 @@
         ... for sticker in stickers.name:
         ...     print(sticker)
         """
         return CommunityStickerList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/sticker-collection?type=community-shared"
         ))
-    
+
+
     @community
-    async def reorder_featured_users(self, userIds: list[str], comId: Union[str, int] = None) -> ApiResponse:
+    async def reorder_featured_users(self, userIds: List[str], comId: Union[str, int] = None) -> ApiResponse:
         """
         Reorders the featured users in the community.
 
         :param userIds: A list of user IDs representing the desired order of the featured users.
         :type userIds: list[str]
         :param comId: The ID of the community to reorder the featured users in. If not provided, the current community ID is used.
         :type comId: Union[str, int], optional
@@ -7218,15 +7231,16 @@
             method = "POST",
             url = f"/x{comId or self.community_id}/s/user-profile/featured/reorder",
             data = {
                 "uidList": userIds,
                 "timestamp": int(time() * 1000)
             }
         ))
-    
+
+
     @community
     async def add_to_favorites(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Adds a user to yout favorite users list in the community.
 
         :param userId: The ID of the user to add to the favorites list.
         :type userId: str
@@ -7246,15 +7260,16 @@
         ... print(response.status_code)
         ... print(response.json())
         """
         return ApiResponse(await self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/user-group/quick-access/{userId}"
         ))
-    
+
+
     @community
     async def fetch_admin_log(self,
                   userId: str = None,
                   blogId: str = None,
                   wikiId: str = None,
                   quizId: str = None,
                   fileId: str = None,
```

### Comparing `pymino-1.2.1.3/pymino/ext/async_context.py` & `pymino-1.2.1.4/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/async_event_handler.py` & `pymino-1.2.1.4/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/async_socket.py` & `pymino-1.2.1.4/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/community.py` & `pymino-1.2.1.4/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -6588,15 +6588,16 @@
             return CommunityStats(
                 self.session.handler(
                     method = "GET",
                     url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
             ))
         except AccessDenied as e:
             raise AccessDenied("You must be a leader to fetch community statistics.") from e
-    
+
+
     @community
     def edit_blog(self, blogId: str,
                   title: str = None,
                   content: str = None,
                   imageList: list = None,
                   categoriesList: list = None,
                   backgroundColor: str = None,
@@ -6668,14 +6669,15 @@
         
         return CBlog(self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/blog/{blogId}",
             data = data
         ))
 
+
     @community
     def delete_notification(self, notificationId: str, comId: Union[str, int]= None) -> ApiResponse:
         """
         Deletes a notification.
 
         :param notificationId: The ID of the notification to delete.
         :type notificationId: str
@@ -6701,15 +6703,16 @@
         ... except:
         ...     print("Failed to delete notification.")
         """
         return ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{comId or self.community_id}/s/notification/{notificationId}"
         ))
-    
+
+
     @community
     def flag(self,
              reason: str,
              flagType: int,
              userId: str = None,
              blogId: str = None,
              wikiId: str = None,
@@ -6780,15 +6783,16 @@
         flagMethod = "g-flag" if asGuest else "flag"
 
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{comId}/s/{flagMethod}",
             data = data
         ))
-    
+
+
     @community
     def promotion(self, noticeId: str, type: str = "accept", comId: Union[str, int]= None) -> ApiResponse:
         """
         Promotes or performs an action on a community notice.
 
         :param noticeId: The ID of the community notice to promote or perform an action on.
         :type noticeId: str
@@ -6817,14 +6821,15 @@
         ...     print("Failed to accept notice promotion.")
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/notice/{noticeId}/{type}"
         ))
 
+
     @community
     def change_vc_permission(self, chatId: str, permission: int, comId: Union[str, int]) -> ApiResponse:
         """
         Changes the voice chat permission for a chat in the community.
 
         :param chatId: The ID of the chat for which the voice chat permission will be changed.
         :type chatId: str
@@ -6860,15 +6865,16 @@
                 data = {
                     "vvChatJoinType": permission,
                     "timestamp": int(time() * 1000)
                 }
             ))
         else:
             raise ValueError("Incorrect permission type.")
-    
+
+
     @community
     def fetch_blocked_users(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Fetches a list of blocked users in the community.
 
         :param start: The starting index of the blocked users to fetch (pagination). Default is 0.
         :type start: int, optional
@@ -6892,14 +6898,15 @@
         ...     print(user.username)
         """
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/block?start={start}&size={size}"
         ))
 
+
     @community
     def search_users(self, nickname: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Searches for users based on their nickname.
 
         :param nickname: The nickname to search for.
         :type nickname: str
@@ -6928,14 +6935,15 @@
         ...     print(profile.nickname)
         """
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/user-profile?type=name&q={nickname}&start={start}&size={size}"
         ))
 
+
     @community
     def fetch_message(self, chatId: str, messageId: str, comId: Union[str, int] = None) -> Message:
         """
         Fetches a specific message from a chat thread.
 
         :param chatId: The ID of the chat thread where the message is located.
         :type chatId: str
@@ -6960,14 +6968,15 @@
         >>> print(message.text)
         """
         return Message(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/message/{messageId}"
         ))
 
+
     @community
     def purchase(self,
                  objectId: str,
                  objectType: int,
                  aminoPlus: bool = True,
                  autoRenew: bool = False,
                  comId: Union[str, int] = None) -> ApiResponse:
@@ -7016,15 +7025,16 @@
                 "paymentContext": {
                     "discountStatus": 1 if aminoPlus else 0,
                     "discountValue": 1,
                     "isAutoRenew": autoRenew
                 }
             }
         ))
-    
+
+
     @community
     def fetch_store_bubbles(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> BubbleList:
         """
         Fetches a list of chat bubbles from the store.
 
         :param start: The starting index of the bubbles to fetch. (Default: 0)
         :type start: int, optional
@@ -7046,14 +7056,15 @@
         ...     print(bubble)
         """
         return Bubble(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}"
         ))
 
+
     @community
     def fetch_store_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> StickerList:
         """
         Fetches a list of stickers from the community store.
 
         :param start: The index of the first sticker to retrieve. (Default: 0)
         :type start: int, optional
@@ -7074,15 +7085,16 @@
         ... for sticker in stickers.name:
         ...     print(sticker)
         """
         return StickerList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/store/items?sectionGroupId=sticker&start={start}&size={size}"
         ))
-    
+
+
     @community
     def fetch_community_stickers(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CommunityStickerList:
         """
         Fetches a list of community stickers.
 
         :param start: The starting index of the sticker list to fetch. (Default: 0)
         :type start: int, optional
@@ -7102,19 +7114,20 @@
 
         >>> stickers = client.community.fetch_community_stickers(start=0, size=10)
         ... for sticker in stickers.name:
         ...     print(sticker)
         """
         return CommunityStickerList(self.session.handler(
             method = "GET",
-            url = f"/x{comId or self.community_id}/s/sticker-collection?type=community-shared"
+            url = f"/x{comId or self.community_id}/s/sticker-collection?type=community-shared&start={start}&size={size}"
         ))
-    
+
+
     @community
-    def reorder_featured_users(self, userIds: list[str], comId: Union[str, int] = None) -> ApiResponse:
+    def reorder_featured_users(self, userIds: List[str], comId: Union[str, int] = None) -> ApiResponse:
         """
         Reorders the featured users in the community.
 
         :param userIds: A list of user IDs representing the desired order of the featured users.
         :type userIds: list[str]
         :param comId: The ID of the community to reorder the featured users in. If not provided, the current community ID is used.
         :type comId: Union[str, int], optional
@@ -7135,15 +7148,16 @@
             method = "POST",
             url = f"/x{comId or self.community_id}/s/user-profile/featured/reorder",
             data = {
                 "uidList": userIds,
                 "timestamp": int(time() * 1000)
             }
         ))
-    
+
+
     @community
     def add_to_favorites(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Adds a user to yout favorite users list in the community.
 
         :param userId: The ID of the user to add to the favorites list.
         :type userId: str
@@ -7163,15 +7177,16 @@
         ... print(response.status_code)
         ... print(response.json())
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{comId or self.community_id}/s/user-group/quick-access/{userId}"
         ))
-    
+
+
     @community
     def fetch_admin_log(self,
                   userId: str = None,
                   blogId: str = None,
                   wikiId: str = None,
                   quizId: str = None,
                   fileId: str = None,
```

### Comparing `pymino-1.2.1.3/pymino/ext/console.py` & `pymino-1.2.1.4/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/context.py` & `pymino-1.2.1.4/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/dispatcher.py` & `pymino-1.2.1.4/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/acm.py` & `pymino-1.2.1.4/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/api_response.py` & `pymino-1.2.1.4/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/bubble.py` & `pymino-1.2.1.4/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.4/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/comments.py` & `pymino-1.2.1.4/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/enums.py` & `pymino-1.2.1.4/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.4/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/general.py` & `pymino-1.2.1.4/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/handlers.py` & `pymino-1.2.1.4/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/link_info.py` & `pymino-1.2.1.4/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/member.py` & `pymino-1.2.1.4/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/messages.py` & `pymino-1.2.1.4/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/notification.py` & `pymino-1.2.1.4/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/sticker.py` & `pymino-1.2.1.4/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/threads.py` & `pymino-1.2.1.4/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.4/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.4/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/handle_queue.py` & `pymino-1.2.1.4/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/socket.py` & `pymino-1.2.1.4/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.4/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.4/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/commands.py` & `pymino-1.2.1.4/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.4/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/generate.py` & `pymino-1.2.1.4/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/menu.py` & `pymino-1.2.1.4/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.4/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.4/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.4/pymino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.3
+Version: 1.2.1.4
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
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.3/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.4/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.3/setup.cfg` & `pymino-1.2.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e33 0d0a 6175  on = 1.2.1.3..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e34 0d0a 6175  on = 1.2.1.4..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.3/setup.py` & `pymino-1.2.1.4/setup.py`

 * *Files identical despite different names*

