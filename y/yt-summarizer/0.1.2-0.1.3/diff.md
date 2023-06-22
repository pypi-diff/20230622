# Comparing `tmp/yt_summarizer-0.1.2.tar.gz` & `tmp/yt_summarizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_summarizer-0.1.2.tar", last modified: Thu Jun 22 10:07:24 2023, max compression
+gzip compressed data, was "yt_summarizer-0.1.3.tar", last modified: Thu Jun 22 12:02:57 2023, max compression
```

## Comparing `yt_summarizer-0.1.2.tar` & `yt_summarizer-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.186218 yt_summarizer-0.1.2/
--rw-r--r--   0 isaacduong   (501) staff       (20)     1062 2023-06-21 20:47:45.000000 yt_summarizer-0.1.2/LICENSE
--rw-r--r--   0 isaacduong   (501) staff       (20)     3456 2023-06-22 10:07:24.186278 yt_summarizer-0.1.2/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)     3070 2023-06-22 10:03:37.000000 yt_summarizer-0.1.2/README.md
--rw-r--r--   0 isaacduong   (501) staff       (20)       79 2023-06-22 10:07:24.186462 yt_summarizer-0.1.2/setup.cfg
--rw-r--r--   0 isaacduong   (501) staff       (20)      886 2023-06-22 10:07:22.000000 yt_summarizer-0.1.2/setup.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.185475 yt_summarizer-0.1.2/yt_summarizer/
--rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:25:30.000000 yt_summarizer-0.1.2/yt_summarizer/__init__.py
--rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:25:17.000000 yt_summarizer-0.1.2/yt_summarizer/youtube_video_summary.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 10:07:24.186106 yt_summarizer-0.1.2/yt_summarizer.egg-info/
--rw-r--r--   0 isaacduong   (501) staff       (20)     3456 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)      285 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)       81 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/requires.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)       14 2023-06-22 10:07:24.000000 yt_summarizer-0.1.2/yt_summarizer.egg-info/top_level.txt
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 12:02:57.223012 yt_summarizer-0.1.3/
+-rw-r--r--   0 isaacduong   (501) staff       (20)     1062 2023-06-21 20:47:45.000000 yt_summarizer-0.1.3/LICENSE
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3467 2023-06-22 12:02:57.223101 yt_summarizer-0.1.3/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3081 2023-06-22 12:00:53.000000 yt_summarizer-0.1.3/README.md
+-rw-r--r--   0 isaacduong   (501) staff       (20)       79 2023-06-22 12:02:57.223421 yt_summarizer-0.1.3/setup.cfg
+-rw-r--r--   0 isaacduong   (501) staff       (20)      886 2023-06-22 12:02:27.000000 yt_summarizer-0.1.3/setup.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 12:02:57.221932 yt_summarizer-0.1.3/yt_summarizer/
+-rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:25:30.000000 yt_summarizer-0.1.3/yt_summarizer/__init__.py
+-rw-r--r--   0 isaacduong   (501) staff       (20)    10680 2023-06-22 11:54:51.000000 yt_summarizer-0.1.3/yt_summarizer/youtube_video_summary.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-22 12:02:57.222838 yt_summarizer-0.1.3/yt_summarizer.egg-info/
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3467 2023-06-22 12:02:57.000000 yt_summarizer-0.1.3/yt_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)      285 2023-06-22 12:02:57.000000 yt_summarizer-0.1.3/yt_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-22 12:02:57.000000 yt_summarizer-0.1.3/yt_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)       81 2023-06-22 12:02:57.000000 yt_summarizer-0.1.3/yt_summarizer.egg-info/requires.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)       14 2023-06-22 12:02:57.000000 yt_summarizer-0.1.3/yt_summarizer.egg-info/top_level.txt
```

### Comparing `yt_summarizer-0.1.2/LICENSE` & `yt_summarizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_summarizer-0.1.2/PKG-INFO` & `yt_summarizer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_summarizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python script to extract video transcripts based on the video id, and summarize the text content using the GPT-3.5 Turbo model.
 Home-page: https://github.com/isaacduong/youtube_summarizer
 Author: Isaac Duong
 Author-email: isaaacduong@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,18 +52,18 @@
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
 
 summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
 
 then 
-transcript = summarizer.get_transcript(video_id)
+lang, transcript = summarizer.get_transcript(video_id)
 
 and afterwards call 
-summary = summarizer.summarize_text(transcript)
+summary = summarizer.summarize_text(transcript,lang)
 
 and if you want to save it to a file ( text or audio file ) 
 
 summarizer.write_to_textfile(video_id,summary)
 or
 summarizer.convert_to_audio(summary)
```

### Comparing `yt_summarizer-0.1.2/README.md` & `yt_summarizer-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
 
 summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
 
 then 
-transcript = summarizer.get_transcript(video_id)
+lang, transcript = summarizer.get_transcript(video_id)
 
 and afterwards call 
-summary = summarizer.summarize_text(transcript)
+summary = summarizer.summarize_text(transcript,lang)
 
 and if you want to save it to a file ( text or audio file ) 
 
 summarizer.write_to_textfile(video_id,summary)
 or
 summarizer.convert_to_audio(summary)
