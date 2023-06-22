# Comparing `tmp/instagpy-0.1.7.tar.gz` & `tmp/instagpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.7.tar", last modified: Thu Jun 15 06:13:21 2023, max compression
+gzip compressed data, was "instagpy-0.1.8.tar", last modified: Thu Jun 22 07:19:41 2023, max compression
```

## Comparing `instagpy-0.1.7.tar` & `instagpy-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.587460 instagpy-0.1.7/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3318 2023-06-15 06:13:21.587460 instagpy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.571818 instagpy-0.1.7/instagpy/
--rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.7/instagpy/__init__.py
--rw-rw-rw-   0        0        0      685 2023-06-15 05:59:08.000000 instagpy-0.1.7/instagpy/config.py
--rw-rw-rw-   0        0        0    24200 2023-06-15 06:06:38.000000 instagpy-0.1.7/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2140 2023-06-14 13:31:23.000000 instagpy-0.1.7/instagpy/path.py
--rw-rw-rw-   0        0        0     1332 2023-06-15 05:49:06.000000 instagpy-0.1.7/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.7/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.7/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.587460 instagpy-0.1.7/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 06:13:21.587460 instagpy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-06-15 06:12:37.000000 instagpy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.859039 instagpy-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3572 2023-06-22 07:19:41.859039 instagpy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-22 07:00:19.000000 instagpy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.843408 instagpy-0.1.8/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.8/instagpy/__init__.py
+-rw-rw-rw-   0        0        0      974 2023-06-22 07:17:43.000000 instagpy-0.1.8/instagpy/config.py
+-rw-rw-rw-   0        0        0    24516 2023-06-22 06:11:52.000000 instagpy-0.1.8/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2140 2023-06-14 13:31:23.000000 instagpy-0.1.8/instagpy/path.py
+-rw-rw-rw-   0        0        0     1421 2023-06-21 13:28:30.000000 instagpy-0.1.8/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.8/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.8/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.859039 instagpy-0.1.8/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3572 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:19:41.859039 instagpy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-22 07:19:09.000000 instagpy-0.1.8/setup.py
```

### Comparing `instagpy-0.1.7/LICENSE` & `instagpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.7/PKG-INFO` & `instagpy-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
@@ -50,15 +50,15 @@
 ```
 
 OR
 
 ```python
 from instagpy import InstaGPy
 
