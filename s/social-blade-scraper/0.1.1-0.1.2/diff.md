# Comparing `tmp/social-blade-scraper-0.1.1.tar.gz` & `tmp/social-blade-scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.1.1.tar", last modified: Thu Jun 22 08:31:10 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.1.2.tar", last modified: Thu Jun 22 12:14:18 2023, max compression
```

## Comparing `social-blade-scraper-0.1.1.tar` & `social-blade-scraper-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.1.1/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-22 08:30:06.000000 social-blade-scraper-0.1.1/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.976841 social-blade-scraper-0.1.1/src/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.1.1/src/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.976841 social-blade-scraper-0.1.1/src/social_blade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/__init__.py
--rw-rw-r--   0 tej       (1000) tej       (1000)     1757 2023-06-21 15:37:54.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/fetch.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/src/social_blade_scraper/stats/
--rw-rw-r--   0 tej       (1000) tej       (1000)    12699 2023-06-22 08:29:25.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/stats/youtube.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      427 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)      659 2023-06-22 08:25:36.000000 social-blade-scraper-0.1.1/tests/test_load.py
--rw-rw-r--   0 tej       (1000) tej       (1000)     2191 2023-06-22 08:29:42.000000 social-blade-scraper-0.1.1/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.1.2/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-22 12:13:40.000000 social-blade-scraper-0.1.2/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.137183 social-blade-scraper-0.1.2/src/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.1.2/src/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.1.2/src/social_blade_scraper/__init__.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)     1757 2023-06-21 15:37:54.000000 social-blade-scraper-0.1.2/src/social_blade_scraper/fetch.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/src/social_blade_scraper/stats/
+-rw-rw-r--   0 tej       (1000) tej       (1000)    13581 2023-06-22 12:13:35.000000 social-blade-scraper-0.1.2/src/social_blade_scraper/stats/youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 12:14:18.000000 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      427 2023-06-22 12:14:18.000000 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-22 12:14:18.000000 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-22 12:14:18.000000 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-22 12:14:18.000000 social-blade-scraper-0.1.2/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 12:14:18.141183 social-blade-scraper-0.1.2/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      659 2023-06-22 08:25:36.000000 social-blade-scraper-0.1.2/tests/test_load.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)     2191 2023-06-22 12:13:12.000000 social-blade-scraper-0.1.2/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.1.1/setup.py` & `social-blade-scraper-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.1.1",
+    version="0.1.2",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
```

### Comparing `social-blade-scraper-0.1.1/src/social_blade_scraper/fetch.py` & `social-blade-scraper-0.1.2/src/social_blade_scraper/fetch.py`

 * *Files identical despite different names*

### Comparing `social-blade-scraper-0.1.1/src/social_blade_scraper/stats/youtube.py` & `social-blade-scraper-0.1.2/src/social_blade_scraper/stats/youtube.py`

 * *Files 12% similar despite different names*

```diff
@@ -182,36 +182,46 @@
         )
 
         data.append(record)
 
     return data
 
 
-async def fetch_homepage(channel_name: str) -> Union[str, None]:
+async def fetch_homepage(channel_identifier: str, is_username: bool = False) -> Union[str, None]:
     """
     Returns home page source code
 
-    :param channel_name: YouTube channel name
+    :param is_username: is identifier username
+    :param channel_identifier: YouTube channel name
     :return: Union[str, None]
     """
-    target_url = f'https://socialblade.com/youtube/c/{channel_name}'
+    if is_username:
+        target_url = f'https://socialblade.com/youtube/c/{channel_identifier}'
+    else:
+        target_url = f'https://socialblade.com/youtube/channel/{channel_identifier}'
+
     response = await fetch(target_url)
 
     if response.status_code == 200:
         return response.text
 
 
-async def fetch_monthly_page(channel_name: str) -> Union[str, None]:
+async def fetch_monthly_page(channel_name: str, is_username: bool) -> Union[str, None]:
     """ Returns source code of monthly stats page
 
+    :param is_username: is identifier username
     :param channel_name: YouTube channel name
     :return: Union[str, None]
     """
 
-    target_url = f'https://socialblade.com/youtube/c/{channel_name}/monthly'
+    if is_username:
+        target_url = f'https://socialblade.com/youtube/c/{channel_name}/monthly'
+    else:
+        target_url = f'https://socialblade.com/youtube/channel/{channel_name}/monthly'
+
     response = await fetch(target_url)
 
     if response.status_code == 200:
         return response.text
 
 
 def total_uploads_search(soup: BeautifulSoup) -> Union[int, None]:
@@ -296,23 +306,24 @@
     if tag:
         category = tag.text.strip()
 
     if category:
         return category
 
 
-async def home_page_scrape(channel_name: str, channel: YouTubeChannel) -> bool:
+async def home_page_scrape(identifier: str, channel: YouTubeChannel, is_username: bool) -> bool:
     """
     Returns True if home page is scraped successfully else false
-    :param channel_name: YouTube channel name
+    :param is_username:
+    :param identifier: YouTube channel name
     :param channel: temporary channel instance to store information
     :return: bool
     """
 
-    code = await fetch_homepage(channel_name)
+    code = await fetch_homepage(identifier, is_username)
     if not code:
         return False
 
     soup = BeautifulSoup(code, 'html.parser')
 
     channel.date_created = date_created_search(soup)
 
@@ -332,52 +343,58 @@
     channel.total_uploads = total_uploads_search(soup)
     channel.total_subscribers = total_subscribers_search(soup)
     channel.total_views = total_views_search(soup)
     channel.country = country_search(soup)
     return True
 
 
-async def daily_stats_scrape(channel_name: str) -> List[DailyStat]:
+async def daily_stats_scrape(identifier: str, is_username: bool) -> List[DailyStat]:
     """
     Returns  30 days daily stats
 
-    :param channel_name: YouTube channel name
+    :param is_username: is channel username
+    :param identifier: YouTube channel name
     :return:
     """
 
-    code = await fetch_monthly_page(channel_name)
+    code = await fetch_monthly_page(identifier, is_username)
     if not code:
         return []
 
     soup = BeautifulSoup(code, 'html.parser')
     return daily_stats_search(soup)
 
 
-async def social_blade_scrape(channel_name: str) -> Union[YouTubeChannel, None]:
+async def social_blade_scrape(identifier: str, is_username: bool) -> Union[YouTubeChannel, None]:
     # Create a BeautifulSoup object with the HTML content
 
     channel = YouTubeChannel()
-    scrape_tasks = await asyncio.gather(home_page_scrape(channel_name, channel), daily_stats_scrape(channel_name))
+    scrape_tasks = await asyncio.gather(home_page_scrape(identifier, channel, is_username),
+                                        daily_stats_scrape(identifier, is_username))
     home_page_scrape_future, daily_stats_scrape_future, = scrape_tasks
 
     # Check if the home page is scraped successfully
     if not home_page_scrape_future:
         # Maybe got 404 status because channel don't exist or something went wrong
         return None
 
     channel.daily_stats = daily_stats_scrape_future
     return channel
 
 
-def get_username_from_url(url: str) -> Union[str, None]:
+def get_user_identifier(url: str) -> Union[Tuple[bool, str], None]:
     # Example YouTube channel link: https://www.youtube.com/@MrFeast
     url_split = url.split('@')
 
-    if len(url_split) > 0:
-        return url_split[-1]
+    if len(url_split) > 1:
+        return True, url_split[-1]
+
+    url_split = url.split('/')
+    if len(url_split) > 1:
+        return False, url_split[-1]
 
 
 async def youtube(url: str = None, channel_name: str = None) -> Union[YouTubeChannel, None]:
     """
     Priority order: channel_name, url
     Start scraping social blade easily.
 
@@ -398,22 +415,29 @@
     :param channel_name: YouTube channel name
     :return: Union[YouTubeChannel, None]
     """
 
     if not (url or channel_name):
         return None
 
+    identifier = channel_name
+    is_username = True
+
     if url:
         # Extract username from URL
-        channel_name = get_username_from_url(url)
+        channel_details = get_user_identifier(url)
+        if not channel_details:
+            return None
+
+        is_username, identifier = channel_details
 
-    if not channel_name:
+    if not identifier:
         return None
 
-    return await social_blade_scrape(channel_name)
+    return await social_blade_scrape(identifier, is_username)
 
 
 def subscribers_count_access_tokens_search(soup: BeautifulSoup) -> Union[Tuple[str, str], None]:
     """
     Finds tokens to access subscribers count page
 
     :param soup: BeautifulSoup object
```

### Comparing `social-blade-scraper-0.1.1/tests/test_load.py` & `social-blade-scraper-0.1.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `social-blade-scraper-0.1.1/tests/test_youtube.py` & `social-blade-scraper-0.1.2/tests/test_youtube.py`

 * *Files identical despite different names*

