# Comparing `tmp/y2mate-api-0.0.6.tar.gz` & `tmp/y2mate-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.6.tar", last modified: Thu Jun 22 12:06:20 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.7.tar", last modified: Thu Jun 22 15:49:55 2023, max compression
```

## Comparing `y2mate-api-0.0.6.tar` & `y2mate-api-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.576863 y2mate-api-0.0.6/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.6/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-22 12:06:20.560863 y2mate-api-0.0.6/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9751 2023-06-22 12:05:24.000000 y2mate-api-0.0.6/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-22 12:06:20.576863 y2mate-api-0.0.6/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.6/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.152863 y2mate-api-0.0.6/tests/
--rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.6/tests/test_download.py
--rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.6/tests/test_queries.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.340863 y2mate-api-0.0.6/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-21 12:36:02.000000 y2mate-api-0.0.6/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.6/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5359 2023-06-22 11:37:15.000000 y2mate-api-0.0.6/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    14243 2023-06-21 13:35:32.000000 y2mate-api-0.0.6/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14761 2023-06-22 12:00:38.000000 y2mate-api-0.0.6/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 12:06:20.548863 y2mate-api-0.0.6/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-22 12:06:19.000000 y2mate-api-0.0.6/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.864275 y2mate-api-0.0.7/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.7/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    10898 2023-06-22 15:49:54.832275 y2mate-api-0.0.7/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9803 2023-06-22 15:45:15.000000 y2mate-api-0.0.7/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-22 15:49:54.868275 y2mate-api-0.0.7/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.428274 y2mate-api-0.0.7/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.7/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.7/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.612275 y2mate-api-0.0.7/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-22 13:44:12.000000 y2mate-api-0.0.7/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.7/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5707 2023-06-22 15:05:00.000000 y2mate-api-0.0.7/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    14654 2023-06-22 15:35:13.000000 y2mate-api-0.0.7/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14730 2023-06-22 12:43:52.000000 y2mate-api-0.0.7/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.808275 y2mate-api-0.0.7/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10898 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.6/LICENSE` & `y2mate-api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.6/PKG-INFO` & `y2mate-api-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.6
+Version: 0.0.7
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
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -176,14 +176,15 @@
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
+  * chunk_size : Size of chunks in KB for downloads
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.6 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.7 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -63,16 +63,17 @@
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
-: Format for generating media filename using the `third_query` response keys
-For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+: Format for generating media filename using the `third_query` response keys *
+chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
+-h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
 unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
 audios by title or link positional arguments: query Youtube video title, link
 or id - None options: -h, --help show this help message and exit -v, --version
 show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
```

### Comparing `y2mate-api-0.0.6/README.md` & `y2mate-api-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -148,14 +148,15 @@
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
+  * chunk_size : Size of chunks in KB for downloads
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
```

#### html2text {}

```diff
@@ -49,16 +49,17 @@
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
-: Format for generating media filename using the `third_query` response keys
-For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+: Format for generating media filename using the `third_query` response keys *
+chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
+-h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
 unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
 audios by title or link positional arguments: query Youtube video title, link
 or id - None options: -h, --help show this help message and exit -v, --version
 show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
```

### Comparing `y2mate-api-0.0.6/setup.py` & `y2mate-api-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.6/tests/test_download.py` & `y2mate-api-0.0.7/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.6/tests/test_queries.py` & `y2mate-api-0.0.7/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.6/y2mate_api/console.py` & `y2mate-api-0.0.7/y2mate_api/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,24 +90,31 @@
         "-t",
         "--timeout",
         help="Http request timeout in seconds - %(default)s",
         type=int,
         default=30,
     )
     parser.add_argument(
+        "-c",
+        "--chunk",
+        help="Chunk-size for downloading files in KB - %(default)s",
+        type=int,
+        default=256,
+    )
+    parser.add_argument(
         "-i",
         "--input",
         help="Path to text file containing query per line - %(default)s",
         metavar="PATH",
     )
     parser.add_argument(
         "-o",
         "--output",
         metavar="FORMAT",
-        help="Format for generating filename %%(key)s : [title,vid,fquality,ftype] - %(default)s",
+        help="Format for generating filename %%(key)s : [title,vid,fquality,ftype] or 'pretty' - %(default)s",
     )
     parser.add_argument(
         "-thr",
         "--thread",
         help="Download [x] amount of videos/audios at once - 1",
         type=int,
         default=0,
@@ -168,15 +175,18 @@
         unique=args.unique,
         thread=args.thread,
     )
     auto_save_args = dict(
         dir=args.dir,
         progress_bar=args.disable_bar == False,
         quiet=args.quiet,
-        naming_format=args.output,
+        naming_format=f"%(title)s{' - %(fquality)s' if args.format=='mp4' else ''}.%(ftype)s"
+        if str(args.output).lower() == "pretty"
+        else args.output,
+        chunk_size=args.chunk,
         format=args.format,
         quality=args.quality,
         resolver=args.resolver,
         limit=args.limit,
         keyword=h_mult_args(args.keyword),
         author=h_mult_args(args.author),
     )
