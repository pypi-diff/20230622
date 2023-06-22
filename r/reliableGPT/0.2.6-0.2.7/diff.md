# Comparing `tmp/reliableGPT-0.2.6.tar.gz` & `tmp/reliableGPT-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.6.tar", last modified: Wed Jun 21 19:51:52 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.7.tar", last modified: Thu Jun 22 19:35:03 2023, max compression
```

## Comparing `reliableGPT-0.2.6.tar` & `reliableGPT-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 19:51:52.755159 reliableGPT-0.2.6/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.6/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 19:51:52.755051 reliableGPT-0.2.6/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.6/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 19:51:52.754387 reliableGPT-0.2.6/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 19:51:52.000000 reliableGPT-0.2.6/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 19:51:52.000000 reliableGPT-0.2.6/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 19:51:52.000000 reliableGPT-0.2.6/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 19:51:52.000000 reliableGPT-0.2.6/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 19:51:52.000000 reliableGPT-0.2.6/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 19:51:52.754804 reliableGPT-0.2.6/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.6/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7452 2023-06-21 19:51:33.000000 reliableGPT-0.2.6/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3904 2023-06-21 19:39:34.000000 reliableGPT-0.2.6/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 19:51:52.755202 reliableGPT-0.2.6/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 19:51:40.000000 reliableGPT-0.2.6/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.881251 reliableGPT-0.2.7/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.7/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 19:35:03.881157 reliableGPT-0.2.7/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.7/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.880304 reliableGPT-0.2.7/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 19:35:03.000000 reliableGPT-0.2.7/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 19:35:03.880909 reliableGPT-0.2.7/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.7/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7690 2023-06-22 19:18:21.000000 reliableGPT-0.2.7/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4491 2023-06-22 19:32:42.000000 reliableGPT-0.2.7/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 19:35:03.881281 reliableGPT-0.2.7/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 19:34:51.000000 reliableGPT-0.2.7/setup.py
```

### Comparing `reliableGPT-0.2.6/LICENSE` & `reliableGPT-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.6/reliablegpt/main.py` & `reliableGPT-0.2.7/reliablegpt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 import requests
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
-def make_LLM_request(new_kwargs):
+def make_LLM_request(new_kwargs, self):
     try:
+        if "embedding" in str(self.openai_create_function):
+            # retry embedding with diff key
+            return openai.Embedding.create(**new_kwargs)
         model = new_kwargs['model']
         if "3.5" or "4" in model: # call ChatCompletion
             print(colored(f"ReliableGPT: Retrying request with model CHAT {model}", "blue"))
             return openai.ChatCompletion.create(**new_kwargs)
         else:
             print(colored(f"ReliableGPT: Retrying request with model TEXT {model}", "blue"))
             new_kwargs['prompt'] = " ".join([message["content"] for message in new_kwargs['messages']])
@@ -32,37 +35,37 @@
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
         result = make_LLM_request(new_kwargs)
         if result != None:
             return result    
     return None
 
-def api_key_handler(args, kwargs, fallback_strategy, user_email, user_token):
+def api_key_handler(args, kwargs, fallback_strategy, user_email, user_token, self=""):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
         if result['status'] == 'failed':
             print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
             return None
 
         fallback_keys = result['response']['openai_api_keys'] # list of fallback keys
         if len(fallback_keys) == 0:
             return None
         for fallback_key in fallback_keys:
             openai.api_key = fallback_key
-            result = make_LLM_request(kwargs)
+            result = make_LLM_request(kwargs, self=self)
             if result != None:
                 return result
     else:
         print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
     return None
 
 
-def handle_openAI_error(args, kwargs, openAI_error, fallback_strategy, graceful_string, user_email="", user_token=""):
+def handle_openAI_error(args, kwargs, openAI_error, fallback_strategy, graceful_string, user_email="", user_token="", self=""):
     # Error Types from https://platform.openai.com/docs/guides/error-codes/python-library-error-types
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
     # 4. APIConnectionError - Check your network settings, proxy configuration, SSL certificates, or firewall rules.
     # 5. InvalidRequestError - User input was bad: context_length_exceeded, 
     # 6. AuthenticationError - API key not working, return default hardcoded message
@@ -76,15 +79,15 @@
             result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
             if result == None:
                 return graceful_string
             else:
                 return result
         if openAI_error.code == "invalid_api_key":
             print(colored("ReliableGPT: invalid request error - invalid_api_key", "red"))
-            result = api_key_handler(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, user_email=user_email, user_token=user_token)
+            result = api_key_handler(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, user_email=user_email, user_token=user_token, self=self)
             if result == None:
                 return graceful_string
             else:
                 return result
 
     # todo: alert on user_email that there is now an auth error 
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
@@ -121,15 +124,16 @@
                 result = handle_openAI_error(
                     args = args,
                     kwargs = kwargs,
                     openAI_error = e.error,
                     fallback_strategy = self.fallback_strategy,
                     graceful_string = self.graceful_string,
                     user_email = self.user_email,
-                    user_token=self.user_token
+                    user_token=self.user_token,
+                    self=self
                 )
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e.error, 'recovered_response': result})
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
                 return result
             except:
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': self.graceful_string})
                 return self.graceful_string
```

### Comparing `reliableGPT-0.2.6/reliablegpt/tests.py` & `reliableGPT-0.2.7/reliablegpt/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import openai
 from main import reliableGPT
 import main
 
 # make openAI reliable and safe
 #openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email="krrish@berri.ai", user_token="rjPyk_xegdh-dpLBpDJzZacS0fVj3kR_zpNCnl5f4e0")
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "krrish@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM')
-openai.api_key = "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"
 
 
+# fallback_priority = {user_emails}
+
 import concurrent.futures
 
 def test_multiple_calls():
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Who won the world series in 2020?"*400},
@@ -48,15 +49,15 @@
     print(f"Fallback response count: {failure_count}")
 
     if error_count == 0:
         print("All calls executed successfully.")
     else:
         print("Some calls returned errors.")
 
-test_multiple_calls()
+#test_multiple_calls()
 
 
 def test_single_call_bad_key():
     openai.api_key = "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"
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
@@ -101,7 +102,22 @@
 #     result = main.delete_keys(account_email="ishaan@berri.ai", account_token="OwfY1OFqy8fxR0zsJQPW_tcMPo8N7_vP8x3YW-dU9R8")
 #     print(result)
 
 
 # test_add_keys()
 # test_delete_keys()
 
+
+def test_embedding_bad_key():
+    from main import reliableGPT
+    openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "krrish@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM')
+
+    openai.api_key = "bad-key"
+    def get_embedding(text, model="text-embedding-ada-002"):
+        text = text.replace("\n", " ")
+        print("text")
+        return openai.Embedding.create(input=[text],
+                                        model=model)["data"][0]["embedding"]
+    result = get_embedding("GM")
+    #print(f"This is the embedding response {result}")
+
+test_embedding_bad_key()
```

