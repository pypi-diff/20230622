# Comparing `tmp/social-blade-scraper-0.1.0.tar.gz` & `tmp/social-blade-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.1.0.tar", last modified: Wed Jun 21 10:58:11 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.1.1.tar", last modified: Thu Jun 22 08:31:10 2023, max compression
```

## Comparing `social-blade-scraper-0.1.0.tar` & `social-blade-scraper-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.1.0/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-21 10:57:30.000000 social-blade-scraper-0.1.0/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.448656 social-blade-scraper-0.1.0/src/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.1.0/src/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.448656 social-blade-scraper-0.1.0/src/social_blade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.1.0/src/social_blade_scraper/__init__.py
--rw-rw-r--   0 tej       (1000) tej       (1000)      894 2023-06-21 10:53:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper/fetch.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/src/social_blade_scraper/stats/
--rw-rw-r--   0 tej       (1000) tej       (1000)    12316 2023-06-21 09:24:07.000000 social-blade-scraper-0.1.0/src/social_blade_scraper/stats/youtube.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:58:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      408 2023-06-21 10:58:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-21 10:58:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-21 10:58:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-21 10:58:11.000000 social-blade-scraper-0.1.0/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:58:11.452656 social-blade-scraper-0.1.0/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)     1923 2023-06-21 09:08:45.000000 social-blade-scraper-0.1.0/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.1.1/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-22 08:30:06.000000 social-blade-scraper-0.1.1/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.976841 social-blade-scraper-0.1.1/src/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.1.1/src/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.976841 social-blade-scraper-0.1.1/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/__init__.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)     1757 2023-06-21 15:37:54.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/fetch.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/src/social_blade_scraper/stats/
+-rw-rw-r--   0 tej       (1000) tej       (1000)    12699 2023-06-22 08:29:25.000000 social-blade-scraper-0.1.1/src/social_blade_scraper/stats/youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      427 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-22 08:31:10.000000 social-blade-scraper-0.1.1/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-22 08:31:10.984841 social-blade-scraper-0.1.1/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      659 2023-06-22 08:25:36.000000 social-blade-scraper-0.1.1/tests/test_load.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)     2191 2023-06-22 08:29:42.000000 social-blade-scraper-0.1.1/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.1.0/setup.py` & `social-blade-scraper-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.1.0",
+    version="0.1.1",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
```

### Comparing `social-blade-scraper-0.1.0/src/social_blade_scraper/stats/youtube.py` & `social-blade-scraper-0.1.1/src/social_blade_scraper/stats/youtube.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 @dataclass
 class YouTubeChannel:
     """
     A data class to hold YouTubeChannel information
     """
 
     identifier: str = None
+    name: str = None
     profile: str = None
     banner: str = None
     category: str = None
     estimated_monthly_earning: str = None
     estimated_yearly_earning: str = None
     total_uploads: int = None
     total_subscribers: int = None
@@ -62,14 +63,27 @@
     """
 
     tag = soup.select_one('#fav-bubble')
     if tag:
         return tag['class'][0]
 
 
+def channel_name_search(soup: BeautifulSoup) -> Union[str, None]:
+    """
+    Logic to search channel name
+
+    :param soup: BeautifulSoup object
+    :return: str
+    """
+
+    tag = soup.select_one('h1')
+    if tag:
+        return tag.text.strip()
+
+
 def profile_search(soup: BeautifulSoup) -> Union[str, None]:
     """
     Logic to search profile url
 
     :param soup: BeautifulSoup object
     :return: str
     """
@@ -273,16 +287,21 @@
        Logic to search channel category
 
        :param soup: BeautifulSoup object
        :return: str
        """
 
     tag = soup.select_one('#youtube-stats-header-channeltype')
+    category = None
+
     if tag:
-        return tag.text.strip()
+        category = tag.text.strip()
+
+    if category:
+        return category
 
 
 async def home_page_scrape(channel_name: str, channel: YouTubeChannel) -> bool:
     """
     Returns True if home page is scraped successfully else false
     :param channel_name: YouTube channel name
     :param channel: temporary channel instance to store information
@@ -300,14 +319,15 @@
     # Check if the page has date created information. If the page don't have, stop scanning further
     if not channel.date_created:
         # Using date_created field as a primary source to check whether the page
         # is valid or not
         return False
 
     channel.identifier = identifier_search(soup)
+    channel.name = channel_name_search(soup)
     channel.profile = profile_search(soup)
     channel.category = channel_category_search(soup)
     channel.banner = f'https://www.banner.yt/{channel.identifier}'
     channel.estimated_monthly_earning = estimated_monthly_earnings_search(soup)
     channel.estimated_yearly_earning = estimated_yearly_earnings_search(soup)
     channel.total_uploads = total_uploads_search(soup)
     channel.total_subscribers = total_subscribers_search(soup)
```

### Comparing `social-blade-scraper-0.1.0/tests/test_youtube.py` & `social-blade-scraper-0.1.1/tests/test_youtube.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import random
 import sys
 import os
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 from src.social_blade_scraper.stats.youtube import youtube, subscribers_count_access_tokens, live_subscriber_count
 
@@ -10,14 +11,15 @@
 target_channel = input('Type here: ')
 
 
 # target_channel = 'mrfeast'
 
 
 async def show_basic():
+    await asyncio.sleep(random.randint(1, 3))
     channel = await youtube(channel_name=target_channel)
     if not channel:
         print('Channel don\'t exist')
         return
 
     print('-------------------------------------------------------')
     print('Monthly earnings: ', channel.estimated_monthly_earning)
@@ -29,14 +31,15 @@
     if channel.daily_stats:
         print('-------------------------------------------------------')
         for stat in channel.daily_stats:
             print(f'{stat.date} | {stat.estimated_earnings} | {stat.subscribers_count} | {stat.total_views}')
         print('-------------------------------------------------------')
 
     print('Channel Identifier:', channel.identifier)
+    print('Channel name:', channel.name)
     print('Profile URL:', channel.profile)
     print('Channel category:', channel.category)
     print('Channel banner:', channel.banner)
     print('Total uploads:', channel.total_uploads)
     print('Total subscribes:', channel.total_subscribers)
     print('Total views:', channel.total_views)
     print('Country:', channel.country)
@@ -49,8 +52,17 @@
 
     if tokens:
         encoded_user, token = tokens
         total_subscribers = await live_subscriber_count(encoded_user, token)
         print(f'Live subscribers: {total_subscribers}')
 
 
-asyncio.run(other_details())
+async def load_test():
+    for e in range(1):
+        tests = []
+        for i in range(1):
+            tests.append(show_basic())
+
+        await asyncio.gather(*tests)
+
+
+asyncio.run(load_test())
```

