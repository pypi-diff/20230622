# Comparing `tmp/tg_bot_ml-0.0.3.tar.gz` & `tmp/tg_bot_ml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bot_ml-0.0.3.tar", last modified: Wed Jun 21 07:03:35 2023, max compression
+gzip compressed data, was "tg_bot_ml-0.0.4.tar", last modified: Wed Jun 21 07:17:18 2023, max compression
```

## Comparing `tg_bot_ml-0.0.3.tar` & `tg_bot_ml-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.3/LICENSE
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.3/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       79 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-21 07:03:28.000000 tg_bot_ml-0.0.3/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/tg_bot_ml/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.3/tg_bot_ml/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3206 2023-06-20 15:20:02.000000 tg_bot_ml-0.0.3/tg_bot_ml/img_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1410 2023-06-20 09:32:12.000000 tg_bot_ml-0.0.3/tg_bot_ml/table_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2109 2023-06-20 09:00:14.000000 tg_bot_ml-0.0.3/tg_bot_ml/tg_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.3/tg_bot_ml/utils.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/top_level.txt
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.4/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.4/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       79 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-21 07:17:13.000000 tg_bot_ml-0.0.4/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/tg_bot_ml/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.4/tg_bot_ml/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-21 07:15:35.000000 tg_bot_ml-0.0.4/tg_bot_ml/img_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1440 2023-06-21 07:16:15.000000 tg_bot_ml-0.0.4/tg_bot_ml/table_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-21 07:16:46.000000 tg_bot_ml-0.0.4/tg_bot_ml/tg_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.4/tg_bot_ml/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:17:18.164345 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-21 07:17:18.000000 tg_bot_ml-0.0.4/tg_bot_ml.egg-info/top_level.txt
```

### Comparing `tg_bot_ml-0.0.3/LICENSE` & `tg_bot_ml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.3/PKG-INFO` & `tg_bot_ml-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_bot_ml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

### Comparing `tg_bot_ml-0.0.3/setup.py` & `tg_bot_ml-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'tg_bot_ml',
   packages = ['tg_bot_ml'],
-  version = '0.0.3',
+  version = '0.0.4',
   license='GPLv3',
   description = 'Simple telegram bot for logging ML statistics.',
   author = 'Dmitry',
   author_email = 'michalych2014@yandex.ru',
   url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats.git', 
   download_url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip',
   keywords = ['Telegram', 'Bot', 'ML', 'Machine Learning', 'Logger'],
```

### Comparing `tg_bot_ml-0.0.3/tg_bot_ml/img_bot.py` & `tg_bot_ml-0.0.4/tg_bot_ml/img_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             stats_imgs[group].append(data)
             plt.close(fig)
         
         return stats_imgs
     
     def send(self, send_statistics=True, send_images=True, send_plots=True):
         self.send_delimiter()
-        self.send_message(self.description)
         if send_statistics:
             statistics = self.collect_statistics()
             self.send_pandas_df(statistics)
         if send_plots:
             plots = self.collect_images()
             for group_name in plots:
                 group_plots = plots[group_name]
```

### Comparing `tg_bot_ml-0.0.3/tg_bot_ml/table_bot.py` & `tg_bot_ml-0.0.4/tg_bot_ml/table_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             self.description += f"{desc_name} : {desc}\n"
 
     def add_record(self, **kwargs):
         df_new_record = pd.DataFrame.from_records(kwargs, index=[0])
         self.records = pd.concat([self.records, df_new_record], ignore_index=True)
 
     def send(self, sort_by=None, ascending=None, round=None):
+        self.send_delimiter()
         tmp_records = self.records
 
         if sort_by is not None and ascending is not None:
             tmp_records = self.records.sort_values(by=sort_by, ascending=ascending)
         elif sort_by is not None:
             tmp_records = self.records.sort_values(by=sort_by)
```

### Comparing `tg_bot_ml-0.0.3/tg_bot_ml/tg_bot.py` & `tg_bot_ml-0.0.4/tg_bot_ml/tg_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.credentials = self.load_credentials(path_to_credentials)
         self.experiment_name = experiment_name
         self.bot = telebot.TeleBot(self.credentials['TOKEN'],
                                    parse_mode=None)
         self.topic = self.bot.create_forum_topic(self.credentials['CHAT_ID'], 
                                                  self.experiment_name)
         self.delimiter = "-"*90
+        self.description = None
 
     def send_message(self, message):
         self.bot.send_message(self.credentials['CHAT_ID'], text=message, 
                               reply_to_message_id=self.topic.message_thread_id)
         
     def send_pandas_df(self, df):
         message = f"<pre>\n{df.to_markdown()}\n</pre>"
@@ -44,15 +45,18 @@
             encoded_imgs.append(InputMediaPhoto(img_enc))
         
         self.bot.send_media_group(self.credentials['CHAT_ID'], encoded_imgs, 
                                   reply_to_message_id=self.topic.message_thread_id)
     
 
     def send_delimiter(self):
-        self.send_message(self.delimiter)
+        if self.description is not None:
+            self.send_message(f"{self.delimiter} \n {self.description}")
+        else:
+            self.send_message(self.delimiter)
 
     @staticmethod
     def load_credentials(path_to_cred):
         with open(path_to_cred, 'r') as read_c:
             credentials = yaml.safe_load(read_c)
         return credentials
```

### Comparing `tg_bot_ml-0.0.3/tg_bot_ml/utils.py` & `tg_bot_ml-0.0.4/tg_bot_ml/utils.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.3/tg_bot_ml.egg-info/PKG-INFO` & `tg_bot_ml-0.0.4/tg_bot_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-bot-ml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

