# Comparing `tmp/y2mate-api-0.0.5.tar.gz` & `tmp/y2mate-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.5.tar", last modified: Wed Jun 21 11:50:21 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.6.tar", last modified: Thu Jun 22 12:06:20 2023, max compression
```

## Comparing `y2mate-api-0.0.5.tar` & `y2mate-api-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.966188 y2mate-api-0.0.5/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.5/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-21 11:50:20.946188 y2mate-api-0.0.5/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9751 2023-06-21 11:45:37.000000 y2mate-api-0.0.5/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-21 11:50:20.966188 y2mate-api-0.0.5/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.5/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.510188 y2mate-api-0.0.5/tests/
--rw-rw----   0 root         (0) everybody  (9997)     1565 2023-06-20 21:34:48.000000 y2mate-api-0.0.5/tests/test_download.py
--rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.5/tests/test_queries.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.662188 y2mate-api-0.0.5/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-21 11:46:18.000000 y2mate-api-0.0.5/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.5/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5333 2023-06-19 18:27:02.000000 y2mate-api-0.0.5/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    14001 2023-06-20 16:45:31.000000 y2mate-api-0.0.5/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14438 2023-06-21 11:48:19.000000 y2mate-api-0.0.5/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.862188 y2mate-api-0.0.5/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.576863 y2mate-api-0.0.6/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.6/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-22 12:06:20.560863 y2mate-api-0.0.6/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9751 2023-06-22 12:05:24.000000 y2mate-api-0.0.6/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-22 12:06:20.576863 y2mate-api-0.0.6/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.6/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.152863 y2mate-api-0.0.6/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.6/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.6/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.340863 y2mate-api-0.0.6/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-21 12:36:02.000000 y2mate-api-0.0.6/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.6/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5359 2023-06-22 11:37:15.000000 y2mate-api-0.0.6/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    14243 2023-06-21 13:35:32.000000 y2mate-api-0.0.6/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14761 2023-06-22 12:00:38.000000 y2mate-api-0.0.6/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.548863 y2mate-api-0.0.6/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.5/LICENSE` & `y2mate-api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.5/PKG-INFO` & `y2mate-api-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.5 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.6 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
```

### Comparing `y2mate-api-0.0.5/README.md` & `y2mate-api-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

### Comparing `y2mate-api-0.0.5/setup.py` & `y2mate-api-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.5/tests/test_download.py` & `y2mate-api-0.0.6/tests/test_download.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,26 @@
                 audio_third_dict,
                 self.dir,
                 False,
                 True,
             )
         self.assertIsInstance(audio_path, str)
         self.assertTrue(os.path.isfile(audio_path))
-        #Tests audio format
+        # Tests audio format
         self.assertIn("128", audio_path)
         self.assertIn(video_id, audio_path)
         self.assertTrue(audio_path.endswith("mp3"))
 
     def test_download_video(self):
         """Downloads video"""
         for video_third_dict in self.handler.run("mp4", "360p"):
             video_path = self.handler.save(video_third_dict, self.dir, False, True)
         self.assertIsInstance(video_path, str)
         self.assertTrue(os.path.isfile(video_path))
-        #Test video format
+        # Test video format
         self.assertIn(video_id, video_path)
         self.assertIn("360", video_path)
         self.assertTrue(video_path.endswith("mp4"))
 
     def tearDown(self):
         shutil.rmtree(self.dir)
```

### Comparing `y2mate-api-0.0.5/tests/test_queries.py` & `y2mate-api-0.0.6/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.5/y2mate_api/console.py` & `y2mate-api-0.0.6/y2mate_api/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     "1080p",
     "720p",
     "480p",
     "360p",
     "240p",
     "144p",
     "auto",
+    "best",
+    "worst",
 ]
 mp3_qualities = ["mp3", "m4a", ".m4a", "128kbps", "192kbps", "328kbps"]
 resolvers = ["m4a", "3gp", "mp4", "mp3"]
 media_qualities = mp4_qualities + mp3_qualities
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s : %(message)s",
     datefmt="%H:%M:%S",
