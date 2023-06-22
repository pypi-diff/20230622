# Comparing `tmp/cs-telegram-bot-api-0.0.8.tar.gz` & `tmp/cs-telegram-bot-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.8.tar", last modified: Wed Jun 14 06:16:57 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.9.tar", last modified: Thu Jun 22 13:00:00 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.8.tar` & `cs-telegram-bot-api-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/cs_telegram_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/get_chat_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:00:00.728973 cs-telegram-bot-api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-22 13:00:00.724972 cs-telegram-bot-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-22 12:59:45.000000 cs-telegram-bot-api-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:00:00.724972 cs-telegram-bot-api-0.0.9/cs_telegram_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 12:59:45.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-22 12:59:45.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-22 12:59:45.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot/get_chat_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:00:00.724972 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-22 13:00:00.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-22 13:00:00.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:00:00.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 13:00:00.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 13:00:00.000000 cs-telegram-bot-api-0.0.9/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:00:00.728973 cs-telegram-bot-api-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-22 12:59:45.000000 cs-telegram-bot-api-0.0.9/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.8/README.md` & `cs-telegram-bot-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.8/cs_telegram_bot/api.py` & `cs-telegram-bot-api-0.0.9/cs_telegram_bot/api.py`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.8/cs_telegram_bot/get_chat_ids.py` & `cs-telegram-bot-api-0.0.9/cs_telegram_bot/get_chat_ids.py`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.8/setup.py` & `cs-telegram-bot-api-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Telegram Bot API Wrapper'
 LONG_DESCRIPTION = 'A Python module for interacting with the Telegram Bot API.'
 
 # Setting up
 setup(
     name="cs-telegram-bot-api",
     version=VERSION,
```

