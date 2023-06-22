# Comparing `tmp/yt_summarizer-0.1.1.tar.gz` & `tmp/yt_summarizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_summarizer-0.1.1.tar", last modified: Thu Jun 22 09:25:12 2023, max compression
+gzip compressed data, was "yt_summarizer-0.1.2.tar", last modified: Thu Jun 22 10:07:24 2023, max compression
```

## Comparing `yt_summarizer-0.1.1.tar` & `yt_summarizer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 09:25:12.807679 yt_summarizer-0.1.1/
--rw-r--r--   0 isaacduong   (501) staff       (20)     1062 2023-06-21 20:47:45.000000 yt_summarizer-0.1.1/LICENSE
--rw-r--r--   0 isaacduong   (501) staff       (20)     3176 2023-06-22 09:25:12.807740 yt_summarizer-0.1.1/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)     2790 2023-06-22 08:53:38.000000 yt_summarizer-0.1.1/README.md
--rw-r--r--   0 isaacduong   (501) staff       (20)       79 2023-06-22 09:25:12.807927 yt_summarizer-0.1.1/setup.cfg
--rw-r--r--   0 isaacduong   (501) staff       (20)      877 2023-06-22 09:25:00.000000 yt_summarizer-0.1.1/setup.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 09:25:12.806803 yt_summarizer-0.1.1/yt_summarizer/
--rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:25:30.000000 yt_summarizer-0.1.1/yt_summarizer/__init__.py
--rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:25:17.000000 yt_summarizer-0.1.1/yt_summarizer/youtube_video_summary.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 09:25:12.807576 yt_summarizer-0.1.1/yt_summarizer.egg-info/
--rw-r--r--   0 isaacduong   (501) staff       (20)     3176 2023-06-22 09:25:12.000000 yt_summarizer-0.1.1/yt_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)      285 2023-06-22 09:25:12.000000 yt_summarizer-0.1.1/yt_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-22 09:25:12.000000 yt_summarizer-0.1.1/yt_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)       72 2023-06-22 09:25:12.000000 yt_summarizer-0.1.1/yt_summarizer.egg-info/requires.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)       14 2023-06-22 09:25:12.000000 yt_summarizer-0.1.1/yt_summarizer.egg-info/top_level.txt
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.186218 yt_summarizer-0.1.2/
+-rw-r--r--   0 isaacduong   (501) staff       (20)     1062 2023-06-21 20:47:45.000000 yt_summarizer-0.1.2/LICENSE
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3456 2023-06-22 10:07:24.186278 yt_summarizer-0.1.2/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3070 2023-06-22 10:03:37.000000 yt_summarizer-0.1.2/README.md
+-rw-r--r--   0 isaacduong   (501) staff       (20)       79 2023-06-22 10:07:24.186462 yt_summarizer-0.1.2/setup.cfg
+-rw-r--r--   0 isaacduong   (501) staff       (20)      886 2023-06-22 10:07:22.000000 yt_summarizer-0.1.2/setup.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.185475 yt_summarizer-0.1.2/yt_summarizer/
+-rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:25:30.000000 yt_summarizer-0.1.2/yt_summarizer/__init__.py
+-rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:25:17.000000 yt_summarizer-0.1.2/yt_summarizer/youtube_video_summary.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.186106 yt_summarizer-0.1.2/yt_summarizer.egg-info/
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3456 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)      285 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)       81 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/requires.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)       14 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/top_level.txt
```

### Comparing `yt_summarizer-0.1.1/LICENSE` & `yt_summarizer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_summarizer-0.1.1/PKG-INFO` & `yt_summarizer-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_summarizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python script to extract video transcripts based on the video id, and summarize the text content using the GPT-3.5 Turbo model.
 Home-page: https://github.com/isaacduong/youtube_summarizer
 Author: Isaac Duong
 Author-email: isaaacduong@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -48,8 +48,23 @@
 
 - Python 3.x
 - Google API Key
 - OpenAI API Key
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
-downloader = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key)
+
+summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
+
+then 
+transcript = summarizer.get_transcript(video_id)
+
+and afterwards call 
+summary = summarizer.summarize_text(transcript)
+
+and if you want to save it to a file ( text or audio file ) 
+
+summarizer.write_to_textfile(video_id,summary)
+or
+summarizer.convert_to_audio(summary)
+
+
```

### Comparing `yt_summarizer-0.1.1/README.md` & `yt_summarizer-0.1.2/yt_summarizer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: yt-summarizer
+Version: 0.1.2
+Summary: Python script to extract video transcripts based on the video id, and summarize the text content using the GPT-3.5 Turbo model.
+Home-page: https://github.com/isaacduong/youtube_summarizer
+Author: Isaac Duong
+Author-email: isaaacduong@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # YouTube Video Summarizer
 
 The YouTube Video Summarizer is a Python script that allows you to extract video transcripts based on the video id, and summarize the 
 text content using the GPT-3.5 Turbo model. You can apply the script to video of any language under the condition the video creator do 
 not disable the transcript of the videos intentionally. By default video in German and English will be summarized in these languages, 
 Summaries of videos spoken in all other languages will be in English. 
 
