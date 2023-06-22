# Comparing `tmp/eAsistentPY-2.1.1.tar.gz` & `tmp/eAsistentPY-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eAsistentPY-2.1.1.tar", last modified: Sat Jun 10 16:48:56 2023, max compression
+gzip compressed data, was "eAsistentPY-2.1.2.tar", last modified: Thu Jun 22 10:31:14 2023, max compression
```

## Comparing `eAsistentPY-2.1.1.tar` & `eAsistentPY-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/eAsisitentPY/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/src/eAsisitentPY/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/src/eAsisitentPY/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 10:30:46.000000 eAsistentPY-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 10:30:46.000000 eAsistentPY-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-22 10:30:46.000000 eAsistentPY-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/src/eAsisitentPY/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 10:30:46.000000 eAsistentPY-2.1.2/src/eAsisitentPY/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-06-22 10:30:46.000000 eAsistentPY-2.1.2/src/eAsisitentPY/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:31:14.171491 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-22 10:31:14.000000 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 10:31:14.000000 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:31:14.000000 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 10:31:14.000000 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 10:31:14.000000 eAsistentPY-2.1.2/src/eAsistentPY.egg-info/top_level.txt
```

### Comparing `eAsistentPY-2.1.1/LICENSE` & `eAsistentPY-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eAsistentPY-2.1.1/PKG-INFO` & `eAsistentPY-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAsistentPY
-Version: 2.1.1
+Version: 2.1.2
 Summary: Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 Home-page: https://github.com/PingIsFun/eAsistentAPI
 Author: PingIsFun
 Author-email: pingisfun@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/PingIsFun/eAsistentAPI/issues
 Project-URL: Help, https://github.com/PingIsFun/eAsistentAPI/discussions/categories/general
```

### Comparing `eAsistentPY-2.1.1/setup.cfg` & `eAsistentPY-2.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eAsistentPY
-version = 2.1.1
+version = 2.1.2
 author = PingIsFun
 author_email = pingisfun@protonmail.com
 description = Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PingIsFun/eAsistentAPI
 project_urls =
```

### Comparing `eAsistentPY-2.1.1/src/eAsisitentPY/scraper.py` & `eAsistentPY-2.1.2/src/eAsisitentPY/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,28 @@
 def _hour_block_partial_equality(hour_block_new1: HourBlock, hour_block2: HourBlock) -> bool:
     return hour_block_new1.subject == hour_block2.subject and hour_block_new1.teacher == hour_block2.teacher \
         and hour_block_new1.classroom == hour_block2.classroom and hour_block_new1.group == hour_block2.group \
         and hour_block_new1.event == hour_block2.event and hour_block_new1.hour == hour_block2.hour
 
 
 def __get_hour_data(section: bs4.element.Tag) -> tuple[str, list, str, str]:
-    subject = section.find(class_=Formatting.SUBJECT_CLASS).text.replace("\n", "").replace("\t", "")
+    try:
+        subject = section.find(class_=Formatting.SUBJECT_CLASS).text.replace("\n", "").replace("\t", "")
+    except AttributeError:
+        subject = None
     group_raw = section.find_all(class_=Formatting.RAW_GROUP_CLASS)
     try:
         teacher_classroom = list(
             section.find(class_=Formatting.TEACHER_CLASSROOM_CLASS)
             .text.replace("\n", "")
             .replace("\t", "")
             .replace("\r", "")
             .split(", ")
         )
     except AttributeError:
-        subject = section.find(class_=Formatting.EVENT_CLASS).text.replace("\n", "").replace("\t", "")
         teacher_classroom = [None, None]
     group = [x.text for x in group_raw]
     group = None if group == [] else group
     return subject, group, teacher_classroom[0], teacher_classroom[1]
 
 
 def __get_event(section: bs4.element.Tag) -> str:
```

### Comparing `eAsistentPY-2.1.1/src/eAsistentPY.egg-info/PKG-INFO` & `eAsistentPY-2.1.2/src/eAsistentPY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAsistentPY
-Version: 2.1.1
+Version: 2.1.2
 Summary: Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 Home-page: https://github.com/PingIsFun/eAsistentAPI
 Author: PingIsFun
 Author-email: pingisfun@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/PingIsFun/eAsistentAPI/issues
 Project-URL: Help, https://github.com/PingIsFun/eAsistentAPI/discussions/categories/general
```