@@ -42,18 +44,18 @@
         help="Specify media type - audio/video",
         choices=["mp3", "mp4"],
         metavar="mp3|mp4",
     )
     parser.add_argument(
         "-q",
         "--quality",
-        help="Media quality -%(default)s",
+        help="Media quality - %(default)s",
         choices=media_qualities,
         metavar="|".join(media_qualities),
-        default="720p",
+        default="auto",
     )
     parser.add_argument(
         "-r",
         "--resolver",
         help="Other media formats incase of multiple options - mp4/mp3",
         choices=resolvers,
         metavar="|".join(resolvers),
```

### Comparing `y2mate-api-0.0.5/y2mate_api/downloader.py` & `y2mate-api-0.0.6/y2mate_api/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,14 +328,19 @@
         :type dir: str
         :type progress_bar: bool
         :type quiet: bool
         :type naming_format: str
         :rtype: None
         """
         if third_dict:
+            assert third_dict.get(
+                "dlink"
+            ), "The video selected does not support that quality, try lower qualities."
+            if third_dict.get("mess"):
+                logging.warning(third_dict.get("mess"))
             resp = requests.get(third_dict["dlink"], stream=True)
             size_in_bits = int(resp.headers.get("content-length", 1000000000000))
             size_in_mb = round(size_in_bits / 1000000, 2)
             chunk_size = 1024
             filename = self.generate_filename(third_dict, naming_format)
             save_to = path.join(dir, filename)
             third_dict["saved_to"] = (
```

### Comparing `y2mate-api-0.0.5/y2mate_api/main.py` & `y2mate-api-0.0.6/y2mate_api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
         def decorator(func):
             def main(*args, **kwargs):
                 try:
                     try:
                         return func(*args, **kwargs)
                     except (KeyboardInterrupt) as e:
+                        print()
                         logging.info(f"^KeyboardInterrupt quitting. Goodbye!")
                         exit(1)
                 except Exception as e:
                     if log:
                         # logging.exception(e)
                         logging.debug(f"Function ({func.__name__}) : {get_excep(e)}")
                         logging.error(get_excep(e))
@@ -253,18 +254,17 @@
     def get_item(self, item_no=0):
         r"""Return specific items on `self.query_one.vitems`"""
         if self.video_dict:
             return self.video_dict
         if self.query_one.is_link:
             return {"v": self.query_one.vid, "t": self.query_one.title}
         all_items = self.query_one.vitems
-        if self.item_no > len(all_items) - 1:
-            raise Exception(
-                f"{self.item_no} is greater than largest item's index :  {len(items)-1}"
-            )
+        assert (
+            self.item_no < len(all_items) - 1
+        ), "The item_no  is greater than largest item's index -  try lower value"
 
         return self.query_one.vitems[item_no or self.item_no]
 
     def get_payload(self):
         return {
             "hl": "en",
             "k_page": "home",
@@ -304,36 +304,38 @@
             self.__setattr__("audio", links.get("mp3"))
             self.__setattr__("related", dict_data.get("related")[0].get("contents"))
             self.__setattr__("raw", dict_data)
             self.processed = True
 
         else:
             logging.debug(f"{resp.headers.get('content-type')} - {resp.content}")
-            logging.error(f"Second query failed - [{resp.status_code} : {resp.reason}")
+            logging.error(f"Second query failed - [{resp.status_code} : {resp.reason}]")
         return self
 
 
 class third_query:
     def __init__(self, query_two: object):
 
         assert query_two.processed, "Unprocessed second_query object parsed"
         self.query_two = query_two
         self.url = "https://www.y2mate.com/mates/convertV2/index"
         self.formats = ["mp4", "mp3"]
+        self.qualities_plus = ["best", "worst"]
         self.qualities = {
             self.formats[0]: [
                 "4k",
                 "1080p",
                 "720p",
                 "480p",
                 "360p",
                 "240p",
                 "144p",
                 "auto",
-            ],
+            ]
+            + self.qualities_plus,
             self.formats[1]: ["mp3", "m4a", ".m4a", "128kbps", "192kbps", "328kbps"],
         }
 
     def __call__(self, *args, **kwargs):
         return self.main(*args, **kwargs)
 
     def __enter__(self):
@@ -358,45 +360,51 @@
 
     def get_payload(self, keys):
         return {"k": keys.get("k"), "vid": self.query_two.vid}
 
     def main(
         self,
         format: str = "mp4",
-        quality="720p",
+        quality="auto",
         resolver: str = None,
         timeout: int = 30,
     ):
         r"""
         :param format: (Optional) Media format mp4/mp3
         :param quality: (Optional) Media qualiy such as 720p
         :param resolver: (Optional) Additional format info : [m4a,3gp,mp4,mp3]
-        :param timeour: (Optional) Http requests timeout
+        :param timeout: (Optional) Http requests timeout
         :type type: str
         :type quality: str
         :type timeout: int
         """
         if not resolver:
             resolver = "mp4" if format == "mp4" else "mp3"
-        if format == "mp3" and quality == "720p":
+        if format == "mp3" and quality == "auto":
             quality = "128kbps"
-        if not format in self.formats:
-
-            raise Exception(f"'{format}' is not in supported formats - {self.formats}")
-
-        if not quality in self.qualities[format]:
+        assert (
+            format in self.formats
+        ), f"'{format}' is not in supported formats - {self.formats}"
+
+        assert (
+            quality in self.qualities[format]
+        ), f"'{quality}' is not in supported qualities - {self.qualities[format]}"
 
-            raise Exception(
-                f"'{quality}' is not in supported qualities - {self.qualities[format]}"
-            )
         items = self.query_two.video if format == "mp4" else self.query_two.audio
         hunted = []
-        for key in items.keys():
-            if items[key].get("q") == quality:
-                hunted.append(items[key])
+        if quality in self.qualities_plus:
+            keys = list(items.keys())
+            if quality == self.qualities_plus[0]:
+                hunted.append(items[keys[0]])
+            else:
+                hunted.append(items[keys[len(keys) - 2]])
+        else:
+            for key in items.keys():
+                if items[key].get("q") == quality:
+                    hunted.append(items[key])
         if len(hunted) > 1:
             for entry in hunted:
                 if entry.get("f") == resolver:
                     hunted.insert(0, entry)
         if hunted:
 
             def hunter_manager(souped_entry: dict = hunted[0], repeat_count=0):
@@ -405,15 +413,15 @@
                 if okay_status:
                     sanitized_feedback = resp.json()
                     if sanitized_feedback.get("c_status") == "CONVERTING":
                         if repeat_count >= 4:
                             return (False, {})
                         else:
                             logging.debug(
-                                f"Converting video  : sleeping for 5s - round {repeat_count}"
+                                f"Converting video  : sleeping for 5s - round {repeat_count+1}"
                             )
                             sleep(5)
                             repeat_count += 1
                             return hunter_manager(souped_entry)
                     return okay_status, resp
                 return okay_status, resp
 
@@ -430,8 +438,8 @@
                     f"Third query failed - [{resp.status_code} : {resp.reason}"
                 )
                 return {}
         else:
             logging.error(
                 f"Zero media hunted with params : {{quality : {quality}, format : {format}  }}"
             )
-            return {}
+            return {}
```

### Comparing `y2mate-api-0.0.5/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.6/y2mate_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.5 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.6 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
```

