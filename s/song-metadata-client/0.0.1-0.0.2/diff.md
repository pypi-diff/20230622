# Comparing `tmp/song_metadata_client-0.0.1.tar.gz` & `tmp/song_metadata_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "song_metadata_client-0.0.1.tar", max compression
+gzip compressed data, was "song_metadata_client-0.0.2.tar", max compression
```

## Comparing `song_metadata_client-0.0.1.tar` & `song_metadata_client-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1063 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     2005 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/README.md
--rw-r--r--   0        0        0     1444 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      550 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/__init__.py
--rw-r--r--   0        0        0      328 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/__init__.py
--rw-r--r--   0        0        0      180 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/clients/__init__.py
--rw-r--r--   0        0        0     5420 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/clients/spotify_metadata_client.py
--rw-r--r--   0        0        0     4990 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/clients/ytmusic_metadata_client.py
--rw-r--r--   0        0        0       74 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/config/__init__.py
--rw-r--r--   0        0        0      419 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/config/spotify_options.py
--rw-r--r--   0        0        0      532 2023-06-16 15:45:46.822973 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/__init__.py
--rw-r--r--   0        0        0      735 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_playlist_handler.py
--rw-r--r--   0        0        0      682 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_search_handler.py
--rw-r--r--   0        0        0      723 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_track_handler.py
--rw-r--r--   0        0        0      741 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_playlist_handler.py
--rw-r--r--   0        0        0      682 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_search_handler.py
--rw-r--r--   0        0        0      726 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_track_handler.py
--rw-r--r--   0        0        0      264 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/playlist_metadata.py
--rw-r--r--   0        0        0      456 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/classes/song_metadata.py
--rw-r--r--   0        0        0       98 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/di/__init__.py
--rw-r--r--   0        0        0      831 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/di/dependency_injector.py
--rw-r--r--   0        0        0       90 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/errors/__init__.py
--rw-r--r--   0        0        0       83 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/errors/metadata_client_error.py
--rw-r--r--   0        0        0       87 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/interfaces/__init__.py
--rw-r--r--   0        0        0      246 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/interfaces/base_metadata_client.py
--rw-r--r--   0        0        0      780 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/main.py
--rw-r--r--   0        0        0        0 2023-06-16 15:45:46.826974 song_metadata_client-0.0.1/song_metadata_client/py.typed
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 song_metadata_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-22 20:38:13.832010 song_metadata_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2005 2023-06-22 20:38:13.836010 song_metadata_client-0.0.2/README.md
+-rw-r--r--   0        0        0     1443 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      550 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/clients/__init__.py
+-rw-r--r--   0        0        0     5420 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/clients/spotify_metadata_client.py
+-rw-r--r--   0        0        0     4990 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/clients/ytmusic_metadata_client.py
+-rw-r--r--   0        0        0       74 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/config/__init__.py
+-rw-r--r--   0        0        0      419 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/config/spotify_options.py
+-rw-r--r--   0        0        0      532 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/__init__.py
+-rw-r--r--   0        0        0      735 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_playlist_handler.py
+-rw-r--r--   0        0        0      682 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_search_handler.py
+-rw-r--r--   0        0        0      723 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_track_handler.py
+-rw-r--r--   0        0        0      741 2023-06-22 20:38:13.840010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_playlist_handler.py
+-rw-r--r--   0        0        0      682 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_search_handler.py
+-rw-r--r--   0        0        0      726 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_track_handler.py
+-rw-r--r--   0        0        0      264 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/classes/playlist_metadata.py
+-rw-r--r--   0        0        0      456 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/classes/song_metadata.py
+-rw-r--r--   0        0        0       98 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/di/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/di/dependency_injector.py
+-rw-r--r--   0        0        0       90 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/errors/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/errors/metadata_client_error.py
+-rw-r--r--   0        0        0       87 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/interfaces/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/interfaces/base_metadata_client.py
+-rw-r--r--   0        0        0      968 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/main.py
+-rw-r--r--   0        0        0        0 2023-06-22 20:38:13.844010 song_metadata_client-0.0.2/song_metadata_client/py.typed
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 song_metadata_client-0.0.2/PKG-INFO
```

### Comparing `song_metadata_client-0.0.1/LICENSE` & `song_metadata_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/README.md` & `song_metadata_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/pyproject.toml` & `song_metadata_client-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "song-metadata-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "A generic client to fetch metadata for any song"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "song_metadata_client"}]
 
 keywords = ["metadata", "python", "song metadata", "spotify", "youtube", "youtube music", "music", "song"]
