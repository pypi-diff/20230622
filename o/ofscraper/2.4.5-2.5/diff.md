# Comparing `tmp/ofscraper-2.4.5.tar.gz` & `tmp/ofscraper-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.4.5.tar", max compression
+gzip compressed data, was "ofscraper-2.5.tar", max compression
```

## Comparing `ofscraper-2.4.5.tar` & `ofscraper-2.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-06-17 21:22:30.912783 ofscraper-2.4.5/LICENSE
--rw-r--r--   0        0        0     5450 2023-06-17 21:22:30.912783 ofscraper-2.4.5/README.md
--rw-r--r--   0        0        0      607 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     7066 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/archive.py
--rw-r--r--   0        0        0     3944 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/init.py
--rw-r--r--   0        0        0     2343 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/me.py
--rw-r--r--   0        0        0     8223 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/messages.py
--rw-r--r--   0        0        0     8634 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/paid.py
--rw-r--r--   0        0        0     4576 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11215 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3593 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7712 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    31644 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/commands/check.py
--rwxr-xr-x   0        0        0    14029 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     5769 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-17 21:22:30.920783 ofscraper-2.4.5/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     1364 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/prompt model.md
--rw-r--r--   0        0        0      696 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     6754 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27282 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      679 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     9292 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9035 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     6158 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10680 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19690 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3155 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5622 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9870 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7654 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3073 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     6042 2023-06-17 21:22:30.924783 ofscraper-2.4.5/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1520 2023-06-17 21:23:02.252707 ofscraper-2.4.5/pyproject.toml
--rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 ofscraper-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-22 06:44:41.511715 ofscraper-2.5/LICENSE
+-rw-r--r--   0        0        0     6001 2023-06-22 06:44:41.511715 ofscraper-2.5/README.md
+-rw-r--r--   0        0        0      607 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     7709 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     4682 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2338 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/me.py
+-rw-r--r--   0        0        0     8507 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9163 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5159 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11529 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3593 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8254 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    14116 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5025 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    13993 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6293 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     6754 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27282 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      744 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    10460 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8893 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     9023 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10680 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    20329 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3022 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     6442 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9870 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7934 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3073 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    28869 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     6089 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1624 2023-06-22 06:45:18.414684 ofscraper-2.5/pyproject.toml
+-rw-r--r--   0        0        0     7503 1970-01-01 00:00:00.000000 ofscraper-2.5/PKG-INFO
```

### Comparing `ofscraper-2.4.5/LICENSE` & `ofscraper-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/README.md` & `ofscraper-2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+# Table-of-contents
+- [Intro](#intro)
+- [Installation](#installation)
+  * [Windows: ](#windows)
+  * [macOS/Linux](#macoslinux)
+  * [Upgrade](#upgrade)
+  * [Authentication](#authentication)
+- [Usage](#usage)
+  * [Liking/Unliking](#likingunliking)
+  * [Selecting specific users](#selecting-specific-users)
+  * [Other menu options    ](#other-menu-options)
+- [Docker Support](#docker-support)
+- [Issues](#issues)
+- [Feature Requests](#feature-requests)
+  * [Common](#common)
+- [Migrating from DC script](#migrating-from-dc-script)
+- [Discord](#discord)
+- [Support](#support)
+
 # Intro
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
@@ -126,16 +145,16 @@
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
   https://github.com/datawhores/OF-Scraper/wiki/command-line-args
 
 # Docker Support
-https://github.com/datawhores/OF-Scraper/pkgs/container/ofscraper
- 
+https://github.com/datawhores/OF-Scraper/wiki/Docker
+
  # Customazation
     
 https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
 https://github.com/datawhores/OF-Scraper/wiki/Config-Options
 
   
 # Issues
@@ -190,15 +209,15 @@
 buymeacoffee.com/datawhores
     
 BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
 ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
 
 
-[![codecov](https://codecov.io/github/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/OF-Scraper)
+[![codecov](https://codecov.io/gh/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/gh/datawhores/OF-Scraper)
```

### Comparing `ofscraper-2.4.5/ofscraper/__init__.py` & `ofscraper-2.5/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/__version__.py` & `ofscraper-2.5/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/api/archive.py` & `ofscraper-2.5/ofscraper/api/archive.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,48 +60,54 @@
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
     if not r.is_error:
         progress.remove_task(task)
         posts = r.json()['list']
+        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
         if not posts:
             posts= []
-        elif len(posts)==0:
-            posts= []
-        elif required_ids==None:
-            attempt.set(0)
-            tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
-        else:
-            [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
-
-
-            #try once more to get id if only 1 left
-            if len(required_ids)==1:
+        if len(posts)==0:
+            log.debug(f" {log_id} -> number of post found 0")
+        elif len(posts)>0:
+            log.debug(f"{log_id} -> number of archived post found {len(posts)}")
+            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")        
+            if required_ids==None:
                 attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+                tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+            else:
+                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
 
-            elif len(required_ids)>0:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
+
+                #try once more to get id if only 1 left
+                if len(required_ids)==1:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+                elif len(required_ids)>0:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
     else:
             log.debug(f"[bold]archived request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]archived response:[/bold] {r.content.decode()}")
             log.debug(f"[bold]archived headers:[/bold] {r.headers}")
             progress.remove_task(task)
             r.raise_for_status()
     return posts
 
 async def get_archived_post(headers,model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting archived media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
-
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
```

### Comparing `ofscraper-2.4.5/ofscraper/api/highlights.py` & `ofscraper-2.5/ofscraper/api/highlights.py`

 * *Files 18% similar despite different names*

```diff
@@ -98,13 +98,31 @@
     return []
 
 
     
 
 
 
-
-
-
+def get_individual_highlight(id,client=None):
+    headers = auth.make_headers(auth.read_auth())
+    url=constants.highlightSPECIFIC.format(id)
+    auth.add_cookies(client)
+    client.headers.update(auth.create_sign(url, headers))
+    r=client.get(url)
+    if not r.is_error:
+        return r.json()
+    log.debug(f"{r.status_code}")
+    log.debug(f"{r.content.decode()}")
+
+def get_individual_stories(id,client=None):
+    headers = auth.make_headers(auth.read_auth())
+    url=constants.storiesSPECIFIC.format(id)
+    auth.add_cookies(client)
+    client.headers.update(auth.create_sign(url, headers))
+    r=client.get(url)
+    if not r.is_error:
+        return r.json()
+    log.debug(f"{r.status_code}")
+    log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.4.5/ofscraper/api/init.py` & `ofscraper-2.5/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/api/me.py` & `ofscraper-2.5/ofscraper/api/me.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 import ofscraper.utils.auth as auth
 import ofscraper.utils.encoding as encoding
 import ofscraper.utils.stdout as stdout
 from ofscraper.utils.logger import updateSenstiveDict
 log=logging.getLogger(__package__)
 console=Console()
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
 def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = constants.meEP
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
-
         r = c.get(url, timeout=None)
         if not r.is_error:
             updateSenstiveDict(r.json()["id"],"userid")
             updateSenstiveDict(r.json()["username"],"username")
             updateSenstiveDict(r.json()["name"],"name")
             return r.json()
         r.raise_for_status()
```

### Comparing `ofscraper-2.4.5/ofscraper/api/messages.py` & `ofscraper-2.5/ofscraper/api/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,25 +135,27 @@
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url, timeout=None)
     if not r.is_error:
+
         messages = r.json()['list']
+        log_id=f"offset messageid:{message_id if message_id else 'init id'}"
         if not messages:
             messages=[]
         if len(messages)==0:
-            log.debug(f"{message_id if message_id else 'init id'} -> number of messages found 0")
+            log.debug(f"{log_id} -> number of messages found 0")
         elif len(messages)>0:
-            log.debug(f"{message_id if message_id else 'init id'} -> number of messages found {len(messages)}")
-            log.debug(f"{message_id if message_id else 'init id'} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-            log.debug(f"{message_id if message_id else 'init id'} -> first ID {messages[0]['id']}")
-            log.debug(f"{message_id if message_id else 'init id'} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-            log.debug(f"{message_id if message_id else 'init id'} -> last ID {messages[-1]['id']}")    
+            log.debug(f"{log_id} -> number of messages found {len(messages)}")
+            log.debug(f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
+            log.debug(f"{log_id} -> first ID {messages[0]['id']}")
+            log.debug(f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
+            log.debug(f"{log_id} -> last ID {messages[-1]['id']}")    
             if (arrow.get( messages[-1].get("createdAt") or messages[-1].get("postedAt")).float_timestamp<(args_.getargs().after or arrow.get(0)).float_timestamp):
                 attempt.set(0)
             elif required_ids==None:
                 attempt.set(0)
                 tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'])))
             else:
                 [required_ids.discard(ele["id"]) for ele in messages]
@@ -172,9 +174,21 @@
 
         progress.remove_task(task)
         r.raise_for_status()
 
     progress.remove_task(task)
     return messages
 
+def get_individual_post(model_id,postid,client=None):
+    headers = auth.make_headers(auth.read_auth())
+    url=constants.messageSPECIFIC.format(model_id,postid)
+
+    auth.add_cookies(client)
+    client.headers.update(auth.create_sign(url, headers))
+    r=client.get(url)
+    if not r.is_error:
+        return r.json()['list'][0]
+    log.debug(f"{r.status_code}")
+    log.debug(f"{r.content.decode()}")
+
```

### Comparing `ofscraper-2.4.5/ofscraper/api/paid.py` & `ofscraper-2.5/ofscraper/api/paid.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         url = constants.purchased_contentEP.format(offset,username)
         c.headers.update(auth.create_sign(url, headers))
         r = await c.get(url, timeout=None)
         sem.release()
     if not r.is_error:
         attempt.set(0)
         media=list(filter(lambda x:isinstance(x,list),r.json().values()))[0]
-        log.debug(f"offset={offset} -> media found {len(media)}")
-        log.debug(f"offset={offset} -> hasmore value in json {r.json().get('hasMore','undefined') }")
+        log.debug(f"offset:{offset} -> media found {len(media)}")
+        log.debug(f"offset:{offset} -> hasmore value in json {r.json().get('hasMore','undefined') }")
         if  r.json().get("hasMore"):
             offset += len(media)
             tasks.append(asyncio.create_task(scrape_paid(username,job_progress,offset=offset)))
         job_progress.remove_task(task)
 
     else:
         log.debug(f"[bold]paid request status code:[/bold]{r.status_code}")
@@ -130,15 +130,15 @@
     output=[]
     min_posts=100
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
         allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
-        log.debug(f"[bold]ALl Paid Cache[/bold] {len(allpaid)} found")
+        log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
         
       
         if len(allpaid)>min_posts:
             splitArrays=[i for i in range(0, len(allpaid), min_posts)]
             #use the previous split for timesamp
             tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=0,count=0,required=0)))
             [ tasks.append(asyncio.create_task(scrape_all_paid(job_progress,count=0,required=0,offset=splitArrays[i])))
@@ -188,33 +188,41 @@
         auth.add_cookies(c)
         url = constants.purchased_contentALL.format(offset)
         offset += 10
         c.headers.update(auth.create_sign(url, headers))
         r = await c.get(url, timeout=None)
         sem.release()
     if not r.is_error:
-        attempt.set(0)     
+        attempt.set(0) 
+        log_id=offset or 0
+
         
         job_progress.remove_task(task)
         media=list(filter(lambda x:isinstance(x,list),r.json().values()))[0]
         if not r.json().get("hasMore"):
             media=[]
         if not media:
             media=[]
-        elif len(media)==0:
-            media=[]
-        elif required==0:
-            attempt.set(0)
-            tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media))))
+        if len(media)==0:
+            log.debug(f"offset:{log_id} -> number of post found 0")
+        elif len(media)>0:
+            log.debug(f"{log_id} -> number of post found {len(media)}")
+            log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
+            log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
+            log.debug(f"{log_id} -> first ID {media[0]['id']}")
+            log.debug(f"{log_id} -> last ID {media[-1]['id']}")
+            if required==0:
+                attempt.set(0)
+                tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media))))
 
-        elif len(count)<len(required):
-            tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media),required=required,count=count+len(media))))
+            elif len(count)<len(required):
+                tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media),required=required,count=count+len(media))))
 
 
-    
+        
 
     else:
         log.debug(f"[bold]paid request status code:[/bold]{r.status_code}")
         log.debug(f"[bold]paid response:[/bold] {r.content.decode()}")
         log.debug(f"[bold]paid headers:[/bold] {r.headers}")
         job_progress.remove_task(task)
         r.raise_for_status()
```

### Comparing `ofscraper-2.4.5/ofscraper/api/pinned.py` & `ofscraper-2.5/ofscraper/api/pinned.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,18 +56,25 @@
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
     if not r.is_error:
         progress.remove_task(task)
         posts = r.json()['list']
+        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
         if not posts:
             posts= []
-        elif len(posts)==0:
-            posts= []
+        if len(posts)==0:
+            log.debug(f"{log_id} -> number of pinned post f found 0")
+        else:
+            log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
+            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
         #post infinite loops            
         # elif required_ids==None:
         #     attempt.set(0)
             # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
     else:
             log.debug(f"[bold]pinned request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]pinned response:[/bold] {r.content.decode()}")
```

### Comparing `ofscraper-2.4.5/ofscraper/api/posts.py` & `ofscraper-2.5/ofscraper/api/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
         self._post = post
-        self._model_id = model_id
+        self._model_id = int(model_id)
         self._username = username
         self._responsetype_ = responsetype or post.get("responseType")
 
     #All media return from API dict
     @property
     def post_media(self):
         if self._responsetype_ == "highlights":
@@ -102,26 +102,26 @@
         if (self.post.get("isOpen") or self.post.get("isOpened") or len(self.media) > 0 or self.price != 0):
             return True
         return False
 
     @property
     def fromuser(self):
         if self._post.get("fromUser"):
-            return self._post["fromUser"]["id"]
+            return int(self._post["fromUser"]["id"])
         else:
             return self._model_id
 
     @property
     def preview(self):
         return self._post.get("preview")
 
     #media object array for media that is unlocked or viewable
     @property
     def media(self):
-        if (self.fromuser != self.model_id):
+        if (int(self.fromuser) != int(self.model_id)):
             return []
         else:
             media = map(lambda x: Media(
                 x[1], x[0], self), enumerate(self.post_media))
             return list(filter(lambda x: x.canview == True, media))
     #media object array for all media
     @property
@@ -191,15 +191,15 @@
             return f"{self._post._post['id']}_{self.count}"
         return self._post._post['id']
 
     @property
     def canview(self):
         if self.responsetype_ == "highlights":
             return True
-        return self._media.get("canView") or False
+        return self._media.get("canView") or True if (self.url or self.mpd)!=None else False
 
     @property
     def responsetype(self):
         return self._post.responsetype
 
     @property
     def responsetype_(self):
@@ -325,24 +325,34 @@
 
        
 
     @property
     def count(self):
         return self._count+1
 
+    #og filename
     @property
     def filename(self):
         if not self.url and not self.mpd:
             return None
         elif not self.responsetype=="Profile":
-            file=re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
-            return re.sub("_source","",file)
+            return re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
         else:
             filename= re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
             return f"{filename}_{arrow.get(self.date).format(config.get_date(config.read_config()))}"
+    @property
+    def filename_(self):
+        if self.filename==None:
+            return None
+        if self.mediatype=="videos":
+            return self.filename if re.search("_source",self.filename) else f"{self.filename}_source"
+        return self.filename
+
+            
+
 
     @property
     def preview(self):
         if self.post.preview:
             return 1
         else:
             return 0
```

### Comparing `ofscraper-2.4.5/ofscraper/api/profile.py` & `ofscraper-2.5/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/api/subscriptions.py` & `ofscraper-2.5/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/api/timeline.py` & `ofscraper-2.5/ofscraper/api/timeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,33 +59,41 @@
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
     if not r.is_error:
         progress.remove_task(task)
         posts = r.json()['list']
+        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
         if not posts:
             posts= []
-        elif len(posts)==0:
-            posts= []
-        elif required_ids==None:
-            attempt.set(0)
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
-        else:
-            [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+        if len(posts)==0:
+            log.debug(f"{log_id} -> number of post found 0")
 
 
-            #try once more to get id if only 1 left
-            if len(required_ids)==1:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+        elif len(posts)>0:
+            log.debug(f"{log_id} -> number of post found {len(posts)}")
+            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
 
-            elif len(required_ids)>0:
+            if required_ids==None:
                 attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
+                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+            else:
+                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+                #try once more to get id if only 1 left
+                if len(required_ids)==1:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+                elif len(required_ids)>0:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
     else:
             log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
             log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
 
             progress.remove_task(task)
             r.raise_for_status()
@@ -152,23 +160,21 @@
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
         cache.set(f"timeline_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
 
         cache.close()
         log.debug("Some post where not retrived resetting cache")
-
     return unduped                                
 
 
 def get_individual_post(id,client=None):
     headers = auth.make_headers(auth.read_auth())
-    with client or httpx.Client(http2=True, headers=headers) as c:
-        url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-        r=c.get(url)
-        if not r.is_error:
-            return r.json()
-        log.debug(f"{r.status_code}")
-        log.debug(f"{r.content.decode()}")
+    url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
+    auth.add_cookies(client)
+    client.headers.update(auth.create_sign(url, headers))
+    r=client.get(url)
+    if not r.is_error:
+        return r.json()
+    log.debug(f"{r.status_code}")
+    log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.4.5/ofscraper/commands/check.py` & `ofscraper-2.5/ofscraper/utils/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,279 +1,33 @@
 import logging
-import re
-import asyncio
-import textwrap
-import httpx
-import arrow
 from textual.app import App, ComposeResult
-from textual.coordinate import Coordinate
-from textual.widgets import Input, DataTable, Button, Checkbox, Label
+from textual.widgets import Input, DataTable, Button, Checkbox, Label,ContentSwitcher,TextLog
 from rich.text import Text
-from textual.containers import Horizontal, VerticalScroll
+from textual.containers import Horizontal, VerticalScroll,Vertical
+import ofscraper.utils.logger as logger
 from textual import events
-import ofscraper.utils.args as args_
-import ofscraper.db.operations as operations
-import ofscraper.api.profile as profile
-import ofscraper.utils.auth as auth
-import ofscraper.api.timeline as timeline
-import ofscraper.api.messages as messages_
-import ofscraper.api.posts as posts_
-import ofscraper.constants as constants
-import ofscraper.api.paid as paid_
-import ofscraper.api.archive as archive
-import ofscraper.api.pinned as pinned
-import ofscraper.api.highlights as highlights_
-
-
+import arrow
+import re
 from diskcache import Cache
+import ofscraper.utils.console as console_
 from ..utils.paths import getcachepath
 cache = Cache(getcachepath())
-
 log = logging.getLogger(__package__)
-args = args_.getargs()
-ROW_NAMES = "Number", "UserName", "Downloaded", "Unlocked", "Times_Detected", "Length", "Mediatype", "Post_Date", "Post_Media_Count", "Responsetype", "Price", "Post_ID", "Media_ID", "Text"
-ROWS = []
-
-
-def post_checker():
-    headers = auth.make_headers(auth.read_auth())
-    user_dict = {}
-    client = httpx.Client(http2=True, headers=headers)
-    links = list(url_helper())
-    for ele in links:
-        name_match = re.search("/([a-z_]+$)", ele)
-        if name_match:
-            user_name = name_match.group(1)
-            log.info(f"Getting Full Timeline for {user_name}")
-            model_id = profile.get_id(headers, user_name)
-        name_match = re.search("^[a-z]+$", ele)
-        if name_match:
-            user_name = name_match.group(0)
-            model_id = profile.get_id(headers, user_name)
-
-        oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
-        if len(oldtimeline) > 0 and not args.force:
-            user_dict[user_name] = oldtimeline
-        elif not user_dict.get(user_name):
-            user_dict[user_name] = {}
-            user_dict[user_name] = user_dict[user_name] or []
-            user_dict[user_name].extend(asyncio.run(
-                timeline.get_timeline_post(headers, model_id)))
-            user_dict[user_name].extend(asyncio.run(
-                pinned.get_pinned_post(headers, model_id)))
-            user_dict[user_name].extend(asyncio.run(
-                archive.get_archived_post(headers, model_id)))
-            cache.set(
-                f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
-
-    # individual links
-    for ele in list(filter(lambda x: re.search("onlyfans.com/[0-9]+/[a-z_]+$", x), links)):
-        name_match = re.search("/([a-z]+$)", ele)
-        num_match = re.search("/([0-9]+)", ele)
-        if name_match and num_match:
-            model_id = num_match.group(1)
-            user_name = name_match.group(1)
-            log.info(f"Getting Invidiual Link for {user_name}")
-
-            if not user_dict.get(user_name):
-                user_dict[name_match.group(1)] = {}
-            data = timeline.get_individual_post(model_id, client)
-            user_dict[user_name] = user_dict[user_name] or []
-            user_dict[user_name].append(data)
-
-    ROWS=[]
-    for user_name in user_dict.keys():
-        downloaded = get_downloaded(user_name, model_id)
-        media = get_all_found_media(user_name, user_dict[user_name])
-        ROWS.extend(row_gather(media, downloaded, user_name))
-    app_run_helper(ROWS)
-
-
-
-def message_checker():
-    links = list(url_helper())
-    user_dict = {}
-    ROWS=[]
-    for item in links:
-        num_match = re.search("/([0-9]+)", item)
-        headers = auth.make_headers(auth.read_auth())
-        if num_match:
-            model_id = num_match.group(1)
-            user_name = profile.scrape_profile(headers, model_id)['username']
-        name_match = re.search("^[a-z_.]+$", item)
-        if name_match:
-            user_name = name_match.group(0)
-            model_id = profile.get_id(headers, user_name)     
-        user_dict[user_name] = user_dict.get(user_name, [])
-        log.info(f"Getting Messages for {user_name}")
-        messages = None
-        oldmessages = cache.get(f"message_check_{model_id}", default=[])
-
-        
-        if len(oldmessages) > 0 and not args.force:
-            messages = oldmessages
-        else:
-            messages = asyncio.run(
-                messages_.get_messages(headers,  model_id))
-            cache.set(f"message_check_{model_id}",
-                        messages, expire=constants.CHECK_EXPIRY)
-        media = get_all_found_media(user_name, messages)
-        downloaded = get_downloaded(user_name, model_id)
-        ROWS.extend(row_gather(media, downloaded, user_name))
-
-    app_run_helper(ROWS)
-
-
-
-def purchase_checker():
-    user_dict = {}
-    headers = auth.make_headers(auth.read_auth())
-    ROWS = []
-    for user_name in args.username:
-        user_dict[user_name] = user_dict.get(user_name, [])
-        model_id = profile.get_id(headers, user_name)
-        oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
-        paid = None
-        
-        if len(oldpaid) > 0 and not args.force:
-            paid = oldpaid
-        else:
-            paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
-            cache.set(f"purchased_check_{model_id}",
-                      paid, expire=constants.CHECK_EXPIRY)
-        downloaded = get_downloaded(user_name, model_id)
-        media = get_all_found_media(user_name, paid)
-        ROWS.extend(row_gather(media, downloaded, user_name))
-
-    app_run_helper(ROWS)
-
-
-def stories_checker():
-    user_dict = {}
-    headers = auth.make_headers(auth.read_auth())
-    ROWS=[]
-    for user_name in args.username:
-        user_dict[user_name] = user_dict.get(user_name, [])
-        model_id = profile.get_id(headers, user_name)    
-        highlights, stories = asyncio.run(highlights_.get_highlight_post(headers, model_id))
-        highlights=list(map(lambda x:posts_.Post(
-        x, model_id, user_name,"highlights"), highlights))
-        stories=list(map(lambda x:posts_.Post(
-        x, model_id, user_name,"stories"), stories))
-            
-
-     
-        downloaded = get_downloaded(user_name, model_id)
-        media=[]
-        [media.extend(ele.all_media) for ele in stories+highlights]
-        ROWS.extend(row_gather(media, downloaded, user_name))
-
-    app_run_helper(ROWS)
-
-  
-
 
-def url_helper():
-    out = []
-    out.extend(args.file or [])
-    out.extend(args.url or [])
-    return map(lambda x: x.strip(), out)
 
 
-def get_all_found_media(user_name, posts):
-    headers = auth.make_headers(auth.read_auth())
 
-    temp = []
-    model_id = profile.get_id(headers, user_name)
-    posts_array=list(map(lambda x:posts_.Post(
-        x, model_id, user_name), posts))
-    [temp.extend(ele.all_media) for ele in posts_array]
-    return temp
 
 
 
 
-def get_downloaded(user_name, model_id):
-    downloaded = {}
-    operations.create_tables(model_id, user_name)
-    [downloaded.update({ele: downloaded.get(ele, 0)+1})
-     for ele in operations.get_media_ids(model_id, user_name)+get_paid_ids(model_id,user_name)]
-    
-    return downloaded
-
-def get_paid_ids(model_id,user_name):
-    oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
-    paid = None
-        
-    if len(oldpaid) > 0 and not args.force:
-         paid = oldpaid
-    else:
-        paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
-        cache.set(f"purchased_check_{model_id}",
-                      paid, expire=constants.CHECK_EXPIRY)
-    media = get_all_found_media(user_name, paid)
-    media=list(filter(lambda x:x.canview==True,media))
-    return list(map(lambda x:x.id,media))
-
-
-def app_run_helper(ROWS_):
-    ROWS = get_first_row()
-    ROWS.extend(ROWS_)
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    app = InputApp()
-    # we have to set properies before run
-    app.table_data = ROWS
-    app.row_names = ROW_NAMES
-    app.set_filtered_rows(reset=True)
-    app.run()
-
-
-def get_first_row():
-    return [ROW_NAMES]
-
-
-def texthelper(text):
-    text=text or ""
-    text = textwrap.dedent(text)
-    text = re.sub(" +$", "", text)
-    text = re.sub("^ +", "", text)
-    text = re.sub("<[^>]*>", "", text)
-    text = text if len(
-        text) < constants.TABLE_STR_MAX else f"{text[:constants.TABLE_STR_MAX]}..."
-    return text
-
-
-def unlocked_helper(ele):
-    return ele.canview
-
-
-def datehelper(date):
-    if date == "None":
-        return "Probably Deleted"
-    return date
-
-
-def times_helper(ele, mediadict, downloaded):
-    return max(len(mediadict.get(ele.id, [])), downloaded.get(ele.id, 0))
-  
-def row_gather(media, downloaded, username):
-
-    # fix text
-
-    mediadict = {}
-    [mediadict.update({ele.id: mediadict.get(ele.id, []) + [ele]})
-     for ele in list(filter(lambda x:x.canview,media))]
-    out = []
-    media = sorted(media, key=lambda x: arrow.get(x.date), reverse=True)
-    for count, ele in enumerate(media):
-        out.append((count+1, username, ele.id in downloaded or cache.get(ele.postid)!=None or  cache.get(ele.filename)!=None , unlocked_helper(ele), times_helper(ele, mediadict, downloaded), ele.length_, ele.mediatype, datehelper(
-            ele.postdate_), len(ele._post.post_media), ele.responsetype_, "Free" if ele._post.price == 0 else "{:.2f}".format(ele._post.price),  ele.postid, ele.id, texthelper(ele.text)))
-    return out
-
+console=console_.shared_console
+class OutConsole(TextLog):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
 class StyledButton(Button):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
 
 class StringField(Horizontal):
@@ -676,149 +430,289 @@
 
     def convertString(self, val):
         match = re.search("[0-9-/\.]+", val)
         if not match:
             return ""
         return match.group(0)
 
-
 class InputApp(App):
 
+    # Events
+    def on_data_table_header_selected(self, event):
+        added= self.get_current_added_rows()
+        self.sort_helper(event.label.plain)
+        self.restore_added_rows(added)
+      
+        # set reverse
+        # use native python sorting until textual has key support
+
+
+
+   
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        if event.button.id == "submit":
+            added=self.get_current_added_rows()
+            self.set_filtered_rows()
+            self.sort_helper()
+            self.make_table()
+            self.restore_added_rows(added)
+        elif event.button.id == "reset":
+            self.set_filtered_rows(reset=True)
+            self.reset_all_inputs()
+            self.set_reverse(init=True)
+            self.make_table()
+        elif event.button.id=="send_downloads":
+            log.info("Adding Downloads to queue")
+            self.add_to_row_queue()
+            self.query_one(ContentSwitcher).current = 'console_page'
+
+        elif event.button.id in ["console","table"]:
+             self.query_one(ContentSwitcher).current = f"{event.button.id}_page"  
     def on_key(self, event: events.Key) -> None:
         if event.key == "escape":
             self.exit()
-        if event.key == "end":
+        if event.character in set([";","'"]):
             table = self.query_one(DataTable)
             cursor_coordinate = table.cursor_coordinate
             if len(table._data) == 0:
                 return
             cell_key = table.coordinate_to_cell_key(cursor_coordinate)
             event = DataTable.CellSelected(
                 self,
                 table.get_cell_at(cursor_coordinate),
                 coordinate=cursor_coordinate,
                 cell_key=cell_key,
             )
             row_name = self.row_names[event.coordinate[1]]
-            self.update_input(row_name, event.value.plain)
-            self.set_filtered_rows()
-            self.make_table()
-        # if event.key=="enter" and arrow.now().float_timestamp-self._lastclick.float_timestamp>3:
-        #     self._lastclick=arrow.now()
-        #     self.set_filtered_rows()
-        #     self.make_table()
-
+            if row_name!="Download_Cart":
+                added=self.get_current_added_rows()
+                self.update_input(row_name, event.value.plain)
+                self.set_filtered_rows()
+                self.make_table()
+                self.restore_added_rows(added)
+            else:
+                self.change_download_cart(event.coordinate)
+    #Main
     def compose(self) -> ComposeResult:
-        with VerticalScroll():
-            with Horizontal():
-                for ele in ["Text"]:
-                    yield StringField(ele)
-                for ele in ["Times_Detected"]:
-                    yield NumField(ele)
-                for ele in ["Media_ID", "Post_ID", "Post_Media_Count"]:
-                    yield NumField(ele)
-            with Horizontal():
-                for ele in ["Price"]:
-                    yield PriceField(ele)
-                for ele in ["Post_Date"]:
-                    yield DateField(ele)
-                for ele in ["Length"]:
-                    yield TimeField(ele)
-
-            with Horizontal():
-                for ele in ["Downloaded", "Unlocked"]:
-                    yield BoolField(ele)
-                for ele in ["Mediatype"]:
-                    yield MediaField(ele)
-        with Horizontal(id="data"):
-            yield StyledButton("Submit", id="submit")
-            yield StyledButton("Reset", id="reset")
-        yield DataTable(fixed_rows=1, id="data-table_page")
+        with Horizontal(id="buttons"):  
+            yield Button("DataTable", id="table")  
+            yield Button("Console", id="console")
+        
+        with ContentSwitcher(initial="table_page"):  
+            with Vertical(id="table_page"):    
+                with VerticalScroll():
+                    with Horizontal():
+                        for ele in ["Text"]:
+                            yield StringField(ele)
+                        for ele in ["Times_Detected"]:
+                            yield NumField(ele)
+                        for ele in ["Media_ID", "Post_ID", "Post_Media_Count"]:
+                            yield NumField(ele)
+                    with Horizontal():
+                        for ele in ["Price"]:
+                            yield PriceField(ele)
+                        for ele in ["Post_Date"]:
+                            yield DateField(ele)
+                        for ele in ["Length"]:
+                            yield TimeField(ele)
+
+                    with Horizontal():
+                        for ele in ["Downloaded", "Unlocked"]:
+                            yield BoolField(ele)
+                        for ele in ["Mediatype"]:
+                            yield MediaField(ele)
+                with Horizontal(id="data"):
+                    yield StyledButton("Submit", id="submit")
+                    yield StyledButton("Reset", id="reset")
+                    yield StyledButton(">> Send Downloads to OF-Scraper", id="send_downloads")
+                yield DataTable(fixed_rows=1, id="data-table_page")
+            with Vertical(id="console_page"):
+                yield OutConsole()
 
-    def on_button_pressed(self, event: Button.Pressed) -> None:
-        if event.button.id == "submit":
-            self.set_filtered_rows()
-            self.sort_helper()
-            self.make_table()
-        elif event.button.id == "reset":
-            self.set_filtered_rows(reset=True)
-            self.reset_all_inputs()
-            self.set_reverse(init=True)
-            self.make_table()
+    def on_mount(self) -> None:
+        self.set_reverse(init=True)
+        self.set_cart_toggle(init=True)
+        self.make_table()
+        self.query_one("#reset").styles.align = ("center", "middle")
+        self.query_one(VerticalScroll).styles.height = "25vh"
+        self.query_one(VerticalScroll).styles.dock = "top"
+        self.query_one(DataTable).styles.height = "60vh"
+        self.query_one("#send_downloads").styles.content_align=("right", "middle")
+        for ele in self.query(Horizontal)[:-1]:
+            ele.styles.height = "10vh"
+        logger.add_widget(self.query_one("#console_page").query_one(OutConsole))
+       
 
-    def on_data_table_header_selected(self, event):
-        self.sort_helper(event.label.plain)
 
-        # set reverse
-        # use native python sorting until textual has key support
+    # Cart
+    def change_download_cart(self,coord):
+        table=self.query_one(DataTable)
+        Download_Cart=table.get_row_at(coord[0])[ self.row_names.index("Download_Cart")]
+        if Download_Cart.plain=="Not Unlocked":
+            return
+        elif Download_Cart.plain=="[]":
+            self.update_downloadcart_cell_coord(coord,"[added]")
+          
+            
+        elif Download_Cart.plain=="[added]":
+            self.update_downloadcart_cell_coord(coord,"[]")
+    
+        elif Download_Cart.plain=="[downloaded]" or "[failed]":
+            self.update_downloadcart_cell_coord(coord,"[]")
+
+    def add_to_row_queue(self):
+        table=self.query_one(DataTable)
+        keys=[str(ele[0]) for ele in self._filtered_rows]
+        index=self.row_names.index("Download_Cart")
+        filter_keys=list(filter(lambda x:table.get_row(x)[index].plain=="[added]",keys))
+        self.update_downloadcart_cell(filter_keys,"[downloading]")
+        log.info(f"Number of Downloads Set to queue {len(filter_keys)}")
+        [self.row_queue.put(ele) for ele in map(lambda x:(table.get_row(x),x),filter_keys)]
+    def get_current_added_rows(self):
+        table=self.query_one(DataTable)
+        keys=[str(ele[0]) for ele in self._filtered_rows]
+        index=self.row_names.index("Download_Cart")
+        filter_keys=list(filter(lambda x:table.get_row(x)[index].plain=="[added]",keys))
+        return filter_keys
+    def restore_added_rows(self,added):
+        table=self.query_one(DataTable)
+        currentkeys=set(map(lambda x:x.value,table.rows.keys()))
+        [table.update_cell(key,"Download_Cart",Text("[added]")) for key in filter(lambda x:x in currentkeys,added)]
+
+
+    def reset_cart(self):
+        index=self.row_names.index("Download_Cart")
+        self.update_downloadcart_cell(  [str(x[0]) for x in list(filter(lambda x:x[index]=="[added]",self.table_data[1:]))],"[]")
+    
+    def reset_filtered_cart(self):
+        index=self.row_names.index("Download_Cart")
+        self.update_downloadcart_cell(  list(filter(lambda x:x[index]!="Not Unlocked",self._filtered_rows)),"[]")
+
+    def update_downloadcart_cell_coord(self,keys,value):
+        index=self.row_names.index("Download_Cart")
+        if not isinstance(keys,list):
+            keys=[keys]
+        with self.mutex:
+            for key in keys:
+                try:
+                    table=self.query_one(DataTable)
+                    table.update_cell_at(key,Text(value))
+                    #table.ordered_rows gets the keys in table order
+                    self.table_data[int(table.ordered_rows[keys[0]].key.value)][index]=value
+
+                except Exception as E:
+                    log.debug("Row was probably removed")
+                    log.debug(E)
+    
+    
+    
+    def update_downloadcart_cell(self,keys,value):
+        self.update_cell(keys,"Download_Cart",value)
+       
+
+    def update_cell(self,keys,name,value,perst=True):
+        index=self.row_names.index(name)
+        if not isinstance(keys,list):
+            keys=[keys]
+        with self.mutex:
+            for key in keys:
+                try:
+                    if perst:
+                        self.table_data[int(key)][index]=value
+                    table=self.query_one(DataTable)
+                    table.update_cell(key,name,Text(str(value)))
+                except Exception as E:
+                    log.debug("Row was probably removed")
+                    log.debug(E)
+    
+
+
+ 
+
+    # Table Functions
 
     def sort_helper(self, label=None):
         # to allow sorting after submit
-        if label != None:
-            self.set_reverse(label=label)
+        if label == None:
+            return
+        index=self.row_names.index(re.sub(" ","_",label))
+        if label=="Download Cart":
+            filtered_status=["[downloading]","Not Unlocked","[downloaded]"]
+            table=self.query_one(DataTable)
+            self.set_cart_toggle()
+            keys=[str(ele[0]) for ele in self._filtered_rows]
+            filter_keys=list(filter(lambda x:table.get_row(x)[index].plain not in filtered_status,keys))
+            [table.update_cell(key,"Download_Cart",self.cart_toggle) for key in filter_keys]
+            
+
+           
+           
+            return
+        self.set_reverse(label=label)
+        
         if label == "Number":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[0], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
             self.make_table()
-        elif label == "Username":
+        elif label == "UserName":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x, reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
             self.make_table()
         elif label == "Downloaded":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[2] == True else 0, reverse=self.reverse)
+                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
             self.make_table()
 
         elif label == "Unlocked":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[3] == True else 0, reverse=self.reverse)
+                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Times Detected":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[4] == True else 0, reverse=self.reverse)
+                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Length":
             helperNode = self.query_one("#Length")
             self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
-                x[5]) if x[5] != "N/A" else 0, reverse=self.reverse)
+                x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Mediatype":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[6], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
             self.make_table()
         elif label == "Post Date":
             helperNode = self.query_one("#Post_Date")
             self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
-                x[7]) if x[7] != "N/A" else 0, reverse=self.reverse)
+                x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Post Media Count":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[8], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
             self.make_table()
 
         elif label == "Responsetype":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[9], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
             self.make_table()
         elif label == "Price":
             self._filtered_rows = sorted(self._filtered_rows, key=lambda x: int(
-                float(x[10])) if x[10] != "Free" else 0, reverse=self.reverse)
+                float(x[index])) if x[index] != "Free" else 0, reverse=self.reverse)
             self.make_table()
 
         elif label == "Post ID":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[11], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Media ID":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[12], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
             self.make_table()
         elif label == "Text":
             self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[13], reverse=self.reverse)
+                self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
             self.make_table()
 
     def set_reverse(self, label=None, init=False):
         if init:
             self.reverse = None
             self.label = None
         if not self.label:
@@ -830,41 +724,39 @@
 
         elif self.label == label and not self.reverse:
             self.reverse = True
 
         elif self.label == label and self.reverse:
             self.reverse = False
 
-    def on_mount(self) -> None:
-        self._lastclick = arrow.now()
-        self.set_reverse(init=True)
-        self.make_table()
-        self.query_one("#reset").styles.align = ("center", "middle")
-        self.query_one(VerticalScroll).styles.height = "35vh"
-        self.query_one(VerticalScroll).styles.dock = "top"
-        self.query_one(DataTable).styles.height = "60vh"
-
-        for ele in self.query(Horizontal)[:-1]:
-            ele.styles.height = "10vh"
+    def set_cart_toggle(self,init=False):
+        if init:
+            self.cart_toggle = Text("[added]")
+        if self.cart_toggle.plain == "[added]":
+            self.cart_toggle = Text("[]")
+        elif self.cart_toggle.plain == "[]":
+            self.cart_toggle = Text("[added]")
 
     def set_filtered_rows(self, reset=False):
         if reset == True:
             self._filtered_rows = self.table_data[1:]
+            self.reset_cart()
         else:
-            rows = self.table_data[1:]
+            filter_rows = self.table_data[1:]
             for count, name in enumerate(self.row_names[1:]):
                 try:
                     targetNode = self.query_one(f"#{name}")
                     if targetNode.empty():
                         continue
-                    rows = list(
-                        filter(lambda x: targetNode.validate(x[count+1]) == True, rows))
+                    filter_rows= list(
+                        filter(lambda x: targetNode.validate(x[count+1]) == True, filter_rows))
                 except:
                     None
-            self._filtered_rows = rows
+            self._filtered_rows=filter_rows
+        self.reset_filtered_cart()
 
     def update_input(self, row_name, value):
         try:
             targetNode = self.query_one(f"#{row_name}")
             targetNode.update_table_val(value)
         except:
             None
@@ -873,23 +765,24 @@
         for ele in self.row_names[1:]:
             try:
                 self.query_one(f"#{ele}").reset()
             except:
                 continue
 
     def make_table(self):
-        table = self.query_one(DataTable)
-        table.clear(True)
-        table.fixed_rows = 0
-        table.zebra_stripes = True
-        [table.add_column(re.sub("_", " ", ele), key=str(ele))
-         for ele in self.table_data[0]]
-        for count, row in enumerate(self._filtered_rows):
-            # Adding styled and justified `Text` objects instead of plain strings.
-            styled_row = [
-                Text(str(cell), style="italic #03AC13") for cell in row
-            ]
-            table.add_row(*styled_row, key=str(count+1))
-
-        if len(table.rows) == 0:
-            table.add_row("All Items Filtered")
-        table.cursor_coordinate = Coordinate(0, 0)
+        with self.mutex:
+            table = self.query_one(DataTable)
+            table.clear(True)
+            table.fixed_rows = 0
+            table.zebra_stripes = True
+            [table.add_column(re.sub("_", " ", ele), key=str(ele))
+            for ele in self.table_data[0]]
+            for count,row in enumerate(self._filtered_rows):
+                # Adding styled and justified `Text` objects instead of plain strings.
+                styled_row=[(Text(str(count+1)))]
+                styled_row.extend( Text(str(cell), style="italic #03AC13") for cell in row[1:])
+                table.add_row(*styled_row, key=str(row[0]))
+
+            
+
+            if len(table.rows) == 0:
+                table.add_row("All Items Filtered")
```

### Comparing `ofscraper-2.4.5/ofscraper/commands/scraper.py` & `ofscraper-2.5/ofscraper/commands/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 def process_post_user_first():
      with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         if args.users_first:
             output=[]
-            userdata=userselector.getselected_usernames() if "None" not in args.posts else []
+            userdata=userselector.getselected_usernames()
             length=len(userdata)
             for count,ele in enumerate(userdata):
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id(headers, ele["name"])
```

### Comparing `ofscraper-2.4.5/ofscraper/constants.py` & `ofscraper-2.5/ofscraper/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 DYNAMIC = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
 
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 purchased_contentALL = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}"
 
+messageSPECIFIC="https://onlyfans.com/my/chats/chat/{}/?firstId={}"
+highlightSPECIFIC="https://onlyfans.com/api2/v2/stories/highlights/{}"
+storiesSPECIFIC="https://onlyfans.com/api2/v2/stories/{}"
+messageSPECIFIC= "https://onlyfans.com/api2/v2/chats/{}/messages?limit=10&order=desc&skip_users=all&firstId={}"
 
 mainPromptChoices = {
     'Download content from a user': 0,
     'Like all of a user\'s posts': 1,
     'Unlike all of a user\'s posts': 2,
     'Edit auth.json file': 3,
     'Edit config.json file': 4,
@@ -119,14 +123,20 @@
 PATH_STR_MAX=200
 TABLE_STR_MAX=100
 
 refreshScreen=20
 
 MP4DECRYPT_LINUX="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-unknown-linux.zip"
 MP4DECRYPT_WINDOWS="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-microsoft-win32.zip"
+MP4DECRYPT_MAC="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.universal-apple-macosx.zip"
 FFMPEG_LINUX="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linux64-gpl.tar.xz"
 FFMPEG_WINDOWS="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip"
+FFMPEG_MAC="https://evermeet.cx/ffmpeg/ffmpeg-111111-gc44fe10160.zip"
+
 
 THREADS_DEFAULT=8
 MAX_SEMAPHORE=8
 AlT_SEM=4
 CODE_EXECUTION_DEFAULT =False
+
+NUMBER_REGEX="[0-9]"
+USERNAME_REGEX="[^/]"
```

### Comparing `ofscraper-2.4.5/ofscraper/db/operations.py` & `ofscraper-2.5/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/db/queries.py` & `ofscraper-2.5/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/interaction/like.py` & `ofscraper-2.5/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.5/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.5/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/prompts/prompts.py` & `ofscraper-2.5/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/start.py` & `ofscraper-2.5/ofscraper/start.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.commands.scraper as scraper
 import ofscraper.commands.check as check
+import ofscraper.commands.manual as manual
+
+
 log=logger.init_logger(logging.getLogger(__package__))
 args=args_.getargs()
 log.debug(args)
 def main():
     if args.command=="post_check":
         check.post_checker()
     elif args.command=="msg_check":
         check.message_checker()
     elif args.command=="paid_check":
         check.purchase_checker()
     elif args.command=="story_check":
         check.stories_checker()
     elif args.command=="manual":
-        None
+        manual.manual_download()
     elif vars(args).get("help"):
         None
     else:
         scraper.main()
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/args.py` & `ofscraper-2.5/ofscraper/utils/args.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 import argparse
 import logging
 import sys
+import re
 import arrow
 import pathlib
 from ofscraper.__version__ import __version__ 
 
 args=None
 log=logging.getLogger(__package__)
 def getargs(input=None):
     global args
     if args and input==None:
         return args
     if "pytest" in sys.modules and input==None:
         input=[]
     elif input==None:
         input=sys.argv[1:]
-
-    parser = argparse.ArgumentParser()
-
-    parser = argparse.ArgumentParser(add_help=False)   
-    general=parser.add_argument_group("General",description="General Args")  
+    parent_parser=argparse.ArgumentParser(add_help=False)
+    general=parent_parser.add_argument_group("General",description="General Args")  
     general.add_argument('-v', '--version', action='version', version=__version__ ,default=__version__)
-    general.add_argument('-h', '--help', action='help')
+    output=parent_parser.add_argument_group("Logging",description="Arguments for output controls")  
 
-                                    
-    general.add_argument(
-        '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=username_helper,action="extend"
+    output.add_argument(
+        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
+    ),
+    output.add_argument(
+        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
     )
-    general.add_argument(
-        '-eu', '--excluded-username', help="select which usernames to exclude  (name,name2)\nThis has preference over --username",type=username_helper,action="extend"
+
+    output.add_argument(
+        '-p', '--output', help = 'set console output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG"]
     )
-    general.add_argument(
+    output.add_argument(
         '-cg', '--config', help="Change location of config folder/file",default=None
     )
-    general.add_argument(
-        '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
+    output.add_argument(
+        '-au', '--auth', help="Change location of auth file",default=None
     )
 
-    general.add_argument(
-        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
-    ),
-    general.add_argument(
-        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
-    )
 
-    general.add_argument(
-        '-p', '--output', help = 'set console output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG"]
+    parser = argparse.ArgumentParser(add_help=False,parents=[parent_parser])  
+    parser.add_argument( '-h', '--help', action='help')
+    scraper=parser.add_argument_group("scraper",description="General Arguments for scraper")                                
+    scraper.add_argument(
+        '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=username_helper,action="extend"
     )
-    general.add_argument(
+    scraper.add_argument(
+        '-eu', '--excluded-username', help="select which usernames to exclude  (name,name2)\nThis has preference over --username",type=username_helper,action="extend"
+    )
+  
+    scraper.add_argument(
+        '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
+    )
+
+    scraper.add_argument(
         '-g', '--original', help = 'don\'t trunicate long paths', default=False,action="store_true"
     )
+
+
     post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
     post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
@@ -79,36 +87,33 @@
     filters.add_argument(
         '-rw', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
     )
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
     filters.add_argument(
-        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and downloading posts',type=arrow.get)
+        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and downloading posts',type=arrow_helper)
  
     filters.add_argument(
-        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow.get)
+        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow_helper)
     
     
     sort=parser.add_argument_group("sort",description="Options on how to sort list")
     sort.add_argument(
         '-st', '--sort', help = 'What to sort the model list by',default="Name",choices=["Name","Subscribed","Expiring","Price"],type=str.lower)
     sort.add_argument(
         '-ds', '--desc', help = 'Sort the model list in descending order',action="store_true",default=False) 
     
     advanced=parser.add_argument_group("Advanced",description="Advanced Args")  
     advanced.add_argument(
         '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
-    # advanced.add_argument(
-    #     '-ml', '--manual', help = 'Download media from post url',default=None,required=False,type = posttype_helper,action='extend'
-    # )
-  
+
     subparser=parser.add_subparsers(help="commands",dest="command")
-    post_check=subparser.add_parser("post_check",help="Check if data from a post\nCache lasts for 24 hours")
+    post_check=subparser.add_parser("post_check",help="Check if data from a post\nCache lasts for 24 hours",parents=[parent_parser])
 
 
     post_check.add_argument("-u","--url",
     help = 'Check if media is in library via url',default=None,required=False,type = check_strhelper,action='extend'
     )
 
 
@@ -116,55 +121,63 @@
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
     )
     
     post_check.add_argument(
         '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
     )
 
-    message_check=subparser.add_parser("msg_check",help="Parse a user's messages and view status of missing media\nCache lasts for 24 hours")
+    message_check=subparser.add_parser("msg_check",help="Parse a user's messages and view status of missing media\nCache lasts for 24 hours",parents=[parent_parser])
     message_check.add_argument(
         '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
     )
     message_check.add_argument("-f","--file",
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
     )
     
 
     message_check.add_argument("-u","--url",
     help = 'link to conversation',type = check_strhelper,action="extend")
     message_check.add_argument("-un","--username",
     help = 'link to conversation',type = check_strhelper,action="extend")
 
-    paid_check=subparser.add_parser("paid_check",help="Parse Purchases sent from a user\nCache last for 24 hours")
+    paid_check=subparser.add_parser("paid_check",help="Parse Purchases sent from a user\nCache last for 24 hours",parents=[parent_parser])
     paid_check.add_argument(
         '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
     )
     paid_check.add_argument("-f","--file",
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
     )
     
 
     paid_check.add_argument("-us","--username",
     help = 'link to conversation',type = check_strhelper,action="extend")
 
 
 
 
-    story_check=subparser.add_parser("story_check",help="Parse Stories/Highlights sent from a user\nCache last for 24 hours")
+    story_check=subparser.add_parser("story_check",help="Parse Stories/Highlights sent from a user\nCache last for 24 hours",parents=[parent_parser])
     story_check.add_argument(
         '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
     )
     story_check.add_argument("-f","--file",
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
     )
     
 
     story_check.add_argument("-us","--username",
     help = 'link to conversation',type = check_strhelper,action="extend")
 
+    manual=subparser.add_parser("manual",help="Manually download content via url or ID",parents=[parent_parser])
+    manual.add_argument("-f","--file",
+    help = 'Pass links/IDs to download via file',default=None,required=False,type = check_filehelper
+    )
+    manual.add_argument("-us","--url",
+    help = 'pass links to download via url',type = check_strhelper,action="extend")
+
+
     args=parser.parse_args(input)
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     args.username=set(args.username or [])
     args.excluded_username=set( args.excluded_username or [])
 
     if args.command=="post_check" and not (args.url or args.file):
@@ -186,26 +199,45 @@
     if isinstance(x,str) and pathlib.Path(x).exists():
         with open(x,"r") as _:
            return _.readlines()
 
    
     
 def posttype_helper(x):
-    choices=set(["highlights","all","archived","messages","timeline","pinned","stories","purchased","profile","none"])
+    choices=set(["Highlights","All","Archived","Messages","Timeline","Pinned","Stories","Purchased","Profile","None"])
     if isinstance(x,str):
         x=x.split(',')
-    if len(list(filter(lambda y:y not in choices,x)))>0:
+        x=list(map(lambda x:x.capitalize() ,x))
+    if len(list(filter(lambda y: y not in choices,x)))>0:
         raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile')")
     return x
 
 def changeargs(newargs):
     global args
     args=newargs
 
 
 def username_helper(x):
     temp=None
     if isinstance(x,list):
         temp=x
     elif isinstance(x,str):
         temp=x.split(",")
-    return temp
+    return temp
+
+def arrow_helper(x):
+    print(x)
+    try:
+        return arrow.get(x)
+    except arrow.parser.ParserError as E:
+        try:
+            x=re.sub("\\byear\\b","years",x)
+            x=re.sub("\\bday\\b","days",x)
+            x=re.sub("\\bmonth\\b","months",x)
+            x=re.sub("\\bweek\\b","weeks",x)
+            print(x)
+            arw=arrow.utcnow()
+            return arw.dehumanize(x)
+        except ValueError as E:
+             raise E
+
+
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/auth.py` & `ofscraper-2.5/ofscraper/utils/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,88 +15,79 @@
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 import httpx
 import browser_cookie3
 from .profiles import get_current_profile
 from ..prompts.prompts import *
-from ..constants import configPath, authFile, DYNAMIC, requestAuth
+from ..constants import configPath, DYNAMIC, requestAuth
+import ofscraper.utils.paths as paths
 
 console=Console()
 
 
 
 def read_auth():
     make_request_auth()
 
-    profile = get_current_profile()
-
-    p = pathlib.Path.home()/configPath/profile
-    if not p.is_dir():
-        p.mkdir(parents=True, exist_ok=True)
-    
-
+    authFile=paths.get_auth_file()
+   
     while True:
         try:
-            with open(p / authFile, 'r') as f:
+            with open(authFile, 'r') as f:
                 authText=f.read()
                 auth = json.loads(authText)
                 for key in list(filter(lambda x:x!="auth_uid_",auth.keys())):
                     if auth[key]==None or  auth[key]=="":
                         console.print("Auth Value not set retriving missing values")
                         make_auth()
                         break
             break
         except FileNotFoundError:
             console.print(
                 "You don't seem to have an `auth.json` file")
-            make_auth(p)
+            make_auth()
         except json.JSONDecodeError as e:
             print("You auth.json has a syntax error")
             print(f"{e}\n\n")
-            with open(p / authFile, 'w') as f:
+            with open( authFile, 'w') as f:
                 f.write(manual_auth_prompt(authText))
     return auth
 
 
 def edit_auth():
-    profile = get_current_profile()
-
-    p = pathlib.Path.home() / configPath / profile 
-    if not p.is_dir():
-        p.mkdir(parents=True, exist_ok=True)
-  
+    authFile=paths.get_auth_file()
     try:
-        with open(p / authFile, 'r') as f:
+        with open(authFile, 'r') as f:
             authText=f.read()
             auth = json.loads(authText)
         print("Hint: Select 'Enter Each Field Manually' to edit your current config\n")
-        make_auth(p, auth)
+        make_auth(auth)
 
         console.print('Your `auth.json` file has been edited.')
     except FileNotFoundError:
         
         if ask_make_auth_prompt():
-            make_auth(p)
+            make_auth(auth)
     except json.JSONDecodeError as e:
             while True:
                 try:
                     print("You auth.json has a syntax error")
                     print(f"{e}\n\n")
-                    with open(p / authFile, 'w') as f:
+                    with open(authFile, 'w') as f:
                         f.write(manual_auth_prompt(authText))
-                    with open(p / authFile, 'r') as f:
+                    with open(authFile, 'r') as f:
                         authText=f.read()
                         auth = json.loads(authText)
                     break
                 except:
                     continue
 
-def make_auth(path=None, auth=None):
-    path= path or  pathlib.Path.home() / configPath / get_current_profile()
+def make_auth( auth=None):
+    authFile=paths.get_auth_file()
     defaultAuth=  {
             'auth': {
                 'app-token': '33d57ade8c02dbc5a333db99ff9ae26a',
                 'sess': '',
                 'auth_id': '',
                 'auth_uid_': '',
                 'user_agent': '',
@@ -139,22 +130,20 @@
            
 
 
     else:
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
         auth['auth'].update(auth_prompt(auth['auth']))
     
-    console.print(f"{auth}\nWriting to {path / authFile}",style="yellow")
-    with open(path / authFile, 'w') as f:
+    console.print(f"{auth}\nWriting to {authFile}",style="yellow")
+    with open(authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
 
 
-def get_auth_id() -> str:
-    auth_id = read_auth()['auth']['auth_id']
-    return auth_id
+
 
 
 def make_headers(auth):
     headers = {
         'accept': 'application/json, text/plain, */*',
         'app-token': auth['auth']['app-token'],
         'user-id': auth['auth']['auth_id'],
@@ -162,32 +151,44 @@
         'referer': 'https://onlyfans.com',
         'user-agent': auth['auth']['user_agent'],
     }
     return headers
 
 
 def add_cookies(client):
-    profile = get_current_profile()
-
-    p = pathlib.Path.home() / configPath / profile
-    with open(p / authFile, 'r') as f:
+    authFile=paths.get_auth_file()
+    with open(authFile, 'r') as f:
         auth = json.load(f)
 
     domain = 'onlyfans.com'
 
     auth_uid = 'auth_uid_{}'.format(auth['auth']['auth_id'])
 
     client.cookies.set('sess', auth['auth']['sess'], domain=domain)
     client.cookies.set('auth_id', auth['auth']['auth_id'], domain=domain)
     if auth['auth']['auth_uid_']:
         client.cookies.set(auth_uid, auth['auth']['auth_uid_'], domain=domain)
+def add_cookies_aio():
+
+    authFile=paths.get_auth_file()
+    with open(authFile, 'r') as f:
+        auth = json.load(f)
+
+    cookies={}
+    cookies.update({"sess": auth['auth']['sess']})
+    cookies.update({"auth_id": auth['auth']['auth_id']})
+
+    if auth['auth']['auth_uid_']:
+        cookies.update({"auth_uid_":  auth['auth']['auth_uid_']})
+
+    return cookies
 def get_cookies():
-    profile = get_current_profile()
-    p = pathlib.Path.home() / configPath / profile
-    with open(p / authFile, 'r') as f:
+    authFile=paths.get_auth_file()
+
+    with open( authFile, 'r') as f:
         auth = json.load(f)
     return  f"auth_id={auth['auth']['auth_id']};sess={auth['auth']['sess']};"
 
 def create_sign(link, headers):
     """
     credit: DC and hippothon
     """
@@ -223,15 +224,16 @@
         }
     )
     return headers
 
 
 def read_request_auth() -> dict:
     profile = get_current_profile()
-    p = pathlib.Path.home() / configPath / profile / requestAuth
+
+    p = paths.get_config_path().parent/profile/ requestAuth
     with open(p, 'r') as f:
         content = json.load(f)
     return content
 
 
 def make_request_auth():
     request_auth = {
@@ -246,15 +248,15 @@
     if result:
         *values, = result
 
         request_auth.update(zip(request_auth.keys(), values))
 
         profile = get_current_profile()
 
-        p = pathlib.Path.home() / configPath / profile
+        p = paths.get_config_path().parent/profile
         if not p.is_dir():
             p.mkdir(parents=True, exist_ok=True)
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/binaries.py` & `ofscraper-2.5/ofscraper/utils/binaries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pathlib
-import logging
 import shutil
 import os
 import tempfile
 import platform
 import httpx
 import ofscraper.constants as constants
 from zipfile import ZipFile
@@ -14,32 +13,30 @@
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     BarColumn,
     DownloadColumn
 )
-from rich.live import Live
-from rich.panel import Panel
-from rich.console import Group
-from rich.table import Column
-import arrow
 import ofscraper.utils.paths as paths_
 def mp4decrypt_download():
     if platform.system() == 'Windows':
         return mp4_decrypt_windows()
-    else:
+    elif platform.system()=="Linux":
         return mp4_decrypt_linux()
+    elif platform.system()=="Darwin":
+        return mp4_decrypt_mac()
 
 def ffmpeg_download():
     if platform.system() == 'Windows':
         return ffmpeg_windows()
-    else:
+    elif platform.system()=="Linux":
         return ffmpeg_linux()   
- 
+    elif platform.system()=="Darwin":
+        return ffmpeg_mac() 
 def mp4_decrypt_windows():
  with tempfile.TemporaryDirectory() as t:
         zip_path=pathlib.Path(t,"mp4decrypt.zip")
         with Progress(  TextColumn("{task.description}"),
         BarColumn(),DownloadColumn()) as download:
             with httpx.stream("GET",constants.MP4DECRYPT_WINDOWS,timeout=None,follow_redirects=True) as r:
                     total = int(r.headers['Content-Length'])
@@ -82,14 +79,38 @@
         shutil.move(list(pathlib.Path(t).glob("**/mp4decrypt"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
       
 
 
+def mp4_decrypt_mac():
+    with tempfile.TemporaryDirectory() as t:
+        zip_path=pathlib.Path(t,"mp4decrypt.zip")
+        with Progress(  TextColumn("{task.description}"),
+        BarColumn(),DownloadColumn()) as download:
+            with httpx.stream("GET",constants.MP4DECRYPT_MAC,timeout=None,follow_redirects=True) as r:
+                    total = int(r.headers['Content-Length'])
+                    task1=download.add_task("mp4decrypt download",total=total)
+                    with open(pathlib.Path(zip_path),"wb") as f:
+                        num_bytes_downloaded = r.num_bytes_downloaded
+                        for chunk in r.iter_bytes(chunk_size=1024):
+                            f.write(chunk)
+                            download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
+                            num_bytes_downloaded = r.num_bytes_downloaded
+            download.remove_task(task1)
+        bin_path=paths_.get_config_path().parent / "bin"/"mp4decrypt"
+        bin_path.parent.mkdir(exist_ok=True,parents=True)
+        with ZipFile(zip_path) as zObject:
+             zObject.extractall(path=t)
+        shutil.move(list(pathlib.Path(t).glob("**/mp4decrypt"))[0],bin_path)
+        st = os.stat(bin_path)
+        os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
+        return str(bin_path)
+
 
 def ffmpeg_windows():
     with tempfile.TemporaryDirectory() as t:
         zip_path=pathlib.Path(t,"ffmpeg.zip")
         with Progress(  TextColumn("{task.description}"),
         BarColumn(),DownloadColumn()) as download:
             with httpx.stream("GET",constants.FFMPEG_WINDOWS,timeout=None,follow_redirects=True) as r:
@@ -102,14 +123,15 @@
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
         bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg.exe"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
+        pathlib.Path(bin_path).unlink(missing_ok=True)
         shutil.move(list(pathlib.Path(t).glob("**/ffmpeg.exe"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
 
 
 def ffmpeg_linux():
@@ -127,11 +149,39 @@
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
         bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with TarFile.open(zip_path,mode="r:xz") as zObject:
              zObject.extractall(path=t)
+        pathlib.Path(bin_path).unlink(missing_ok=True)
+        shutil.move(list(pathlib.Path(t).glob("**/ffmpeg"))[0],bin_path)
+        st = os.stat(bin_path)
+        os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
+        return str(bin_path)
+    
+
+
+def ffmpeg_mac():
+    with tempfile.TemporaryDirectory() as t:
+        zip_path=pathlib.Path(t,"ffmpeg.zip")
+        with Progress(  TextColumn("{task.description}"),
+        BarColumn(),DownloadColumn()) as download:
+            with httpx.stream("GET",constants.FFMPEG_MAC,timeout=None,follow_redirects=True) as r:
+                    total = int(r.headers['Content-Length'])
+                    task1=download.add_task("ffmpeg download",total=total)
+                    num_bytes_downloaded = r.num_bytes_downloaded
+                    with open(pathlib.Path(zip_path),"wb") as f:
+                        for chunk in r.iter_bytes(chunk_size=1024):
+                            f.write(chunk)
+                            download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
+                            num_bytes_downloaded = r.num_bytes_downloaded
+            download.remove_task(task1)
+        bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg"
+        bin_path.parent.mkdir(exist_ok=True,parents=True)
+        with ZipFile(zip_path) as zObject:
+             zObject.extractall(path=t)
+        pathlib.Path(bin_path).unlink(missing_ok=True)
         shutil.move(list(pathlib.Path(t).glob("**/ffmpeg"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/config.py` & `ofscraper-2.5/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/dates.py` & `ofscraper-2.5/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/download.py` & `ofscraper-2.5/ofscraper/utils/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,30 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import math
 import pathlib
+from random import randint
 import platform
 import shutil
 import traceback
 import re
 import logging
+import aiohttp
 import httpx
 import contextvars
 import json
 import subprocess
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TimeElapsedColumn,
-    TotalFileSizeColumn,
+    DownloadColumn,
     TransferSpeedColumn,
     TextColumn,
     TaskProgressColumn,
     BarColumn,
     TimeRemainingColumn
 )
 from rich.live import Live
@@ -39,158 +41,153 @@
 from bs4 import BeautifulSoup
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 from tenacity import retry,stop_after_attempt,wait_random,retry_if_result
 
-
-import ffmpeg
 import ofscraper.utils.config as config_
 import ofscraper.utils.separate as seperate
 import ofscraper.db.operations as operations
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
-
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 from diskcache import Cache
 
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
-from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
-sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
 
 
 async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
         overall_progress=Progress(  TextColumn("{task.description}"),
         BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
         job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
-        TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),TotalFileSizeColumn())
+        TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),DownloadColumn())
         progress_group = Group(
         overall_progress
         , Panel(Group(job_progress,fit=True)))
+        # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
+        global sem
+        sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
+
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
                 if not args_.getargs().dupe:
                     media_ids = set(operations.get_media_ids(model_id,username))
                     medialist = seperate.separate_by_id(medialist, media_ids)
                     medialist=seperate.seperate_avatars(medialist)
                     log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
                 else:
-                    log.info("forcing all downloads")
+                    log.info(f"forcing all downloads media count {len(medialist)}")
                 file_size_limit = config_.get_filesize()
-                global sem
                   
                 aws=[]
                 photo_count = 0
                 video_count = 0
                 audio_count=0
                 skipped = 0
                 total_bytes_downloaded = 0
                 data = 0
                 desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
-            
-                
 
                 
-                for ele in medialist:
-                    with paths.set_directory(paths.getmediadir(ele,username,model_id)):
-                        aws.append(asyncio.create_task(download(ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
-                task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=True)
-                # progress_group.renderables[1].height=max(15,console.shared_console.size[1]-2)
-                for coro in asyncio.as_completed(aws):
-                        try:
-                            media_type, num_bytes_downloaded = await coro
-                        except Exception as e:
-                            log.traceback(e)
-                            log.traceback(traceback.format_exc())
-                            media_type = "skipped"
-                            num_bytes_downloaded = 0
-
-                        total_bytes_downloaded += num_bytes_downloaded
-                        data = convert_num_bytes(total_bytes_downloaded)
-                        if media_type == 'images':
-                            photo_count += 1 
-
-                        elif media_type == 'videos':
-                            video_count += 1
-                        elif media_type == 'audios':
-                            audio_count += 1
-                        elif media_type == 'skipped':
-                            skipped += 1
-                        overall_progress.update(task1,description=desc.format(
-                                    p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
+
+                async with aiohttp.ClientSession(cookies=auth.add_cookies_aio()) as c: 
+                    for ele in medialist:
+                        with paths.set_directory(paths.getmediadir(ele,username,model_id)):
+                            aws.append(asyncio.create_task(download(c,ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
+                    task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=True)
+                    # progress_group.renderables[1].height=max(15,console.shared_console.size[1]-2)
+                    for coro in asyncio.as_completed(aws):
+                            try:
+                                media_type, num_bytes_downloaded = await coro
+                            except Exception as e:
+                                log.traceback(e)
+                                log.traceback(traceback.format_exc())
+                                media_type = "skipped"
+                                num_bytes_downloaded = 0
+
+                            total_bytes_downloaded += num_bytes_downloaded
+                            data = convert_num_bytes(total_bytes_downloaded)
+                            if media_type == 'images':
+                                photo_count += 1 
+
+                            elif media_type == 'videos':
+                                video_count += 1
+                            elif media_type == 'audios':
+                                audio_count += 1
+                            elif media_type == 'skipped':
+                                skipped += 1
+                            overall_progress.update(task1,description=desc.format(
+                                        p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
         overall_progress.remove_task(task1)
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
+    return photo_count+video_count+audio_count,skipped
 def retry_required(value):
     return value == ('skipped', 1)
 
 @retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
-async def download(ele,path,model_id,username,file_size_limit,progress):
+async def download(c,ele,path,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)
     
     try:
         if ele.url:
-           return await main_download_helper(ele,path,file_size_limit,username,model_id,progress)
+           return await main_download_helper(c,ele,path,file_size_limit,username,model_id,progress)
         elif ele.mpd:
             return await alt_download_helper(ele,path,file_size_limit,username,model_id,progress)
         else:
-            return "skipped",1
+            return None
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
-async def main_download_helper(ele,path,file_size_limit,username,model_id,progress):
+async def main_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
     url=ele.url
     path_to_file=None
     async with sem:
-            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {url}")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
             log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
-
-            async with httpx.AsyncClient(http2=True, follow_redirects=True, timeout=None) as c: 
-                auth.add_cookies(c)        
-                async with c.stream('GET',url) as r:
-                    if not r.is_error:
-                        rheaders=r.headers
-                        total = int(rheaders['Content-Length'])
-                        if file_size_limit>0 and total > int(file_size_limit): 
-                                return 'skipped', 1       
-                        content_type = rheaders.get("content-type").split('/')[-1]
-                        filename=createfilename(ele,username,model_id,content_type)
-                        path_to_file = paths.trunicate(pathlib.Path(path,f"{filename}"))                 
-                        pathstr=str(path_to_file)
-                        temp=paths.trunicate(f"{path_to_file}.part")
-                        pathlib.Path(temp).unlink(missing_ok=True)
-                        task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-                        with open(temp, 'wb') as f:                           
-                            num_bytes_downloaded = r.num_bytes_downloaded
-                            progress.update(task1,visible=True )
-                            async for chunk in r.aiter_bytes(chunk_size=1024):
-                                f.write(chunk)
-                                progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
-                                num_bytes_downloaded = r.num_bytes_downloaded
-                            progress.remove_task(task1) 
-        
-                    else:
-                        r.raise_for_status()
+            async with c.get(url) as r:
+                if r.ok:
+                    rheaders=r.headers
+                    total = int(rheaders['Content-Length'])
+                    if file_size_limit>0 and total > int(file_size_limit): 
+                            return 'skipped', 1       
+                    content_type = rheaders.get("content-type").split('/')[-1]
+                    filename=createfilename(ele,username,model_id,content_type)
+                    path_to_file = paths.trunicate(pathlib.Path(path,f"{filename}"))                 
+                    pathstr=str(path_to_file)
+                    temp=paths.trunicate(f"{path_to_file}.part")
+                    pathlib.Path(temp).unlink(missing_ok=True)
+                    task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+                    with open(temp, 'wb') as f:                           
+                        progress.update(task1,visible=True )
+                        async for chunk in r.content.iter_chunked(1024):
+                            f.write(chunk)
+                            progress.update(task1, advance=len(chunk))
+                        progress.remove_task(task1) 
+    
+                else:
+                    r.raise_for_status()
     if not pathlib.Path(temp).exists():
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {temp} was not created") 
         return "skipped",1
     elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
-        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         return "skipped",1 
     else:
-        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
         shutil.move(temp,path_to_file)
         if ele.postdate:
             newDate=dates.convert_local_time(ele.postdate)
             log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
@@ -199,69 +196,68 @@
             operations.write_media_table(ele,path_to_file,model_id,username)
         set_cache_helper(ele)
         return ele.mediatype,total
 
 async def alt_download_helper(ele,path,file_size_limit,username,model_id,progress):
     async with sem:
         log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
-        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {ele.mpd}")
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {ele.mpd}")
         video = None
         audio = None
         base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
         mpd=await ele.parse_mpd
         path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}'))
-        temp_path=paths.trunicate(pathlib.Path(path,f"tem{ele.id or ele.filename}.mkv"))
-
+        temp_path=paths.trunicate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}_{randint(100,999)}.mp4"))
         for period in mpd.periods:
             for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
                 kId=None
                 for prot in adapt_set.content_protections:
                     if prot.value==None:
                         kId = prot.pssh[0].pssh 
                         break
                 maxquality=max(map(lambda x:x.height,adapt_set.representations))
                 for repr in adapt_set.representations:
+                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
                     if repr.height==maxquality:
-                        video={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video"}
+                        video={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video","name":name}
                         break
             for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
                 kId=None
+                name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
                 for prot in adapt_set.content_protections:
                     if prot.value==None:
                         kId = prot.pssh[0].pssh 
                         logger.updateSenstiveDict(kId,"pssh_code")
                         break
                 for repr in adapt_set.representations:
-                    audio={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio"}
+                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
+                    audio={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio","name":name}
                     break
             for item in [audio,video]:
-                url=f"{base_url}{item['name']}"
-                log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['name']} with {url}")
+                url=f"{base_url}{item['origname']}"
+                log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
                 params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
-                async with httpx.AsyncClient(http2=True, headers = auth.make_headers(auth.read_auth()), follow_redirects=True, timeout=None,params=params) as c: 
-                    auth.add_cookies(c) 
-                    async with c.stream('GET',url) as r:
-                        if not r.is_error:
+                async with aiohttp.ClientSession(cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as c: 
+                    async with c.get(url,params=params) as r:
+                        if r.ok:
                             rheaders=r.headers
                             total = int(rheaders['Content-Length'])
                             item["total"]=total
                             if file_size_limit>0 and total > int(file_size_limit): 
                                     return 'skipped', 1       
                             temp= paths.trunicate(pathlib.Path(path,f"{item['name']}.part"))
                             temp.unlink(missing_ok=True)
                             item["path"]=temp
                             pathstr=str(temp)
                             task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                             with open(temp, 'wb') as f:                           
-                                num_bytes_downloaded = r.num_bytes_downloaded
                                 progress.update(task1,visible=True )
-                                async for chunk in r.aiter_bytes(chunk_size=1024):
+                                async for chunk in r.content.iter_chunked(1024):
                                     f.write(chunk)
-                                    progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
-                                    num_bytes_downloaded = r.num_bytes_downloaded
+                                    progress.update(task1, advance=len(chunk))
                                 progress.remove_task(task1) 
                         else:
                             r.raise_for_status()
     log.debug(f"Media:{ele.id} Post:{ele.postid} video name:{video['name']}")
     log.debug(f"Media:{ele.id} Post:{ele.postid} audio name:{audio['name']}")
     for item in [audio,video]:
         if not pathlib.Path(item["path"]).exists():
@@ -275,24 +271,32 @@
         key=await key_helper(item["pssh"],ele.license,ele.id)
         if key==None:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
         log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
-        subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)])
+        r=subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
+        if not pathlib.Path(newpath).exists():
+            log.debug(f"Media:{ele.id} Post:{ele.postid} mp4decrypt failed")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} mp4decrypt {r.stderr.decode()}")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} mp4decrypt {r.stdout.decode()}")
+        else:
+            log.debug(f"Media:{ele.id} Post:{ele.postid} mp4decrypt success {newpath}")    
         pathlib.Path(item["path"]).unlink(missing_ok=True)
         item["path"]=newpath
     
     path_to_file.unlink(missing_ok=True)
     temp_path.unlink(missing_ok=True)
-    t=subprocess.run([config_.get_ffmpeg(config_.read_config()),"-i",str(video["path"]),"-i",str(audio["path"]),"-c","copy",str(temp_path)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
+    t=subprocess.run([config_.get_ffmpeg(config_.read_config()),"-i",str(video["path"]),"-i",str(audio["path"]),"-c","copy","-movflags", "use_metadata_tags",str(temp_path)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
     if t.stderr.decode().find("Output")==-1:
-        log.debug(t.stdout.decode())
-        log.debug(t.stderr.decode())
+        log.debug(f"Media:{ele.id} Post:{ele.postid} ffmpeg failed")
+        log.debug(f"Media:{ele.id} Post:{ele.postid} ffmpeg {t.stderr.decode()}")
+        log.debug(f"Media:{ele.id} Post:{ele.postid} ffmpeg {t.stdout.decode()}")
+
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
     log.debug(f"Moving intermediate path {temp_path} to {path_to_file}")
     shutil.move(temp_path,path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
@@ -353,21 +357,21 @@
 def get_error_message(content):
     error_content = content.get('error', 'No error message available')
     try:
         return error_content.get('message', 'No error message available')
     except AttributeError:
         return error_content
 def createfilename(ele,username,model_id,ext):
-    filename=ele.filename
+    filename=ele.filename_
     sitename="Onlyfans"
     site_name="Onlyfans"
     post_id=ele.postid_
     media_id=ele.id
     first_letter=username[0]
-    mediatype=ele.mediatype,
+    mediatype=ele.mediatype
     value=ele.value
     text=ele.text_
     date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config()))
     model_username=username
     responsetype=ele.responsetype
 
     if ele.responsetype_ =="profile":
@@ -379,10 +383,10 @@
 
     
 
 def set_cache_helper(ele):
     if  ele.postid and ele.responsetype_=="profile":
         cache.set(ele.postid ,True)
         cache.close()
-    elif  ele.filename and ele.responsetype_=="highlights":
-        cache.set(ele.filename,True)
+    elif  ele.filename_ and ele.responsetype_=="highlights":
+        cache.set(ele.filename_,True)
         cache.close()
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/encoding.py` & `ofscraper-2.5/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/exit.py` & `ofscraper-2.5/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/filters.py` & `ofscraper-2.5/ofscraper/utils/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,14 @@
     media=dupefilter(media)
     media=post_datesorter(media)
     media=posts_type_filter(media)
     media=posts_date_filter(media)
     media=post_timed_filter(media)
     media=post_user_filter(media)
     media=sort_media(media)
-    # if args.manual_download():
-    #     args.dupe=True
-    #     args_.changeargs(args)
-    #     media=post_manual_filter(media)
     return media
 
 def sort_media(media):
     return sorted(media,key=lambda x:x.date)
 
 def post_manual_filter():
     None
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/logger.py` & `ofscraper-2.5/ofscraper/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import httpx
 import logging
 import threading
 import time
 import queue
 from rich.logging import RichHandler
+
 from tenacity import retry,stop_after_attempt,wait_fixed
 
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
 import ofscraper.constants as constants
@@ -36,14 +37,36 @@
         log_entry=f"{log_entry}\n\n"
         if url==None or url=="":
             return
         #convert markup
         log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
         discord_queue.put((url,log_entry))
 
+
+
+class TextHandler(logging.Handler):
+    def __init__(self):
+        logging.Handler.__init__(self)
+        self._widget=None
+    def emit(self, record):
+        # only emit after widget is set
+        if self._widget==None:
+            return
+        log_entry = self.format(record)
+        log_entry=f"{log_entry}"
+        self._widget.write(log_entry)
+        
+    @property
+    def widget(self):
+        return self._widget
+    @widget.setter
+    def widget(self,widget):
+        self._widget=widget
+
+
 def discord_messenger():
     with httpx.Client() as c:
         while True:
             url,message=discord_queue.get()   
             if url=="exit":
                 return
             try:
@@ -69,15 +92,15 @@
 def start_discord_queue():
     worker_thread = threading.Thread(target=discord_messenger)
     worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
-        if s.find("Avatar :"):
+        if s.find("Avatar :")!=-1:
             None
         else:
             s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
             s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
             s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
             for ele in senstiveDict.items():
                 s=re.sub(re.escape(str(ele[0])),str(ele[1]),s)
@@ -141,16 +164,20 @@
     cord.setLevel(getLevel(args.getargs().discord))
     cord.setFormatter(SensitiveFormatter('%(message)s'))
     #console
     sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.shared_console)
     sh.setLevel(getLevel(args.getargs().output))
     sh.setFormatter(SensitiveFormatter('%(message)s'))
     sh.addFilter(NoDebug())
+    tx=TextHandler()
+    tx.setLevel(getLevel(args.getargs().output))
+    tx.setFormatter(SensitiveFormatter('%(message)s'))
     log.addHandler(cord)
     log.addHandler(sh)
+    log.addHandler(tx)
     if args.getargs().log!="OFF":
         stream=open(paths.getlogpath(), encoding='utf-8',mode="a",)
         fh=logging.StreamHandler(stream)
         fh.setLevel(getLevel(args.getargs().log))
         fh.setFormatter(LogFileFormatter('%(asctime)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh.addFilter(NoDebug())
         log.addHandler(fh)
@@ -164,12 +191,14 @@
         log.addHandler(sh2)
     if args.getargs().log=="DEBUG":
         fh2=logging.StreamHandler(stream)
         fh2.setLevel(getLevel(args.getargs().log))
         fh2.setFormatter(LogFileFormatter('%(asctime)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh2.addFilter(DebugOnly())
         log.addHandler(fh2)
-    return log
+    
 
+    return log
 
-   
 
+def add_widget(widget):
+    [setattr(ele,"widget",widget) for ele in list(filter(lambda x:isinstance(x,TextHandler),logging.getLogger("ofscraper").handlers))]
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/of.py` & `ofscraper-2.5/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/paths.py` & `ofscraper-2.5/ofscraper/utils/paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 import logging
 import arrow
 from InquirerPy.utils import patched_print
 import ofscraper.constants as constants
 import ofscraper.utils.profiles as profiles
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
-import ofscraper.utils.paths as paths_
 import ofscraper.utils.console as console_
+from .profiles import get_current_profile
+
 
 console=console_.shared_console
 homeDir=pathlib.Path.home()
 log=logging.getLogger(__package__)
 
 
 @contextmanager
@@ -111,17 +112,17 @@
 
 
 
 
 
 
 def cleanup():
-    log.info("Cleaning up .part files\n\n")
+    log.info("Cleaning up temp files\n\n")
     root= pathlib.Path((config_.get_save_location(config_.read_config())))
-    for file in list(filter(lambda x:re.search("\.part$",str(x))!=None,root.glob("**/*"))):
+    for file in list(filter(lambda x:re.search("\.part$|^temp_",str(x))!=None,root.glob("**/*"))):
         file.unlink(missing_ok=True)
 
 
 def getcachepath():
     profile = profiles.get_current_profile()
     path= get_config_path().parent/ profile/"cache"
     createDir(path.parent)
@@ -175,15 +176,15 @@
             target=small
         elif len(file[:large].encode('utf8'))>maxbytes:
             large=int((small+large)/2)
         elif len(file[:large].encode('utf8'))<maxbytes:
              small=large
              large=int((large+maxLength)/2)        
     newFile=f"{file[:target]}{ext}"
-    log.debug(f"path: {path} filename_bytePsize: {len(newFile.encode('utf8'))}")
+    log.debug(f"path: {path} filename bytesize: {len(newFile.encode('utf8'))}")
     return pathlib.Path(dir,newFile)
 
 
 
 def mp4decryptchecker(x):
    return mp4decryptpathcheck(x) and mp4decryptexecutecheck(x)
 
@@ -232,8 +233,17 @@
 def get_config_path():
     t=pathlib.Path(args_.getargs().config or pathlib.Path.home() / constants.configPath)        
     if t.is_file():
          return t
     elif t.parent.is_dir():
         t/constants.configFile
     return t/constants.configFile
+
+def get_auth_file():
+    profile = get_current_profile()
+    auth= get_config_path().parent/profile /constants.authFile if not args_.getargs().auth else args_.getargs().auth
+    if auth.is_dir():
+        raise Exception("Auth File must be a file")
+    return auth
+
+
```

### Comparing `ofscraper-2.4.5/ofscraper/utils/profiles.py` & `ofscraper-2.5/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/separate.py` & `ofscraper-2.5/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/stdout.py` & `ofscraper-2.5/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.5/ofscraper/utils/userselector.py` & `ofscraper-2.5/ofscraper/utils/userselector.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 def getselected_usernames():
     #username list will be retrived once per daemon run
     # manual prompt will need to recertify options every call
     global selectedusers
     scraper_bool=len(args.posts)>0 or args.action
     #always return with correct args
+    if "None" in args.posts:
+        return []
     if selectedusers and scraper_bool:
             return selectedusers
     if scraper_bool:
         selectedusers=selectuserhelper()
     #create in these situations
     #set at least once
     elif args.username and not selectedusers:
```

### Comparing `ofscraper-2.4.5/pyproject.toml` & `ofscraper-2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.4.5"
+version = "2.5"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
@@ -22,14 +22,16 @@
 xxhash = "^3.2.0"
 mpegdash = "^0.3.1"
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
 textual = "^0.27.0"
+aiohttp = {extras = ["speedups"], version = "^3.8.4"}
+faust-cchardet = "^2.1.18"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
@@ -38,14 +40,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-check = { version = "2.1.4", python = ">3.7" }
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 random-unicode-emoji = "^2.8"
+random-emoji = "^1.0.15"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
 ofscraper = "ofscraper.start:main"
```

### Comparing `ofscraper-2.4.5/PKG-INFO` & `ofscraper-2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.4.5
+Version: 2.5
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: dunamai (>=1.17.0,<2.0.0)
+Requires-Dist: faust-cchardet (>=2.1.18,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
@@ -29,14 +31,33 @@
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: textual (>=0.27.0,<0.28.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Homepage, https://github.com/datawhores/OF-Scraper
 Description-Content-Type: text/markdown
 
+# Table-of-contents
+- [Intro](#intro)
+- [Installation](#installation)
+  * [Windows: ](#windows)
+  * [macOS/Linux](#macoslinux)
+  * [Upgrade](#upgrade)
+  * [Authentication](#authentication)
+- [Usage](#usage)
+  * [Liking/Unliking](#likingunliking)
+  * [Selecting specific users](#selecting-specific-users)
+  * [Other menu options    ](#other-menu-options)
+- [Docker Support](#docker-support)
+- [Issues](#issues)
+- [Feature Requests](#feature-requests)
+  * [Common](#common)
+- [Migrating from DC script](#migrating-from-dc-script)
+- [Discord](#discord)
+- [Support](#support)
+
 # Intro
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
@@ -161,16 +182,16 @@
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
   https://github.com/datawhores/OF-Scraper/wiki/command-line-args
 
 # Docker Support
-https://github.com/datawhores/OF-Scraper/pkgs/container/ofscraper
- 
+https://github.com/datawhores/OF-Scraper/wiki/Docker
+
  # Customazation
     
 https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
 https://github.com/datawhores/OF-Scraper/wiki/Config-Options
 
   
 # Issues
@@ -225,15 +246,15 @@
 buymeacoffee.com/datawhores
     
 BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
 ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
 
 
-[![codecov](https://codecov.io/github/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/OF-Scraper)
+[![codecov](https://codecov.io/gh/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/gh/datawhores/OF-Scraper)
```

