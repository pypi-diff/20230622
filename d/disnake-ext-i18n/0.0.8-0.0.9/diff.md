# Comparing `tmp/disnake-ext-i18n-0.0.8.tar.gz` & `tmp/disnake-ext-i18n-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-ext-i18n-0.0.8.tar", last modified: Fri May 26 16:00:06 2023, max compression
+gzip compressed data, was "disnake-ext-i18n-0.0.9.tar", last modified: Thu Jun 22 19:55:03 2023, max compression
```

## Comparing `disnake-ext-i18n-0.0.8.tar` & `disnake-ext-i18n-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.301166 disnake-ext-i18n-0.0.8/
--rw-rw-rw-   0        0        0     9514 2023-05-26 16:00:06.301166 disnake-ext-i18n-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8802 2023-05-21 18:17:54.000000 disnake-ext-i18n-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.272158 disnake-ext-i18n-0.0.8/disnake/
-drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.272158 disnake-ext-i18n-0.0.8/disnake/ext/
-drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.279160 disnake-ext-i18n-0.0.8/disnake/ext/i18n/
--rw-rw-rw-   0        0        0      119 2023-05-26 16:00:04.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/__init__.py
--rw-rw-rw-   0        0        0    15473 2023-05-26 15:58:45.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/agent.py
--rw-rw-rw-   0        0        0     2496 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/cache.py
--rw-rw-rw-   0        0        0    13517 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/language.py
--rw-rw-rw-   0        0        0    14314 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.300164 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/
--rw-rw-rw-   0        0        0     9514 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-05-26 16:00:06.302165 disnake-ext-i18n-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1491 2023-05-21 18:32:48.000000 disnake-ext-i18n-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:55:03.016412 disnake-ext-i18n-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9537 2023-06-22 19:55:03.015412 disnake-ext-i18n-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8802 2023-05-21 18:17:54.000000 disnake-ext-i18n-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 19:55:02.997900 disnake-ext-i18n-0.0.9/disnake/
+drwxrwxrwx   0        0        0        0 2023-06-22 19:55:02.997900 disnake-ext-i18n-0.0.9/disnake/ext/
+drwxrwxrwx   0        0        0        0 2023-06-22 19:55:03.003899 disnake-ext-i18n-0.0.9/disnake/ext/i18n/
+-rw-rw-rw-   0        0        0      119 2023-05-26 16:00:04.000000 disnake-ext-i18n-0.0.9/disnake/ext/i18n/__init__.py
+-rw-rw-rw-   0        0        0    15450 2023-06-22 19:50:42.000000 disnake-ext-i18n-0.0.9/disnake/ext/i18n/agent.py
+-rw-rw-rw-   0        0        0     2496 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.9/disnake/ext/i18n/cache.py
+-rw-rw-rw-   0        0        0    13517 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.9/disnake/ext/i18n/language.py
+-rw-rw-rw-   0        0        0    14154 2023-06-22 19:43:13.000000 disnake-ext-i18n-0.0.9/disnake/ext/i18n/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:55:03.014412 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/
+-rw-rw-rw-   0        0        0     9537 2023-06-22 19:55:02.000000 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-22 19:55:02.000000 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:55:02.000000 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 19:55:02.000000 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 19:55:02.000000 disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 19:55:03.016412 disnake-ext-i18n-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-06-22 19:54:56.000000 disnake-ext-i18n-0.0.9/setup.py
```

### Comparing `disnake-ext-i18n-0.0.8/PKG-INFO` & `disnake-ext-i18n-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: disnake-ext-i18n
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fork of the Pycord extension to support automatic text translations in 107 languages to also support Disnake.
 Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym
 License: MIT
 Project-URL: Issue tracker, https://github.com/jaymart95/disnake-ext-i18n/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # A forked [Disnake](https://github.com/Disnake-Dev/disnake) extension for internationalization
 
 <a href="https://discord.gg/disnake"><img src="https://img.shields.io/badge/GET SUPPORT-DISCORD-orange?style=for-the-badge&logo=discord&logoColor=white&color=5865F2"></a>
 <a href="https://github.com/Disnake-Dev/disnake"><img src="https://img.shields.io/badge/Pycord-%3E=2.0.0b5-orange?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://pypi.org/project/disnake-ext-i18n"><img src="https://img.shields.io/pypi/v/discord-ext-i18n?style=for-the-badge&logo=pypi&logoColor=white&color=green"></a>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.8 Summary: A fork of
+Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.9 Summary: A fork of
 the Pycord extension to support automatic text translations in 107 languages to
 also support Disnake. Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym License: MIT Project-URL: Issue tracker, https://github.com/
 jaymart95/disnake-ext-i18n/issues Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.10 Requires-Python: >=3.7 Description-Content-Type: text/markdown #
-A forked [Disnake](https://github.com/Disnake-Dev/disnake) extension for
-internationalization [https://img.shields.io/badge/GET_SUPPORT-DISCORD-
-orange?style=for-the-badge&logo=discord&logoColor=white&color=5865F2] [https://
-img.shields.io/badge/Pycord-%3E=2.0.0b5-orange?style=for-the-
-badge&logo=python&logoColor=white] [https://img.shields.io/pypi/v/discord-ext-
-i18n?style=for-the-badge&logo=pypi&logoColor=white&color=green] ## Key Features
-- Automatic text translations for messages, embeds [etc..](#fields-covered-by-
-automatic-translation) - Zero code change necessary - Fully customizable -
-Forward Compatible The extension is able to automatically translate all
-specified objects [here](#fields-covered-by-automatic-translation) into any
-registered language depending on the preferences of the destination channel or
-guild. For instance, if a channel has the preference for Spanish, any messages,
-embeds etc.. that are being sent to the channel will be automatically
-translated into Spanish before it is sent. Translations will carry over
-markdown! ```diff + I've set the language to `English`
-ð´ó §ó ¢ó ¥ó ®ó §ó ¿! + He establecido el idioma en `Spanish` ðªð¸!
-+ áá«áá¬áá¬ááá¬á¸áá­á¯áá¬á¸áááº `áá¼ááºáá¬
+Python :: 3.10 Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE # A forked [Disnake](https://github.com/Disnake-Dev/
+disnake) extension for internationalization [https://img.shields.io/badge/GET
+SUPPORT-DISCORD-orange?style=for-the-
+badge&logo=discord&logoColor=white&color=5865F2] [https://img.shields.io/badge/
+Pycord-%3E=2.0.0b5-orange?style=for-the-badge&logo=python&logoColor=white]
+[https://img.shields.io/pypi/v/discord-ext-i18n?style=for-the-
+badge&logo=pypi&logoColor=white&color=green] ## Key Features - Automatic text
+translations for messages, embeds [etc..](#fields-covered-by-automatic-
+translation) - Zero code change necessary - Fully customizable - Forward
+Compatible The extension is able to automatically translate all specified
+objects [here](#fields-covered-by-automatic-translation) into any registered
+language depending on the preferences of the destination channel or guild. For
+instance, if a channel has the preference for Spanish, any messages, embeds
+etc.. that are being sent to the channel will be automatically translated into
+Spanish before it is sent. Translations will carry over markdown! ```diff +
+I've set the language to `English` ð´ó §ó ¢ó ¥ó ®ó §ó ¿! + He
+establecido el idioma en `Spanish` ðªð¸! +
+áá«áá¬áá¬ááá¬á¸áá­á¯áá¬á¸áááº `áá¼ááºáá¬
 (ááá¬)` ð²ð²! ``` _GoogleTranslated string in different languages with
 formatting maintained_ Check out the [FAQ](#faq), [Examples](#Examples) and
 [other feathers](#features-extended) for more information. This extension is
 relatively new so please report any bugs at [issues](https://github.com/
 Rickaym/discord-ext-i18n/issues)! ## Fields Covered by Automatic Translation -
 `Messages` - `Interaction Messages` - `Embeds` - `Buttons` - `Selects` -
 `Modals` (beta) - `Webhooks` (beta) ## Installing This is an extension for
```

### Comparing `disnake-ext-i18n-0.0.8/README.md` & `disnake-ext-i18n-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.8/disnake/ext/i18n/agent.py` & `disnake-ext-i18n-0.0.9/disnake/ext/i18n/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Messageable_send = Messageable.send
 Message_edit = Message.edit
 HTTPClient_edit_message = HTTPClient.edit_message
 HTTPClient_send_message = HTTPClient.send_message
 InteractionResponse_send_message = InteractionResponse.send_message
 InteractionResponse_edit_message = InteractionResponse.edit_message
-#InteractionResponse_send_modal = InteractionResponse.send_modal
+InteractionResponse_send_modal = InteractionResponse.send_modal
 AsyncWebhookAdapter_create_interaction_response = (
     AsyncWebhookAdapter.create_interaction_response
 )
 AsyncWebhookAdapter_execute_webhook = AsyncWebhookAdapter.execute_webhook
 Webhook_send = Webhook.send
 WebhookMessage_edit = WebhookMessage.edit
 
@@ -146,28 +146,28 @@
                     kwds["payload"]["content"],
                 ) = TranslationAgent.translate_payload(
                     lang, kwds["payload"], content, **Agent.translate_config()
                 )
     return AsyncWebhookAdapter_execute_webhook(self, *args, **kwds)
 
 
-#async def i18n_InteractionResponse_send_modal(self: InteractionResponse, modal: Modal):
-#    """
-#    Language code is appended to the modal title if there is a language
-#    preference.
-#
-#    TODO: Very problematic if translation functions are slow, often ends up
-#    timing out on responses.
-#    """
-#    dest_lang = await Agent.detector.first_language_of(self)
-#    if dest_lang:
-#        modal.title = TranslationAgent.encode_lang_str(
-#            Agent.source_lang, modal.title, dest_lang
-#        )
-#    return await InteractionResponse_send_modal(self, modal)
+async def i18n_InteractionResponse_send_modal(self: InteractionResponse, modal: Modal):
+    """
+    Language code is appended to the modal title if there is a language
+    preference.
+
+    TODO: Very problematic if translation functions are slow, often ends up
+    timing out on responses.
+    """
+    dest_lang = await Agent.detector.first_language_of(self)
+    if dest_lang:
+        modal.title = TranslationAgent.encode_lang_str(
+            Agent.source_lang, modal.title, dest_lang
+        )
+    return await InteractionResponse_send_modal(self, modal)
 
 
 def isinstancemethod(func: Callable) -> bool:
     """
     Returns whether if a given function is a staticmethod or an
     instancemethod/classmethod.
     """
@@ -245,15 +245,15 @@
     def __init__(
         self,
         translate_all: Optional[bool] = None,
         translate_messages: Optional[bool] = None,
         translate_embeds: Optional[bool] = None,
         translate_buttons: Optional[bool] = None,
         translate_selects: Optional[bool] = None,
-        #translate_modals: Optional[bool] = None,
+        translate_modals: Optional[bool] = None,
         source_lang: Optional[Language] = None,
     ):
         """
         A context menu to temporarily reconfigure the translation settings until
         it has been exited.
 
         ### Parameters:
@@ -287,15 +287,15 @@
         """
 
         vmap = {
             "translate_messages": translate_messages,
             "translate_embeds": translate_embeds,
             "translate_buttons": translate_buttons,
             "translate_selects": translate_selects,
-            #"translate_modals": translate_modals,
+            "translate_modals": translate_modals,
             "source_lang": source_lang,
         }
         self.prior = {key: getattr(Agent, key, None) for key in vmap}
 
         for key, val in vmap.items():
             if translate_all and key.startswith("translate_"):
                 setattr(Agent, key, True)
@@ -315,28 +315,28 @@
     translator = Translator()
     detector = Detector()
 
     translate_messages = True
     translate_embeds = False
     translate_buttons = False
     translate_selects = False
-    #translate_modals = False
+    translate_modals = False
     source_lang = Language.English
     _instantiated = False
 
     def __init__(
         self,
         translator: Optional[Translator] = None,
         detector: Optional[Detector] = None,
         translate_all: Optional[bool] = None,
         translate_messages: Optional[bool] = None,
         translate_embeds: Optional[bool] = None,
         translate_buttons: Optional[bool] = None,
         translate_selects: Optional[bool] = None,
-        #translate_modals: Optional[bool] = None,
+        translate_modals: Optional[bool] = None,
         source_lang: Optional[Language] = None,
         handle_webhooks: bool = True,
     ):
         """
         Sets initialized injectors to override high and low level.
         At any given case, you cannot initialize this class more than
         once.
@@ -377,24 +377,24 @@
         setattr(
             InteractionResponse,
             "edit_message",
             wrap_i18n_editer(InteractionResponse_edit_message),
         )
         setattr(WebhookMessage, "edit", wrap_i18n_editer(WebhookMessage_edit))
         setattr(HTTPClient, "edit_message", i18n_HTTPClient_edit_message)
-        #setattr(InteractionResponse, "send_modal", i18n_InteractionResponse_send_modal)
+        setattr(InteractionResponse, "send_modal", i18n_InteractionResponse_send_modal)
 
         for key, val in {
             "translator": translator,
             "detector": detector,
             "translate_messages": translate_messages,
             "translate_embeds": translate_embeds,
             "translate_buttons": translate_buttons,
             "translate_selects": translate_selects,
-            #"translate_modals": translate_modals,
+            "translate_modals": translate_modals,
             "source_lang": source_lang,
         }.items():
             if translate_all and key.startswith("translate_"):
                 setattr(Agent, key, True)
             elif val is not None:
                 setattr(Agent, key, val)
 
@@ -406,15 +406,15 @@
         """
         return {
             "source_lang": Agent.source_lang,
             "translator": Agent.translator,
             "translate_components": (
                 Agent.translate_buttons
                 or Agent.translate_selects
-                #or Agent.translate_modals
+                or Agent.translate_modals
             ),
             "translate_messages": Agent.translate_messages,
             "translate_embeds": Agent.translate_embeds,
             "translate_buttons": Agent.translate_buttons,
             "translate_selects": Agent.translate_selects,
-            #"translate_modals": Agent.translate_modals,
+            "translate_modals": Agent.translate_modals,
         }
```

### Comparing `disnake-ext-i18n-0.0.8/disnake/ext/i18n/cache.py` & `disnake-ext-i18n-0.0.9/disnake/ext/i18n/cache.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.8/disnake/ext/i18n/language.py` & `disnake-ext-i18n-0.0.9/disnake/ext/i18n/language.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.8/disnake/ext/i18n/preprocess.py` & `disnake-ext-i18n-0.0.9/disnake/ext/i18n/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,18 +197,15 @@
                         ):
                             if "placeholder" in item and item["placeholder"]:
                                 item["placeholder"] = agent.translate(
                                     item["placeholder"]
                                 )
                             for opt in item["options"]:
                                 opt["label"] = agent.translate(opt["label"])
-                        elif (
-                            translate_modals
-                            and item["type"] == ComponentType.input_text.value
-                        ):
+                        
                             if item["label"]:
                                 item["label"] = agent.translate(item["label"])
                             if "placeholder" in item and item["placeholder"]:
                                 item["placeholder"] = agent.translate(
                                     item["placeholder"]
                                 )
                             if "value" in item and item["value"]:
```

### Comparing `disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/PKG-INFO` & `disnake-ext-i18n-0.0.9/disnake_ext_i18n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: disnake-ext-i18n
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fork of the Pycord extension to support automatic text translations in 107 languages to also support Disnake.
 Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym
 License: MIT
 Project-URL: Issue tracker, https://github.com/jaymart95/disnake-ext-i18n/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # A forked [Disnake](https://github.com/Disnake-Dev/disnake) extension for internationalization
 
 <a href="https://discord.gg/disnake"><img src="https://img.shields.io/badge/GET SUPPORT-DISCORD-orange?style=for-the-badge&logo=discord&logoColor=white&color=5865F2"></a>
 <a href="https://github.com/Disnake-Dev/disnake"><img src="https://img.shields.io/badge/Pycord-%3E=2.0.0b5-orange?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://pypi.org/project/disnake-ext-i18n"><img src="https://img.shields.io/pypi/v/discord-ext-i18n?style=for-the-badge&logo=pypi&logoColor=white&color=green"></a>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.8 Summary: A fork of
+Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.9 Summary: A fork of
 the Pycord extension to support automatic text translations in 107 languages to
 also support Disnake. Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym License: MIT Project-URL: Issue tracker, https://github.com/
 jaymart95/disnake-ext-i18n/issues Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.10 Requires-Python: >=3.7 Description-Content-Type: text/markdown #
-A forked [Disnake](https://github.com/Disnake-Dev/disnake) extension for
-internationalization [https://img.shields.io/badge/GET_SUPPORT-DISCORD-
-orange?style=for-the-badge&logo=discord&logoColor=white&color=5865F2] [https://
-img.shields.io/badge/Pycord-%3E=2.0.0b5-orange?style=for-the-
-badge&logo=python&logoColor=white] [https://img.shields.io/pypi/v/discord-ext-
-i18n?style=for-the-badge&logo=pypi&logoColor=white&color=green] ## Key Features
-- Automatic text translations for messages, embeds [etc..](#fields-covered-by-
-automatic-translation) - Zero code change necessary - Fully customizable -
-Forward Compatible The extension is able to automatically translate all
-specified objects [here](#fields-covered-by-automatic-translation) into any
-registered language depending on the preferences of the destination channel or
-guild. For instance, if a channel has the preference for Spanish, any messages,
-embeds etc.. that are being sent to the channel will be automatically
-translated into Spanish before it is sent. Translations will carry over
-markdown! ```diff + I've set the language to `English`
-ð´ó §ó ¢ó ¥ó ®ó §ó ¿! + He establecido el idioma en `Spanish` ðªð¸!
-+ áá«áá¬áá¬ááá¬á¸áá­á¯áá¬á¸áááº `áá¼ááºáá¬
+Python :: 3.10 Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE # A forked [Disnake](https://github.com/Disnake-Dev/
+disnake) extension for internationalization [https://img.shields.io/badge/GET
+SUPPORT-DISCORD-orange?style=for-the-
+badge&logo=discord&logoColor=white&color=5865F2] [https://img.shields.io/badge/
+Pycord-%3E=2.0.0b5-orange?style=for-the-badge&logo=python&logoColor=white]
+[https://img.shields.io/pypi/v/discord-ext-i18n?style=for-the-
+badge&logo=pypi&logoColor=white&color=green] ## Key Features - Automatic text
+translations for messages, embeds [etc..](#fields-covered-by-automatic-
+translation) - Zero code change necessary - Fully customizable - Forward
+Compatible The extension is able to automatically translate all specified
+objects [here](#fields-covered-by-automatic-translation) into any registered
+language depending on the preferences of the destination channel or guild. For
+instance, if a channel has the preference for Spanish, any messages, embeds
+etc.. that are being sent to the channel will be automatically translated into
+Spanish before it is sent. Translations will carry over markdown! ```diff +
+I've set the language to `English` ð´ó §ó ¢ó ¥ó ®ó §ó ¿! + He
+establecido el idioma en `Spanish` ðªð¸! +
+áá«áá¬áá¬ááá¬á¸áá­á¯áá¬á¸áááº `áá¼ááºáá¬
 (ááá¬)` ð²ð²! ``` _GoogleTranslated string in different languages with
 formatting maintained_ Check out the [FAQ](#faq), [Examples](#Examples) and
 [other feathers](#features-extended) for more information. This extension is
 relatively new so please report any bugs at [issues](https://github.com/
 Rickaym/discord-ext-i18n/issues)! ## Fields Covered by Automatic Translation -
 `Messages` - `Interaction Messages` - `Embeds` - `Buttons` - `Selects` -
 `Modals` (beta) - `Webhooks` (beta) ## Installing This is an extension for
```

### Comparing `disnake-ext-i18n-0.0.8/setup.py` & `disnake-ext-i18n-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 from re import search, MULTILINE
 
 pkg_name = "i18n"
 prj_path = "disnake/ext/{}/".format(pkg_name)
 prj_name = "disnake-ext-{}".format(pkg_name)
 descriptors = ("./README.md",)
 long_description = ""
-version = ""
-
-with open("{}/__init__.py".format(prj_path)) as fp:
-    version = search(
-        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fp.read(), MULTILINE
-    ).group(1)  # type: ignore
+version = "0.0.9"
 
 for desc in descriptors:
     with open(desc, encoding="utf-8") as f:
         long_description += f.read()
 
 setup(
     name=prj_name,
```