-InstaGPy(proxies=proxies, max_retries=3, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
+InstaGPy(use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
 ```
 
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
@@ -70,14 +70,30 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](instagpy/docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from instagpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](instagpy/docs/config.md)
+
 ## Features
 
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details along with Contact Details (Phone, WhatsApp, Email & Address)
 - Extracts Instagram Profile Media
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.7 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.8 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -22,20 +22,22 @@
  Profiles. Scrape data from user's profile like username, userid, bio, email,
 phone, followers/followings list, profile media, account_type, etc. > _Note_ :
 `Use it on Your Own Risk. Scraping with Residential proxies is advisable while
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
-    from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
-        use_mutiple_account=False, session_ids=None, min_requests=None,
-    max_requests=None) ``` > ### Example - Get Basic User Details of a User
-          ```python from instagpy import InstaGPy insta = InstaGPy()
-   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
-  Documentation Check out step by step guide. [Documentation](instagpy/docs/
-docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
- Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
-       Email & Address) - Extracts Instagram Profile Media ## Authors -
- [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
-   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
-   contact me on Social Media @iSarabjitDhiman ## Support For support, email
-                           hello@sarabjitdhiman.com
+       from instagpy import InstaGPy InstaGPy(use_mutiple_account=False,
+session_ids=None, min_requests=None, max_requests=None) ``` > ### Example - Get
+ Basic User Details of a User ```python from instagpy import InstaGPy insta =
+ InstaGPy() insta.get_user_basic_details('champagnepapi',print_formatted=True)
+ ``` ## Documentation Check out step by step guide. [Documentation](instagpy/
+  docs/docs.md) ## Configuration > ### Example - Config Usage ```python from
+instagpy import config config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+    config.TIMEOUT = 10 ``` Check out configuration docs for the available
+  settings. [Configurations](instagpy/docs/config.md) ## Features - Extracts
+User's Followers - Extracts User's Followings - Extracts User's Profile Details
+   along with Contact Details (Phone, WhatsApp, Email & Address) - Extracts
+Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.7/README.md` & `instagpy-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```
 
 OR
 
 ```python
 from instagpy import InstaGPy
 
-InstaGPy(proxies=proxies, max_retries=3, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
+InstaGPy(use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
 ```
 
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
@@ -48,14 +48,30 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](instagpy/docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from instagpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](instagpy/docs/config.md)
+
 ## Features
 
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details along with Contact Details (Phone, WhatsApp, Email & Address)
 - Extracts Instagram Profile Media
```

#### html2text {}

```diff
@@ -7,20 +7,22 @@
  Profiles. Scrape data from user's profile like username, userid, bio, email,
 phone, followers/followings list, profile media, account_type, etc. > _Note_ :
 `Use it on Your Own Risk. Scraping with Residential proxies is advisable while
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
-    from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
-        use_mutiple_account=False, session_ids=None, min_requests=None,
-    max_requests=None) ``` > ### Example - Get Basic User Details of a User
-          ```python from instagpy import InstaGPy insta = InstaGPy()
-   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
-  Documentation Check out step by step guide. [Documentation](instagpy/docs/
-docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
- Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
-       Email & Address) - Extracts Instagram Profile Media ## Authors -
- [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
-   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
-   contact me on Social Media @iSarabjitDhiman ## Support For support, email
-                           hello@sarabjitdhiman.com
+       from instagpy import InstaGPy InstaGPy(use_mutiple_account=False,
+session_ids=None, min_requests=None, max_requests=None) ``` > ### Example - Get
+ Basic User Details of a User ```python from instagpy import InstaGPy insta =
+ InstaGPy() insta.get_user_basic_details('champagnepapi',print_formatted=True)
+ ``` ## Documentation Check out step by step guide. [Documentation](instagpy/
+  docs/docs.md) ## Configuration > ### Example - Config Usage ```python from
+instagpy import config config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+    config.TIMEOUT = 10 ``` Check out configuration docs for the available
+  settings. [Configurations](instagpy/docs/config.md) ## Features - Extracts
+User's Followers - Extracts User's Followings - Extracts User's Profile Details
+   along with Contact Details (Phone, WhatsApp, Email & Address) - Extracts
+Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.7/instagpy/instagpy.py` & `instagpy-0.1.8/instagpy/instagpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from . import utils
 from . import path
 from .request_util import make_request
 
 
 class InstaGPy:
 
-    def __init__(self, max_retries=None, proxies=None, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None, timeout=None):
+    def __init__(self, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None):
         """
 
         Args:
-            max_retries (int, optional): Number of retires for each request. Defaults to None.
-            proxies (dict, optional): Proxies as a dictionary {'http': proxy_here,'https':proxy_here}. Residential Proxies are recommended. Defaults to None.
             use_mutiple_account (bool, optional): Set to True if want to scrape data with mutiple account sessions So that you don't get blocked. Defaults to False.
             session_ids (list, optional): List of Session IDs from Cookies. Applicable only if use_mutiple_accounts is True. Defaults to False.
             min_requests (int, optional): Minimum requests to make before shuffling a session ID. Defaults to None.
             max_requests (int, optional): Maximum requests to make before shuffling a session ID. Defaults to None.
             timeout (int, optional): Request timeout. Defaults to None.
         """
         if use_mutiple_account and not session_ids:
@@ -35,17 +33,14 @@
             self.min_requests = min_requests or config.MIN_REQUESTS
             self.max_requests = max_requests or config.MAX_REQUESTS
             self.shuffle_session_after = random.randint(
                 self.min_requests, self.max_requests)
             self.session_ids_container = None
         self.session_ids = session_ids
         self.use_mutiple_account = use_mutiple_account
-        self.max_retries = max_retries or config.MAX_RETRIES
-        self.timeout = timeout or config.TIMEOUT
-        self.proxies = proxies
         self.generate_session()
 
     @property
     def me(self):
         """Returns Logged in User Information.
 
         Returns:
@@ -56,32 +51,30 @@
 
     def _get_meta_data(self):
         """Returns Browser's and User's Meta Data.
 
         Returns:
             dict: Meta Data.
         """
-        response = make_request(
-            path.META_DATA_URL, session=self.session, max_retries=self.max_retries)
+        response = make_request(path.META_DATA_URL)
         return response
 
     def generate_session(self, session_id=None):
         """Generates Required Headers and Cookies. OR Generates Session from an existing Session ID.
 
         Args:
             session_id (str, optional): Session Id from Instagram Session Cookies. Defaults to None.
         """
         self.session = requests.Session()
-        if self.proxies is not None:
-            self.session.proxies = self.proxies
+        if config.PROXY is not None:
+            self.session.proxies = config.PROXY
             self.session.verify = False
         self.session.headers.update(
-            {"User-Agent": random.choice(config.USER_AGENTS)})
-        make_request(path.BASE_URL, session=self.session,
-                     max_retries=self.max_retries)
+            {"User-Agent": random.choice(config._USER_AGENTS)})
+        make_request(path.BASE_URL, session=self.session)
         response = requests.get(path.LOGIN_URL)
         if not response.cookies:
             for _ in range(self.max_retries):
                 response = self.session.get(path.LOGIN_URL)
                 if response.cookies:
                     break
         csrf_token = dict(response.cookies)["csrftoken"]
@@ -92,14 +85,15 @@
             # load an existing session with session_id
             self.session.cookies.update({'sessionid': session_id})
 
         try:
             self.me
         except:
             pass
+        config._DEFAULT_SESSION = self.session
         return self.session
 
     def shuffle_session(self, ignore_requests_limit=False):
         """Shuffle session/cookies. Takes a new session ID from self.session_ids if using with mutiple accounts.
 
         Args:
             ignore_requests_limit (bool, optional): Set to True to shuffle session manually regardless of min/max number of requests. Defaults to False.
@@ -191,53 +185,79 @@
         payload = {
             'username': username,
             'enc_password': f'#PWD_INSTAGRAM_BROWSER:0:{timestamp}:{password}',
             'queryParams': {},
             'optIntoOneTap': 'false',
             'trustedDeviceRecords': {}
         }
-        response = self.session.post(path.LOGIN_URL, data=payload).json()
+        user = self.session.post(path.LOGIN_URL, data=payload).json()
         try:
-            if response["authenticated"]:
-                print("\nSuccessfully Logged In....")
+            if user["authenticated"]:
+                user_id = user["userId"]
+                # test if the account is working
+                user = self.session.get(
+                    path.USER_DATA_ENDPOINT.format(user_id)).json()
+                if user['status'] != 'ok':
+                    raise Exception(
+                        f"Not Working! Check if the given account is working.")
+                user_fullname = user['user']['full_name']
+                print(f"{user_fullname} : Successfully Logged In....")
                 if save_session:
                     session_util.save_session(
                         session=self.session, filename=username)
                 return
             raise Exception("Couldn't LogIn, Try again...")
-        except Exception as e:
-            print('\n', e)
-            return response
+        except Exception as error:
+            print('\n', error)
+            utils.check_for_errors(user)
 
     def logged_in(self):
         """Check if user is logged in.
 
         Returns:
             bool: Returns True if user is logged in.
         """
         if 'sessionid' in self.session.cookies.keys():
             return True
         return False
 
+    def get_session_id(self, username=None, password=None, new_session=False):
+        """Get sessionID of the current session OR a new login session. By default returns current one if logged in.
+
+        Args:
+            username (str): Username OR Email.
+            password (str): Password
+            new_session (bool, optional): Set to True if want to get session ID of new session. Otherwise It will return the already logged In session ID. Defaults to False.
+
+        Returns:
+            str: Session ID.
+        """
+        if new_session:
+            self.generate_session()
+            self.login(username, password)
+        if self.logged_in():
+            return self.session.cookies['sessionid']
+        raise Exception(
+            "You are not logged In. Set new_session=True to generate a new session.")
+
     def get_user_id(self, username):
         if isinstance(username, int) or username.isnumeric():
             return username
         return self.get_user_info(username)['data']['user']['id']
 
     def get_user_info(self, username):
         """Extracts user details.
 
         Args:
             username (str): Instagram username.
 
         Returns:
             dict: user info like username,id,bio,follower/following count etc.
         """
-        response = make_request(path.USER_PROFILE_ENDPOINT.format(
-            username), session=self.session, max_retries=self.max_retries)
+        response = make_request(path.USER_PROFILE_ENDPOINT.format(username))
         self.shuffle_session()
         return response
 
     def get_user_data(self, user_id):
         """Extracts user details. With Contact Info Like email, phone and address.
 
         Args:
@@ -246,16 +266,15 @@
         Returns:
             dict: user info along with contact info.
         """
         # returns almost as same data as get_user_info method Except this one returns contact info (email/phone) as well. |LOGIN REQUIRED|
         if not self.logged_in():
             self.login()
         user_id = self.get_user_id(user_id)
-        response = make_request(path.USER_DATA_ENDPOINT.format(
-            user_id), session=self.session, max_retries=self.max_retries)
+        response = make_request(path.USER_DATA_ENDPOINT.format(user_id))
         self.shuffle_session()
         return response
 
     def get_user_basic_details(self, username=None, print_formatted=False):
         """Get a brief overview of an Instagram Profile.
 
         Args:
@@ -323,16 +342,15 @@
                 elif followings_list:
                     url = path.USER_FOLLOWINGS_ENDPOINT.format(user['id'])
                     max_data = 200
                 query_params = self.generate_query(
                     count=max_data, end_cursor=end_cursor)
 
             try:
-                response = make_request(
-                    url, params=query_params, session=self.session, max_retries=self.max_retries)
+                response = make_request(url, params=query_params)
                 if followers_list and user['is_verified']:
                     data = response['data']['user']['edge_followed_by']
                     has_next_page = data['page_info']['has_next_page']
                     end_cursor = data['page_info']['end_cursor']
                     data = data['edges']
                 else:
                     data = response['users']
@@ -397,15 +415,15 @@
         print(f'Started at : {utils.format_datetime(time.time())}\n')
         try:
             while True:
                 query_params = self.generate_query(
                     query=path.USER_FEED_QUERY, user_id=user_id, count=50, end_cursor=end_cursor, is_graphql=True)
                 try:
                     response = make_request(
-                        path.GRAPHQL_URL, params=query_params, session=self.session, max_retries=self.max_retries)
+                        path.GRAPHQL_URL, params=query_params)
                     data = response['data']['user']['edge_owner_to_timeline_media']
                     posts_count = data['count']
                     has_next_page = data['page_info']['has_next_page']
                     cursor = data['page_info']['end_cursor']
                     if cursor:
                         end_cursor = cursor
                     user_posts_data.extend(filter_by_date(data['edges']))
@@ -441,16 +459,15 @@
         Returns:
             dict: All the details like post_id,datetime,caption,url,location etc.
         """
         post_id = utils.get_post_id(post_url)
         url = path.GRAPHQL_URL
         query_params = self.generate_query(
             query=path.POST_DETAILS_QUERY, shortcode=post_id, is_graphql=True)
-        response = make_request(
-            url, params=query_params, session=self.session, max_retries=self.max_retries)
+        response = make_request(url, params=query_params)
         self.shuffle_session()
         return response
 
     def get_media_url(self, response):
         """Extracts High Resolution/Quality Media URL from post details response returned from get_post_details method.
 
         Args:
@@ -480,26 +497,26 @@
             dict: User About Dataset.
         """
         if not self.logged_in():
             self.login()
         user_id = self.get_user_id(username)
         data = {'referer_type': 'ProfileUsername', 'target_user_id': user_id, 'bk_client_context': {
             'bloks_version': path.ABOUT_USER_QUERY, 'style_id': 'instagram'}, 'bloks_versioning_id': path.ABOUT_USER_QUERY}
-        response = make_request(path.ABOUT_USER_URL, method='POST', data=data,
-                                session=self.session, max_retries=self.max_retries)
+        response = make_request(path.ABOUT_USER_URL, method='POST', data=data)
         if print_formatted:
             return utils.format_about_data(response)
         self.shuffle_session()
         return response
 
     def get_hashtag_posts(self, hashtag=None, end_cursor=None, max=None):
         """Get media posts from hashtags.
 
         Args:
-            hashtag (str): Hashtag that you want to extract data from. Accepts both formats i.e. hashtag or #hashtag. Defaults to None.
+            # hashtag. Defaults to None.
+            hashtag (str): Hashtag that you want to extract data from. Accepts both formats i.e. hashtag or
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             max (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
 
         Returns:
             dict: Hashtag posts data.
         """
         if hashtag is None:
@@ -512,16 +529,15 @@
         max_data = 50
         print(f'Started at : {utils.format_datetime(time.time())}\n')
         while True:
             query_params = self.generate_query(
                 query=path.HASHTAG_QUERY, hashtag=hashtag, count=max_data, end_cursor=end_cursor, is_graphql=True)
 
             try:
-                response = make_request(
-                    url, params=query_params, session=self.session, max_retries=self.max_retries)
+                response = make_request(url, params=query_params)
                 data = response['data']['hashtag']['edge_hashtag_to_media']
                 has_next_page = data['page_info']['has_next_page']
                 end_cursor = data['page_info']['end_cursor']
                 count = data['count']
                 data = data['edges']
 
                 hashtag_posts.extend(data)
```

