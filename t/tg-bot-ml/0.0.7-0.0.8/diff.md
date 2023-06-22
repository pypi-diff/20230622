# Comparing `tmp/tg_bot_ml-0.0.7.linux-x86_64.tar.gz` & `tmp/tg_bot_ml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bot_ml-0.0.7.linux-x86_64.tar", last modified: Thu Jun 22 08:04:42 2023, max compression
+gzip compressed data, was "tg_bot_ml-0.0.8.tar", last modified: Thu Jun 22 08:06:02 2023, max compression
```

## Comparing `tg_bot_ml-0.0.7.linux-x86_64.tar` & `tg_bot_ml-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,18 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.062780 ./
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.062780 ./home/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.062780 ./home/dmitry/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.062780 ./home/dmitry/anaconda3/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.062780 ./home/dmitry/anaconda3/envs/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.082780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 06:12:46.000000 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__init__.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      176 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3538 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/img_bot.cpython-38.pyc
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1688 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/table_bot.cpython-38.pyc
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2601 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/tg_bot.cpython-38.pyc
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      867 2023-06-22 08:04:42.066780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/__pycache__/utils.cpython-38.pyc
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-22 07:54:23.000000 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/img_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1383 2023-06-22 06:12:46.000000 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/table_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-22 06:12:46.000000 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/tg_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-22 06:12:46.000000 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/utils.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:04:42.086780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 08:04:42.078780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-22 08:04:42.082780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-22 08:04:42.078780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-22 08:04:42.078780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-22 08:04:42.078780 ./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/top_level.txt
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-22 06:12:10.000000 tg_bot_ml-0.0.8/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      149 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-22 08:05:49.000000 tg_bot_ml-0.0.8/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/tg_bot_ml/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-22 07:54:23.000000 tg_bot_ml-0.0.8/tg_bot_ml/img_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1383 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/table_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/tg_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/top_level.txt
```

### Comparing `./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/img_bot.py` & `tg_bot_ml-0.0.8/tg_bot_ml/img_bot.py`

 * *Files identical despite different names*

### Comparing `./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/table_bot.py` & `tg_bot_ml-0.0.8/tg_bot_ml/table_bot.py`

 * *Files identical despite different names*

### Comparing `./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/tg_bot.py` & `tg_bot_ml-0.0.8/tg_bot_ml/tg_bot.py`

 * *Files identical despite different names*

### Comparing `./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml/utils.py` & `tg_bot_ml-0.0.8/tg_bot_ml/utils.py`

 * *Files identical despite different names*

### Comparing `./home/dmitry/anaconda3/envs/tel_bot/lib/python3.8/site-packages/tg_bot_ml-0.0.7-py3.8.egg-info/PKG-INFO` & `tg_bot_ml-0.0.8/tg_bot_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-bot-ml
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

