# Comparing `tmp/tg_bot_ml-0.0.4.tar.gz` & `tmp/tg_bot_ml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bot_ml-0.0.4.tar", last modified: Wed Jun 21 07:17:18 2023, max compression
+gzip compressed data, was "tg_bot_ml-0.0.5.tar", last modified: Thu Jun 22 05:01:55 2023, max compression
```

## Comparing `tg_bot_ml-0.0.4.tar` & `tg_bot_ml-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.4/LICENSE
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.4/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       79 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-21 07:17:13.000000 tg_bot_ml-0.0.4/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/tg_bot_ml/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.4/tg_bot_ml/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-21 07:15:35.000000 tg_bot_ml-0.0.4/tg_bot_ml/img_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1440 2023-06-21 07:16:15.000000 tg_bot_ml-0.0.4/tg_bot_ml/table_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-21 07:16:46.000000 tg_bot_ml-0.0.4/tg_bot_ml/tg_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.4/tg_bot_ml/utils.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/top_level.txt
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 05:01:55.015156 tg_bot_ml-0.0.5/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.5/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 05:01:55.015156 tg_bot_ml-0.0.5/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.5/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       83 2023-06-22 05:01:55.015156 tg_bot_ml-0.0.5/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-22 05:00:13.000000 tg_bot_ml-0.0.5/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 05:01:55.015156 tg_bot_ml-0.0.5/tg_bot_ml/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.5/tg_bot_ml/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-21 07:15:35.000000 tg_bot_ml-0.0.5/tg_bot_ml/img_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1383 2023-06-22 04:58:56.000000 tg_bot_ml-0.0.5/tg_bot_ml/table_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-21 07:16:46.000000 tg_bot_ml-0.0.5/tg_bot_ml/tg_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.5/tg_bot_ml/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 05:01:55.015156 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 05:01:54.000000 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-22 05:01:54.000000 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-22 05:01:54.000000 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-22 05:01:54.000000 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-22 05:01:54.000000 tg_bot_ml-0.0.5/tg_bot_ml.egg-info/top_level.txt
```

### Comparing `tg_bot_ml-0.0.4/LICENSE` & `tg_bot_ml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.4/PKG-INFO` & `tg_bot_ml-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_bot_ml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

### Comparing `tg_bot_ml-0.0.4/setup.py` & `tg_bot_ml-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'tg_bot_ml',
   packages = ['tg_bot_ml'],
-  version = '0.0.4',
+  version = '0.0.5',
   license='GPLv3',
   description = 'Simple telegram bot for logging ML statistics.',
   author = 'Dmitry',
   author_email = 'michalych2014@yandex.ru',
   url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats.git', 
   download_url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip',
   keywords = ['Telegram', 'Bot', 'ML', 'Machine Learning', 'Logger'],
```

### Comparing `tg_bot_ml-0.0.4/tg_bot_ml/img_bot.py` & `tg_bot_ml-0.0.5/tg_bot_ml/img_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.4/tg_bot_ml/table_bot.py` & `tg_bot_ml-0.0.5/tg_bot_ml/table_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,13 +28,11 @@
             tmp_records = self.records.sort_values(by=sort_by, ascending=ascending)
         elif sort_by is not None:
             tmp_records = self.records.sort_values(by=sort_by)
         
         if round:
             tmp_records_floats = tmp_records.select_dtypes(include=[float])
             tmp_records[tmp_records_floats.columns] = tmp_records_floats.round(round)
-        print(tmp_records)
-        self.send_delimiter()
         self.send_pandas_df(tmp_records)
```

### Comparing `tg_bot_ml-0.0.4/tg_bot_ml/tg_bot.py` & `tg_bot_ml-0.0.5/tg_bot_ml/tg_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.4/tg_bot_ml/utils.py` & `tg_bot_ml-0.0.5/tg_bot_ml/utils.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.4/tg_bot_ml.egg-info/PKG-INFO` & `tg_bot_ml-0.0.5/tg_bot_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-bot-ml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

