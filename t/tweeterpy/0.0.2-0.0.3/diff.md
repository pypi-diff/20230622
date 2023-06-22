# Comparing `tmp/tweeterpy-0.0.2.tar.gz` & `tmp/tweeterpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.2.tar", last modified: Thu Jun 22 07:55:06 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.3.tar", last modified: Thu Jun 22 07:59:27 2023, max compression
```

## Comparing `tweeterpy-0.0.2.tar` & `tweeterpy-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3389 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-06-22 07:47:50.000000 tweeterpy-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.863202 tweeterpy-0.0.2/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.2/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.2/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      481 2023-06-22 07:37:42.000000 tweeterpy-0.0.2/tweeterpy/config.py
--rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.2/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-20 11:23:57.000000 tweeterpy-0.0.2/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.2/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0    20755 2023-06-21 13:16:47.000000 tweeterpy-0.0.2/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3259 2023-06-22 07:37:42.000000 tweeterpy-0.0.2/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      221 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.596127 tweeterpy-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:59:27.596127 tweeterpy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-06-22 07:57:46.000000 tweeterpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.3/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.3/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      481 2023-06-22 07:37:42.000000 tweeterpy-0.0.3/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.3/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-20 11:23:57.000000 tweeterpy-0.0.3/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.3/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0    20755 2023-06-21 13:16:47.000000 tweeterpy-0.0.3/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     3259 2023-06-22 07:37:42.000000 tweeterpy-0.0.3/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      221 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.2/LICENSE` & `tweeterpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/PKG-INFO` & `tweeterpy-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
-Home-page: https://github.com/iSarabjitDhiman/TwitterPy
+Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
-Keywords: twitterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
+Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.2 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.3 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
-TwitterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
-License: MIT Keywords: twitterpy,twitter scraper,tweet scraper,twitter data
+TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
+License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
```

### Comparing `tweeterpy-0.0.2/README.md` & `tweeterpy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/setup.py` & `tweeterpy-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
 
@@ -14,17 +14,17 @@
     version=VERSION,
     description=SHORT_DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Sarabjit Dhiman",
     author_email="hello@sarabjitdhiman.com",
     license="MIT",
-    url="https://github.com/iSarabjitDhiman/TwitterPy",
+    url="https://github.com/iSarabjitDhiman/TweeterPy",
     packages=["tweeterpy"],
-    keywords=["twitterpy", "twitter scraper", "tweet scraper",
+    keywords=["tweeterpy", "twitter scraper", "tweet scraper",
               "twitter data extraction", "twitter api",
               "twitter python", "tweet api", "tweetpy"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `tweeterpy-0.0.2/tweeterpy/api_util.py` & `tweeterpy-0.0.3/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy/constants.py` & `tweeterpy-0.0.3/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy/login_util.py` & `tweeterpy-0.0.3/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy/request_util.py` & `tweeterpy-0.0.3/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.3/tweeterpy/tweeterpy.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy/util.py` & `tweeterpy-0.0.3/tweeterpy/util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.2/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.3/tweeterpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
-Home-page: https://github.com/iSarabjitDhiman/TwitterPy
+Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
-Keywords: twitterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
+Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.2 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.3 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
-TwitterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
-License: MIT Keywords: twitterpy,twitter scraper,tweet scraper,twitter data
+TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
+License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
```