@@ -185,9 +195,9 @@
         for query in open(args.input).read().strip().split("\n"):
             handler_init_args["query"] = query
             auto_save_args["limit"] = 1
             Handler(**handler_init_args).auto_save(**auto_save_args)
     else:
         Handler(**handler_init_args).auto_save(**auto_save_args)
     logging.info(
-        f"Done downloading [{args.limit}] {'audio' if args.format=='mp3' else 'video'}{'' if args.limit==1 else 's'}"
+        f"Done downloading ({args.limit}) {'audio' if args.format=='mp3' else 'video'}{'' if args.limit==1 else 's'}"
     )
```

### Comparing `y2mate-api-0.0.6/y2mate_api/downloader.py` & `y2mate-api-0.0.7/y2mate_api/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             else:
                 logging.warning("Dropping unprocessed query_two object")
                 yield
 
     def run(
         self,
         format: str = "mp4",
-        quality: str = "720p",
+        quality: str = "auto",
         resolver: str = None,
         limit: int = 1,
         keyword: str = None,
         author: str = None,
     ):
         r"""Generate and yield video dictionary
         :param format: (Optional) Media format mp4/mp3
@@ -250,42 +250,45 @@
         fnm = (
             f"{naming_format}" % third_dict
             if naming_format
             else f"{third_dict['title']} {third_dict['vid']}_{third_dict['fquality']}.{third_dict['ftype']}"
         )
 
         def sanitize(nm):
-            trash = ["\\", "/", ":", "*", "?", '"', "<", "|", ">"]
+            trash = ["\\", "/", ":", "*", "?", '"', "<", "|", ">","y2mate.com","y2mate com"]
             for val in trash:
                 nm = nm.replace(val, "")
-            return nm
+            return nm.strip()
 
         return sanitize(fnm)
 
     def auto_save(
         self,
         dir: str = "",
         iterator: object = None,
         progress_bar=True,
         quiet: bool = False,
         naming_format: str = None,
+        chunk_size: int = 512,
         *args,
         **kwargs,
     ):
         r"""Query and save all the media
         :param dir: (Optional) Path to Directory for saving the media files
         :param iterator: (Optional) Function that yields third_query object - `Handler.run`
         :param progress_bar: (Optional) Display progress bar
         :param quiet: (Optional) Not to stdout anything
         :param naming_format: (Optional) Format for generating filename
+        :param chunk_size: (Optional) Chunk_size for downloading files in KB
         :type dir: str
         :type iterator: object
         :type progress_bar: bool
         :type quiet: bool
         :type naming_format: str
+        :type chunk_size: int
         args & kwargs for the iterator
         :rtype: None
         """
         iterator_object = iterator or self.run(*args, **kwargs)
 
         for x, entry in enumerate(iterator_object):
 
@@ -294,80 +297,85 @@
                     target=self.save,
                     args=(
                         entry,
                         dir,
                         False,
                         quiet,
                         naming_format,
+                        chunk_size,
                     ),
                 )
                 t1.start()
                 thread_count = x + 1
                 if thread_count % self.thread == 0 or thread_count == self.total:
                     logging.debug(
                         f"Waiting for current running threads to finish - thread_count : {thread_count}"
                     )
                     t1.join()
             else:
-                self.save(entry, dir, progress_bar, quiet, naming_format)
+                self.save(entry, dir, progress_bar, quiet, naming_format, chunk_size)
 
     def save(
         self,
         third_dict: dict,
         dir: str = "",
         progress_bar=True,
         quiet: bool = False,
         naming_format: str = None,
+        chunk_size: int = 512,
     ):
         r"""Download media based on response of `third_query` dict-data-type
         :param third_dict: Response of `third_query.run()`
         :param dir: (Optional) Directory for saving the contents
         :param progress_bar: (Optional) Display download progress bar
         :param quiet: (Optional) Not to stdout anything
         :param naming_format: (Optional) Format for generating filename
