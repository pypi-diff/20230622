# Comparing `tmp/reliableGPT-0.2.7.tar.gz` & `tmp/reliableGPT-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.7.tar", last modified: Thu Jun 22 19:35:03 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.8.tar", last modified: Thu Jun 22 21:44:10 2023, max compression
```

## Comparing `reliableGPT-0.2.7.tar` & `reliableGPT-0.2.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.881251 reliableGPT-0.2.7/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.7/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 19:35:03.881157 reliableGPT-0.2.7/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.7/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.880304 reliableGPT-0.2.7/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.880909 reliableGPT-0.2.7/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.7/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7690 2023-06-22 19:18:21.000000 reliableGPT-0.2.7/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4491 2023-06-22 19:32:42.000000 reliableGPT-0.2.7/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 19:35:03.881281 reliableGPT-0.2.7/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 19:34:51.000000 reliableGPT-0.2.7/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.494677 reliableGPT-0.2.8/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.8/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 21:44:10.494584 reliableGPT-0.2.8/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.8/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.493584 reliableGPT-0.2.8/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.494455 reliableGPT-0.2.8/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.8/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8355 2023-06-22 21:33:04.000000 reliableGPT-0.2.8/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.8/reliablegpt/send_notifications.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4539 2023-06-22 21:42:44.000000 reliableGPT-0.2.8/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 21:44:10.494711 reliableGPT-0.2.8/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 21:43:46.000000 reliableGPT-0.2.8/setup.py
```

### Comparing `reliableGPT-0.2.7/LICENSE` & `reliableGPT-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.7/README.md` & `reliableGPT-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.7/reliablegpt/main.py` & `reliableGPT-0.2.8/reliablegpt/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import openai
 from termcolor import colored
 import time
 import functools
 import copy
 import requests
 from posthog import Posthog
+from send_notifications import send_emails_task
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 def make_LLM_request(new_kwargs, self):
     try:
@@ -99,20 +100,30 @@
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
 class reliableGPT:
-    def __init__(self, openai_create_function, fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], graceful_string="Sorry, the OpenAI API is currently down", user_email="", user_token=""):
+    def __init__(
+            self, 
+            openai_create_function, 
+            fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], 
+            graceful_string="Sorry, the OpenAI API is currently down", 
+            user_email="", 
+            user_token="",
+            send_notification=False
+            ):
         self.openai_create_function = openai_create_function
         self.graceful_string = graceful_string
         self.fallback_strategy = fallback_strategy
         self.user_email = user_email
         self.user_token = user_token
+        self.send_notification = send_notification
+
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
     def __call__(self, *args, **kwargs):
         try:
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
@@ -129,17 +140,21 @@
                     graceful_string = self.graceful_string,
                     user_email = self.user_email,
                     user_token=self.user_token,
                     self=self
                 )
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e.error, 'recovered_response': result})
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
+                if result == self.graceful_string:
+                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Normal Retry"}, self.send_notification)
                 return result
-            except:
+            except Exception as e:
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': self.graceful_string})
+                if result == self.graceful_string:
+                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Got Exception on Retry", "2nd Error": e}, self.send_notification)
                 return self.graceful_string
 
 
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
```

### Comparing `reliableGPT-0.2.7/reliablegpt/tests.py` & `reliableGPT-0.2.8/reliablegpt/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import openai
 from main import reliableGPT
 import main
 
 # make openAI reliable and safe
 #openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email="krrish@berri.ai", user_token="rjPyk_xegdh-dpLBpDJzZacS0fVj3kR_zpNCnl5f4e0")
-openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "krrish@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM')
+openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "ishaan@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM', send_notification=True)
 
 
 # fallback_priority = {user_emails}
 
 import concurrent.futures
 
 def test_multiple_calls():
@@ -105,15 +105,15 @@
 
 # test_add_keys()
 # test_delete_keys()
 
 
 def test_embedding_bad_key():
     from main import reliableGPT
-    openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "krrish@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM')
+    openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "ishaan@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM', send_notification=True)
 
     openai.api_key = "bad-key"
     def get_embedding(text, model="text-embedding-ada-002"):
         text = text.replace("\n", " ")
         print("text")
         return openai.Embedding.create(input=[text],
                                         model=model)["data"][0]["embedding"]
```

