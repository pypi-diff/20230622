# Comparing `tmp/yud102023-0.1.0.tar.gz` & `tmp/yud102023-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.1.0.tar", last modified: Thu Jun 22 15:02:41 2023, max compression
+gzip compressed data, was "yud102023-0.1.1.tar", last modified: Thu Jun 22 15:09:26 2023, max compression
```

## Comparing `yud102023-0.1.0.tar` & `yud102023-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.481431 yud102023-0.1.0/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.1.0/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:02:41.481258 yud102023-0.1.0/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.1.0/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-22 15:02:31.000000 yud102023-0.1.0/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-22 15:02:41.481490 yud102023-0.1.0/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.478281 yud102023-0.1.0/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.479956 yud102023-0.1.0/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    31029 2023-06-22 15:01:31.000000 yud102023-0.1.0/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.1.0/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:02:41.480960 yud102023-0.1.0/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/requires.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-22 15:02:41.000000 yud102023-0.1.0/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:09:26.015007 yud102023-0.1.1/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.1.1/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:09:26.014842 yud102023-0.1.1/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.1.1/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-22 15:09:17.000000 yud102023-0.1.1/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-22 15:09:26.015074 yud102023-0.1.1/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:09:26.012098 yud102023-0.1.1/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:09:26.013612 yud102023-0.1.1/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    32055 2023-06-22 15:08:55.000000 yud102023-0.1.1/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.1.1/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-22 15:09:26.014599 yud102023-0.1.1/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-22 15:09:26.000000 yud102023-0.1.1/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-22 15:09:26.000000 yud102023-0.1.1/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-22 15:09:26.000000 yud102023-0.1.1/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-22 15:09:26.000000 yud102023-0.1.1/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-22 15:09:26.000000 yud102023-0.1.1/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.1.0/LICENSE` & `yud102023-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.1.0/PKG-INFO` & `yud102023-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.1.0/pyproject.toml` & `yud102023-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yud102023"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Tomereliel", email="tomereliel.dev@gmail.com" },
 ]
 description = "A small creactive goodbye project for my students"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yud102023-0.1.0/src/yud102023/goodbye.py` & `yud102023-0.1.1/src/yud102023/goodbye.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 'ron':'''
 Your brilliance shines brightly in the classroom.
 Your ability to do any mission with success sets you apart.
 I am grateful to have had the opportunity to teach such a remarkable student like you.
 
 Keep pushing yourself to new heights and know that you have the potential to achieve anything you set your mind to.
 ''',
+'itay':'''
+You are super intelligent students.
+It's was my pleasure to teach you.
+You are talented and friendly and it's fun to around you.
+
+Stay as you are!
+''',
 'itai':'''
 You are super intelligent students.
 It's was my pleasure to teach you.
 You are talented and friendly and it's fun to around you.
 
 Stay as you are!
 ''',
@@ -66,20 +73,33 @@
 ''',
 'yonatan':'''
 You adds color to the class.
 Your unique character makes it fun to be around you.
 
 I had the pleasure to have you in my class - stay awesome as you are!
 ''',
+'yehonatan':'''
+You adds color to the class.
+Your unique character makes it fun to be around you.
+
+I had the pleasure to have you in my class - stay awesome as you are!
+''',
 'ido':'''
 I'm proud of the way you did this year.
 No matter what you didn't give up.
 
 You are good friend and intelligent.
 Good luck next year!
+''',
+'edo':'''
+I'm proud of the way you did this year.
+No matter what you didn't give up.
+
+You are good friend and intelligent.
+Good luck next year!
 '''
 }
 
 IDS = {"oren":b'$\x06Z\xd4\xaa\xbd\xedG{\xaf\x8d\xe2\xfb\xee\xfbt',
        "daniel":b'\x1c\x90\x07\xb1\x19\x1fV\xca\xf9\xc8~S\x99\xf2\xae\x8e',
        "yonatan":b'$\xf18\xa3P\x17\xc5\x05+\xd1\xe1KK}\x90\xdc',
       "yehonatan":b'$\xf18\xa3P\x17\xc5\x05+\xd1\xe1KK}\x90\xdc',
@@ -208,14 +228,25 @@
 יונתן היקר!
 אני גאה בך בטירוף על הדרך שעשית השנה - 
 כל פעם כשהיה קצת קשה הפקת לקחים ויצאת משופר וחזק יותר
 בסוף השנה אני מסתכל ואני רואה חניך מעולה עם יכולות גבוהות שלא מפסיק להפתיע.
 
 אתה חבר טוב ואדם נעים. כיף להיות סביבך ונהנתי מאוד מחברתך.
 אני בטוח שתגיע רחוק!
+תומר אליאל.
+רשתות, מגשימים 2023.
+''',
+"yonatan":'''
+יונתן היקר!
+אני גאה בך בטירוף על הדרך שעשית השנה - 
+כל פעם כשהיה קצת קשה הפקת לקחים ויצאת משופר וחזק יותר
+בסוף השנה אני מסתכל ואני רואה חניך מעולה עם יכולות גבוהות שלא מפסיק להפתיע.
+
+אתה חבר טוב ואדם נעים. כיף להיות סביבך ונהנתי מאוד מחברתך.
+אני בטוח שתגיע רחוק!
 תומר אליאל.
 רשתות, מגשימים 2023.
 ''',
 "ido":'''
 עידו היקר,
 עשית דרך משמעותית מאוד השנה.
 עבדת קשה מאוד, לא תמיד זה היה קל וראיתי איך למרות הכל אתה לא מוותר וממשיך.
```

### Comparing `yud102023-0.1.0/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.1.1/src/yud102023.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

