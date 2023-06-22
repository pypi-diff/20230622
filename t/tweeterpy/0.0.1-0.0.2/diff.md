# Comparing `tmp/tweeterpy-0.0.1.tar.gz` & `tmp/tweeterpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.1.tar", last modified: Tue Jun 20 15:32:55 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.2.tar", last modified: Thu Jun 22 07:55:06 2023, max compression
```

## Comparing `tweeterpy-0.0.1.tar` & `tweeterpy-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:32:55.479891 tweeterpy-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3100 2023-06-20 15:32:55.479891 tweeterpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2023-06-20 15:07:32.000000 tweeterpy-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 15:32:55.479891 tweeterpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-06-20 15:32:43.000000 tweeterpy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:32:55.464250 tweeterpy-0.0.1/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.1/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.1/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      302 2023-06-20 11:28:45.000000 tweeterpy-0.0.1/tweeterpy/config.py
--rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.1/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-20 11:23:57.000000 tweeterpy-0.0.1/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.1/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0    20627 2023-06-20 15:06:49.000000 tweeterpy-0.0.1/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3258 2023-06-20 11:31:40.000000 tweeterpy-0.0.1/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:32:55.479891 tweeterpy-0.0.1/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3100 2023-06-20 15:32:55.000000 tweeterpy-0.0.1/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-20 15:32:55.000000 tweeterpy-0.0.1/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:32:55.000000 tweeterpy-0.0.1/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      221 2023-06-20 15:32:55.000000 tweeterpy-0.0.1/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 15:32:55.000000 tweeterpy-0.0.1/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-06-22 07:47:50.000000 tweeterpy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.863202 tweeterpy-0.0.2/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.2/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.2/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      481 2023-06-22 07:37:42.000000 tweeterpy-0.0.2/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.2/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-20 11:23:57.000000 tweeterpy-0.0.2/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.2/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0    20755 2023-06-21 13:16:47.000000 tweeterpy-0.0.2/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     3259 2023-06-22 07:37:42.000000 tweeterpy-0.0.2/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:55:06.878817 tweeterpy-0.0.2/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      221 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 07:55:06.000000 tweeterpy-0.0.2/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.1/LICENSE` & `tweeterpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.1/PKG-INFO` & `tweeterpy-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TwitterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: twitterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -70,21 +70,37 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from tweeterpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](docs/config.md)
+
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media
+- Extracts Twitter Profile Media and so on.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.1 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.2 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TwitterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: twitterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
@@ -24,13 +24,17 @@
 scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.`
  **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._** ## Installation
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
- [Documentation](docs/docs.md) ## Features - Extracts Tweets - Extracts User's
-  Followers - Extracts User's Followings - Extracts User's Profile Details -
-    Extracts Twitter Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+  [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
+        ```python from tweeterpy import config config.PROXY = {"http":
+      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
+configuration docs for the available settings. [Configurations](docs/config.md)
+  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
+ Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
+      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

### Comparing `tweeterpy-0.0.1/README.md` & `tweeterpy-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -48,21 +48,37 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from tweeterpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](docs/config.md)
+
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media
+- Extracts Twitter Profile Media and so on.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -10,13 +10,17 @@
 scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.`
  **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._** ## Installation
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
- [Documentation](docs/docs.md) ## Features - Extracts Tweets - Extracts User's
-  Followers - Extracts User's Followings - Extracts User's Profile Details -
-    Extracts Twitter Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+  [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
+        ```python from tweeterpy import config config.PROXY = {"http":
+      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
+configuration docs for the available settings. [Configurations](docs/config.md)
+  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
+ Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
+      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

### Comparing `tweeterpy-0.0.1/setup.py` & `tweeterpy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-0.0.1/tweeterpy/api_util.py` & `tweeterpy-0.0.2/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.1/tweeterpy/constants.py` & `tweeterpy-0.0.2/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.1/tweeterpy/login_util.py` & `tweeterpy-0.0.2/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.1/tweeterpy/request_util.py` & `tweeterpy-0.0.2/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.1/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.2/tweeterpy/tweeterpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 
             except Exception as error:
                 print(error)
                 return data_container
 
     def generate_session(self):
         self.session = requests.Session()
+        if config.PROXY is not None:
+            self.session.proxies = config.PROXY
+            self.session.verify = False
         self.session.headers.update(util.generate_headers())
         make_request(Path.BASE_URL, session=self.session)
         guest_token = make_request(
             Path.GUEST_TOKEN_URL, method="POST", session=self.session)['guest_token']
         self.session.headers.update({'X-Guest-Token': guest_token})
         self.session.cookies.update({'gt': guest_token})
         config._DEFAULT_SESSION = self.session
```

### Comparing `tweeterpy-0.0.1/tweeterpy/util.py` & `tweeterpy-0.0.2/tweeterpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def generate_headers():
     headers = {"Authority": Path.DOMAIN,
                "Accept-Encoding": "gzip, deflate, br",
                "Accept-Language": "en-US,en;q=0.9",
                "Authorization": PUBLIC_TOKEN,
                "Cache-Control": "no-cache",
                "Referer": Path.BASE_URL,
-               "User-Agent": config.USER_AGENT,
+               "User-Agent": config._USER_AGENT,
                "X-Twitter-Active-User": "yes",
                "X-Twitter-Client-Language": "en"
                }
     return headers
 
 
 def generate_features(default_features=True, user_data_features=False, user_info_feautres=False, additional_features=False):
```

### Comparing `tweeterpy-0.0.1/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.2/tweeterpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TwitterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: twitterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -70,21 +70,37 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from tweeterpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](docs/config.md)
+
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media
+- Extracts Twitter Profile Media and so on.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.1 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.2 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TwitterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: twitterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
@@ -24,13 +24,17 @@
 scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.`
  **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._** ## Installation
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
- [Documentation](docs/docs.md) ## Features - Extracts Tweets - Extracts User's
-  Followers - Extracts User's Followings - Extracts User's Profile Details -
-    Extracts Twitter Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+  [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
+        ```python from tweeterpy import config config.PROXY = {"http":
+      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
+configuration docs for the available settings. [Configurations](docs/config.md)
+  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
+ Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
+      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