```

### Comparing `yt_summarizer-0.1.2/setup.py` & `yt_summarizer-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='yt_summarizer',
-    version='0.1.2',
+    version='0.1.3',
     author='Isaac Duong',
     author_email='isaaacduong@gmail.com',
     license='MIT',    
     url='https://github.com/isaacduong/youtube_summarizer',
     description=("Python script to extract video transcripts " 
                  "based on the video id, and summarize the " 
                  "text content using the GPT-3.5 Turbo model."),
```

### Comparing `yt_summarizer-0.1.2/yt_summarizer/youtube_video_summary.py` & `yt_summarizer-0.1.3/yt_summarizer/youtube_video_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         """
         Get the transcript of a YouTube video.
 
         Parameters:
         - video_id (str): The ID of the YouTube video.
 
         Returns:
+        - video language(str): the language of title
         - transcript (str): The transcript of the video.
         """
         
         langs = list(set([language, self.video_lang(video_id)] ))
         
         try:
             transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
@@ -139,22 +140,22 @@
             video_lang = self.extract_language_code(str(transcript_list))
             if video_lang is not None:
                 langs = list(set([language, video_lang, self.video_lang(video_id)] ))
             logging.warning(langs)
             for lang in langs:
                 try:
                     transcript = transcript_list.find_manually_created_transcript([lang])
-                    return '.'.join(section['text'] for section in transcript.fetch())
+                    return self.video_lang(video_id), '.'.join(section['text'] for section in transcript.fetch())
                 
                 except NoTranscriptFound as e:
                     
                     try:
                         transcript = transcript_list.find_generated_transcript([lang])
                         logging.info(f'Auto-generiert transcript.')
-                        return '.'.join(section['text'] for section in transcript.fetch())  
+                        return self.video_lang(video_id),'.'.join(section['text'] for section in transcript.fetch())  
                     except NoTranscriptFound as e:
                         
                         logging.warning(f'failed to retrieve transcript in {lang}. Try to retrieve transcript in {set(langs).difference(set(lang))}')
                         continue
                 except Exception as e:
         
                     logging.warning(f"Error retrieving transcript for video: {video_id}. {e}")
@@ -216,28 +217,27 @@
             chunk = tokens[i: i+token_lim]  
             section = ' '.join(chunk)
             chunks.append(section) 
             
         return chunks
 
     
-    def summarize_text(self, text,video_id, max_tokens = 200):
+    def summarize_text(self, text,lang, max_tokens = 200):
         """
         Summarize text using OpenAI's GPT model.
 
         Parameters:
         - text (str): The text to summarize.
         - video_id (str): The ID of the associated video.
         - max_tokens (int): The maximum number of tokens in the summary (default: 200).
 
         Returns:
         - summary (str): The summarized text.
         """
         
-        lang = self.video_lang(video_id)
         openai.api_key = self.openai_api_key
     
         content = "Du bist ein hilfreicher Assistent, der Texte zusammenfasst" if lang =="de" \
                 else "You are a helpful assistant that summarizes text."
         
         # reduce number of tokens when reaching token limit 
         for token_lim in range(2000,0,-500):
@@ -299,17 +299,17 @@
 
 
 if __name__ == "__main__":
     
     
     video_id = input("Youtube Video ID: ") # video_id is the characters after v= inside the link such as https://www.youtube.com/watch?v=cupU_lyNY2w
     downloader = YouTubeVideoSummarizer()
-    text = downloader.get_transcript(video_id)
+    lang, text = downloader.get_transcript(video_id)
     if text:
-        summarized_text = downloader.summarize_text(text,video_id, max_tokens = 200)
+        summarized_text = downloader.summarize_text(text,lang, max_tokens = 200)
         print(summarized_text)
         # you can also write the summarized transcript to file :
         # downloader.write_to_textfile(video_id,summarized_text)
         # or as mp3 file downloader.convert_to_audio(summarized_text)
     else:
         print("problem retrieving transcript")
```

### Comparing `yt_summarizer-0.1.2/yt_summarizer.egg-info/PKG-INFO` & `yt_summarizer-0.1.3/yt_summarizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-summarizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python script to extract video transcripts based on the video id, and summarize the text content using the GPT-3.5 Turbo model.
 Home-page: https://github.com/isaacduong/youtube_summarizer
 Author: Isaac Duong
 Author-email: isaaacduong@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,18 +52,18 @@
 
 ## usage 
 you have to pass your Youtube API Key and OpenAI API Key as parameters to the YouTubeVideoSummarizer constructor as following
 
 summarizer = YouTubeVideoSummarizer(your Youtube API Key, your OpenAI API Key) 
 
 then 
-transcript = summarizer.get_transcript(video_id)
+lang, transcript = summarizer.get_transcript(video_id)
 
 and afterwards call 
-summary = summarizer.summarize_text(transcript)
+summary = summarizer.summarize_text(transcript,lang)
 
 and if you want to save it to a file ( text or audio file ) 
 
 summarizer.write_to_textfile(video_id,summary)
 or
 summarizer.convert_to_audio(summary)
```