@@ -37,8 +48,23 @@
 
 - Python 3.x
 - Google API Key
 - OpenAI API Key
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
-downloader = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key)
+
+summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
+
+then 
+transcript = summarizer.get_transcript(video_id)
+
+and afterwards call 
+summary = summarizer.summarize_text(transcript)
+
+and if you want to save it to a file ( text or audio file ) 
+
+summarizer.write_to_textfile(video_id,summary)
+or
+summarizer.convert_to_audio(summary)
+
+
```

### Comparing `yt_summarizer-0.1.1/setup.py` & `yt_summarizer-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='yt_summarizer',
-    version='0.1.1',
+    version='0.1.2',
     author='Isaac Duong',
     author_email='isaaacduong@gmail.com',
     license='MIT',    
     url='https://github.com/isaacduong/youtube_summarizer',
     description=("Python script to extract video transcripts " 
                  "based on the video id, and summarize the " 
                  "text content using the GPT-3.5 Turbo model."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['yt_summarizer'],
     install_requires=[            # I get to this in a second
-          'googleapiclient',
+          'google-api-python-client',
           'youtube_transcript_api',
           'openai',
           'tqdm',
           'nltk',
           'gtts',
           'langdetect',
       ],
```

### Comparing `yt_summarizer-0.1.1/yt_summarizer/youtube_video_summary.py` & `yt_summarizer-0.1.2/yt_summarizer/youtube_video_summary.py`

 * *Files identical despite different names*

### Comparing `yt_summarizer-0.1.1/yt_summarizer.egg-info/PKG-INFO` & `yt_summarizer-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: yt-summarizer
-Version: 0.1.1
-Summary: Python script to extract video transcripts based on the video id, and summarize the text content using the GPT-3.5 Turbo model.
-Home-page: https://github.com/isaacduong/youtube_summarizer
-Author: Isaac Duong
-Author-email: isaaacduong@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # YouTube Video Summarizer
 
 The YouTube Video Summarizer is a Python script that allows you to extract video transcripts based on the video id, and summarize the 
 text content using the GPT-3.5 Turbo model. You can apply the script to video of any language under the condition the video creator do 
 not disable the transcript of the videos intentionally. By default video in German and English will be summarized in these languages, 
 Summaries of videos spoken in all other languages will be in English. 
 
@@ -48,8 +37,23 @@
 
 - Python 3.x
 - Google API Key
 - OpenAI API Key
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
-downloader = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key)
+
+summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
+
+then 
+transcript = summarizer.get_transcript(video_id)
+
+and afterwards call 
+summary = summarizer.summarize_text(transcript)
+
+and if you want to save it to a file ( text or audio file ) 
+
+summarizer.write_to_textfile(video_id,summary)
+or
+summarizer.convert_to_audio(summary)
+
+
```

