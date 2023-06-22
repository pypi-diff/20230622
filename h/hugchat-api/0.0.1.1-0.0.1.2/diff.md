# Comparing `tmp/hugchat_api-0.0.1.1.tar.gz` & `tmp/hugchat_api-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat_api-0.0.1.1.tar", last modified: Wed Jun 21 16:35:16 2023, max compression
+gzip compressed data, was "hugchat_api-0.0.1.2.tar", last modified: Thu Jun 22 16:48:40 2023, max compression
```

## Comparing `hugchat_api-0.0.1.1.tar` & `hugchat_api-0.0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 16:35:16.916566 hugchat_api-0.0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5490 2023-06-21 16:35:16.916566 hugchat_api-0.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4620 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 16:35:16.902574 hugchat_api-0.0.1.1/hugchat_api/
--rw-rw-rw-   0        0        0      280 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:35:16.914566 hugchat_api-0.0.1.1/hugchat_api/core/
--rw-rw-rw-   0        0        0    12943 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/Bot.py
--rw-rw-rw-   0        0        0     1344 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/Message.py
--rw-rw-rw-   0        0        0     6507 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/Sign.py
--rw-rw-rw-   0        0        0     1278 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/ThreadPool.py
--rw-rw-rw-   0        0        0     4078 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/WebSearch.py
--rw-rw-rw-   0        0        0      758 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/core/__init__.py
--rw-rw-rw-   0        0        0     6400 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/terminal_cli.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:35:16.915568 hugchat_api-0.0.1.1/hugchat_api/utils/
--rw-rw-rw-   0        0        0     1420 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/hugchat_api/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:35:16.907586 hugchat_api-0.0.1.1/hugchat_api.egg-info/
--rw-rw-rw-   0        0        0     5490 2023-06-21 16:35:16.000000 hugchat_api-0.0.1.1/hugchat_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-06-21 16:35:16.000000 hugchat_api-0.0.1.1/hugchat_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 16:35:16.000000 hugchat_api-0.0.1.1/hugchat_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-21 16:35:16.000000 hugchat_api-0.0.1.1/hugchat_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 16:35:16.000000 hugchat_api-0.0.1.1/hugchat_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 16:35:16.917575 hugchat_api-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1227 2023-06-21 16:34:48.000000 hugchat_api-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.171840 hugchat_api-0.0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6097 2023-06-22 16:48:40.170840 hugchat_api-0.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5229 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.151840 hugchat_api-0.0.1.2/hugchat_api/
+-rw-rw-rw-   0        0        0      283 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.168841 hugchat_api-0.0.1.2/hugchat_api/core/
+-rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Bot.py
+-rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Exceptions.py
+-rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Message.py
+-rw-rw-rw-   0        0        0     6507 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Sign.py
+-rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/ThreadPool.py
+-rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/WebSearch.py
+-rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/__init__.py
+-rw-rw-rw-   0        0        0     6829 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/terminal_cli.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.169840 hugchat_api-0.0.1.2/hugchat_api/utils/
+-rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.157840 hugchat_api-0.0.1.2/hugchat_api.egg-info/
+-rw-rw-rw-   0        0        0     6097 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-06-22 16:48:40.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 16:48:40.171840 hugchat_api-0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1227 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/setup.py
```

### Comparing `hugchat_api-0.0.1.1/LICENSE` & `hugchat_api-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.1/PKG-INFO` & `hugchat_api-0.0.1.2/hugchat_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hugchat_api
-Version: 0.0.1.1
+Name: hugchat-api
+Version: 0.0.1.2
 Summary: Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: curl
 License-File: LICENSE
 
 # Huggingchat api
-> I will be glad if this works perfectly and you also like it. I did as much as possible to make it works perfectly on my machine.
 
