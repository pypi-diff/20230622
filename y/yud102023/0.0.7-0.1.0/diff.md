# Comparing `tmp/yud102023-0.0.7.tar.gz` & `tmp/yud102023-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.7.tar", last modified: Mon Jun 19 16:16:21 2023, max compression
+gzip compressed data, was "yud102023-0.1.0.tar", last modified: Thu Jun 22 15:02:41 2023, max compression
```

## Comparing `yud102023-0.0.7.tar` & `yud102023-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 16:16:21.522641 yud102023-0.0.7/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.7/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 16:16:21.522391 yud102023-0.0.7/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.7/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 16:14:57.000000 yud102023-0.0.7/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 16:16:21.522731 yud102023-0.0.7/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 16:16:21.519048 yud102023-0.0.7/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 16:16:21.521030 yud102023-0.0.7/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    30411 2023-06-19 16:15:00.000000 yud102023-0.0.7/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.7/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 16:16:21.521977 yud102023-0.0.7/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 16:16:21.000000 yud102023-0.0.7/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 16:16:21.000000 yud102023-0.0.7/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 16:16:21.000000 yud102023-0.0.7/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 16:16:21.000000 yud102023-0.0.7/src/yud102023.egg-info/requires.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 16:16:21.000000 yud102023-0.0.7/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.481431 yud102023-0.1.0/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.1.0/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:02:41.481258 yud102023-0.1.0/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.1.0/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-22 15:02:31.000000 yud102023-0.1.0/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-22 15:02:41.481490 yud102023-0.1.0/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.478281 yud102023-0.1.0/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.479956 yud102023-0.1.0/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    31029 2023-06-22 15:01:31.000000 yud102023-0.1.0/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.1.0/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.480960 yud102023-0.1.0/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.7/LICENSE` & `yud102023-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.7/PKG-INFO` & `yud102023-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.7
+Version: 0.1.0
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.0.7/pyproject.toml` & `yud102023-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yud102023"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Tomereliel", email="tomereliel.dev@gmail.com" },
 ]
 description = "A small creactive goodbye project for my students"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yud102023-0.0.7/src/yud102023/goodbye.py` & `yud102023-0.1.0/src/yud102023/goodbye.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,27 @@
 בסוף השנה אני מסתכל ואני רואה חניך מעולה עם יכולות גבוהות שלא מפסיק להפתיע.
 
 אתה חבר טוב ואדם נעים. כיף להיות סביבך ונהנתי מאוד מחברתך.
 אני בטוח שתגיע רחוק!
 תומר אליאל.
 רשתות, מגשימים 2023.
 ''',
+"ido":'''
+עידו היקר,
+עשית דרך משמעותית מאוד השנה.
+עבדת קשה מאוד, לא תמיד זה היה קל וראיתי איך למרות הכל אתה לא מוותר וממשיך.
+לבסוף אתה קוצר את הפירות וסיימת את השנה בהצלחה מרובה.
+
+אתה חבר טוב וגבר אמיתי,
+אני שמח שאתה בכיתה שלי וזכיתי ללמד אותך השנה.
+תשמור על התכונות הטובות שבך והן יובילו אותך רחוק.
+מעריך המון,
+תומר אליאל.
+רשתות, מגשימים 2023.
+''',
 "edo":'''
 עידו היקר,
 עשית דרך משמעותית מאוד השנה.
 עבדת קשה מאוד, לא תמיד זה היה קל וראיתי איך למרות הכל אתה לא מוותר וממשיך.
 לבסוף אתה קוצר את הפירות וסיימת את השנה בהצלחה מרובה.
 
 אתה חבר טוב וגבר אמיתי,
@@ -477,15 +490,15 @@
     sleep(5)
     keyboard.press('f11')
     sleep(40)
     os.system('exit')
 
 
 
-STUDENTS = {"oren":"test","daniel":"test","ron":"test","avi":"test","yehonatan":"test","yonatan":"test","ido":"test","itai":"test","itay":"test","shahar":"test","shachar":"test","eliya":"test","lior":"test","yarden":"test"}
+STUDENTS = {"oren":"test","daniel":"test","edo":"test","ron":"test","avi":"test","yehonatan":"test","yonatan":"test","ido":"test","itai":"test","itay":"test","shahar":"test","shachar":"test","eliya":"test","lior":"test","yarden":"test"}
 try:
   bye()
   sys.stdout.flush()
   sleep(5)
   os.system('color 07')
   os.system('exit')
 except KeyboardInterrupt:
```

### Comparing `yud102023-0.0.7/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.1.0/src/yud102023.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.7
+Version: 0.1.0
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

