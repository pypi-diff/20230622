# Comparing `tmp/worddfn-0.1.2.tar.gz` & `tmp/worddfn-0.1.3.tar.gz`

## Comparing `worddfn-0.1.2.tar` & `worddfn-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0   137387 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Black_logo-no_background.png
--rwxr-xr-x   0        0        0   198761 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Color_logo-no_background.png
--rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Color_logo-no_background_RM.png
--rwxr-xr-x   0        0        0   151331 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/White_logo-no_background.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/__init__.py
--rw-r--r--   0        0        0    23496 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/__main__.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/dictionaryAPI.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/setting.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.2/LICENSE
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 worddfn-0.1.2/README.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 worddfn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 worddfn-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0   137387 2020-02-02 00:00:00.000000 worddfn-0.1.3/images/logo/Black_logo-no_background.png
+-rwxr-xr-x   0        0        0   198761 2020-02-02 00:00:00.000000 worddfn-0.1.3/images/logo/Color_logo-no_background.png
+-rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 worddfn-0.1.3/images/logo/Color_logo-no_background_RM.png
+-rwxr-xr-x   0        0        0   151331 2020-02-02 00:00:00.000000 worddfn-0.1.3/images/logo/White_logo-no_background.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 worddfn-0.1.3/worddfn/__init__.py
+-rw-r--r--   0        0        0    23496 2020-02-02 00:00:00.000000 worddfn-0.1.3/worddfn/__main__.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 worddfn-0.1.3/worddfn/dictionaryAPI.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.3/worddfn/setting.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 worddfn-0.1.3/README.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 worddfn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 worddfn-0.1.3/PKG-INFO
```

### Comparing `worddfn-0.1.2/images/logo/Black_logo-no_background.png` & `worddfn-0.1.3/images/logo/Black_logo-no_background.png`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/images/logo/Color_logo-no_background.png` & `worddfn-0.1.3/images/logo/Color_logo-no_background.png`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/images/logo/Color_logo-no_background_RM.png` & `worddfn-0.1.3/images/logo/Color_logo-no_background_RM.png`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/images/logo/White_logo-no_background.png` & `worddfn-0.1.3/images/logo/White_logo-no_background.png`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/worddfn/__main__.py` & `worddfn-0.1.3/worddfn/__main__.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/worddfn/dictionaryAPI.py` & `worddfn-0.1.3/worddfn/dictionaryAPI.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/worddfn/setting.py` & `worddfn-0.1.3/worddfn/setting.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/LICENSE` & `worddfn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/README.md` & `worddfn-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-<img src= "./images/logo/Color_logo-no_background_RM.png" />  
+<img src= "https://github.com/SirX7/wordDFN/blob/main/images/logo/Color_logo-no_background_RM.png?raw=true" />  
 
 ## Search for definition with example, verbs, synonyms and antonyms of a given word. 
 <br/>
 </div>  
 
 # About wordDFN 
 worddfn is a wordnik API CLI client that uses the **[wordnik](https://developer.wordnik.com/)** API to retrieve data about a single word and parse it into the cli (terminal) for the user.
```

### Comparing `worddfn-0.1.2/pyproject.toml` & `worddfn-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.2/PKG-INFO` & `worddfn-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worddfn
-Version: 0.1.2
+Version: 0.1.3
 Summary: worddfn, lookup word meaning and forms via the wordnik api
 Project-URL: Homepage, https://github.com/SirX7/wordDFN
 Project-URL: Bug Tracker, https://github.com/SirX7/wordDFN/issues
 Author-email: Shall Mcfield <xhall.mc@protonmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: requests==2.30.0
 Description-Content-Type: text/markdown
 
 <div align="center">
-<img src= "./images/logo/Color_logo-no_background_RM.png" />  
+<img src= "https://github.com/SirX7/wordDFN/blob/main/images/logo/Color_logo-no_background_RM.png?raw=true" />  
 
 ## Search for definition with example, verbs, synonyms and antonyms of a given word. 
 <br/>
 </div>  
 
 # About wordDFN 
 worddfn is a wordnik API CLI client that uses the **[wordnik](https://developer.wordnik.com/)** API to retrieve data about a single word and parse it into the cli (terminal) for the user.
```