+**Leave a star and you could win a billion(**
+
+> This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
+
+[![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+
+[![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
+
+```shell
+pip install hugchat-api
+```
 
 ## Sign in
 Here's a example of how to log into huggingface and get cookies
 ```python
 import os
 from hugchat_api import HuggingChat
 
@@ -56,43 +67,46 @@
 - Create Bot
 ```python
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 ```
 - Get all chat histories by conversation_id
 ```python
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 ```
 - Delete a conversation
 ```python
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 ```
 - Create a new conversation
 ```python
 conversation_id = bot.createConversation()
 ```
 - Chat
 ```python
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 **Code:**
@@ -113,34 +127,37 @@
 sign = HUG.getSign(EMAIL, PASSWD)   
 # sign in or...
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
 # create bot
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 # get all conversations and see one's title
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 # get all chat histories by conversation_id
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 # delete a conversation
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 # create a new conversation
 conversation_id = bot.createConversation()
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
@@ -180,21 +197,18 @@
 | web        | Switch 'Search Web' enable option      |
 
 Anything not start with `/` will be seen as chat message.
 
 Example:
 ```text
 (None) > /ls
-#* Conversations that have been established:
-#
-#        0. Assistant: "It's February 24th."
-#        1. Today is Wednesday, July 12th, 2034
-#        2. "What is today's date?"
-#        3. "April 2nd."
+#* Conversations established:
 #
+#       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
+#       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
 #(Open-Assistant): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
```

### Comparing `hugchat_api-0.0.1.1/README.md` & `hugchat_api-0.0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,42 @@
+Metadata-Version: 2.1
+Name: hugchat_api
+Version: 0.0.1.2
+Summary: Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.
+Home-page: https://github.com/ogios/huggingchat-api
+Author: ogios
+Author-email: 2134692955@qq.com
+License: GNU General Public License v3.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: curl
+License-File: LICENSE
+
 # Huggingchat api
-> I will be glad if this works perfectly and you also like it. I did as much as possible to make it works perfectly on my machine.
 
+**Leave a star and you could win a billion(**
+
+> This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
+
+[![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+
+[![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
+
+```shell
+pip install hugchat-api
+```
 
 ## Sign in
 Here's a example of how to log into huggingface and get cookies
 ```python
 import os
 from hugchat_api import HuggingChat
 
@@ -35,43 +67,46 @@
 - Create Bot
 ```python
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 ```
 - Get all chat histories by conversation_id
 ```python
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 ```
 - Delete a conversation
 ```python
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 ```
 - Create a new conversation
 ```python
 conversation_id = bot.createConversation()
 ```
 - Chat
 ```python
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 **Code:**
@@ -92,34 +127,37 @@
 sign = HUG.getSign(EMAIL, PASSWD)   
 # sign in or...
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
 # create bot
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 # get all conversations and see one's title
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 # get all chat histories by conversation_id
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 # delete a conversation
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 # create a new conversation
 conversation_id = bot.createConversation()
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
@@ -159,27 +197,24 @@
 | web        | Switch 'Search Web' enable option      |
 
 Anything not start with `/` will be seen as chat message.
 
 Example:
 ```text
 (None) > /ls
-#* Conversations that have been established:
-#
-#        0. Assistant: "It's February 24th."
-#        1. Today is Wednesday, July 12th, 2034
-#        2. "What is today's date?"
-#        3. "April 2nd."
+#* Conversations established:
 #
+#       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
+#       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
 #(Open-Assistant): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
 #(Open-Assistant): ...
 ```
 
-</details>
+</details>
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/Bot.py` & `hugchat_api-0.0.1.2/hugchat_api/core/Bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import re
 from typing import Callable, Tuple
 
 from .WebSearch import WebSearch
 from .Message import Message
 from .ThreadPool import ThreadPool
 from ..utils import getTime
+from .Exceptions import *
 
 
 class Bot:
     def __init__(
             self,
             email: str,
             cookies: requests.sessions.RequestsCookieJar,
@@ -42,33 +43,36 @@
         self.url_initConversation = "https://huggingface.co/chat/conversation"
         self.headers = {
             "Referer": "https://huggingface.co/chat",
             "Content-Type": "application/json",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
         }
         self.cookies = cookies
-        self.conversations = list()
+        # self.conversations = list()
+        self.conversations = dict()
         self.current_conversation = None
         self.fetchConversations()
     
     def fetchConversations(self):
         """
         Get conversation a from a html and extract them using re
         """
-        self.conversations = []
+        logging.info("Fetching all conversations...")
+        self.conversations = dict()
         res = self._requestsGet(self.url_index)
         html = res.text
         conversation_ids = list(set(re.findall('href="/chat/conversation/(.*?)"', html)))
         for i in conversation_ids:
             title = re.findall(f'href="/chat/conversation/{i}.*?<div class="flex-1 truncate">(.*?)</div>', html, re.S)
             if len(title) > 0:
                 title = title[0].strip()
             else:
                 title = "Untitled conversation"
-            self.conversations.append({"id": i, "title": title})
+            self.conversations[i] = title
+            # self.conversations.append({"id": i, "title": title})
     
     def _requestsGet(self, url: str, params=None, stream=False) -> requests.Response:
         """
         GET
         """
         res = requests.get(
             url,
@@ -207,14 +211,16 @@
         for i in range(max_tries):
             res = self._requestsPost(url, stream=True, data=json.dumps(data))
             if res.status_code == 500:
                 logging.error("Internal error, may due to model overload, retrying...")
             else:
                 exp = self._parseData(res, message=message)
                 if not exp:
+                    if not self.conversations[conversation_id]:
+                        self.updateTitle(conversation_id)
                     if callback != None:
                         callback[0](*callback[-1])
                     return
             time.sleep(1)
             continue
         message.setError(exp)
     
@@ -256,60 +262,61 @@
             self.thread_pool.submit(self._getReply, (conversation_id, text, message, "", max_tries, callback))
         return message
     
     def updateTitle(self, conversation_id) -> str:
         """
         Get conversation summary
         """
+        if not self.conversations.__contains__(conversation_id):
+            raise ConversationNotExistError(f"The given conversation is not in the map: {conversation_id}")
         url = self.url_initConversation + f"/{conversation_id}/summarize"
         res = self._requestsPost(url)
         if res.status_code != 200:
             raise Exception("get conversation title failed")
         js = res.json()
-        for i in range(len(self.conversations)):
-            if self.conversations[i]["id"] == conversation_id:
-                self.conversations[i]["title"] = js["title"]
-                break
+        self.conversations[conversation_id] = js["title"]
+        # for i in range(len(self.conversations)):
+        #     if self.conversations[i]["id"] == conversation_id:
+        #         self.conversations[i]["title"] = js["title"]
+        #         break
         return js["title"]
     
     def createConversation(self) -> str:
         """
         start a new conversation
         """
         data = {"model": self.model}
         res = self._requestsPost(self.url_initConversation, data=json.dumps(data))
         if res.status_code != 200:
             raise Exception("create conversation fatal")
         js = res.json()
         conversation_id = js["conversationId"]
         # message = self.chat(text, conversation_id, web=web)
-        conversation = {"id": conversation_id, "title": "None"}
-        self.conversations.append(conversation)
+        self.conversations[conversation_id] = None
+        # conversation = {"id": conversation_id, "title": "None"}
+        # self.conversations.append(conversation)
         self.current_conversation = conversation_id
         return conversation_id
     
-    def removeConversation(self, index: int):
+    def removeConversation(self, conversation_id: str):
         """
         Remove conversation through the index of self.conversations
         """
-        if not 0 <= index <= len(self.conversations) - 1:
-            logging.info("Index out of bounds")
-            return
-        conversation_id = self.conversations[index]["id"]
+        if not self.conversations.__contains__(conversation_id):
+            raise ConversationNotExistError(f"The given conversation is not in the map: {conversation_id}")
         logging.info(f"Deleting conversation <{conversation_id}>")
         url = self.url_initConversation + f"/{conversation_id}"
         res = requests.delete(url, headers=self.headers, cookies=self.cookies)
         if res.status_code != 200:
             logging.info(f"{res.text}")
             logging.info("Delete conversation fatal")
-            return
-        del self.conversations[index]
+            raise Exception("Delete conversation fatal")
+        del self.conversations[conversation_id]
         if self.current_conversation == conversation_id:
             self.current_conversation = None
-        return 1
     
     def _getHistoriesByID(self, conversation_id):
         """
         :return: [{
             "conversation_id"
             "is_user"
             "text"
@@ -334,28 +341,29 @@
                             "conversation_id": conversation_id,
                             "is_user": 1 if history[his["from"]] == "user" else 0,
                             "text": history[his["content"]],
                             "text_id": history[his["id"]],
                         })
         return histories
     
-    def getHistoriesByID(self, conversation_id=None):
+    def getHistoriesByID(self, conversation_id=None) -> list:
         conversation_id = self.current_conversation if not conversation_id else conversation_id
         if not conversation_id:
             return []
         logging.info(f"Getting histories for {self.email}:{conversation_id}...")
         histories = self._getHistoriesByID(conversation_id)
         if histories == None:
             raise Exception("Something went wrong")
         else:
-            
             return histories
     
-    def getConversations(self):
+    def getConversations(self) -> dict:
         return self.conversations
     
-    def switchConversation(self, option: int):
-        self.current_conversation = self.conversations[option]["id"]
+    def switchConversation(self, conversation_id: str):
+        if not self.conversations.__contains__(conversation_id):
+            raise ConversationNotExistError(f"The given conversation is not in the map: {conversation_id}")
+        self.current_conversation = conversation_id
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/Message.py` & `hugchat_api-0.0.1.2/hugchat_api/core/Message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+import logging
+
+
 class Message:
     def __init__(self, conversation_id: str, web_search_enabled: bool):
+        self.done: bool = False
         self.stream_text: list = []
         self.final_text: str = None
-        self.web_search_steps = None
-        self.done: bool = False
         self.web_search_enabled = web_search_enabled
+        self.web_search_done = False
+        self.web_search_steps = list()
         self.error: Exception = None
         self.conversation_id: str = conversation_id
     
     def getConversation(self) -> str:
         return self.conversation_id
     
     def setError(self, error: Exception):
         self.error = error
         
     def setWebSearchSteps(self, process):
         self.web_search_steps = process
     
+    # def setWebSearchSteps(self, process):
+    #     logging.info(f"updating websearch: {process}")
+    #     self.web_search_steps.append(process)
+    
     def getWebSearchSteps(self):
         if self.error:
             raise self.error
         return self.web_search_steps
     
     def setText(self, text, done: bool = False):
+        if not self.web_search_done:
+            self.web_search_done = True
         self.stream_text.append(text)
         if done:
             self.done = True
     
     def getText(self) -> list:
         if self.error:
             raise Exception(self.error)
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/Sign.py` & `hugchat_api-0.0.1.2/hugchat_api/core/Sign.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/ThreadPool.py` & `hugchat_api-0.0.1.2/hugchat_api/core/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/WebSearch.py` & `hugchat_api-0.0.1.2/hugchat_api/core/WebSearch.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,20 +35,23 @@
 							js = json.loads(chunk)
 							self.message.setWebSearchSteps(js)
 						except:
 							logging.info(f"load fatal: {chunk}")
 							continue
 						try:
 							if js["messages"][-1]["type"] == "result":
+								# self.message.setWebSearchSteps(js["messages"][-1])
+								self.message.web_search_done = True
 								return js
-							elif len(js["messages"]) - 1 > index:
-								if index == -1:
-									index = 0
-								for message in js["messages"][index+1:]:
-									index += 1
+							# elif len(js["messages"]) - 1 > index:
+							# 	if index == -1:
+							# 		index = 0
+							# 	for message in js["messages"][index+1:]:
+							# 		self.message.setWebSearchSteps(message)
+							# 		index += 1
 						except:
 							pass
 		except Exception as e:
 			logging.error(str(e))
 			traceback.format_exc()
 		res.close()
 		return
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api/core/__init__.py` & `hugchat_api-0.0.1.2/hugchat_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.1/hugchat_api/terminal_cli.py` & `hugchat_api-0.0.1.2/hugchat_api/terminal_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import gc, os, argparse, time
 import getpass
 import logging
 import traceback
-from rich.console import Console
-from rich.markdown import Markdown
+# from rich.console import Console
+# from rich.markdown import Markdown
 
 from .core import HuggingChat
 from .core.Message import Message
 from .core.Sign import Sign
 from .core.Bot import Bot
-from .utils import color, formatHistory, formatConversations, getTextFromInput
+from .utils import color, formatHistory, formatConversations, getTextFromInput, getIdByIndex
 
 COOKIE_DIR_PATH = os.path.abspath(os.path.dirname(__file__)) + "/usercookies"
-CONSOLE = Console()
+# CONSOLE = Console()
 hug = HuggingChat()
 
 # FLAG = False
 WEB_SEARCH = False
 NEW_CONVERSATION = False
 
 logging.getLogger().setLevel(logging.INFO)
@@ -54,26 +54,36 @@
         if message.error:
             logging.error(str(message.error))
             return
         time.sleep(0.5)
         
     msg = message.getFinalText()
     string = f"({color('Open-Assistant', 'blue')}): {msg}"
-    try:
-        markdown = Markdown(string)
-        CONSOLE.print(markdown)
-    except:
-        print(string)
+    print(string)
+    # try:
+    #     markdown = Markdown(string)
+    #     CONSOLE.print(markdown)
+    # except:
+    #     print(string)
 
 
 def updateWebSearch(message: Message):
     if not message.web_search_enabled:
         return
-    message.getWebSearchSteps()
-    pass
+    # length = 0
+    while not message.web_search_done:
+        # c = message.getWebSearchSteps()
+        # if len(c) > length:
+        #     for i in c[length-1:]:
+        #         print(i)
+        #         length += 1
+        time.sleep(0.5)
+    # print("======")
+    # print("======")
+    print(message.web_search_steps)
     # if js["type"] == "web_search" and js.__contains__("data"):
     #     data: dict = js["data"]
     #     if data["type"] == "update" and data.__contains__("message"):
     #         string = f"* {data['message']}{' - ' + str(data['args']) if data.__contains__('args') else ''}"
     #         print(string)
     #     elif data["type"] == "result":
     #         print(f"* result - {data['id']}")
@@ -119,73 +129,76 @@
     elif not checkCookies(u):
         p = getpass.getpass() if not PASSWD else PASSWD
     else:
         p = None
     
     cookies = login(u, p, force)
     print(f"You are now logged in as <{u}>")
-    openassistant: Bot = hug.getBot(u, cookies=cookies)
+    bot: Bot = hug.getBot(u, cookies=cookies)
     gc.collect()
     while 1:
         try:
             gc.collect()
             # while FLAG:
             #     time.sleep(0.1)
             #     continue
-            text = getTextFromInput(openassistant.current_conversation)
+            text = getTextFromInput(bot.current_conversation)
             command = text.strip()
             if command[0] == "/":
                 command = command[1:].split(" ")
                 if command[0] == "exit" or command[0] == "q":
                     os._exit(0)
                 elif command[0] == "new":
-                    openassistant.createConversation()
+                    bot.createConversation()
                     NEW_CONVERSATION = True
                 elif command[0] == "ls":
-                    print(formatConversations(openassistant.getConversations()))
+                    print(formatConversations(bot.getConversations()))
                 elif command[0] == "cd":
                     try:
-                        openassistant.switchConversation(int(command[1]))
+                        tmp_id = getIdByIndex(bot.conversations, int(command[1]))
+                        bot.switchConversation(tmp_id)
                     except:
                         print("cd fatal")
                 elif command[0] == "rm":
                     try:
-                        openassistant.removeConversation(int(command[1]))
+                        tmp_id = getIdByIndex(bot.conversations, int(command[1]))
+                        bot.removeConversation(tmp_id)
                     except Exception as e:
                         
                         print(f"remove conversation fatal: {e}")
                 elif command[0] == "old":
-                    print(formatHistory(openassistant.getHistoriesByID()))
+                    print(formatHistory(bot.getHistoriesByID()))
                 elif command[0] == "web":
                     changeWeb_search()
                 elif command[0] == "reload":
                     print("Reloading conversations...")
-                    openassistant.fetchConversations()
-                    for i in openassistant.conversations:
-                        openassistant.updateTitle(i['id'])
+                    bot.fetchConversations()
+                    for i in bot.conversations:
+                        bot.updateTitle(i['id'])
                     print("done.")
-                    print(formatConversations(openassistant.getConversations()))
+                    print(formatConversations(bot.getConversations()))
                 else:
                     print("wrong command。")
                     continue
             else:
-                if not openassistant.current_conversation:
+                if not bot.current_conversation:
                     print(
                         "Please select or create a conversation using '/ls' and '/cd <int>' or '/new'.")
                     continue
                 
-                message = openassistant.chat(
+                message = bot.chat(
                     text,
-                    web=WEB_SEARCH,
-                    callback=(openassistant.updateTitle, (openassistant.current_conversation,)) if NEW_CONVERSATION else None
+                    conversation_id=bot.current_conversation,
+                    web_search=WEB_SEARCH,
+                    # callback=(bot.updateTitle, (bot.current_conversation,)) if NEW_CONVERSATION else None
                 )
                 updateWebSearch(message)
                 updateMSG(message)
                 # FLAG = True
         except Exception as e:
             traceback.print_exc()
 
 
 if __name__ == "__main__":
-    EMAIL = ""
+    EMAIL = os.getenv("EMAIL")
     PASSWD = ""
     main(EMAIL, PASSWD)
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api/utils/__init__.py` & `hugchat_api-0.0.1.2/hugchat_api/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,21 +34,29 @@
 def getTextFromInput(conversation_id, addition: str = ""):
     while 1:
         text = input(f"{addition}({conversation_id}) > ")
         if not text:
             continue
         else:
             return text
-        
 
-def formatConversations(conversations: List[dict]):
+
+def formatConversations(conversations: dict):
     string = "* Conversations established:\n\n"
-    for i in range(len(conversations)):
-        string += f"	{i}. {conversations[i]['title']}\n"
+    # for i in conversations:
+    #     string += f"	{i}. {conversations[i]}\n"
+    cons = tuple(conversations.items())
+    for i in range(len(cons)):
+        string += f"	{i}. [{cons[i][0]}] - {cons[i][-1]}\n"
     # string += "\n"
     return string
 
 
 def getTime():
     return str(datetime.datetime.now())
 
 
+def getIdByIndex(conversations: dict, index: int) -> str:
+    cons = list(conversations.keys())
+    if 0 <= index <= len(cons):
+        return cons[index]
+    raise Exception("Index out of bounds")
```

### Comparing `hugchat_api-0.0.1.1/hugchat_api.egg-info/PKG-INFO` & `hugchat_api-0.0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1
-Name: hugchat-api
-Version: 0.0.1.1
-Summary: Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.
-Home-page: https://github.com/ogios/huggingchat-api
-Author: ogios
-Author-email: 2134692955@qq.com
-License: GNU General Public License v3.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: curl
-License-File: LICENSE
-
 # Huggingchat api
-> I will be glad if this works perfectly and you also like it. I did as much as possible to make it works perfectly on my machine.
 
+**Leave a star and you could win a billion(**
+
+> This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
+
+[![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
+
+[![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
+
+```shell
+pip install hugchat-api
+```
 
 ## Sign in
 Here's a example of how to log into huggingface and get cookies
 ```python
 import os
 from hugchat_api import HuggingChat
 
@@ -56,43 +46,46 @@
 - Create Bot
 ```python
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 ```
 - Get all chat histories by conversation_id
 ```python
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 ```
 - Delete a conversation
 ```python
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 ```
 - Create a new conversation
 ```python
 conversation_id = bot.createConversation()
 ```
 - Chat
 ```python
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 **Code:**
@@ -113,34 +106,37 @@
 sign = HUG.getSign(EMAIL, PASSWD)   
 # sign in or...
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
 # create bot
 bot = HUG.getBot(email=EMAIL, cookies=cookies)
 # get all conversations and see one's title
 conversations = bot.getConversations()
-print(conversations[0]["title"])
+conv_id = list(conversations.keys())[0]
+print(conversations[conv_id])
 # get all chat histories by conversation_id
-histories = bot.getHistoriesByID(conversation_id=conversations[0]["id"])
+histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
 # delete a conversation
-bot.removeConversation(index=0)
+bot.removeConversation(conversation_id=conv_id)
 # create a new conversation
 conversation_id = bot.createConversation()
 # chat
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
-    callback=(bot.updateTitle, (conversation_id,))
+    # callback=(bot.updateTitle, (conversation_id,))
 )
 # wait the full text or...
-while not message.isDone():
+while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
+while not message.isDone():
+    time.sleep(0.1)
 print(message.getFinalText())
 # get the stream text instantly
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
@@ -180,21 +176,18 @@
 | web        | Switch 'Search Web' enable option      |
 
 Anything not start with `/` will be seen as chat message.
 
 Example:
 ```text
 (None) > /ls
-#* Conversations that have been established:
-#
-#        0. Assistant: "It's February 24th."
-#        1. Today is Wednesday, July 12th, 2034
-#        2. "What is today's date?"
-#        3. "April 2nd."
+#* Conversations established:
 #
+#       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
+#       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
 #(Open-Assistant): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
```

### Comparing `hugchat_api-0.0.1.1/setup.py` & `hugchat_api-0.0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from distutils.core import setup
 setup(
     name="hugchat_api",
-    version="0.0.1.1",
+    version="0.0.1.2",
     author="ogios",
     author_email="2134692955@qq.com",
     description="Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.",
     url="https://github.com/ogios/huggingchat-api",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
```