@@ -29,15 +29,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 spotipy = "^2.23.0"
 rapidfuzz = "^3.1.1"
 python-slugify = "^8.0.1"
 ytmusicapi = "^1.0.2"
-taipan-di = "^0.0.5"
+taipan-di = "0.0.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 vcrpy = "^4.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
```

### Comparing `song_metadata_client-0.0.1/song_metadata_client/__init__.py` & `song_metadata_client-0.0.2/song_metadata_client/__init__.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/clients/spotify_metadata_client.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/clients/spotify_metadata_client.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/clients/ytmusic_metadata_client.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/clients/ytmusic_metadata_client.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/__init__.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_playlist_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_search_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_search_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/spotify_track_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/spotify_track_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_playlist_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_search_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_search_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/classes/handlers/ytmusic_track_handler.py` & `song_metadata_client-0.0.2/song_metadata_client/classes/handlers/ytmusic_track_handler.py`

 * *Files identical despite different names*

### Comparing `song_metadata_client-0.0.1/song_metadata_client/main.py` & `song_metadata_client-0.0.2/song_metadata_client/di/dependency_injector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from typing import Union
-from taipan_di import DependencyCollection
+from taipan_di import ServiceCollection
 
-from song_metadata_client.classes import SongMetadata, PlaylistMetadata, SpotifyOptions
-from song_metadata_client.di import add_song_metadata_client
+from song_metadata_client.classes import (
+    SpotifyOptions,
+    SpotifyMetadataClient,
+    YTMusicMetadataClient,
+)
+from song_metadata_client.classes.handlers import *
 from song_metadata_client.interfaces import BaseMetadataClient
 
+__all__ = ["add_song_metadata_client"]
 
-class SongMetadataClient:
-    def __init__(self, spotify_options: SpotifyOptions = None):
-        services = DependencyCollection()
-        add_song_metadata_client(services)
 
-        if spotify_options is not None:
-            services.register_singleton_instance(SpotifyOptions, spotify_options)
+def add_song_metadata_client(services: ServiceCollection) -> ServiceCollection:
+    services.register(SpotifyOptions).as_singleton().with_self()
 
-        self._client = services.build().resolve(BaseMetadataClient)
+    services.register(SpotifyMetadataClient).as_factory().with_self()
+    services.register(YTMusicMetadataClient).as_factory().with_self()
 
-    def search(self, url_or_query: str) -> Union[SongMetadata, PlaylistMetadata]:
-        return self._client.exec(url_or_query)
+    services.register_pipeline(BaseMetadataClient).add(SpotifyTrackHandler).add(
+        SpotifyPlaylistHandler
+    ).add(YTMusicTrackHandler).add(YTMusicPlaylistHandler).add(SpotifySearchHandler).add(
+        YTMusicSearchHandler
+    ).as_factory()
+
+    return services
```

### Comparing `song_metadata_client-0.0.1/PKG-INFO` & `song_metadata_client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: song-metadata-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A generic client to fetch metadata for any song
 Home-page: https://github.com/Billuc/song-metadata-client
 License: MIT
 Keywords: metadata,python,song metadata,spotify,youtube,youtube music,music,song
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Utilities
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: spotipy (>=2.23.0,<3.0.0)
-Requires-Dist: taipan-di (>=0.0.5,<0.0.6)
+Requires-Dist: taipan-di (==0.0.7)
 Requires-Dist: ytmusicapi (>=1.0.2,<2.0.0)
 Project-URL: Documentation, https://github.com/Billuc/song-metadata-client
 Project-URL: Repository, https://github.com/Billuc/song-metadata-client
 Description-Content-Type: text/markdown
 
 # Song Metadata Client
```