### Comparing `instagpy-0.1.7/instagpy/path.py` & `instagpy-0.1.8/instagpy/path.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.7/instagpy/session_util.py` & `instagpy-0.1.8/instagpy/session_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.7/instagpy/utils.py` & `instagpy-0.1.8/instagpy/utils.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.7/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.8/instagpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
@@ -50,15 +50,15 @@
 ```
 
 OR
 
 ```python
 from instagpy import InstaGPy
 
-InstaGPy(proxies=proxies, max_retries=3, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
+InstaGPy(use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None)
 ```
 
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
@@ -70,14 +70,30 @@
 
 ## Documentation
 
 Check out step by step guide.
 
 [Documentation](instagpy/docs/docs.md)
 
+## Configuration
+
+> ### Example - Config Usage
+
+```python
+from instagpy import config
+
+config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+config.TIMEOUT = 10
+
+```
+
+Check out configuration docs for the available settings.
+
+[Configurations](instagpy/docs/config.md)
+
 ## Features
 
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details along with Contact Details (Phone, WhatsApp, Email & Address)
 - Extracts Instagram Profile Media
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.7 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.8 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -22,20 +22,22 @@
  Profiles. Scrape data from user's profile like username, userid, bio, email,
 phone, followers/followings list, profile media, account_type, etc. > _Note_ :
 `Use it on Your Own Risk. Scraping with Residential proxies is advisable while
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
-    from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
-        use_mutiple_account=False, session_ids=None, min_requests=None,
-    max_requests=None) ``` > ### Example - Get Basic User Details of a User
-          ```python from instagpy import InstaGPy insta = InstaGPy()
-   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
-  Documentation Check out step by step guide. [Documentation](instagpy/docs/
-docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
- Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
-       Email & Address) - Extracts Instagram Profile Media ## Authors -
- [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
-   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
-   contact me on Social Media @iSarabjitDhiman ## Support For support, email
-                           hello@sarabjitdhiman.com
+       from instagpy import InstaGPy InstaGPy(use_mutiple_account=False,
+session_ids=None, min_requests=None, max_requests=None) ``` > ### Example - Get
+ Basic User Details of a User ```python from instagpy import InstaGPy insta =
+ InstaGPy() insta.get_user_basic_details('champagnepapi',print_formatted=True)
+ ``` ## Documentation Check out step by step guide. [Documentation](instagpy/
+  docs/docs.md) ## Configuration > ### Example - Config Usage ```python from
+instagpy import config config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
+    config.TIMEOUT = 10 ``` Check out configuration docs for the available
+  settings. [Configurations](instagpy/docs/config.md) ## Features - Extracts
+User's Followers - Extracts User's Followings - Extracts User's Profile Details
+   along with Contact Details (Phone, WhatsApp, Email & Address) - Extracts
+Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://www.github.com/
+ iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
+ at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
+             Support For support, email hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.7/setup.py` & `instagpy-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