+        :param chunk_size: (Optional) Chunk_size for downloading files in KB
         :type third_dict: dict
         :type dir: str
         :type progress_bar: bool
         :type quiet: bool
         :type naming_format: str
+        :type chunk_size: int
         :rtype: None
         """
         if third_dict:
             assert third_dict.get(
                 "dlink"
             ), "The video selected does not support that quality, try lower qualities."
             if third_dict.get("mess"):
                 logging.warning(third_dict.get("mess"))
             resp = requests.get(third_dict["dlink"], stream=True)
-            size_in_bits = int(resp.headers.get("content-length", 1000000000000))
-            size_in_mb = round(size_in_bits / 1000000, 2)
-            chunk_size = 1024
+            size_in_bytes = int(resp.headers.get("content-length", 1000000000000))
+            size_in_mb = round(size_in_bytes / 1000000, 2)
+            chunk_size_in_bytes = chunk_size * 1024
             filename = self.generate_filename(third_dict, naming_format)
             save_to = path.join(dir, filename)
+
             third_dict["saved_to"] = (
                 save_to
                 if any([save_to.startswith("/"), ":" in save_to])
                 else path.join(getcwd(), dir, filename)
             )
             if progress_bar:
                 if not quiet:
                     print(f"{filename}")
                 with tqdm(
-                    total=size_in_bits,
+                    total=size_in_bytes,
                     bar_format="%s%d MB %s{bar} %s{l_bar}%s"
                     % (Fore.GREEN, size_in_mb, Fore.CYAN, Fore.YELLOW, Fore.RESET),
                 ) as p_bar:
                     with open(save_to, "wb") as fh:
-                        for chunks in resp.iter_content(chunk_size=chunk_size):
+                        for chunks in resp.iter_content(chunk_size=chunk_size_in_bytes):
                             fh.write(chunks)
-                            p_bar.update(chunk_size)
+                            p_bar.update(chunk_size_in_bytes)
                     utils.add_history(third_dict)
                     return save_to
             else:
                 with open(save_to, "wb") as fh:
-                    for chunks in resp.iter_content(chunk_size=chunk_size):
+                    for chunks in resp.iter_content(chunk_size=chunk_size_in_bytes):
                         fh.write(chunks)
                 utils.add_history(third_dict)
                 logging.info(f"{filename} - {size_in_mb}MB ✅")
                 return save_to
         else:
             logging.error(f"Empty `third_dict` parameter parsed : {third_dict}")
```

### Comparing `y2mate-api-0.0.6/y2mate_api/main.py` & `y2mate-api-0.0.7/y2mate_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         return self.main(timeout)
 
     def main(self, timeout=30):
         r"""Sets class attributes
         :param timeout: (Optional) Http requests timeout
         :type timeout: int
         """
-        self.processed = False
         logging.debug(f"Making first query  : {self.payload.get('k_query')}")
         okay_status, resp = utils.post(self.url, data=self.payload, timeout=timeout)
         # print(resp.headers["content-type"])
         # print(resp.content)
         if okay_status:
             dict_data = resp.json()
             self.__setattr__("raw", dict_data)
```

### Comparing `y2mate-api-0.0.6/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.7/y2mate_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.6
+Version: 0.0.7
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
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.6&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -176,14 +176,15 @@
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
+  * chunk_size : Size of chunks in KB for downloads
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.6 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.7 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -63,16 +63,17 @@
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
-: Format for generating media filename using the `third_query` response keys
-For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+: Format for generating media filename using the `third_query` response keys *
+chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
+-h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
 unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
 audios by title or link positional arguments: query Youtube video title, link
 or id - None options: -h, --help show this help message and exit -v, --version
 show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
```

