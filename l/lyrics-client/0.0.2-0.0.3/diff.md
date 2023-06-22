# Comparing `tmp/lyrics_client-0.0.2.tar.gz` & `tmp/lyrics_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_client-0.0.2.tar", max compression
+gzip compressed data, was "lyrics_client-0.0.3.tar", max compression
```

## Comparing `lyrics_client-0.0.2.tar` & `lyrics_client-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/LICENSE
--rw-r--r--   0        0        0     2093 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/README.md
--rw-r--r--   0        0        0      440 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/__init__.py
--rw-r--r--   0        0        0      159 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/__init__.py
--rw-r--r--   0        0        0      355 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/__init__.py
--rw-r--r--   0        0        0     3975 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/abstract_lyrics_client.py
--rw-r--r--   0        0        0     2723 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/azlyrics_lyrics_client.py
--rw-r--r--   0        0        0     2575 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/genius_lyrics_client.py
--rw-r--r--   0        0        0     2165 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/musixmatch_lyrics_client.py
--rw-r--r--   0        0        0      245 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/fetch_lyrics_command.py
--rw-r--r--   0        0        0      209 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/fetch_lyrics_result.py
--rw-r--r--   0        0        0       83 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/di/__init__.py
--rw-r--r--   0        0        0      520 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/di/dependency_injector.py
--rw-r--r--   0        0        0      211 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/__init__.py
--rw-r--r--   0        0        0       71 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/bad_format_error.py
--rw-r--r--   0        0        0       79 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/bad_title_match_error.py
--rw-r--r--   0        0        0       69 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/no_result_error.py
--rw-r--r--   0        0        0       81 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/interfaces/__init__.py
--rw-r--r--   0        0        0      240 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/interfaces/base_lyrics_client.py
--rw-r--r--   0        0        0      841 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/main.py
--rw-r--r--   0        0        0        0 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/py.typed
--rw-r--r--   0        0        0     1341 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 lyrics_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2093 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/README.md
+-rw-r--r--   0        0        0      440 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/__init__.py
+-rw-r--r--   0        0        0     3975 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/abstract_lyrics_client.py
+-rw-r--r--   0        0        0     2723 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/azlyrics_lyrics_client.py
+-rw-r--r--   0        0        0     2575 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/genius_lyrics_client.py
+-rw-r--r--   0        0        0     2165 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/musixmatch_lyrics_client.py
+-rw-r--r--   0        0        0      245 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/fetch_lyrics_command.py
+-rw-r--r--   0        0        0      257 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/fetch_lyrics_result.py
+-rw-r--r--   0        0        0       83 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/di/__init__.py
+-rw-r--r--   0        0        0      513 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/di/dependency_injector.py
+-rw-r--r--   0        0        0      211 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/bad_format_error.py
+-rw-r--r--   0        0        0       79 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/bad_title_match_error.py
+-rw-r--r--   0        0        0       69 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/no_result_error.py
+-rw-r--r--   0        0        0       81 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/interfaces/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/interfaces/base_lyrics_client.py
+-rw-r--r--   0        0        0      978 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/main.py
+-rw-r--r--   0        0        0        0 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/py.typed
+-rw-r--r--   0        0        0     1340 2023-06-22 20:30:21.092970 lyrics_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 lyrics_client-0.0.3/PKG-INFO
```

### Comparing `lyrics_client-0.0.2/LICENSE` & `lyrics_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/README.md` & `lyrics_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/lyrics_client/classes/clients/abstract_lyrics_client.py` & `lyrics_client-0.0.3/lyrics_client/classes/clients/abstract_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/lyrics_client/classes/clients/azlyrics_lyrics_client.py` & `lyrics_client-0.0.3/lyrics_client/classes/clients/azlyrics_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/lyrics_client/classes/clients/genius_lyrics_client.py` & `lyrics_client-0.0.3/lyrics_client/classes/clients/genius_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/lyrics_client/classes/clients/musixmatch_lyrics_client.py` & `lyrics_client-0.0.3/lyrics_client/classes/clients/musixmatch_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.2/lyrics_client/di/dependency_injector.py` & `lyrics_client-0.0.3/lyrics_client/di/dependency_injector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from taipan_di import DependencyCollection
+from taipan_di import ServiceCollection
 
 from lyrics_client.interfaces import BaseLyricsClient
 from lyrics_client.classes.clients import GeniusLyricsClient, AZLyricsLyricsClient, MusixmatchLyricsClient
 
 __all__ = ["add_lyrics_client"]
 
-def add_lyrics_client(services: DependencyCollection) -> DependencyCollection:
+def add_lyrics_client(services: ServiceCollection) -> ServiceCollection:
     services.register_pipeline(BaseLyricsClient)\
         .add(GeniusLyricsClient)\
         .add(AZLyricsLyricsClient)\
         .add(MusixmatchLyricsClient)\
-        .register()
+        .as_factory()
     
     return services
```

### Comparing `lyrics_client-0.0.2/lyrics_client/main.py` & `lyrics_client-0.0.3/lyrics_client/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from typing import List
-from taipan_di import DependencyCollection
+from taipan_di import ServiceCollection
 
 from lyrics_client.classes import FetchLyricsCommand, FetchLyricsResult
 from lyrics_client.di import add_lyrics_client
 from lyrics_client.interfaces import BaseLyricsClient
+from lyrics_client.errors import NoResultError
 
 __all__ = ["LyricsClient"]
 
 
 class LyricsClient:
     def __init__(self):
-        services = DependencyCollection()
+        services = ServiceCollection()
         add_lyrics_client(services)
 
         self._clients = services.build().resolve(BaseLyricsClient)
 
     def get_lyrics(self, request: FetchLyricsCommand) -> List[FetchLyricsResult]:
-        return self._clients.exec(request)
-    
-    def get_from_song(self, song_title: str, song_artists: str, clients: List[str] = ["genius"]) -> List[FetchLyricsResult]:
+        result = self._clients.exec(request)
+
+        if result is None:
+            raise NoResultError("No result")
+
+        return result
+
+    def get_from_song(
+        self, song_title: str, song_artists: str, clients: List[str] = ["genius"]
+    ) -> List[FetchLyricsResult]:
         command = FetchLyricsCommand(song_title, song_artists, clients)
-        return self._clients.exec(command)
-        
+        return self.get_lyrics(command)
```

### Comparing `lyrics_client-0.0.2/pyproject.toml` & `lyrics_client-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-client"
-version = "0.0.2"
+version = "0.0.3"
 description = "A generic client to fetch lyrics from a song's data"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["lyrics client", "lyrics", "python", "genius", "azlyrics, musixmatch"]
 
@@ -26,15 +26,15 @@
 
 include = ["lyrics_client/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.2"
 requests = "^2.31.0"
-taipan-di = "^0.0.4"
+taipan-di = "0.0.7"
 python-slugify = "^8.0.1"
 rapidfuzz = "^3.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.3.0"
```

### Comparing `lyrics_client-0.0.2/PKG-INFO` & `lyrics_client-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A generic client to fetch lyrics from a song's data
 Home-page: https://github.com/Billuc/lyrics-client
 License: MIT
 Keywords: lyrics client,lyrics,python,genius,azlyrics, musixmatch
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: taipan-di (>=0.0.4,<0.0.5)
+Requires-Dist: taipan-di (==0.0.7)
 Project-URL: Documentation, https://github.com/Billuc/lyrics-client
 Project-URL: Repository, https://github.com/Billuc/lyrics-client
 Description-Content-Type: text/markdown
 
 # Lyrics-Client
 
 **Get the lyrics of your favorite musics !**
```

